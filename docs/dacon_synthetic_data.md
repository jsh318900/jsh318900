
# 프로젝트 개요
[대회 링크](https://dacon.io/competitions/official/236107/overview/description)<br>
데이터 애널리스트 트랙 부트캠프 수강 기간 중, 2명의 팀원과 같이 데이콘 합성데이터 기반 객체 탐지 AI 경진대회에 참여. 인공적으로 만들어진 도로 위 자동차 사진을 사용하여 차량을 탐지하고 모델명으로 분류하는 모델을 훈련시키고, 실제 사진을 테스트셋으로 활용하는 경진대회.

# 개인 기여도
- 팀 인원: 3명
- 기여도: 34%
- 담당 파트: 어떤 모델과 증강방법으로 접근할지 같이 브레인스토밍하고, 각각 모델을 하나씩 골라서 모델 훈련 진행.<br>

## 사용 모델 구조:
FasterRCNN의 ROI Head 부분에 [Dual Attention Newtork [Fu et al. CVPR 2019]](https://openaccess.thecvf.com/content_CVPR_2019/papers/Fu_Dual_Attention_Network_for_Scene_Segmentation_CVPR_2019_paper.pdf)를 추가한 모델로 훈련을 진행함.<br>
오픈 소스 라이브러리인 MMDetection에서 제공하는 FasterRCNN 모델에 논문 내용을 바탕으로 직접 구현한 Dual Attention Network를 integration하여 훈련 진행.<br>
### Dual Attention Networks 모델 구조
![Dual Attention(1)](https://github.com/jsh318900/jsh318900/assets/22267053/65dd0e48-e2b4-4fb8-8e7b-497695113d38)

# 사용 기술
- Python, PyTorch, MMDetection

# 참고 자료
- [전체 코드베이스](https://github.com/jsh318900/mini_project_4_team_1)
- [Dual Attention Network 구현 코드 및 모델 훈련 코드](https://nbviewer.org/gist/jsh318900/3b4f6bcb62c46ba1351a6f8aa32d9a4f)
- [프로젝트 발표 자료](https://github.com/jsh318900/mini_project_4_team_1/blob/main/%EB%AF%B8%EB%8B%88%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%204%20%ED%8C%80%201%20%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C%20.pdf)
