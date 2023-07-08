# Absenteeism_at_work

본 프로젝트는 Absenteeism_at_work.csv 파일을 이용하여 군집화 분석을 수행하였습니다.

1.1 데이터 수집
- 아래 data repository에서 원하는 dataset 선택 (변수가 10개 이상, 그리고 실제 label이 있는 데이터 선정)
  https://archive.ics.uci.edu/ml/datasets.php
- 데이터에 대해서 이해한대로 설명

1.2 전처리
- 범주형 변수(categorical variable)는 적절한 변환 처리 필요
- 필요에 따라 스케일링(Scaling), 정규화(Normalization) 수행
(※ 거리정보에 기반한 군집화의 경우 특정 변수 값의 크기(스케일)에 크게 좌우될 수 있기 때문)

1.3 군집화 분석
- K-Means, Hierarchical clustering, DBSCAN, Affinity propagation 등 학습한 군집화 분석을 수행
- 각 알고리즘의 hyperparameter tuning 수행
- 군집화 적용 결과비교: metric(SSE, Silhouette score 등) 기반으로 군집 결과를 기술
  
1.4 군집 결과 분석 및 가시화
- 군집화 분석 결과가 적당했는지, 실제 레이블을 기준으로 평가 (관측치의 색으로 표기)
  ※ 군집화 분석은 비지도학습 기법이나, 연구 수행 시 알고리즘의 유효성 평가를 위해 레이블이 있는 데이터에 대해 실험
- PCA 같은 차원축소 등을 통해 2차원 상에 가시화 (예시, 실제 label을 관측치의 색으로 표시)
  - 예시> https://in2techs.com/mnist-visualization-using-pca-and-tsne-in-python/
