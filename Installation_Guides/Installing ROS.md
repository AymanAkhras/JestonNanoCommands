<h1 align="center">
Installing ROS
</h1> 


#### To get ROS on the Jeston Nano the following setups must be taken: 

Github repository used:  https://github.com/JetsonHacksNano/installROS

##### Step 1: Clone the following Repo
```
git clone https://github.com/JetsonHacksNano/installROS
cd installROS/
./installROS.sh -p ros-melodic-desktop
```

##### Step 2: Catkin Setup

It's workspace is a folder where you modify, build, and. install catkin packages. 
```
./setupCatkinWorkspace.sh
```
To create a ROS_MASTER_URI AND ROS_IP. You must change the values in the bashrc script. 
```
command gedit ~/.bashrc
 ```
* Local host should match the port number
* ROS_IP should match the ip of the machine 

##### Step 3: Upon fixing those two values write the command:
```
source ~/.bashrc
```
open up a new terminal 
```
roscore
rostopic list
```
If it prints /rosout & /rosout_agg the installation is complete. 
