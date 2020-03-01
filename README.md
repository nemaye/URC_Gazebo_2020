# The Ultimate Gazebo Workspace - rhinoceROS #

## Contents: 

[realsense_gazebo_plugin](https://github.com/marsrovermanipal/URC_Gazebo_2020/tree/master/rhinoceROS/src/realsense_gazebo_plugin) - A package containing a mutlipurpose differential drive robot equipped with IntelRealSense, LIDAR, Ultrasonics, GPS, IMU, Magnetometer and a pair of cameras.
![default_gzclient_camera(1)-2020-03-01T10_31_13 704653](https://user-images.githubusercontent.com/45683974/75619976-046bdd80-5ba9-11ea-8aa8-0c2a41eddb12.jpg)


[rover_sensors_final](https://github.com/marsrovermanipal/URC_Gazebo_2020/tree/master/rhinoceROS/src/rover_sensors_final) - A package containing containing the fully functional rover of Mars Rover Manipal team of University Rover Challenge 2020. 
![default_gzclient_camera(1)-2020-03-01T10_16_08 118908](https://user-images.githubusercontent.com/45683974/75619859-4e53c400-5ba7-11ea-9be7-b6258e59b31d.jpg)


Installation
------------

Install git-lfs using apt-get:

    sudo apt-get install git-lfs

Clone using git lfs:

    git lfs clone https://github.com/marsrovermanipal/URC_Gazebo_2020.git

Run a catkin make in the rhinoceROS folder:

    catkin_make

Source the bash script in the devel folder in rhinoceROS:

    source ~/URC_Gazebo_2020/rhinoceROS/devel/setup.bash
    
For basic bot simulation:

    roslaunch realsense_gazebo_plugin spawn_my_bot.launch

For complete rover simulation:

    roslaunch rover_sensors_final gazebo.launch


Errors
------------
-- 1) Run the following command if the LED Matrix does not glow red: 

    sudo apt-get install ros-melodic-gazebo-* && sudo apt-get install gazebo9 && sudo apt-get install libgazebo9* && sudo apt-get --reinstall install libignition-math4 && sudo apt-get --reinstall install libignition-math4-dev && sudo apt-get upgrade
    
-- 2) Run the following command if the GPS and IMU sensors values are not seen through a rostopic list: 

    sudo apt-get install ros-melodic-hector-gazebo-plugins

-- 3) In case if you don't have the ROS package ar track alvar: 

    sudo apt-get install ros-melodic-ar-track-alvar

    

