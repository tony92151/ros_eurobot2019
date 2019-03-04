# eurobot2019

official wedsite
http://www.eurobot.org/eurobot/eurobot-2019


<img src="https://github.com/tony92151/ros_eurobot2019/blob/master/image/gazebo3.jpg"/>

<img src="https://github.com/tony92151/ros_eurobot2019/blob/master/image/gazebo.gif"/>
<img src="https://github.com/tony92151/ros_eurobot2019/blob/master/image/gazebo2.gif"/>


## Starup setting

> cd ~/catkin_ws/src

> git clone https://github.com/tony92151/ros_eurobot2019.git

> cd ~/catkin_ws/src/ros_eurobot2019/models

> cp -R * ~/.gazebo/models/

and compile

## Launch field

launch field without atoms

> roslaunch eurobot2019 gazebo.launch

launch field with atoms

> roslaunch eurobot2019 gazebo_field_only.launch

### 機器人構想

1. mapping：
   1. depth to laser： 
    http://wiki.ros.org/depthimage_to_laserscan
    因為場地圍牆高度較低，若只取一直線之深度會有超出範圍之危險；必須計算高度後，取某一高度之深度值當圍牆
   2. rtabmap：
   使用depth camera做mapping & navigation
        
2. opencv shift object detect
    偵測atom位置
    http://wiki.ros.org/object_recognition
    https://docs.opencv.org/3.4/d1/de0/tutorial_py_feature_homography.html

3. infinite state machine:
   使機器人做出決策，fuzzy control
4. mpc controller模型預測控制
   




