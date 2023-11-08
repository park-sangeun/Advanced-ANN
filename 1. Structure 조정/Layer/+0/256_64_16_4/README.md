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

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.018669 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f657f274-72cd-4285-b9f9-ec529bb67efc" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 LR을 5e-3 -> 5e-4로 줄임 </br>
  
### [Test Error] 2
<b> 0.018233 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/06bdb37f-7924-4e5d-8d83-d61a2b026fe5" width = "600">

---

### [Hyper parameter] 3
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 1e-4 </br>

> 1에서 LR을 5e-3 -> 1e-4로 줄임 </br>
  
### [Test Error] 3
<b> 0.019113 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f24a6b32-62f8-4d29-8de7-4ddd992d69ec" width = "600">

---

### [Hyper parameter] 4
BATCH_SIZE = 128 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 1e-3 </br>

> 1에서 BATCH를 64->128로 증가함에 따라 LR을 5e-3 -> 1e-3로 사용 </br>
  
### [Test Error] 4
<b> 0.018119 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/c5c3a96f-40f4-433d-862d-c71886428b27" width = "600">

---

Result
---
batch_size = 64인 경우 LR은 5e-4가 최적
batch_size = 128인 경우 1e-3이 최적
