# LiDAR_Camera_Calibration
Autoware camera lidar calibrator extracted from the [autoware_ai_utilities](https://github.com/autowarefoundation/autoware_ai_utilities/tree/master/autoware_camera_lidar_calibrator)

Dependence Packages:
- [autoware_build_flags](https://github.com/autowarefoundation/autoware_ai_common/tree/master/autoware_build_flags)
- [calibration_publisher](https://github.com/AbangLZU/Autoware/tree/master/ros/src/sensing/fusion/packages/calibration_publisher)
- [image_processor](https://github.com/AbangLZU/Autoware/tree/master/ros/src/sensing/filters/packages/image_processor)
- [image_view2](https://github.com/jsk-ros-pkg/jsk_common/tree/master/jsk_ros_patch/image_view2)

## How to use
1. Launch `roslaunch autoware_camera_lidar_calibrator camera_lidar_calibration.launch` (modify the launch file with proper input topics)
2. For the image, click on the image_view2