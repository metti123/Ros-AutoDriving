# ROS-AutoDriving

## Introduction to Creative Engineering Design AD Project(class-02-group 5)

### Autonomous vehicles

### 1.lane recognition using  OpenCV <br>
Uses IMU sensors to accelerate up and down

### 2.recognizes and Avoids obstacles: <br>
![avoid_obstacle](https://user-images.githubusercontent.com/54922683/116533912-e0c33500-a91c-11eb-8138-b147b1877149.gif)<br><br>
uses ultrasonic waves to recognize an obstacle<br>
step 1-Locate Obstacle-Free Directions <br>
step 2-Driving in that direction<br>
step 3-Return when the obstacle is cleared.<br><br>

-Using lane recognition algorithms, it determines direction through the difference between the mean of left and right to the center of the image from the camera.<br>
-If there's an obstacle on the left, adjust the right to 480 else, adjust the left to 160.<br><br>

### 3.recognizes obstacles and slows down then stops 30cm away: <br>

### 4.recognizes traffic lights and stops: <br>
Uses usb_cam and open cv. recognizes red circle using Hough Circle and stops when the circle is found.<br>
1.Replace self.isStop value with True if circle found(linedetector.py)<br>
2.if self.isStop is TRUE then LineDetector.Stop value will be changed to True as well which leads to the self-driving car to stop. (autodrive.py)<br><br>


#### self driving(lane detection and stops after a full circle) video link: https://youtu.be/pOI2LmDWan8 <br>
#### Avoid obstacles video link: https://youtu.be/H6NFf2J4Vlw <br>
#### Stop after recognizing traffic lights video link: https://youtu.be/mEHLbnFlSdU <br>
#### recognizes obstacle and stops(30cm away) video link: https://youtu.be/zwvPO03l2jA <br>





