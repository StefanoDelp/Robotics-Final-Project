# Robotics-Final-Project
Robotics Final Project

To run the maze put the Explore folder in catkin/src
do a catkin make 

open a terminal and run these commands (you also need to source and set turtulebot for every new terminal)
export TURTLEBOT3_MODEL=waffle_pi && source ~/catkin_ws/devel/setup.bash

roslaunch turtlebot3_gazebo turtlebot3_FinalMaze.launch

roslaunch turtlebot3_slam turtlebot3_slam.launch slam_method:=gmapping

roslaunch turtlebot3_navigation move_base.launch 

roslaunch explore_lite explore.launch
