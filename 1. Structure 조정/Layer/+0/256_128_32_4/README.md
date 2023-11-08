## Structure 조정_Layer 수 +0_Hidden Node 변경

### [Structure]
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 32 </br>

LATENT_VECTOR = 4

DECODER_1 = 32 </br>
DECODER_2 = 128 </br>
DECODER_3 = 256 </br>

> basic model에서 256, 128, 32, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/08be5efc-931a-449c-9650-eac9f284194b" width = "400">

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error]
<b> 0.018658 </b>

![1 Layer3_256_128_32_4](https://github.com/park-sangeun/Advanced-ANN/assets/90459890/92b18579-eafe-4c70-a4bd-862e34db96b7)
