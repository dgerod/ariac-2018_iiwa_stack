cmake_minimum_required(VERSION 2.8.3)
project(iiwa_control)

find_package(catkin REQUIRED)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES rrbot_control
#  CATKIN_DEPENDS other_catkin_pkg
#  DEPENDS system_lib
)

# Install all the launch files
install(DIRECTORY launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch)

# Install all the config files
install(DIRECTORY config/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/config)
