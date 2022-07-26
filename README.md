# second task -with-edit
## install-arduino-robot-arm
```
its divided into three stages

```
## First stage (Install_arduino_robot_Arm)  ##

## 1- add the (arduino robot arm) packge to the (src) folder :
```
$cd ~/catkin_ws/src

$sudo apt install git

$git clone https://github.com/smart-methoods/arduino_robot_arm.git
```
## 2-(Install and initilzie rosdep)
 ```
 $ sudo apt install python3-rosdep2
 $ rosdep install --from-paths src --ignore-src -r -y
```


## 3- (Dependencies)
```

if use noetic distro

```
```
$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
```

## 4- write this command (sudo nano ~/.bashrc)
```
then go to the last line and write (source /home/your name/catkin_ws/devel/setup.bash)with your name
```
## second stage (Install arduino) ##
## 1- (download Arduino IDE in Ubuntu https://www.arduino.cc/en/software) :
```
then write this commands:

$ sudo apt update
$ mkdir arduino
$ cd arduino/
$ wget https://downloads.arduino.cc/arduino-1.8.15-linux64.tar.xz
$ cd arduino-1.8.15/
$ sudo ./install.sh
```
## 2- (Install rosserial):
```
write this commands:

$ sudo apt-get install ros-noetic-rosserial-arduino
$ sudo apt-get install ros-noetic-rosserial
```
## 3- Install ros_lib
```
go to the arduino file right click and select the terminal 

then type the following commands:
 ```
  ```
$ cd libraries
$ rosrun rosserial_arduino make_libraries.py
 ```

## Thired stage (Launch for the package arm) ##
```
1- launch RViz

$ roslaunch robot_Arm_pkg check_motors.launch 

2-lanuch gazebo

$ roslaunch robot_Arm_pkg check_motors_gazebo.launch

```
 
## my results ## 
<![Screenshot from 2022-07-25 15-47-56](https://user-images.githubusercontent.com/108955178/180866447-62f5f458-b5a5-4b4b-ba3d-8b65f9bd36f7.png)
>
<![Screenshot from 2022-07-25 15-43-10](https://user-images.githubusercontent.com/108955178/180866667-983bbde7-f404-4666-a365-dcc30d400856.png)
>
<![Screenshot from 2022-07-25 15-10-38](https://user-images.githubusercontent.com/108955178/180866765-f04cefce-d32a-471a-805a-a1b899ff67d5.png)
>
<![Screenshot from 2022-07-25 15-42-51](https://user-images.githubusercontent.com/108955178/180866870-d239ff1a-83be-47e6-9a2e-aa727ceab9e7.png)
>
<![Screenshot from 2022-07-25 15-47-42](https://user-images.githubusercontent.com/108955178/180866959-a9f721f6-8669-458e-881e-3ca8638dbedc.png)
>
<![Screenshot from 2022-07-25 15-26-56](https://user-images.githubusercontent.com/108955178/180867077-e731ecea-b7f2-4adb-a5eb-59d30f0d987a.png)

<![83863](https://user-images.githubusercontent.com/108955178/180867987-0f2e0cca-7103-43cf-97db-30b839a8df4d.jpg)




 


 



