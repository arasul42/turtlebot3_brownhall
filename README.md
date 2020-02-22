# turtlebot3_navigation

This is a ROS package for navigation and simulation with Turtlebot3

ROS - The Turtlebot Simulator
ME 4140 - Introduction to Robotics - Fall 2019
1. Update your linux system before you get started.
sudo apt-get update
2. Install the necessary nodes into your ROS system. This tutorial comes from here.
turtlebot3
sudo apt-get install ros-melodic-turtlebot3
turtlebot3_simulations
sudo apt-get install ros-melodic-turtlebot3-simulations
turtlebot3_gazebo
sudo apt-get install ros-melodic-turtlebot3-gazebo
1ME 4140 Fall 2019—The Robotic Operating System
2
3. Test the simulator. First set the environment variable TURTLEBOT_MODEL. Add
this line to the .bashrc script so you do not have to do it for each terminal.
export TURTLEBOT3_MODEL=burger
Then turn on the simulator.
roslaunch turtlebot3_gazebo turtlebot3_world.launch
You should see the gazebo window open containing your robot. Test that the keyboard
drives the robot. This may take some time.
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
4. Now turn on the node to produce robot data in the simulated world.
roslaunch turtlebot3_gazebo turtlebot3_simulation.launch
Open RVIZ to view the data. This is a very useful tool.
roslaunch turtlebot3_gazebo turtlebot3_gazebo_rviz.launch
5. Next we are going to learn about SLAM and GMAPPING ! Please see the tutorial
referenced above if you are ready to proceed.
