<h1 align="center">Go Chase It!</h1>
**Project Go Chase It**: Following white ball chaser. Applied simple tracking tachnique.

[image1]: project_img/img1.png "img1"
[image2]: project_img/img2.png "img2"

![alt text][image1]

![alt text][image2]

## Introduction
This is a project for Udacity's Robotics NanoDegree. It's a robot that is capable of finding a white ball in a forward-facing camera, and driving toward it.

## Concepts and Classes
Concepts explored in this project:

  - ROS package
  - ROS publishers, subscribers, and services
  - Gazebo model and world-building
  - Gazebo Plugins
  - URDF
  - RVIZ
  - C++

## Getting Started
To view this project, you must have Gazebo and ROS installed on Linux.

Following Instructions:

[ROS installation instructions](http://wiki.ros.org/ROS/Installation).

[Gazebo download and installation instructions](http://gazebosim.org).

With Gazebo and ROS installed, you first need to create a catkin workspace. Navigate to your home directory and execute:
```bash
$ mkdir -p catkin_ws/src
$ cd catkin_ws/src
$ catkin_init_workspace
```

Next, download/clone the repository and copy the ```my_robot``` and ```ball_chaser``` directories into the src directory:
```bash
$ git clone https://github.com/bmaxdk/RoboticsND-Go-Chase-It.git
$ cp -R RoboticsND-Go-Chase-It/my_robot RoboticsND-Go-Chase-It/ball_chaser .
$ rm -rf RoboticsND-Go-Chase-It
```

Then navigate up to the top-level catkin workspace directory and build the executables:
```bash
$ cd ..
$ catkin_make
```

Next, you can open Gazebo with the robot in it:
```bash
$ source devel/setup.bash
$ roslaunch my_robot world.launch
```

To make the robot chase the white ball, open a new terminal and execute the following:
```bash
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch
```

Now place the white ball at different positions in front of the robot and see if the robot is chasing the ball!
