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

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f21db750-9af8-4d11-b6c8-5bc2132ed0c3" width="400">

### [Test Error] 1-1
test error: 0.004376 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/74abb22b-e499-4cd0-8738-5f16c83e7ab0" width = "600">

### [Structure] 1-2
512 - 256 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6d6a680d-0b75-43bf-aa17-d11d3ac626cb" width="400">

### [Test Error] 1-2
test error: 0.003682 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/382325ab-e740-4715-baa5-1a74f4277043" width = "600">

---
### [Structure] 2-1
512 - 256 - 128 - 32 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/26ff663c-ff90-4ee7-9105-9f522b0a91d4" width = "400">

### [Test Error] 2-1
test error: 0.004228  </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6d07e767-dc80-4035-82bb-0a56aa7dd58d" width = "600">

### [Structure] 2-2
512 - 256 - 128 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/2f2d8897-cdd4-4c3c-97af-5a05be221fe6" width="400">

### [Test Error] 2-2
test error: 0.003726 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/586a9c0a-e93a-42a0-98d0-997a0e64295b" width = "600">


### [Structure] 2-3
512 - 256 - 128 - 32 </br>
Dropout: 0.2 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/02e03c36-4a38-41bf-92db-2390a369b54e" width="400">

### [Test Error] 2-3
test error: 0.003720 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/97573788-d610-4891-b2a5-2ad5f1ec3191" width = "600">

---
### [Structure] 3-1
512 - 128 - 64 - 32 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/b9baa2ec-6156-4bf8-9bcd-2254a04aa512" width = "400">

### [Test Error] 3-1
test error: 0.004760  </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/417ab762-6a14-41c5-8c62-fb4ab1ca9006" width = "600">

### [Structure] 3-2
512 - 128 - 64 - 32 </br>
Dropout: 0.3 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/ad1bcd3d-56c8-417f-90fe-99274f8131b1" width="400">

### [Test Error] 3-2
test error: 0.003675 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/293c9eda-2151-4566-a439-f69110743bf8" width = "600">

### [Structure] 3-3
512 - 128 - 64 - 32 </br>
Dropout: 0.2 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/d6896c46-e4cc-4b43-b6ed-976d1f0c516a" width = "400">

### [Test Error] 3-3
test error: 0.003817  </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/fc98a5ea-fa79-4656-bd9d-be4a66a2e182" width = "600">

---

### [Structure] 4-1
256 - 128 - 64 - 32 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/9ae90555-b621-4305-b012-b1a74a72288d" width="400">

### [Test Error] 4-1
test error: 0.005238 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/ed5effbe-df2c-4606-921e-a31252f0f428" width = "600">
