cmake_minimum_required(VERSION 2.8.3)
project(teknofest_simulator)

find_package(catkin REQUIRED
  rospy
  uuv_sensor_ros_plugins
  uuv_descriptions
  uuv_gazebo_ros_plugins
  uuv_assistants
  uuv_descriptions
  uuv_gazebo
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES turquoise_description
#  CATKIN_DEPENDS other_catkin_pkg
#  DEPENDS system_lib
)

include_directories(
# include
# ${catkin_INCLUDE_DIRS}
)

install(PROGRAMS
  scripts/depth_estimator.py
  scripts/world_to_odom_tf_publisher.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
