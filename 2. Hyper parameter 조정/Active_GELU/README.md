## Hyper parameter 조정

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 300 </br>
LEARNING_RATE = 1e-4 </br>

### [Activation function] GELU 1
>고정 Layer는 512 - 256 - 64 - 16 이다.

### [Hyper parameter] 1

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0058df1c-d1b1-447f-b0b2-169891a0de9b" width="400">

### [Test Error] 1
test error: 0.009614 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/0acc8a1b-06e4-404d-aa31-7bf92176be9e" width = "600">

---

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.2) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/745e1703-5b53-4324-9fee-1e54bb98a4d4" width="400">

### [Test Error] 2
test error: 0.009763 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/158266d9-2c43-424a-894f-3495f081543f" width = "600">

---

### [Hyper parameter] 3
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6190725d-a67e-414d-8eec-0840e57a5a5c" width="400">

### [Test Error] 3
test error:  </br>

<img src = "" width = "600">

---

### [Hyper parameter] 3
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.5) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/06292e44-6cfc-4da0-aa98-50efd6916b94" width="400">

### [Test Error] 3
test error: 0.009670 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/cf6eccf6-5310-4555-a2fd-11a3949ec790" width = "600">

---

### [Activation function] GELU 2
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [Hyper parameter] 1

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/b82df396-acd5-4960-b05b-889daa346c66" width="400">

### [Test Error] 1
test error:  </br>

<img src = "" width = "600">

---

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder 각 층마다 nn.Dropout(p=0.2) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fd1784a1-e3ef-4844-8fb3-26e8c0544617" width="400">

### [Test Error] 2
test error: 0.009984 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/58530c8d-8d94-4136-b515-90f9dd2322bd" width = "600">

---
