## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 64 </br>
ENCODER_5 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
DECODER_5 = 512 </br>

> basic model에서 512, 256, 128, 64, 16, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/21ea5e41-ebc7-423c-8eae-8e273a6ca863" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.017126 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/da692717-d944-47ec-b2d5-d4eb20932b62" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 1e-3 </br>

> batch_size 64, LR 1e-3, epochs만 50->100 </br>
  
### [Test Error] 2
<b> 0.017741 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/09b1628d-091e-4ce8-bc77-22a90358dd74" width = "600">

---

### [Hyper parameter] 3
BATCH_SIZE = 32 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 32, LR 5e-4, epochs만 50->100 </br>
  
### [Test Error] 3
<b> 0.016840 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/63049202-234f-4bce-81e2-c108e86715c1" width = "600">

---

Result
---
batch_size = 64인 경우 LR은 가 최적 </br>
batch_size = 128인 경우 LR은 이 최적 </br>
