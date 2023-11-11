## Hyper parameter 조정
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 300 </br>
LEARNING_RATE = 5e-4 </br>

### [기본 model Test Error]
BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 5e-4 </br>
>Epochs 300 x 200 o 임을 감안해야 한다.

<b> 0.012647  </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d1c6ec53-bc92-447a-86bd-3a3e8b76154a" width = "600">

---

### [Hyper parameter] 1
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder, Decoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

### [Test Error] 1
test error: 0.011452 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f352c358-d7c1-4b2a-a44b-55dafc8064c0" width = "600">

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder, Decoder 각 층마다 nn.Dropout(p=0.5) 추가 </br>

### [Test Error] 2
test error: 0.011209 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/9eb47a30-7160-4b41-a6fc-3a6d7401b202" width = "600">

