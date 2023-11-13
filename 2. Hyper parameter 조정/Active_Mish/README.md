## Hyper parameter 조정

### [고정 Hyper parameter]
>비교를 위해 Batch size, Epochs, LR 고정

BATCH_SIZE = 64 </br>
EPOCHS = 300 </br>
LEARNING_RATE = 1e-4 </br>

### [Activation function] Mish 1
>고정 Layer는 512 - 256 - 128 - 64 - 32 - 16 이다.

### [Hyper parameter] 1

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/90300a8a-f1f6-457d-9acf-b04bbfdae6bf" width="400">

### [Test Error] 1
test error: 0.013250 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/f248ae97-65c8-4141-b69f-a18abdb81736" width = "600">


### [Hyper parameter] 2
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder, Decoder 각 층마다 nn.Dropout(p=0.3) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/39412f7d-1326-4b9a-9a70-d828dda9bd79" width="400">

### [Test Error] 2
test error: 0.009746 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/da9ce67b-8ebf-48f2-af5e-702bc8f09906" width = "600">

---

### [Hyper parameter] 3
Encoder, Decoder 각 층마다 nn.BatchNorm1d 추가 </br>
Encoder, Decoder 각 층마다 nn.Dropout(p=0.5) 추가 </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/5f67f355-3d7f-40b6-9301-2192ec7b212f" width="400">

### [Test Error] 3
test error: 0.009678  </br>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/ce0e1e27-e31d-440e-aad9-181f895fc043" width = "600">
