cmake_minimum_required(VERSION 3.0.2)
project(airlab_gazebo)

find_package(catkin REQUIRED)

catkin_package()
install(DIRECTORY launch models worlds urdf meshes
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
        PATTERN "*~" EXCLUDE)

