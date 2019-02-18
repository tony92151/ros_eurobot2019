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

> cp -R atom* ~/.gazebo/models/

and compile

## Launch field

launch field without atoms

> roslaunch eurobot2019 gazebo.launch

launch field with atoms

> roslaunch eurobot2019 gazebo_field_only.launch
