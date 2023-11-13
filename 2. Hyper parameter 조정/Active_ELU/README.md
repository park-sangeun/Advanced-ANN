## Hyper parameter 조정

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 300 </br>
LEARNING_RATE = 1e-4 </br>

### [Activation function] ELU 1
>고정 Layer는 512 - 256 - 64 - 16 이다.

### [Hyper parameter] 1
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/59d6ab93-2261-4822-9231-f39075e2f942" width="400">

### [Test Error] 1
test error:  </br>

<img src = "" width = "600">

---

### [Activation function] ELU 2
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [Hyper parameter] 1

<img src = "" width="400">

### [Test Error] 1
test error:  </br>

<img src = "" width = "600">

---

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0a0834e9-efff-44a4-a96f-d81eea7a062c" width="400">

### [Test Error] 2
test error: 0.009451 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/9314ef6a-5ba4-44a8-a5f3-7a8dbec27084" width = "600">

---

### [Hyper parameter] 3
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.5) 추가 </br>

<img src = "" width="400">

### [Test Error] 3
test error:  </br>

<img src = "" width = "600">

---
