# brc_arm_ws
Initial workspace required for moveit implementation for robot arm subteam
Runs on ROS2 Humble with Moveit Humble on Ubuntu 22.04 LTS

## Instalation:
1. Install Ubuntu 22.04 LTS and [ROS2 Humble](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)
2. Clone this repository, it will serve as the workspace as well
3. Run `colcon build --mixin release` until the code compiles. This may need to be ran multiple times (like a lot of times)
