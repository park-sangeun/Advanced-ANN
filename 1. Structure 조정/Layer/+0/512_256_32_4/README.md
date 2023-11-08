## Structure 조정_Layer 수 +0_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 32 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 32 </br>
DECODER_2 = 256 </br>
DECODER_3 = 512 </br>

> basic model에서 512, 256, 32, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f1c0994f-e742-4c5a-8a0b-941d2e07ab5b" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.018578 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/76f2daf0-493c-4b8d-8824-4ab9ed528458" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 LR을 5e-3 -> 5e-4로 줄임 </br>
  
### [Test Error] 2
<b> 0.017443 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f8802eb4-8a84-44ab-8da4-70b2e7736e31" width = "600">

---

### [Hyper parameter] 3
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 1e-4 </br>

> 1에서 LR을 5e-3 -> 1e-4로 줄임 </br>
  
### [Test Error] 3
<b> 0.018671 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0c36a3a6-60c8-467f-8f3a-a26859a77500" width = "600">

---

### [Hyper parameter] 4
BATCH_SIZE = 128 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 1e-3 </br>

> 1에서 BATCH를 64->128로 증가함에 따라 LR을 5e-3 -> 1e-3로 사용 </br>
  
### [Test Error] 4
<b> 0.017405 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/a2ca86f0-a5c3-4dd1-8e2b-0547a9696198" width = "600">

---

Result
---
batch_size = 64인 경우 LR은 5e-4가 최적 </br>
batch_size = 128인 경우 LR은 1e-3이 최적 </br>
