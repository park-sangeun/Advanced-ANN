## Layer 내 Hidden Node에 따른 성능 비교
>Latent_Vector 32 고정

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 1e-4 </br>

### [고정 Loss & Optimizer]
loss_fn = nn.SmoothL1Loss() </br>
optimizer = torch.optim.Adam(model.parameters(), lr=LEARNING_RATE) </br>

---

### [Structure] 1
512 - 256 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6d6a680d-0b75-43bf-aa17-d11d3ac626cb" width="400">

### [Test Error] 1
test error: 0.003682 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/382325ab-e740-4715-baa5-1a74f4277043" width = "600">

### [Structure] 2
512 - 256 - 128 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/2f2d8897-cdd4-4c3c-97af-5a05be221fe6" width="400">

### [Test Error] 2
test error: 0.003726 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/586a9c0a-e93a-42a0-98d0-997a0e64295b" width = "600">

### [Structure] 3
512 - 128 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/ad1bcd3d-56c8-417f-90fe-99274f8131b1" width="400">

### [Test Error] 3
test error: 0.003675 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/293c9eda-2151-4566-a439-f69110743bf8" width = "600">
