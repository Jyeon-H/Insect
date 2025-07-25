# 병해충 정보 제공 시스템
<br>

## 💬 개요
기후 데이터를 기반으로 작물별 병해충 발생 여부 예측 및 방제 정보 제공 시스템
<br><br>

## 📌 목표
- 귀농인의 병해충 정보 부족 문제 해결
- 지역 기후 데이터 기반 병해충 예측 모델 구축
- 작물 이미지 분류 모델 구현 및 웹 인터페이스 제공
<br><br>

## 🙋🏻‍♀️ 수행 역할
- 4인 협업 프로젝트에서 **데이터 수집, 전처리, 모델 학습 전반 주도**
- 공공 데이터 포털 Open API를 통해 병해충 및 지역별 기후 데이터 수집
- 수집된 데이터 전처리 및 MySQL DB 저장
- 로지스틱 회귀 기반 병해충 예측 모델 구현
<br><br>

## 🗂️ 데이터
- **기상 및 병해충 정보** :
  - 출처 : 공공데이터 포털
  - 내용 : 지역별 기상 관측소 정보, 연도별 측정 기상 정보, 작물별 병해충 발생 이력
- **작물 이미지** :
  - 출처 : Kaggle
  - 내용 : 15가지 작물 이미지<br>
![농생명_화살표](https://github.com/user-attachments/assets/a8341a62-2868-4ce7-937c-6ff240abbb2e)
<br><br>

## 🔍 모델 및 방법
- **주요 기술** : Python, Pandas, Numpy, scikit-learn, MySQL, Streamlit
- **병해충 예측** :
  - *모델* : Logistic Regression
  - *입력* : 지역 기후 데이터 (온도, 습도 등)
  - *출력* : 병해충 발생 여부 (미발생 : 0, 발생 : 1)
- **이미지 분류** :
  - *모델* : InceptionResNetV2, VGG16, Xception
  - *입력* : 작물 이미지
  - *출력* : 작물 종류
<br><br>

## 📊 주요 결과
- 병해충 발생 예측 모델 정확도 : **약 63%**
- 작물 이미지 분류 모델 성능 평가
  |Model|Loss|Accuracy|Rate|
  |---|---|---|---|
  |InceptionResNetV2|0.1281|0.9750|<img width="300" height="270" alt="image" src="https://github.com/user-attachments/assets/7a4ace4f-c0b0-42ea-b721-97a7cb650d30" />|
  |VGG16|0.1581|0.9750|<img width="300" height="250" alt="image" src="https://github.com/user-attachments/assets/e434b155-195b-441e-9790-eeb59212a417" />|
  |Xception|0.0466|0.9875|<img width="300" height="240" alt="image" src="https://github.com/user-attachments/assets/115c3eb4-5332-4b87-892b-6cb736ff92d3" />|
- 웹 페이지 예시
<img width="700" height="500" alt="web1" src="https://github.com/user-attachments/assets/780c249e-92ce-4c88-b6c3-aed351f7c7d1" />
<img width="700" height="500" alt="web2" src="https://github.com/user-attachments/assets/9ac88351-7e27-41dd-9fa1-efc71030d977" />
<img width="700" height="500" alt="web3" src="https://github.com/user-attachments/assets/64516891-291e-483e-beab-1d9914efa734" />


## 🔁 회고
사회문제를 해결하기 위해 AI 기술이 적용되는 과정을 처음 접하고, 흥미를 가지게 되었습니다.
