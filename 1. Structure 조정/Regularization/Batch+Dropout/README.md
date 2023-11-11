## Structure 조정_Batch+Dropout 추가

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 32 </br>
LATENT_VECTOR = 8 </br>
DECODER_1 = 32 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

> basic model에서 512, 256, 128, 64, 32, Latent_vector 3->8 </br>
<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f49b48ce-137b-4c4c-b645-918b969c6577" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 1
<b> 0.013028  </b>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fa0739b8-a415-4de0-900d-939650847688" width="600">
