# Voice-ontrolled-Robot

control any ros robot with voice and gui commnad

### voice commander app 
https://play.google.com/store/apps/details?id=com.jrlandau.robotcmdr  

## Build your custom robot or use ROS based robot eg.Turtlebot--etc

For this simulation Install all necessary packages for Turtle_bot3 from 

https://emanual.robotis.com/docs/en/platform/turtlebot3/simulation/#ros-1-simulation  folow along for installation

launch turtlebot using this commnad in terminal

$ `<roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch>`

### Install Rosbridge server using 
$ `<sudo apt-get install ros-<rosdistro>-rosbridge-server>`

##### Editing rosbridge webserver 
Find rosbridge_server package inside opt/ros/<distro>/share make sure the arguements follow below for security less information transfers
  
<arg name="ssl" default="false" />
<arg name="certfile" default="" />
<arg name="keyfile" default="" /> 

##### cured and detailed server building follow

https://github.com/UbiquityRobotics/speech_commands


Cofigure the newtwork of the robot Master uri run the rosbridge connect using the app by inserting your robotip in robotcommander app
use 
$ `<echo $ROS_MASTER_URI>` to find the robot ip adress


