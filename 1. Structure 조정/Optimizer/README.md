## Structure 조정_Optimizer 변경

### [Optimizer] RMSprop

### [Structure] 1
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

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 1
test error: 0.017195 </br>

<img src = "https://github.com/park-sangeun/Back-end-Practice/assets/90459890/10b96d89-07af-41d7-bf85-a96866776d78" width = "600">

### [Hyper parameter] 2
BATCH_SIZE = 32 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 2
test error: 0.017217 </br>

<img src = "https://github.com/park-sangeun/Park-sangeun/assets/90459890/6c9b2a0c-3469-46f1-a6a1-eed125e12e3e" width = "600">

---

### [Structure] 2
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 16 </br>
LATENT_VECTOR = 8 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

> basic model에서 512, 256, 128, 64, 16, Latent_vector 3->8 </br>

### [Hyper parameter] 
BATCH_SIZE = 32 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 
test error: 0.013900 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fbab7260-3ea3-488b-b862-dbc86f3c6b42" width="600">

---

### [Structure] 3
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 32 </br>
LATENT_VECTOR = 16 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

### [Hyper parameter] 
BATCH_SIZE = 32 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 
test error: 0.013746 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/91892c8e-a9bf-4be7-846c-881baf3b6e8a" width="600">
