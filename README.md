# LH_PredictionContest
구내식당 식수 인원 예측 AI 경진대회
![image](https://user-images.githubusercontent.com/71416249/132821714-8c2df1a7-c9b2-4c6e-a0c9-887d84705cba.png)


# 1. 프로젝트 소개

## 1.1 참여 프로젝트
구내식당 식수 인원 예측 AI 경진대회
(구내식당의 요일별 점심, 저녁식사를 먹는 인원을 예측)


## 1.2 대회 기간
2021.06.03 ~ 2021.07.23 


## 1.3 팀원 소개
김정진, 김하영, 최소연

## 1.4 평가 규칙
- 평가산식 : MAE(Mean Absolute Error)
- Public 평가 : 전체 Test 데이터 중 무작위 30 % (15일)
- Private 평가 : 전체 Test 데이터 중 나머지 70 % (35일)


## 1.4 순위
![image](https://user-images.githubusercontent.com/71416249/132822520-85df8ef0-ebe6-4950-8641-a478db099976.png)
public: 480팀 중 95위


![image](https://user-images.githubusercontent.com/71416249/132822702-7ad88839-351e-4dc7-b231-cc38a1f9001a.png)
private: 480팀 중 10위(상위 4%)

# 2. 프로젝트 요약

## 2.1 데이터 전처리 및 EDA
- '식사가능자수‘, ‘출근’ 등의 변수 추가
- 단순 인원 대신 비율 변수 추가
- '공휴일전', '공휴일후', '공휴일합' 변수 추가
- '자기계발의날' 변수 추가
- '전날대비확진자'를 로그 변환한 변수 추가


## 2.2 사용한 외부 데이터
- date.csv: 공휴일과 관련된 외부 데이터.
- covid_정리_하영_로그1.csv: 코로나 확진자와 관련된 외부 데이터.


## 2.3 사용한 모델링 방법
compare_models를 사용해 모델을 혼합하여 최종 MAE를 도출함. 이때 도출을 위한 모델의 개수는 가장 작은 MAE를 기록한 모델 5개로 고정함. 


## 2.4 결과 도출
![image](https://user-images.githubusercontent.com/71416249/132826123-240e00c3-94d4-4b6c-8516-a93d4feeb635.png)

하략

