## Structure 조정_Layer 수 +0_Hidden Node 변경

### [Structure]
ENCODER_1 = 256 </br>
ENCODER_2 = 64 </br>
ENCODER_3 = 16 </br>

LATENT_VECTOR = 4

DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 256 </br>

> basic model에서 256, 64, 16, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/3b68eeca-3948-4c91-82d3-0400a0e9367f" width = "400">

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error]
<b> 0.018669 </b>

![1 Layer3_256_64_16_4](https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f657f274-72cd-4285-b9f9-ec529bb67efc)

