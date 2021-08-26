# Computer_vision_team_1 : YOLO v1 논문 구현 시도
---

<img width="618" alt="YOLO_architecture" src="https://user-images.githubusercontent.com/50979281/130927332-1aefef43-c67e-48db-98fe-68cd0a1ad629.png">
쿠아이 하계 컨퍼런스를 위해 컴퓨터비전 1팀에서 YOLO v1(You Only Look Once: Unified, Real-Time Object Detection)을 텐서플로우와 파이토치로 구현했습니다. 

YOLO v1 : https://arxiv.org/abs/1506.02640

## Members
강민기(소프트웨어학부), 김민규(전자전기공학부), 김태윤(소프트웨어학부),이승연(소프트웨어학부)

## 멤버별 구현 방식

### 텐서플로우를 이용해 구현 - 강민기, 김민규

강민기 : 

김민규 : 구현 난이도를 이유로 Backbone을 VGG-16으로 변경하고 데이터 증강을 구현하지 않았습니다. 훈련 방법은 논문에 나온 값(배치 사이즈, 에포크 등)을 그대로 사용했고 매 에포크마다 검증 로스(검증용 데이터셋에 대한 로스, Verification Loss)가 줄어들면 저장하여 검증 로스가 가장 낮은 모델을 최종 훈련 모델로 선택하였습니다. 
테스트 결과, 훈련용 데이터셋에 오버피팅되어 테스트용 데이터셋에서는 좋지 못한 성능을 보여줬습니다. 데이터 증강을 구현하지 못한 것이 오버피팅의 주요 원인이라 생각됩니다.

### 파이토치를 이용해 구현 - 김태윤, 이승연

김태윤 : 

이승연 : 


