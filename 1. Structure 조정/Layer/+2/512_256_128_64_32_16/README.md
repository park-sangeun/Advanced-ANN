## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 32 </br>
LATENT_VECTOR = 16 </br>
DECODER_1 = 32 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

> basic model에서 512, 256, 128, 64, 32, Latent_vector 3->16 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/80a0ab14-2d81-4528-8b6d-02e77b2a875d" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.012647  </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d1c6ec53-bc92-447a-86bd-3a3e8b76154a" width = "600">

---
