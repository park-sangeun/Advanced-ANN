## Structure 조정_Layer 수 +0_Hidden Node 변경
> Layer는 basic model과 동일, 각 layer의 hidden node와 각 경우에 따른 test error 소개

기본정보 1
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 0.005 </br>

<b>[Structure]</b></br>
* Activation function 등 basic과 동일 </br>

Result 1
---
* Layer: 128 - 64 - 32 - 4 - 32 - 64 - 128 </br>
test error: 0.019304 </br>

* Layer: 256 - 128 - 32 - 4 - 32 - 128 - 256 </br>
test error: 0.018658 </br>

* Layer: 256 - 64 - 16 - 4 - 16 - 64 - 256 </br>
test error: 0.018669 </br>

* Layer: 512 - 256 - 32 - 4 - 32 - 256 - 512 </br>
test error: 0.018578 </br>

기본정보 2
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 5e-4 </br>

<b>[Structure]</b></br>
* Activation function 등 basic과 동일 </br>

Result 2
---
* Layer: 128 - 64 - 32 - 4 - 32 - 64 - 128 </br>
test error:  </br>

* Layer: 256 - 128 - 32 - 4 - 32 - 128 - 256 </br>
test error:  </br>

* Layer: 256 - 64 - 16 - 4 - 16 - 64 - 256 </br>
test error: 0.018233 </br>

* Layer: 512 - 256 - 32 - 4 - 32 - 256 - 512 </br>
test error: 0.017443 </br>

기본정보 3
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 1e-4 </br>

<b>[Structure]</b></br>
* Activation function 등 basic과 동일 </br>

Result 3
---
* Layer: 128 - 64 - 32 - 4 - 32 - 64 - 128 </br>
test error:  </br>

* Layer: 256 - 128 - 32 - 4 - 32 - 128 - 256 </br>
test error:  </br>

* Layer: 256 - 64 - 16 - 4 - 16 - 64 - 256 </br>
test error:  </br>

* Layer: 512 - 256 - 32 - 4 - 32 - 256 - 512 </br>
test error: 0.018671 </br>
