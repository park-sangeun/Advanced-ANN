## Structure 조정_Layer 수 +1에 dropout 추가

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Structure] 1
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
Dropout() </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> ENCODER_4 다음에 DROPOUT() 추가, dropout_rate: 0.5
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0644ace4-c0bb-4135-872d-3d3e1849120c" width = "400">

### [Test Error] 1
<b> 0.017523 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/01f7c008-1377-46fc-b851-859972fb883f" width = "600">

---

### [Structure] 2
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
Dropout() </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> ENCODER_4 다음에 DROPOUT() 추가, dropout_rate: 0.2
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d5bb5625-7a5b-4136-bd2f-5665843b59f4" width = "400">

### [Test Error] 2
<b> 0.017762 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/859599fa-87b9-4125-81fb-20044ea78fee" width = "600">

---

### [Structure] 3
ENCODER_1 = 256 </br>
Dropout() </br>
ENCODER_2 = 128 </br>
Dropout() </br>
ENCODER_3 = 64 </br>
Dropout() </br>
ENCODER_4 = 16 </br>
Dropout() </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> ENCODER마다 DROPOUT() 추가, dropout_rate: 0.2
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/cd6cdce8-b319-4de3-8ec5-ffbb6978ec84" width = "400">

### [Test Error] 3
<b> 0.017598 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/eb3a3666-68c7-441d-88cf-9f80bea09075" width = "600">

---

### [Structure] 4
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
Dropout() </br>
DECODER_2 = 64 </br>
Dropout() </br>
DECODER_3 = 128 </br>
Dropout() </br>
DECODER_4 = 256 </br>
Dropout() </br>

> DECODER마다 DROPOUT() 추가, dropout_rate: 0.2
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d97ad04c-c5b5-4899-b9a9-ebc7c3b14b04" width = "400">

### [Test Error] 4
<b> 0.017574 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/a3f289db-f9ed-48a6-b5b3-bf016b2dc928" width = "600">

---

### [Structure] 5
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>
Dropout() </br>

> DECODER_4 다음에 DROPOUT() 추가, dropout_rate: 0.2
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0add5415-1b9f-4370-8b5d-e988f3eebdb2" width = "400">

### [Test Error] 5
<b> 0.017996 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/869ad378-99bf-4ffb-bfb3-a20761b68558" width = "600">
