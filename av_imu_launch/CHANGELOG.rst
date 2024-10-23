^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package av_imu_launch
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.0.0 (2024-10-23)
------------------
* Add rear imu to launch
  - Append mount location to imu topics namespaces
  - /sensor/imu/front/*
  - /sensor/imu/rear/*
  - Rename av_gx5_15.yaml to gx5_15_front.yaml
  - Add gx5_15_rear.yaml

* Contributors: Hector Cruz (@hect95)

1.2.1 (2024-06-06)
------------------
* Remove pinned IMU driver version no longer available from Dockerfile
* Contributors: Alejandro Bordallo

1.2.0 (2024-06-05)
------------------
* Add bash args to optionally load local cyclone_dds
* Contributors: Alejandro Bordallo, hect95

1.1.0 (2024-05-21)
------------------
* Add cyclone DDS as ROS RMW  + configurate it to support high msg throughput
* Port `microstrain_launch.py` to XML ROS launch
* Simplify Imu parameters
* Fix wrong sensor topic namespace, using `/sensor/imu/*`
* Imu is set to run at 200 Hz instead of 100 Hz
* Enable colorised ROS log
* Synchronise host time with docker container

1.0.0 (2024-04-26)
------------------
* Implement automated build of docker images on github (`#3 <https://github.com/ipab-rad/imu/issues/3>`_)
* Improve repository and standardise docker setup (`#2 <https://github.com/ipab-rad/imu/issues/2>`_)
  - Split dockerfile into multiple stages for runtime and dev workflows
  - Add scripts for docker image and container ease of use
  - Update README to reflect the updated repo workflow
* Create imu launch pkg, setup and add Dockerfile (`#1 <https://github.com/ipab-rad/imu/issues/1>`_)
  Co-authored-by: hect95 <hector_cruz95@live.com>
  Co-authored-by: Hector Cruz <hcruzgo@ed.ac.uk>
* Contributors: Alejandro Bordallo
