cmake_minimum_required(VERSION 3.5)
project(ar4_robot)

unset( CATKIN_INSTALL_INTO_PREFIX_ROOT )

find_package(ament_cmake REQUIRED)

install(DIRECTORY config launch rviz srdf urdf driver meshes
  DESTINATION share/${PROJECT_NAME}
)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})

ament_package()
