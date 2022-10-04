# brc_arm_ws
Initial workspace required for moveit implementation for robot arm subteam

Runs on ROS2 Humble with Moveit Humble on Ubuntu 22.04 LTS

## Instalation:
1. Install Ubuntu 22.04 LTS (Virtual machine, WSL2, or bare metal all work) and [ROS2 Humble](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)
2. Clone this repository, it will serve as the workspace as well
3. Follow the steps listed in this [Moveit2 tutorial](https://moveit.picknik.ai/humble/doc/tutorials/getting_started/getting_started.html)
   - **Skip steps "Create A Colcon Workspace and Download Tutorials", and "Download Source Code of MoveIt and the Tutorials"**
   - Run `colcon build --mixin release` until the code compiles. This may need to be ran multiple times (like a lot of times)
6. Move on to this [tutorial](https://moveit.picknik.ai/humble/doc/tutorials/quickstart_in_rviz/quickstart_in_rviz_tutorial.html) and ensure Moveit2 has been installed correctly
