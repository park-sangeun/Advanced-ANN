## Structure 조정_Layer 수 +0_Hidden Node 변경

### [Structure]
ENCODER_1 = 128 </br>
ENCODER_2 = 64 </br>
ENCODER_3 = 32 </br>

LATENT_VECTOR = 4

DECODER_1 = 32 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>

> basic model에서 63->64, 12->32, Latent_vector 3->4 </br>

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error]
<b> 0.019304  </b>

![1 Layer3_128_64_32_4](https://github.com/park-sangeun/Advanced-ANN/assets/90459890/749f548b-95c3-404b-b4d6-c27550172699)
