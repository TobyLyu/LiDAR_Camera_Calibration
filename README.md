# LiDAR_Camera_Calibration
Autoware camera lidar calibrator extracted from the [autoware_ai_utilities](https://github.com/autowarefoundation/autoware_ai_utilities/tree/master/autoware_camera_lidar_calibrator)
Tested on Ubuntu 20.04 with ROS Noetic

Dependence Packages from Autoware:
- [autoware_build_flags](https://github.com/autowarefoundation/autoware_ai_common/tree/master/autoware_build_flags)
- [autoware_msgs](https://github.com/AbangLZU/Autoware/tree/master/ros/src/msgs/autoware_msgs)
- [calibration_publisher](https://github.com/AbangLZU/Autoware/tree/master/ros/src/sensing/fusion/packages/calibration_publisher)
- [image_processor](https://github.com/AbangLZU/Autoware/tree/master/ros/src/sensing/filters/packages/image_processor)

## Preparation
### Install Dependence Packages
```
sudo apt-get install ros-noetic-jsk-common
sudo apt-get install ros-noetic-jsk-recognition
```
### Prepare Required data
Intrinsic parameter of camera is needed.

## How to use
1. Launch `roslaunch autoware_camera_lidar_calibrator camera_lidar_calibration.launch` (modify the launch file with proper input topics and intrinsic file)
2. Play the rosbag.
3. For the image, click on the image_view2 windows ONCE (do not drag).
4. For the point cloud, use `Publish Point` to click the corresponding point.
5. One point in image, followed by one point in point cloud.