## Structure 조정_Layer 수 +1에 dropout 추가

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Structure] 1
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
Dropout() </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> ENCODER_4 다음에 DROPOUT() 추가, dropout_rate: 0.5
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0644ace4-c0bb-4135-872d-3d3e1849120c" width = "400">

### [Test Error] 1
<b> 0.017523 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/01f7c008-1377-46fc-b851-859972fb883f" width = "600">

