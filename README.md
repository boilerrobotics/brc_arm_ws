# brc_arm_ws
- Workspace for robot arm subteam [Moveit2](https://moveit.picknik.ai/humble/index.html) development
- Runs on [ROS2 Humble](https://docs.ros.org/en/humble/index.html) with Moveit Humble on Ubuntu 22.04 LTS
- Should be ran on a powerful computer (base station or jetson)
- BRC arm specific packages found [here](https://github.com/boilerrobotics/brc_arm) and implemented as submodules

## Installation (For base Moveit2):
1. Install Ubuntu 22.04 LTS (Virtual machine, WSL2, or bare metal) and [ROS2 Humble](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html)
2. Clone this repository, it will serve as the workspace as well
3. Follow the steps listed in this [Moveit2 tutorial](https://moveit.picknik.ai/humble/doc/tutorials/getting_started/getting_started.html)
   - **Skip steps "Create A Colcon Workspace and Download Tutorials", and "Download Source Code of MoveIt and the Tutorials"**
   - Run `colcon build --packages-skip-regex brc_arm_[a-zA-Z]+ --mixin release` until the code compiles
      - This may need to be ran multiple times, `--parallel-workers 1` argument may be needed if limited on ram
      - If one package is taking a long time, try building it individualy: `colcon build --packages-select <package_name> --mixin release`
6. Follow this [tutorial](https://moveit.picknik.ai/humble/doc/tutorials/quickstart_in_rviz/quickstart_in_rviz_tutorial.html) and ensure Moveit2 has been installed correctly
7. Compile all files, including brc_arm packages using `colcon build --mixin release` (does not compile as of 10/04/2022)
