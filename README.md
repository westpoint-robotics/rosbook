# rosbook
This repository contains example code to accompany the book [Programming Robots with ROS](http://www.amazon.com/Programming-Robots-ROS-Practical-Introduction/dp/1449323898/ref=sr_1_1?ie=UTF8&qid=1453484937&sr=8-1)

# Followbot Instructions
1. Install OpenCV dependecies.
2. Clone rosbook
 - `cd ~/catkin_ws/src`
 - `git clone https://github.com/westpoint-robotics/usma_mavros`
3. Build
 - `cd ~/catkin_ws/`
 - `catkin_make -DMAVLINK_DIALECT=common`
4. Configure mavros on computer:
 - In `px4.launch`, 
  - The computer is connecting through `ttyUSB0:921600` instead of `ttyACM0:57600`.
  - Chage the `gcs_url` argument default to `default="udp://:14556@192.168.XX.XX:14550"` to match the IP of the ground control station.
  - QGC can connect to the autopilot using the Default UDP link.  
5. Execute mavros
 - `roslaunch usma_mavros px4.launch`
 - Check that there is a heartbeat with the PX4. 
 - `[INFO] [1573276705.686808500]: CON: Got HEARTBEAT, connected. FCU: ArduPilot`
 
----- Need to update indoor operations and below ------




### Errata
We are grateful to the readers who have found and reported errata in the book. There is an [official Errata page](http://www.oreilly.com/catalog/errata.csp?isbn=0636920024736) on the O'Reilly website which lists the known errata in the printed book. The code available in this Github repo has the errata corrected, and therefore may be slightly different from the code listings provided in the book.
