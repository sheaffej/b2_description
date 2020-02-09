cmake_minimum_required(VERSION 2.8.3)
project(b2_description)

find_package(catkin REQUIRED COMPONENTS)
catkin_package()

# Install files
install(DIRECTORY launch meshes rviz urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

# Tests
#if (CATKIN_ENABLE_TESTING)
#  find_package(roslaunch REQUIRED)
#  roslaunch_add_file_check(launch)
#  catkin_add_nosetests(tests)
#endif()

