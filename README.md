# Sensor Fusion course - 1st Project - Lidar Obstacle Detection

### Lidar Principle

**Lidar** sensing gives us high resolution data by sending out thousands of laser signals. These lasers bounce off objects, returning to the sensor where we can then determine how far away objects are by timing how long it takes for the signal to return. Also we can tell a little bit about the object that was hit by measuring the intesity of the returned signal. Each laser ray is in the infrared spectrum, and is sent out at many different angles, usually in a 360 degree range. While lidar sensors gives us very high accurate models for the world around us in 3D, they are currently very expensive, upwards of $60,000 for a standard unit.

### Project Description

* Detection of other cars on the road using raw Lidar data from Udacity's real self-driving car.
* Implementation of 3D Ransac for segmentation and Clustering executed by Euclidean Clustering Algorithm along with KD-Tree.
* Bounding boxes used for obstacles (cars) detection.

### My Result

* Perspective View 
* <image src= "https://github.com/Srivaths-V/Lidar-Obstacle-Detection/blob/main/Lidar%20result.gif" width = "700" />

* Side View 
* <image src= "https://github.com/Srivaths-V/Lidar-Obstacle-Detection/blob/main/Lidar%20side%20view.gif" width = "700" />
 
### Dependencies
* cmake >= 2.8
* All OSes: click for installation instructions - https://cmake.org/install/
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
* Linux: make is installed by default on most Linux distros
* Mac: install Xcode command line tools to get make - https://developer.apple.com/xcode/features/
* Windows: Click here for installation instructions - http://gnuwin32.sourceforge.net/packages/make.htm
* PCL, C++
* The link here is very helpful, https://larrylisky.com/2014/03/03/installing-pcl-on-ubuntu/
* gcc/g++ >= 5.4
* Linux: gcc / g++ is installed by default on most Linux distros
* Mac: same deal as make - install Xcode command line tools - https://developer.apple.com/xcode/features/
* Windows: recommend using MinGW

### Linux Ubuntu 16

Install PCL, C++

The link here is very helpful, 
https://larrylisky.com/2014/03/03/installing-pcl-on-ubuntu/

A few updates to the instructions above were needed.

* libvtk needed to be updated to libvtk6-dev instead of (libvtk5-dev). The linker was having trouble locating libvtk5-dev while building, but this might not be a problem for everyone.

* BUILD_visualization needed to be manually turned on, this link shows you how to do that,
http://www.pointclouds.org/documentation/tutorials/building_pcl.php

