# The Ultimate Gazebo Workspace - rhinoceROS #

## Contents: 

[realsense_gazebo_plugin](https://github.com/marsrovermanipal/URC_Gazebo_2020/tree/master/rhinoceROS/src/realsense_gazebo_plugin) - A package containing a mutlipurpose differential drive robot equipped with IntelRealSense, LIDAR, Ultrasonics, GPS, IMU, Magnetometer and a pair of cameras.


[rover_sensors_final](https://github.com/marsrovermanipal/URC_Gazebo_2020/tree/master/rhinoceROS/src/rover_sensors_final) - A package containing containing the fully functional rover of Mars Rover Manipal team of University Rover Challenge 2020. 


Installation
------------

Install git-lfs using apt-get:

    sudo apt-get install git-lfs

Run a catkin make in the rhinoceROS folder:

    catkin_make
    
For basic bot simulation:

    roslaunch realsense_gazebo_plugin spawn_my_bot.launch

For complete rover simulation:

    roslaunch rover_sensors_final gazebo.launch
    

