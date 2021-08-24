# 수입 화물 이상 탐지, 우범도 예측, 우범화물 선별 모델

## 블로그 포스팅 링크
https://blog.naver.com/hwankko27/222482906001

#### AI 경진대회
- 주관: 관세청, 충남대학교
- 주제 : AI를 활용하여 우리나라로 수입되는 화물의 우범도를 예측하는 모델 개발


#### 배경 및 목적 :
- 관세청은 우리나라로 들어오거나 나가는 모든 물품을 신속하게 통관하는 한편, 관련 법규를 엄정하게 진행함으로써 튼튼한 경제, 안전한 사회를 위해 관세국경을 수호화는 기관임
- 매년 약 1천백만건, 매달 약 1백만건이 수입신고되는 상황에서 수입 화물을 검사할 수 있는 인력은 한정되어 있다 보니, 관세국경단계에서 사회안전, 국민건강 등을 위협하는 고위험물품을 선별(타겟팅) 하여 선제적으로 차단하는 기능이 필요함
- 검사 기준 수립에 다양한 선별 기법이 활용되고 있는 가운데, 요즘 가장 핫한 AI를 활용하여 수입화물의 우범도를 예측하는 모델의 개발이 필요함

### 사용 모델
- Random Forest
- Gradient Boosting
- XGBoost


### 수입 통관 진행 과정
<img width="359" alt="수입통관 흐름" src="https://user-images.githubusercontent.com/49335804/130654461-9a27253b-ecbb-4ca6-aa32-bec801a02290.png">

### 데이터셋 예시
<img width="596" alt="dataset1" src="https://user-images.githubusercontent.com/49335804/130654528-48a47b96-40ce-4ea6-8685-4bbd2faaed35.png">
<img width="598" alt="dataset2" src="https://user-images.githubusercontent.com/49335804/130654554-2976cd11-62b0-4226-a75e-e00f7ca89525.png">
<img width="175" alt="dataset3" src="https://user-images.githubusercontent.com/49335804/130654577-bb4ef5ec-e81c-45eb-8d0a-abf44b6c9856.png">

#### 의사결정 트리 시각화
![트리시각화1](https://user-images.githubusercontent.com/49335804/130654799-f413ab30-9a8d-4863-8dbf-bf3a3838171c.png)
![트리시각화2](https://user-images.githubusercontent.com/49335804/130654825-7af35199-1ff2-4365-827b-303cd7f65889.png)


#### 모델 성능 시각화
![xg4](https://user-images.githubusercontent.com/49335804/130654879-82e4175b-4e5b-4e62-8def-137709006ff3.png)


#### PR_curve
![pr4](https://user-images.githubusercontent.com/49335804/130654921-ff8510ec-4518-456d-84b0-36d3a7a848de.png)

#### 모델 기여도가 높은 변수 시각화
![다운로드 (1)](https://user-images.githubusercontent.com/49335804/130654991-e797b4a7-5b65-4f51-ab16-2957a921d565.png)
![다운로드 (3)](https://user-images.githubusercontent.com/49335804/130655021-7d1174bc-961e-4ca1-bab0-27f1e396aa79.png)

