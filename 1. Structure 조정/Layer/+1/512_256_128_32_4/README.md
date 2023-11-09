## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 32 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 32 </br>
DECODER_2 = 128 </br>
DECODER_3 = 256 </br>
DECODER_4 = 512 </br>

> basic model에서 512, 256, 128, 32, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/5eebf595-381b-4505-9995-11b43d4226a8" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.017144 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/93766901-6b69-44fb-a6d4-303e3a9c9be0" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 32 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 batch_size 64->32, epochs만 50->300 </br>
  
### [Test Error] 1
<b> 0.017439 </b>

<img src = "https://github.com/park-sangeun/Back-end-Practice/assets/90459890/6b160e39-423b-4d11-9218-eb0936e9d046" width = "600">

---

Result
---
batch_size = 64인 경우 LR은 가 최적 </br>
batch_size = 128인 경우 LR은 이 최적 </br>
