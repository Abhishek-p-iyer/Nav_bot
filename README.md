# Autonomous Navigation of a 2 wheeled bot using ROS


In this project, I have modelled a basic 2 wheeled bot structure using Fusion 360 and exported the CAD model into ros using a python script that converts ROS Fusion files into ROS packages which includes the basic launch files to launch the bot in Gazebo and Rviz. After which we model the environment for our bot to interact with.

Running the package 

Open up a terminal and give the following command



Step-1: Run catkin_make in your terminal 

```
<ROS_workspace_location>$catkin_make
```

Open up another terminal and execute the following command 

Step-2: Launching the bot into Gazebo

```
$roslaunch New_bot_description gazebo.launch
```

![gazebo](https://user-images.githubusercontent.com/67633494/148681401-9867a560-8426-4735-a6a6-0d683127e403.png)


Step-3: Launching all the necessary navigation files

```
$roslaunch New_bot_description new_bot_nav.launch
```

![2nd](https://user-images.githubusercontent.com/67633494/148681587-3b76f35e-c3fd-489e-9c02-5a868303c906.png)


After launching, you need to use the 2D nav goal tool in Rviz and the bot will plan the path and avoid objects. 

![3rd](https://user-images.githubusercontent.com/67633494/148681745-8015f411-48e5-4c75-997c-ed010cfddc34.png)
  

NOTE: Please ignore Gazebo's warning of package names starting with a capital letter as it does not affect the performance of the bot. 

