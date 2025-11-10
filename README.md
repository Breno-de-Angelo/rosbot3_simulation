# ROSbot3 simulation

This is the root workspace for the ROSbot3 simulation created as part of the evaluation for the Mobile Autonomous Robotics subject being offered at UFES by Helio Perroni Filho.

The project uses different packages as git submodules to create a complete simulation of the ROSbot3 robot. The main packages are:

- [ros_commons](https://github.com/ros2amr/ros_commons): Basic robot-agnostic utilities for ROS.
- [rosbot3_description](https://github.com/ros2amr/rosbot3_description): ROSbot3 simulator-agnostic URDF description with basic utilities for robot visualization.
- [rosbot3_gazebo](https://github.com/ros2amr/rosbot3_description): Gazebo-specific ROSbot3 URDF, gazebo worlds and launch file for spawning and controlling robot in the simulator.

# Instalation

It is recommended to use Docker for running the project. This package is compatible with the docker environment available [here](https://github.com/ros2amr/docker_environment). Follow the instructions of that repo for creating and running the Docker container.

Once inside the container, navigate to this directory and build the project.

# Usage

For quick visualization of the ROSbot3 basic URDF run:

```bash
ros2 launch rosbot3_description display.launch
```

For full simulation using gazebo, run:
```bash
ros2 launch rosbot3_gazebo start.launch
```
