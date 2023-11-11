## Structure 조정_Layer 수 +1에 batch_regularization 추가

Layer 1
---
256-128-64-16-4
### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 100 </br>
LEARNING_RATE = 5e-4 </br>

### [Structure] 1
> DECODER마다 nn.BatchNorm1d() 추가
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/1aa32846-33e9-48c4-9bfb-8f2415a73f76" width = "400">

### [Test Error] 1
<b> 0.017214 </b>

<img src = "https://github.com/park-sangeun/Advanced-ANN/assets/90459890/070255ea-d185-4fa6-ab69-eb1dc03e0f64" width = "600">

---

### [Structure] 2
> ENCODER마다 nn.BatchNorm1d() 추가
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/6162aeb2-3ec2-4f5a-b313-6d2ccf0cf7c5" width = "400">

### [Test Error] 2
<b> 0.017334 </b>

<img src = "https://github.com/park-sangeun/Back-end-Practice/assets/90459890/d8c4d83f-7776-463d-96fd-67d4ec599c29" width = "600">

---

Layer 2
---
512-256-128-64-32-8
### [Hyper parameter]
BATCH_SIZE = 64 </br>
EPOCHS = 300 </br>
LEARNING_RATE = 5e-4 </br>

### [Structure] 1
> ENCODER, DECODER마다 nn.BatchNorm1d() 추가
<img src="https://github.com/park-sangeun/Advanced-ANN/assets/90459890/01e6d3da-5187-4173-a6e8-601a4c341a53" width = "400">

### [Test Error] 1
<b> 0.013239 </b>

<img src = "https://github.com/park-sangeun/Park-sangeun/assets/90459890/604c534c-e48f-4c2f-b669-ddf79ead2f2e" width = "600">

---
