## Structure 조정_Layer 수 +0_Hidden Node 변경
> Layer는 basic model과 동일, 각 layer의 hidden node와 각 경우에 따른 test error 소개

기본정보
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 0.005 </br>

<b>[Structure]</b></br>
* Activation function 등 basic과 동일 </br>

Result
---
* Layer: 128 - 64 - 32 - 4 - 32 - 64 - 128 </br>
test error: 0.019304 </br>

* Layer: 256 - 128 - 32 - 4 - 32 - 128 - 256 </br>
test error: 0.018658 </br>

* Layer: 256 - 64 - 16 - 4 - 16 - 64 - 256 </br>
test error: 0.018669 </br>

* Layer: 512 - 256 - 32 - 4 - 32 - 256 - 512 </br>
test error: 0.018578 </br>

