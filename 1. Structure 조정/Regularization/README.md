## Structure 조정_Layer 수 +1_에서 정규화 추가
> Layer를 +1한 모델에 정규화 추가에 따른 test error 소개

기본정보
---
<b>[Hyper parameter]</b></br>
* BATCH_SIZE = 64 </br>
* EPOCHS = 100 </br>
* LEARNING_RATE = 5e-4 </br>

<b>[Structure]</b></br>
* Dropout=0.5로 설정한 후 레이어에 추가 </br>

Result
---
*Encoder_4 다음에 dropout() 추가
test_error: </br>

