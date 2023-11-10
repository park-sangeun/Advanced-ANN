## Structure 조정_Optimizer 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

> basic model에서 512, 256, 128, 64, 16, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Back-end-Practice/assets/90459890/c55e54be-dc3d-47d5-a612-691ff69c0d56" width = "400">

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Optimizer] 1 RMSprop

### [Test Error] 1
test error: 0.017195 </br>

<img src = "https://github.com/park-sangeun/Back-end-Practice/assets/90459890/10b96d89-07af-41d7-bf85-a96866776d78" width = "600">
