## nav_bot
Autonomous Navigation of a 2 wheeled bot using ROS 

In this project, I have modelled a basic 2 wheeled bot structure using Fusion 360 and exported the CAD model into ros using a python script that converts ROS Fusion files into ROS packages which includes the basic launch files to launch the bot in Gazebo and Rviz. After which we model the environment for our bot to interact with.


Running the package 
Open up a terminal and give the following command

roslaunch New_bot_description gazebo.launch 

Now that the bot and envrionment are ready we can go ahead and launch the navigation file

roslaunch New_bot_description new_bot_nav.launch 
After launching, you need to use the 2D nav goal tool in Rviz and the bot will plan the path and avoid objects. 

NOTE: Please ignore Gazebo's warning of package names starting with a capital letter as it does not affect the performance of the bot. 
