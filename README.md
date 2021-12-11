# Navigation Package: Explore the Unknown

Author and Maintainer: **Ryan King-Shepard**

## **Description**

This package contains:

- nodes:
    1. `explorer` ~ 
        Contains logic driving robot toward exploration. Uses a combination of frontier exploration and random walk to explore the space and produce a map   
- launch:
    - `start_slam.launch` ~ 
        Launches gazebo and rviz simulation with keyboard control of the robot to show slam
    - `nav_stack.launch` ~ 
        Launches gazebo and rviz simulation with custom map to explore with amcl localization. Allows for robot setting goal point with rviz 2D Nav goal
    - `slam_stack.launch` ~ 
        Launches gazebo and rviz with slam toolbox and nav stack. Allows for robot setting goal point with rviz 2D Nav goal
    - `frontier_exp.launch` ~
        Launches gazebo and rviz with slam toolbox and nav stack. Robot maps house with frontier exploration and random walk hybrid control.
- `map_gazebo.pgm` ~
    Example map image produced from keyboard operation of robot
- `map_gazebo.yaml` ~
    Example map image configuration from keyboard operation of robot
- `expl.pgm` ~
    Example map image produced from automated exploration. Note due to some dwa planner errors, the robot has trouble at certain locations
- `expl.yaml` ~
    Example map image configuration from automated exploration
- `package.xml`
    * Package configuration
- `CMakeLists.tx`
    * Build configuration
- `README.md`
    * Now in HD!


## **Dependencies and Installation**

### *ROS Dependencies*
This package was developed and tested in ros-noetic. Package ros_navi was designed and built using catkin. This package also requires the turtlebot3, turtlebot3_simulations, slam toolbox, and dwa local planner packages package to run. The full list of ros package dependencies can be found in `package.xml`. 

### *Python Dependencies*
All code for this package was developed and test in Python 3 (specfically 3-8-10).  
This package requires `numpy` in order to run. The version used was 1-17.4, however there is no 
strong attachment to this version; other versions should work fine as long as they compatitble with
the python version. Refer to [Numpy docs](https://numpy.org/install/) for installation information. 

This package requires `open_cv2` in order to run. Refer to the [OpenCv docs](https://docs.opencv.org/4.5.4/index.html)

## **Execution**

To run the robot with frontier exploration, use the command file `roslaunch ros_navi frontier_exp.launch`. 

To run only the gazebo and rviz to use the 2D Nav Goal to guide the robot, use the command `roslaunch ros_navi slam_stack.launch`.

To run only the navigation stack and use the 2D Nav Goal to gudie the robot, use the command `roslaunch ros_navi nav_stack.launch`


