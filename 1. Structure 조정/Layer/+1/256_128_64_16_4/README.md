## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> basic model에서 256, 128, 64, 16, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/852c410e-24fd-4e8e-9915-4399a35c8e1b" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.017712 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/adb8bba7-9fbf-4c06-a9ae-87cb3b566776" width = "600">

---


---

Result
---
batch_size = 64인 경우 LR은 가 최적 </br>
batch_size = 128인 경우 LR은 이 최적 </br>
