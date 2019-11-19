# GIT Preparing, Not Complete  

## Description 
Open manipulator application pacakges.   
2019 R-BIZ ROBOTIS Open Manipulator Challenge.   
Auturbo team potman   

## HW Block Diagram 
<img src="/picture/1.PNG" width="100%" height="100%">  


## SW Block Diagram 
<img src="/picture/2.PNG" width="100%" height="100%">  

## PC Setting  
1. 
```bash
```

## First Phone Setting to voicecommand 

## Second Phone Setting to facetracking   


## PC Run 
```bash
roslaunch open_manipulator_controller open_manipulator_controller.launch
roslaunch open_manipulator_potman yolo_jsk_pose.launch camera_model:=realsense_d435
roslaunch open_manipulator_potman potman.launch
roslaunch open_manipulator_potman key_command.launch
```

## First Phone Run

## First Phone Run

## Operation Mode 

There is 9 mode, You can control by PC( terminal of key_command.launch ) or phone ( voice control or button )   
### 0. Start Pour
Click image to link to YouTube video.   
[![Video Label](http://img.youtube.com/vi/TuQmHOsT_p8/0.jpg)](https://youtu.be/TuQmHOsT_p8?t=0s)    

### 1. Start cheers ( Picking cup & Cup tracking )
Click image to link to YouTube video.   
[![Video Label](http://img.youtube.com/vi/rtBZDF8icJw/0.jpg)](https://youtu.be/rtBZDF8icJw?t=0s)   
[![Video Label](http://img.youtube.com/vi/esYlpivZYQo/0.jpg)](https://youtu.be/esYlpivZYQo?t=0s)   

### 2. Stop cheers ( Realease Cup )   
### 3. Serve Food    
Click image to link to YouTube video.   
[![Video Label](http://img.youtube.com/vi/dL8CXf71Wz4/0.jpg)](https://youtu.be/dL8CXf71Wz4?t=0s)   
[![Video Label](http://img.youtube.com/vi/Kr8EuuMiMAU/0.jpg)](https://youtu.be/Kr8EuuMiMAU?t=0s)   

### 4. Start Phone ( PICKING phone & face tracking )   
Click image to link to YouTube video.   
[![Video Label](http://img.youtube.com/vi/hsZrGeCw8Zo/0.jpg)](https://youtu.be/hsZrGeCw8Zo?t=0s)   

### 5. Stop Phone ( Realease Phone )   
### 6. Stop    
### 7. Restart    
### 8. Panorama Shot    

## Run Gazebo ( PC Side ) 
```bash
roslaunch open_manipulator_gazebo open_manipulator_gazebo_potman.launch
roslaunch open_manipulator_controller open_manipulator_controller.launch use_platform:=false
roslaunch open_manipulator_potman yolo_jsk_pose.launch camera_model:=realsense_d435 use_platform:=false
roslaunch open_manipulator_potman potman.launch use_platform:=false
roslaunch open_manipulator_potman key_command.launch
``` 
Click image to link to YouTube video.   
[![Video Label](http://img.youtube.com/vi/u4CAUhD-lkU/0.jpg)](https://youtu.be/u4CAUhD-lkU?t=0s)  

## How to make movement file ( fixed movement by file )  
0. Start Pour and 3. Serve Food  is fixed movement by file.   
0. Start Pour use https://github.com/minwoominwoominwoo7/open_manipulator_potman/blob/master/cfg/output_pour.txt   
3. Serve Food use https://github.com/minwoominwoominwoo7/open_manipulator_potman/blob/master/cfg/output_serve.txt   
you can make movement file by open_manipulator_save_and_load   
https://github.com/minwoominwoominwoo7/open_manipulator_save_and_load   

[![Video Label](http://img.youtube.com/vi/PH-7JwGH9uM/0.jpg)](https://youtu.be/PH-7JwGH9uM?t=0s)    

