#first Launch Simulation World
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_gazebo turtlebot3_world.launch
#next Run Navigation Node
export TURTLEBOT3_MODEL=burger
roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml
#next Estimate Initial Pose
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
#the last Set Navigation Goal
Click the 2D Nav Goal button in the RViz menu.
Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.

<img width="1016" alt="Screen Shot 1442-11-30 at 10 02 44 PM" src="https://user-images.githubusercontent.com/56722657/125206883-12983680-e292-11eb-86b9-cb0d5adb01bd.png">
