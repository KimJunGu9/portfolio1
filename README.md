# :pushpin: 중고차 가격 예측하기

</br>

## 1. Overview

- Project Title : '인도 중고차 예측하기' 데이터셋으로 중고차 가격 예측
- Authors : 이소희, 신경훈, 안은정, 김준구 총 4인 
- Date : 23/04/23 ~ 23/05/13


</br>

## 2. 사용 기술

  - Pandas
  - Numpy
  - Matplotlib
  - Seaborn
  - Sklearn
  - Linear Regression
  - Random Forest
  - LightGBM
</br>

## 3. Dataset

- Data:  https://www.kaggle.com/datasets/avikasliwal/used-cars-price-prediction

- Kaggle에서 주최한 "인도 중고차 예측하기" 데이터셋의 train data를 바탕으로 중고차 가격 예측하기

- ***6019*** rows and ***14*** columns
  
## 프로젝트 과정
1. 구조 파악 및 column 검토
2. 데이터 전처리
3. 모델 분석 및 구축
  - LinearRegression 모델 구축
  - RandomForest 모델 구축
  - GradientBoost 모델 구축
  - XGBoost 모델 구축
  - LightGBM 모델 구축
4. 모델 검증
- LinearRegression 모델 검증
    - 결정계수 : 0.71, RMSE : 5.88
- RandomForest 모델 검증
    - 결정계수 : 0.90, RMSE : 3.47
- GradientBoost 모델 검증
    - 결정계수 : 0.90, RMSE : 3.48
- XGBoost 모델 검증
    - 결정계수 : 0.91, RMSE : 3.27
- LightGBM 모델 검증
    - 결정계수 : 0.92, RMSE : 2.98


 

## 프로젝트 결과


- 사용 한 모델 중 모델링을 돌려 본 결과 'LightGBM' 정확도가 높아 채택
- 프로젝트 과정에서 4. 모델검증에 나와있듯이 'LightGBM'의 결정계수와 RMSE가 다른 모델들에 비해 좋음
- 중고차 가격 예측값
  - 현대차 (가격 2.35라크)
    - LinearRegression 모델 : 1.48라크로 예측
    - RandomForest 모델 : 2.79라크로 예측
    - LightGBM 모델 : 3.12라크로 예측
  - BMW (가격 7.0라크)
    - LinearRegression 모델 : 8.32라크로 예측
    - RandomForest 모델 : 8.64라크로 예측
    - LightGBM 모델 : 10.84라크로 예측
- 중고차 가격을 잘 받을 수 있는 인도 지역 예측
  - LightGBM 모델로 Porsche 거래 시  Coimbatore 지역
