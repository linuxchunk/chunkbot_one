## Robot Package for automous navigation and mapping

## Overview
This package contains the launch files, nodes, and topics required for autonomous navigation and mapping. The robot is a 4 wheel drive robot with a lidar. The robot is controlled by a raspberry pi 4. The robot uses ROS2 humble.

## Dependencies
### Software
* [ROS2 Humble](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)
* [Ubuntu 22.04](https://ubuntu.com/download/desktop)
### Hardware (In simulation its optional)
* [Raspberry Pi 4](https://www.raspberrypi.org/products/raspberry-pi-4-model-b/) or [Jetson Orin nano](https://developer.nvidia.com/embedded/jetson-orin)
* [Lidar](https://www.robotshop.com/en/rplidar-a1m8-360-degree-laser-scanner-development-kit.html) (optional)
* [Arduino nano](https://store.arduino.cc/usa/arduino-nano)
* [Camera module](https://www.raspberrypi.org/products/camera-module-v2/)




## Installation
```shell
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src
git clone https://github.com/linuxchunk/chunkbot_one.git
cd ~/catkin_ws
colcon make
```

## Usage
```shell
source ~/catkin_ws/install/setup.bash
ros2 launch chunkbot_one launch_robot.launch.py
```

## Launching with Simulation
```shell
source ~/catkin_ws/install/setup.bash
ros2 launch chunkbot_one launch_sim.launch.py
```