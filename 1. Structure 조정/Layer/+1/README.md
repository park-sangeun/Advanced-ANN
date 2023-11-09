## Structure 조정_Layer 수 +1_Hidden Node 변경
> Layer는 basic model에서 1개 추가, 각 layer의 hidden node와 각 경우에 따른 test error 소개

기본정보
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 5e-4 </br>

<b>[Structure]</b></br>
* Activation function 등 basic과 동일 </br>

Result
---
* Layer: 128 - 64 - 32 - 4 - 32 - 64 - 128 </br>
test error:  </br>

* Layer: 256 - 128 - 64 - 16 - 4 - 16 - 64 - 128 - 256 </br>
test error:  </br>

* Layer: 256 - 64 - 16 - 4 - 16 - 64 - 256 </br>
test error:  </br>

* Layer: 512 - 256 - 64 - 32 - 4 - 32 - 64 - 256 - 512 </br>
test error: 0.017263 </br>

* Layer: 512 - 256 - 128 - 32 - 8 - 32 - 128 - 256 - 512 </br>
test error:  </br>
