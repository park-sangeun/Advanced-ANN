## Structure 조정_Layer 수 +1_Hidden Node 변경

### [Structure]
ENCODER_1 = 512 </br>
ENCODER_2 = 256 </br>
ENCODER_3 = 128 </br>
ENCODER_4 = 32 </br>
LATENT_VECTOR = 8 </br>
DECODER_1 = 32 </br>
DECODER_2 = 128 </br>
DECODER_3 = 256 </br>
DECODER_4 = 512 </br>

> basic model에서 512, 256, 128, 32, Latent_vector 3->8 </br>

<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/cf8f177b-9d8e-420d-9aae-294b78fa1e9b" width = "400">

### [Hyper parameter] 1
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 1
<b> 0.012941 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/8715fde2-549c-448d-8203-a0d127864af3" width = "600">

---

### [Hyper parameter] 2
BATCH_SIZE = 32 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

> batch_size 64, epochs만 50->100 </br>
  
### [Test Error] 2
<b> 0.012593 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/da646616-2183-496d-bb1b-f4097cf33a3c" width = "600">

---

Result
---
Latent_vector가 4일 때보다 8인 경우 test error가 확연하게 줄었다.
