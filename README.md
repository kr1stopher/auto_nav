# auto_nav
ROS node written in Python for autonomous navigation of the turtlebot3 in a simulated environment. The simulated environment used is Gazebo, and more information on turtlebot3 can be found at: https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/

This node utilizes the built-in lidar featured on the turtlebot3 to detect and avoid obstacles while driving through the simulated environment. Once launched the turtlebot3 will drive around the simulated environment going primarily forward, avoiding obstacles such as walls, pillars, etc. 

# Package Contents:

  auto_nav.py (primary file, in nodes folder)
  
  auto_nav.launch
  
  package.xml
  
  CMakeLists.txt
  
  setup.py
 
  changelog
  
  psuedocode
  
  
  
  
# Requirements:

  ROS (noetic), Gazebo, turtlebot3 packages (https://github.com/ROBOTIS-GIT/turtlebot3)
  
# Running:
  Launch turtlebot3 in simulated gazebo environment eg:
  
  Terminal 1:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ roscore 
    
  Terminal 2:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ TURTLEBOT3_MODEL='waffle
    
    $ roslaunch turtlebot3_gazebo turtlebot3_world.launch 
    
  Terminal 3:
  
    $ cd ~/catkin_ws
    
    $ source opt/ros/noetic/setup.bash
    
    $ source ./devel/setup.bash
    
    $ TURTLEBOT3_MODEL='waffle
    
    $ roslaunch auto_nav auto_nav.launch 
    
    
