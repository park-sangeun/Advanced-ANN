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

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/8c3b83ca-10e8-47c9-a77b-36a4f1196080" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 0.005 </br>

> basic model과 동일한 파라미터로 진행, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.019304  </b>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/749f548b-95c3-404b-b4d6-c27550172699" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 LR을 5e-3 -> 5e-4로 줄임 </br>
  
### [Test Error] 2
<b> 0.018763 </b>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6e04a7f4-57a5-4f37-ac74-930e45e7ca37" width = "600">

---

### [Hyper parameter] 3
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 LR을 5e-3 -> 1e-4로 줄임 </br>
  
### [Test Error] 3
<b> 0.020138 </b>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/4feb43dc-e38b-4824-8826-79997fdf83d7" width = "600">

---

### [Hyper parameter] 4
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> 1에서 BATCH를 64->128로 증가함에 따라 LR을 5e-3 -> 1e-3로 사용 </br>
  
### [Test Error] 4
<b>  </b>

<img src="" width = "600">

---

Result
---
batch_size = 64인 경우 LR은 가 최적 </br>
batch_size = 128인 경우 LR은 이 최적 </br>
