## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 32 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 32 </br>
DECODER_2 = 64 </br>
DECODER_3 = 256 </br>
DECODER_4 = 512 </br>

> basic model에서 512, 256, 64, 32, Latent_vector 3->4 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f8f8beeb-ae77-42fc-83ec-69ab714c4b45" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b>  </b>

<img src = "" width = "600">

---


---

Result
---
batch_size = 64인 경우 LR은 가 최적 </br>
batch_size = 128인 경우 LR은 이 최적 </br>
