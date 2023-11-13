## Hyper parameter 조정
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [기본 model Test Error] Adam
BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>
>Epochs 300 x 200 o 임을 감안해야 한다.

<b> 0.012647 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d1c6ec53-bc92-447a-86bd-3a3e8b76154a" width = "600">

---

### [Hyper parameter] RMSprop

BATCH_SIZE = 32 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>

### [Test Error] 
test error: 0.013746 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/91892c8e-a9bf-4be7-846c-881baf3b6e8a" width="600">

---

### [Hyper parameter] 1
Encoder, Decoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/9b7b5bf5-5fee-4241-b838-c1bf7673b18d" width = "400">

### [Test Error] 1
test error: 0.013832 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/c47ab1ff-48b9-4117-bc54-d11444c387ec" width = "600">

---

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.Dropout(p=0.5) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fd756d97-20d3-4d14-a590-6f97bf8b5b5a" width = "400">

### [Test Error] 2
test error: 0.014052 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/ce4ee43a-ef6e-4a6a-b1ea-e6584bf9e1a7" width = "600">
