![header](https://capsule-render.vercel.app/api?type=waving&color=CC9E6B&height=230&section=header&text=PM10%20Clustering&fontSize=60&fontColor=6F5941)
# description
지역별 미세먼지 분포가 어떻게 다른지 알아보기 위해 대기정보 데이터 중 PM10의 일데이터를 통해 군집 분류를 한다.
# data
+ 에어코리아 https://www.airkorea.or.kr
+ 지역
  - 서울, 경기, 인천, 세종, 대전, 충남
+ 기간
  - 2018년 ~ 2021년 사이의 겨울 데이터
  - 11월 ~ 3월 사이
+ StandardScaler
  - 평균, 표준편차를 이용해 정규화
# clustering
+ ### TimeSeriesKMeans
  시계열 데이터에 대한 K개의 클러스터링
+ ### DTW(동적시간워핑)
  비슷한 두개의 다른 속도의 시간축의 파장의 유사성을 측정하는 알고리즘으로 유클리드 거리와는 달리 거리가 가장 짧은 시점을 연결
  ![image](https://user-images.githubusercontent.com/72387067/153740727-562f29b1-7cd0-48e5-bd25-6f963e83fb4f.png)

-------------------------
#### 4개의 Clusters
<img src="https://user-images.githubusercontent.com/72387067/153728442-5ac4d796-b03a-48e0-a411-34e164d9be8d.png" width="600" height="905"/>

## Map
<img src="https://user-images.githubusercontent.com/72387067/153728479-dc8a7074-9e34-4622-860f-2480a32bcd92.png" width="441" height="662"/>
