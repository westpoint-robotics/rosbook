# rosbook
This repository contains example code to accompany the book [Programming Robots with ROS](http://www.amazon.com/Programming-Robots-ROS-Practical-Introduction/dp/1449323898/ref=sr_1_1?ie=UTF8&qid=1453484937&sr=8-1)

# Followbot Instructions
1. Install OpenCV dependecies (if required).
2. Clone rosbook
 - `cd ~/catkin_ws/src`
 - `git clone https://github.com/westpoint-robotics/rosbook.git`
3. Build
 - `cd ~/catkin_ws/`
 - `catkin_make`
4. Export the waffle_pi model in your .bashrc 
5. Launch the Gazebo line follower world
- `roslaunch followbot followbot.launch`
