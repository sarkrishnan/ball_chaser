# ball_chaser
This is a project I made for the Robotics Software Engineer Nanodegree from Udacity. This project involved creating a gazebo world (please check my [gazebo_world repository](https://github.com/sarkrishnan/gazebo_world "Aravinda's gazebo world github repository"), adding a differential drive robot using URDF and making the robot chase a white colored ball with the building (in the gazebo world).

# Quickstart

## Requirement

Please install [**__ROS Kinetic__**](http://wiki.ros.org/kinetic/Installation "ROS Kinetic Installation") (choose your platform. I have used Ubuntu which is ROS supported/recommended platform)

## Building the project

Create a new catkin workspace (generally named as catkin_ws) and a src folder within it . Example `mkdir -p catkin_ws\src`. (new catkin workspace is preferred in order to avoid conflicts with other existing catkin repositories)

Navigate into the src folder. `cd catkin_ws\src` and run the `catkin_init_workspace` command to initialize the catkin workspace. 

Clone the project into the src folder. `git clone https://github.com/sarkrishnan/ball_chaser.git`

Navigate into the catkin workspace. `cd catkin_ws` and run `catkin_make` command to build the ball_chaser repository

## Running the ball chaser

After successful build, source the setup file. `source devel/setup.bash` (Here I have assumed that you are at the top of the catkin_ws meaning if you run `pwd` command it would show __../catkin_ws__

Run `roslaunch ball_chaser ball_chaser.launch` to open the gazebo world with the differential drive robot. 

Move the ball from outside the building into the view of the Robot. (The camera is red colored). The robot will start to move towards the ball. Congratulations. 

## Suggestions for tinkering with the code

Change the color of the ball and save the gazebo world. Now, change the ball chaser image processing code to chase a different colored ball. 

