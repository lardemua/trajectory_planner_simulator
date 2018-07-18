# trajectory_planner_simulator
Master thesis local navagation simulator meta-package. 
This mate-package contains all the packages and Ackermann steer link controllers to simulate a car like robot in Gazebo.

## Getting Started

Instructions install the the software.

### Prerequisites

You need to install the ROS Kinect and Gazebo.

### Installing

Download the meta-package and compile it in a catkin_make workspace.

## Running

### Subscribed topics

* /cmd_vel(geometry_msgs::Twist) - Linear and angular velocity.

### Published topics

* /simulator_laser_scan(sensor_msgs::LaserScan) - Physical obstacles' laser scan.
* /line_pcl(sensor_msgs::LaserScan) - Center line's laser scan.
* /reduced_pcl(sensor_msgs::PointCloud2) - Physical obstacles' point cloud.
* /line_pcl(sensor_msgs::PointCloud2) - Center line's point cloud.

### Running Gazebo simulator

ROS launch command.

```
roslaunch cirkit_unit03_gazebo ackermann_vehicle_simulator.launch 
```

## Built With

* [CIR-KIT-Unit03](https://github.com/CIR-KIT-Unit03) - Controller and robot framework used.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
