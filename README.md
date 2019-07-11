# task1
Detect a checkerboard in a camera frame

Estimate the camera pose relative to said checkerboard

Detect features around the checkerboard

While moving the camera around the checkerboard create a 3D pointcloud and descriptors of the surrounding features

After a couple seconds, localize the camera from the natural features, i.e., detect features in a camera frame, match them with the pointcloud, and estimate the camera pose (do not use the checkerboard!)

Compare the estimated camera pose from natural features with pose estimation from a checkerboard

Continue tracking the camera even when the checkerboard is not visible, while adding additional features to the database
