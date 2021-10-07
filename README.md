# digital-health-hackathon

## EDA - Exploratory Data Analysis

1. 상관관계 분석
2. 변수 분포 확인

## Code : Jupyter Notebook Files

1. 유효하지 않은 환자 데이터 제거 - eliminate_invalid_data.ipynb
2. 치료효능률 계산을 위한 가상 환자 데이터 생성 - make_virtual_data.ipynb
3. 은닉층을 가진 CoxPH 딥러닝 모델 학습 - train_deep_coxph_model.ipynb
4. 학습된 모델의 치료효능률 결과 분석 - analyze_result.ipynb

## CSV Files

0. dataset 폴더 - 대회 주최 측에서 제공한 원본 데이터
1. all-in-one.csv - 주최 측에서 제공한 데이터를 하나로 만든 파일
2. all-in-one-modified.csv - 유효하지 않은 값을 가진 환자 데이터를 제거한 파일 
3. virtual-data.csv - 치료효능률 계산을 위해 만든 가상 환자 데이터를 담은 파일
4. train results 폴더 - 학습시킨 모델의 결과를 저장한 csv파일
  - ratio_123_100_4000.csv : 학습시킨 모델들의 모든 결과를 하나로 통합한 파일

## Trained Networks

- 160 + 480 + 480 = 1120가지의 모델

### Number of Hidden Layer : 1
- Node : 100 ~ 4000 까지 100단위로 40가지
- Node Decreasing Rate : 1
- Learning Rate : 0.0001, 0.001, 0.01, 0
- 40 * 1 * 4 = 160 가지의 모델

### Number of Hidden Layer : 2
- Node : 100 ~ 4000 까지 100단위로 40가지
- Node Decreasing Rate : 1, 1/2, 1/4
- Learning Rate : 0.0001, 0.001, 0.01, 0
- 40 * 3 * 4 = 480 가지의 모델

### Number of Hidden Layer : 3
- Node : 100 ~ 4000 까지 100단위로 40가지
- Node Decreasing Rate : 1, 1/2, 1/4
- Learning Rate : 0.0001, 0.001, 0.01, 0
- 40 * 3 * 4 = 480 가지의 모델
