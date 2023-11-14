## 1차 제출 Code

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 150 </br>
LEARNING_RATE = 1e-4 </br>

### [Layer]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 64 </br>
LATENT_VECTOR =16 </br>
DECODER_1 = 64 </br>
DECODER_2 = 256 </br>
DECODER_3 = 512 </br>

### [Structure]
loss_fn = nn.MSELoss() </br>
optimizer = torch.optim.Adam(model.parameters(), lr=LEARNING_RATE) </br>

### [AutoEncoder Model]
```
class Autoencoder(nn.Module): 
    def __init__(self, dropout_rate=0.3):
        super().__init__()
        self.encoder = nn.Sequential(
            nn.Linear(input_shape,ENCODER_1),
            nn.GELU(),
            nn.BatchNorm1d(ENCODER_1),
            nn.Dropout(p=dropout_rate),
            nn.Linear(ENCODER_1, ENCODER_2),
            nn.GELU(),
            nn.BatchNorm1d(ENCODER_2),
            nn.Dropout(p=dropout_rate),
            nn.Linear(ENCODER_2, ENCODER_3),
            nn.GELU(),
            nn.BatchNorm1d(ENCODER_3),
            nn.Dropout(p=dropout_rate),
            nn.Linear(ENCODER_3, LATENT_VECTOR)
        )

        self.decoder = nn.Sequential(
            nn.Linear(LATENT_VECTOR, DECODER_1),
            nn.GELU(),
            nn.BatchNorm1d(DECODER_1),
            nn.Linear(DECODER_1, DECODER_2),
            nn.GELU(),
            nn.BatchNorm1d(DECODER_2),
            nn.Linear(DECODER_2, DECODER_3),
            nn.GELU(),
            nn.BatchNorm1d(DECODER_3),
            nn.Linear(DECODER_3, input_shape),
            nn.Sigmoid()
        )

    def forward(self, x):
        encoded = self.encoder(x)
        decoded = self.decoder(encoded)
        return decoded
model = Autoencoder().to(device)
print(model)
```

### [Test Error] 
test error: 0.009401 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/9898b436-8b16-461a-8a4a-3fbcdb4d2b47" width = "600">
