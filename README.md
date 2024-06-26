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

#### LiDAR
터틀봇에 내장된 LiDAR는 SLAM 및 Mapping에 특화되어, 구현 가능성 및 완성도를 고려하였을 때 제외하는 것으로 판단

##### RECORD

24.04.05
계획 구체화 및 플로우차트 완성
24.04.11
주제 수정 및 터틀봇 세팅 완료
24.04.18
주제 수정 및 중간 발표 자료 제작

24.04.29 ~ 24.05.05
turtlebot3 setting
-turtlebot3 관련 ROS 패키지 및 Turtlebot3 패키지 다운, Network Configuration 진행함.
-turtlebot3 구동을 위한 OpenCR Setup 진행
-Bring up 및 teleop 실행


<실행 순서>
- 마스터 PC -
roscore

- 터틀 봇 - 
roslaunch turtlebot3_bringup turtlebot3_robot3_robot.launch

- 마스터 PC -
roslaunch turtlebot3_navigation turtlebot3_navigation map:=~

- 터틀 봇 -
roslaunch usb_cam usb_cam-test.launch
