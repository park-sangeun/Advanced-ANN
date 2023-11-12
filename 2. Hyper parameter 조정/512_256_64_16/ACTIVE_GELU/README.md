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
test error: 0.009763 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/158266d9-2c43-424a-894f-3495f081543f" width = "600">

---

### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder, Decoder 각 층마다 nn.Dropout(p=0.2) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/745e1703-5b53-4324-9fee-1e54bb98a4d4" width="400">

### [Test Error] 2
test error:  </br>

<img src = "" width = "600">

---

### [Activation function] GELU 2
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [Hyper parameter] 1

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fd1784a1-e3ef-4844-8fb3-26e8c0544617" width="400">

### [Test Error] 1
test error:  </br>

<img src = "" width = "600">

---
