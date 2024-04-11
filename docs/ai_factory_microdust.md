
# 프로젝트 개요
[대회링크](https://aifactory.space/task/2317/overview)<br>
데이터 애널리스트 트랙 부트캠프 수강 기간 중, 3명의 팀원과 같이 대전 지역에 미세먼지 농도(PM2.5)를 예측하는 모델을 개발하는 경진대회에 참여.

# 개인 기여도
- 팀 인원: 4명
- 기여도: 30%
- 담당 파트: 같이 선행 연구 조사 및 브레인 스토밍을 진행한 뒤, 3가지의 접근법을 정하여 그 중 하나를 단독으로 담당함. 

## 사용 모델 구조:
여러 지역에 걸쳐져있는 기상 정보 및 미세먼지 데이터를 종합적으로 활용하기 위해서, [A Deep CNN-LSTM Model for Particulate Matter (PM2.5) Forecasting in Smart Cities [Huang & Kuo 2018]](https://www.mdpi.com/1424-8220/18/7/2220) 논문을 참고한 CNN-LSTM 모델을 Pytorch로 직접 구현. 

### Feature2DEncoder 모델 구조:
![AI Spark 모델 Feature Encoder](https://github.com/jsh318900/jsh318900/assets/22267053/55a85395-704b-432a-a584-d35d30562e69)
### 모델 전체 구조:
![AI Spark 전체 모델](https://github.com/jsh318900/jsh318900/assets/22267053/1cb7ce63-a71f-4a01-90c7-358836f78abd)


# 사용 기술
- PyTorch, Pandas

# 참고 자료
- [전체 코드베이스](https://github.com/jsh318900/ai_spark_challenge)
- [모델 구현 및 훈련 코드](https://nbviewer.org/gist/jsh318900/9438c231bd8915e294a72165094807ee)

