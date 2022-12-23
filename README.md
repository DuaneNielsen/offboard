# ROS offboard package

mavros package for ROS Noetic

## build

check out into a catkin_ws


```commandline
catkin_make install
```


## launch

flight controller connected on usb /dev/ttyACM0
```commandline
. ~/catkin_ws/install/setup.bash
roslaunch offboard offboard.launch
```

flight controller over UDP
```commandline
. ~/catkin_ws/install/setup.bash
roslaunch offboard offboard.launch fcu_url:=udp://192.168.1.200:14550?ids=255,240@
```
