##### autonomous_driving


##### FLOWCHART
<img width="624" alt="flowchart" src="https://github.com/UsunAndTurtle/autonomous_driving/assets/112847633/8a80811f-5132-43f9-a536-14d53cc2a0aa">

1. LiDAR를 이용한 SLAM으로 Map 제작
2. Map에 노드 선언
3. Path planning
4. Control

#### SLAM
1. 터틀봇의 슬램 노드 실행
2. teleoperation 노드 실행, 원격 조종을 이용한 Mapping의 정밀도 향상
3. maxUrange, map_update_interval 등의 파라미터 튜닝 필요
4. odometry, tf 기반의 맵 생성 후 저장(white - collision free, black - inaccessible area, gray - unknown area)

### Object Detection
터틀봇 내부에 있는 LiDAR는 SLAM 및 Mapping에 특화되어, 구현 가능성 및 완성도를 고려하였을때 제외하는 것으로 판단

##### RECORD

24.04.05
계획 구체화 및 플로우차트 완성
24.04.11
주제 수정 및 터틀봇 세팅 완료
24.04.18
주제 수정 및 중간 발표 자료 제작
