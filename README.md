# Camera Pose Estimation (Checkerboard and Natural features)
Detect a checkerboard in a camera frame

Estimate the camera pose relative to said checkerboard

Detect features around the checkerboard

While moving the camera around the checkerboard create a 3D pointcloud and descriptors of the surrounding features

After a couple seconds, localize the camera from the natural features, i.e., detect features in a camera frame, match them with the pointcloud, and estimate the camera pose (do not use the checkerboard!)

Compare the estimated camera pose from natural features with pose estimation from a checkerboard

Continue tracking the camera even when the checkerboard is not visible, while adding additional features to the database

# Environment 
python==3.6  
numpy==1.16.4  
opencv==4.1.0  
matplotlib==2.2.2  

# How to run
0. Calibrate camera using camera_calibration.py
1. Put 9*6 checkerboard in the range of webcam
2. Run capture_video.py to take video-file which focus on the checkerboard as the training dataset
3. Take video around the checkerboard
4. Push key "q" on the opencv-popup-window
5. Run pose_estimator.py

# Result
You can see the error of the estimated camera-poses between the pose based on checkerboard adn the pose based on natural-feature.
![an example of result](https://github.com/liupeiming600/Camera-Pose-Estimation/result.PNG "result")
