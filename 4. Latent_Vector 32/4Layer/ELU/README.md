## Layer 내 Hidden Node에 따른 성능 비교
>Latent_Vector 32 고정

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 200 </br>
LEARNING_RATE = 1e-4 </br>

### [고정 Loss & Optimizer]
loss_fn = nn.SmoothL1Loss() </br>
optimizer = torch.optim.Adam(model.parameters(), lr=LEARNING_RATE) </br>

---

### [Structure] 1-1
512 - 256 - 64 - 32 </br>

<img src = "" width="400">

### [Test Error] 1-1
test error:  </br>

<img src = "" width = "600">

### [Structure] 1-2
512 - 256 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/511aa157-a50a-4ea9-94fa-8ab5f196e4a2" width="400">

### [Test Error] 1-2
test error: 0.003608 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/07d1f1b3-fc0d-4fda-98e5-7b5e668f2960" width = "600">

---
### [Structure] 2-1
512 - 256 - 128 - 32 </br>

<img src = "" width = "400">

### [Test Error] 2-1
test error:  </br>

<img src = "" width = "600">

### [Structure] 2-2
512 - 256 - 128 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/49668efb-9999-4ec5-b2b9-d1853928b784" width="400">

### [Test Error] 2-2
test error: 0.003575 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/8d25e6d9-ede6-4722-a11d-13b2b980633c" width = "600">


### [Structure] 2-3
512 - 256 - 128 - 32 </br>
Dropout: 0.2 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/2e62b04b-c269-49ee-a34a-06c02555fec1" width="400">

### [Test Error] 2-3
test error: 0.003612 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/de05c5b0-17c1-4411-962c-305933c045f5" width = "600">

---

### [Structure] 3-1
512 - 128 - 64 - 32 </br>

<img src = "" width = "400">

### [Test Error] 3-1
test error:   </br>

<img src = "" width = "600">

### [Structure] 3-2
512 - 128 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/a1cda6d1-b85b-43d9-9cfb-292ac26332a1" width="400">

### [Test Error] 3-2
test error: 0.003664 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fa16f24a-7d16-4b01-b6b5-334ff98724da" width = "600">

### [Structure] 3-3
512 - 128 - 64 - 32 </br>
Dropout: 0.2 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/493bc230-b1b5-462e-aa75-453a840a516d" width = "400">

### [Test Error] 3-3
test error: 0.003660  </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/af1bff55-b89a-4309-bb83-aec094c63bdf" width = "600">

---

### [Structure] 4-1
256 - 128 - 64 - 32 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/84654557-61ae-42e6-8f6b-9ebd94f11565" width="400">

### [Test Error] 4-1
test error: 0.004953 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/57ae0f74-4414-4206-9c78-7869a11f2223" width = "600">
