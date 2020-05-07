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

# Human Trials

To run the maze:

	roslaunch turtlebot3_gazebo turtlebot3_FinalMaze.launch

To run Rviz:

	roslaunch turtlebot3_slam turtlebot3_slam.launch slam_method:=gmapping

** Turn off laser sensor and map and allow camera feed to be displayed by pressing "add" at the bottom left of RVIZ GUI,
** going into the "By Topic" tab, selecting /camera/rgb/image_raw/camera, then pressing "OK". Drag the window and expand 
** to make it easier to see.

To run teleop:

	roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

Then time the user on how long it takes them to find the exit out of the map
