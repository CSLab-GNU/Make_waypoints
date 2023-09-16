# Make_waypoints
Map에서 A-Star 알고리즘을 통해 waypoint를 작성하는 패키지입니다.

### System Requirements
* Ubuntu 18.04
* ROS Melodic

### Installation
catkin_ws/src 폴더에 해당 Repository 를 Clone 합니다
```bash
$ mkdir ~/catkin_ws/src
$ cd ~/catkin_ws/src
$ git clone https://github.com/CSLab-GNU/Make_waypoints.git
$ cd ..
$ catkin_make
$ source devel/setup.bash

### Run

$ roslaunch astar astar.launch

#### Change Map
환경에 설정된 맵을 변경하는 방법은 다음과 같습니다.

launch 폴더의 astar.launch에서 맵을 변경할 수 있습니다.
"InflateRadius"를 조절하여 맵에 가상벽을 생성하고 waypoint를 찍을 수 있습니다.
