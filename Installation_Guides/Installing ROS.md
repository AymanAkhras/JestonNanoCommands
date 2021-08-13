### Installation to ROS  ON THE JESTON NANO 

Github Repository used: https://github.com/JetsonHacksNano/installROS

> git clone https://github.com/JetsonHacksNano/installROS
Cd into the file directory 
> cd installROS/
> ./installROS.sh -p ros-melodic-desktop

##### What is CATKIN? 
- It's is workspace is a folder where you modify, build, and. install catkin packages. 

##### CATKIN SETUP 

> cd installROS/
> ./setupCatkinWorkspace.sh

To create a ROS_MASTER_URI AND ROS_IP. You must change the values in the bashrc script. 
- Scroll down to the bottom where you will find a localhost: ##### 
- Scroll down to the bottom where you will find a ROS_IP: ##### 
- Change those to match your Personal Device
- Local host should match the port number
- ROS_IP should match the ip of the machine 

##### Check the installation is Complete 
> command gedit ~/.bashrc
> roscore
> rostopic list

- Should output the following below:  
- /rosout
- /rosout-agg
