cmake_minimum_required(VERSION 3.8)
project(haptic_device_interfaces)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# find dependencies
find_package(ament_cmake REQUIRED)
find_package(geometry_msgs REQUIRED)
find_package(tf2_geometry_msgs REQUIRED)
find_package(example_interfaces REQUIRED)
find_package(rosidl_default_generators REQUIRED)

# Declare ROS2 interfaces like messages and services
set(interface_files 
  # Messages
  "msg/Sigma7.msg"
  "msg/Delta3.msg"
  # msg/Message.msg"
  # etc

  # Services (TO-DO when needed)
  #"srv/service_when_needed.srv"
)

rosidl_generate_interfaces(${PROJECT_NAME}
  ${interface_files}
  DEPENDENCIES
    geometry_msgs
    tf2_geometry_msgs
    example_interfaces
 )
ament_export_dependencies(rosidl_default_runtime)


if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)
  # the following line skips the linter which checks for copyrights
  # comment the line when a copyright and license is added to all source files
  set(ament_cmake_copyright_FOUND TRUE)
  # the following line skips cpplint (only works in a git repo)
  # comment the line when this package is in a git repo and when
  # a copyright and license is added to all source files
  set(ament_cmake_cpplint_FOUND TRUE)
  ament_lint_auto_find_test_dependencies()
endif()

ament_package()
