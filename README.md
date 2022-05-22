# Datamining-Team-Project
## 주제 : 한국인의 고혈압 발생 요인 분석 및 예측

### 분석 배경
우리나라의 고혈압 유병률(만 30세 이상)은 2019년 기준 27.2%로 성인 인구 100명 당 27명 꼴로 고통받고 있다.(질병관리청, 2019)\
인구의 평균수명이 증가함에 따라 고혈압의 유병 기간도 길어질 것으로 예상됨에 따라 고혈압은 지속적으로 국가의 중요한 보건문제가 될 것이다.(OECD, 2013; 윤희숙, 2013)

연령이 높이질수록 복합만성질환을 많이 보유하고 있는데 고혈압은 그 자체보다는 합병증인 관상동맥 심장질환, 만성심부전, 뇌졸중과 같은 질환이 발생 시
환자에게 많은 고통을 줄 뿐만 아니라 경제적 부담까지 가중시키기 때문에 국가적인 관리가 요구되는 매우 중요한 질환이다.

### 분석 목적
1. 머신러닝 기법 중 White Box에 속하는 Decision Tree와, feature importance를 볼 수 있는 Random forest를 사용하여 어떤 요인들이 고혈압을 발생시키는지 알아본다.
   또한 파악된 요인들을 어떻게 개선시킬 것인지 방안을 제안해 보고자 한다.

2. SVM(support vector machine)과 KNN(K-Nearest Neighbors) 머신러닝을 사용하여 고혈압 발생환자를 예측하고, 현재는 고혈압 환자가 아니지만 추후에 고혈압이 발생될 가능성이 있는지 판별할 수 있도록 예측모델을 만들어보고자 한다.

### 데이터 획득
KoGES 자료를 Kaggle에서 데이터를 획득
한국인유전체조사사업(Korean Genome and Epidemiology Study; KoGES)은 한국인에게 흔한 만성 질환의 위험요인을 규명하여 맞춤 예방의학 구현의 과학적 근거를 마련하고자 질병관리청 국립보건 연구원이 수행하는 코호트 사업이다.\
2001년부터 일반 인구집단을 대상으로 참여자를 모집하여 건강 및 생활습관 관련 설문조사와 검진을 수행하고, 혈액, 소변, DNA 등의 인체유래물을 수집하였고, 새로운 질병발생과 생활습관 변화에 대한 추적조사를 진행하였다.\
KoGES 출처 : https://www.kdca.go.kr/contents.es?mid=a40504010000
Kaggle 출처 : https://www.kaggle.com/datasets/junsoopablo/korean-genome-and-epidemiology-study-koges

### 분석과정
``` python

import numpy as np

```
