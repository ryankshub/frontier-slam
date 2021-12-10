# Navigation Package: Explore the Unknown

Author and Maintainer: **Ryan King-Shepard**

## **Description**

This package contains:

- nodes:
    
- config:
     
- launch 
   
- srv
    
- `package.xml`
    * Package configuration
- `CMakeLists.tx`
    * Build configuration
- test
    
- worlds
  
- `README.md`
    * Now in HD!


## **Dependencies and Installation**

### *ROS Dependencies*
This package was developed and tested in ros-noetic. ros_navi was designed and built using catkin. This package also requires the turtlesim package to run. This should usually come with your ros installation, but to check this run: 

This should result a little screen with a turtle in the center. If the window doesn't pop up, refer to [ROS wiki](http://wiki.ros.org) to install turtlesim on your machine.

The full list of ros package dependencies can be found in `package.xml`. Two big dependencies to note are the interbotix_xsarm_moveit and the moveit packages. To set up the proper environment, do the following:
1. Set up your moveit_ws; run `catkin_make` and `source devel/setup.[terminal_file]` where terminal_file is the type of terminal you are running (e.g bash). Instructions to assist with moveit can be found [here](https://ros-planning.github.io/moveit_tutorials/doc/getting_started/getting_started.html)
2. Set up a custom_ws with [interbotix](https://github.com/Interbotix/interbotix_ros_manipulators) and `catkin_make` and `source devel/setup.[terminal_file]` for the *interbotix_xasrm_moveit* package.
3. Ensure that you have the other dependencies found in `package.xml`.

### *Python Dependencies*
All code for this package was developed and test in Python 3 (specfically 3-8-10).  
This package requires `numpy` in order to run. The version used was 1-17.4, however there is no 
strong attachment to this version; other versions should work fine as long as they compatitble with
the python version. Refer to [Numpy docs](https://numpy.org/install/) for installation information. 

## **Execution**





