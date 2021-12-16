# heyrobo
Teleoperation and Autonomous navigation of a 2 wheeled mobile robot using ros is performed here.
The ros version `noetic` is used here. Change the keyword `noetic` as per which ros version you're using.


#### In-order to launch the robot in gazebo and rviz type these commands in terminal
* `roslaunch heyrobo_description gazebo.launch`
* `roslaunch heyrobo_description display.launch`
#### In-order to teleoperate the mobile robot
* `sudo apt-get install ros-noetic-teleop-twist-keyboard`
* `rosrun teleop_twist_keyboard teleop_twist_keyboard.py`
#### Mapping
* `sudo apt-get install ros-noetic-gmapping`
* `rosrun gmapping slam_gmapping`
#### To save the generated map
* `sudo apt-get install ros-noetic-map-server`
* `rosrun map_server map_saver -f filename`
#### download the dependencies for the parameters to run
* `sudo apt-get install ros-noetic-amcl`
* `sudo apt-get install ros-noetic-move-base`
* `sudo apt-get install ros-noetic-dwa-local-planner`
#### To perform Navigation 
* `roslaunch heyrobo_navigation heyrobo_navigation.launch`
