# 3rd-Team-Project
These Are My Own Works that can determine whether your dogs are obese or normal👦

## 개발 목적
- 가설 설정
  - 코로나 상황이 장기화됨에 따라 반려동물의 비만도는 증가할 것으로 가설 설정
  - 농림축산식품부 조사 결과, 2020년 기준 반려동물 양육자 수는 1,500만 명에 달함
- 문제 제기
  - 비만으로 인한 합병증(당뇨, 관절염 등)이 초래
  - 견주로서 책임감을 가지고 반려동물을 건강하게 양육해야 함
- 결론 : 개발의 필요성
  - 반려동물의 건강과 행복을 위해 꾸준히 비만도를 측정하는 서비스 개발의 필요성을 느낌

## 이미지 수집과 레이블링
- 3만장을 웹 크롤링으로 수집한다.
  - 이미지를 하나씩 확인하여 6천장의 이미지를 선별한다.
- 수집된 6천장을 직접 정상과 비만으로 분류한다.
  - B.C.S (Body Condition Scoring) 기준을 활용한다.

## 모델 학습

### TensorFlow CNN
- 직접 Conv2D층과 MaxPooling을 쌓는다.

### Pytorch
- Transfer Leraning
  - resnet에는 18, 34, 50, 101, 152 레이어를 쌓을 수 있다.
  - 본 학습에선 resnet34 활용한다.
  - 신경망 층을 전이학습 API가 알아서 구성해준다.
  - 신경망 구성 [출처 : https://www.analyticsvidhya.com/blog/2021/09/building-resnet-34-model-using-pytorch-a-guide-for-beginners/]
  
![image](https://user-images.githubusercontent.com/95407799/163902795-08680779-6da5-4821-9e40-aefbbaec69a9.png)

## 
