cmake_minimum_required(VERSION 2.8.3)
project(turtlebot_scripts)

find_package(catkin REQUIRED)


catkin_package()

install(DIRECTORY config
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(PROGRAMS scripts/create_rplidar_udev_rules
        DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
install(PROGRAMS scripts/create_swlidar_udev_rules
        DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
