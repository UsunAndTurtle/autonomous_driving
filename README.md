##### autonomous_driving


##### FLOWCHART
<img width="624" alt="flowchart" src="https://github.com/UsunAndTurtle/autonomous_driving/assets/112847633/8a80811f-5132-43f9-a536-14d53cc2a0aa">


- RVIZ를 이용한 지정위치 탐색

1. LiDAR를 이용한 SLAM으로 Map 제작.
2. MAP 저장.
3. RVIZ 에서 저장된 맵을 불러옴.
4. 현재 위치를 계속 업데이트 하기위해 SLAM을 이용한 Localization.
5. RVIZ에서 직접 마우스로 목표 지점 클릭.
6. 목표 지점을 가기위한 LOCAL_PATH_PLANNG(A* 알고리즘).
7. 경로 계획한 다음 경로 추종.




##### RECORD

24.04.05
계획 구체화 및 플로우차트 완성

