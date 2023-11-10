## Structure 조정_Layer 수 +1에 batch_regularization 추가

### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Structure] 1
ENCODER_1 = 256 </br>
ENCODER_2 = 128 </br>
ENCODER_3 = 64 </br>
ENCODER_4 = 16 </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
nn.BatchNorm1d(16) </br>
DECODER_2 = 64 </br>
nn.BatchNorm1d(64) </br>
DECODER_3 = 128 </br>
nn.BatchNorm1d(128) </br>
DECODER_4 = 256 </br>
nn.BatchNorm1d(256) </br>

> DECODER마다 nn.BatchNorm1d() 추가
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/1aa32846-33e9-48c4-9bfb-8f2415a73f76" width = "400">

### [Test Error] 1
<b> 0.017214 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/070255ea-d185-4fa6-ab69-eb1dc03e0f64" width = "600">

---

### [Structure] 1
ENCODER_1 = 256 </br>
nn.BatchNorm1d(256) </br>
ENCODER_2 = 128 </br>
nn.BatchNorm1d(128) </br>
ENCODER_3 = 64 </br>
nn.BatchNorm1d(64) </br>
ENCODER_4 = 16 </br>
nn.BatchNorm1d(16) </br>
LATENT_VECTOR = 4 </br>
DECODER_1 = 16 </br>
DECODER_2 = 64 </br>
DECODER_3 = 128 </br>
DECODER_4 = 256 </br>

> ENCODER마다 nn.BatchNorm1d() 추가
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6162aeb2-3ec2-4f5a-b313-6d2ccf0cf7c5" width = "400">

### [Test Error] 1
<b> 0.017334 </b>

<img src = "https://github.com/park-sangeun/Back-end-Practice/assets/90459890/d8c4d83f-7776-463d-96fd-67d4ec599c29" width = "600">

---
