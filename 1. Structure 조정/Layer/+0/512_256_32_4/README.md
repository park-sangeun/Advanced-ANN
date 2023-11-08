## Structure 조정_Layer 수 +0_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 32 </br>

LATENT_VECTOR = 4

DECODER_1 = 32 </br>
DECODER_2 = 256 </br>
DECODER_3 = 512 </br>

> basic model에서 512, 256, 32, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f1c0994f-e742-4c5a-8a0b-941d2e07ab5b" width = "400">

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error]
<b> 0.018578 </b>

![1 Layer3_512_256_32_4](https://github.com/park-sangeun/Advanced-ANN/assets/90459890/76f2daf0-493c-4b8d-8824-4ab9ed528458)
