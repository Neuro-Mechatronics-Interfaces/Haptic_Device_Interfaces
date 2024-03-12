<!-- License

Copyright 2024-2025 Neuromechatronics Lab, Carnegie Mellon University (a.whit)

Created by: Jonathan Shulgach (jshulgac@andrew.cmu.edu)

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at https://mozilla.org/MPL/2.0/.
-->

# Haptic Device Interfaces ROS2 Package

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/ros/ros-original-wordmark.svg" />

This package contains custom ROS2 interfaces for haptic robot devices. While 
there are plenty of existing ROS2 message types for common robot interfaces, there are 
no standard message types for haptic devices. This package aims to fill that gap by 
providing a set of custom message types for interfacing with haptic devices. 

If you'd like to learn how to make your own ROS2 messages, follow this great post from 
the [Robotics Back-End](https://roboticsbackend.com/ros2-create-custom-message/#Add_the_message_in_CMakeListstxt).

## Currently Supported devices

* [ForceDimension simga7](https://www.forcedimension.com/products/sigma)
* [ForceDimension delta3](https://www.forcedimension.com/products/delta)

## Installation

#### Note: These installation steps are taylored to a linux or WSL2 environment. Tested in Ubuntu 22.04 and WSL2 on Windows 11.

The package can be placed inside a ROS2 workspace and build like any other [ROS2 Package].
1. Navigate to your ROS2 workspace directory. [Create the workspace](https://docs.ros.org/en/iron/Tutorials/Beginner-Client-Libraries/Creating-A-Workspace/Creating-A-Workspace.html) with the `src` folder if not present.
   ```
   cd /path/to/workspace
   ```
2. Clone, and build
   ```
   git clone https://github.com/Neuro-Mechatronics-Interfaces/haptic_device_interfaces.git src/haptic_device_interfaces
   colcon build --packages-select haptic_device_interfaces
   ```
3. Source the workspace to include the newly built package.

   * For Linux users:
   ```
   source install/setup.bash
   ```
   * For Windows users:
   ```
   call install/setup.bat
   ```
4. That's it, enjoy!

## General usage

To include these message types in your own project, general instructions are as follows:
* if you have a `CMakeLists.txt` file in your package, modify it to include the following:
```
find_package(haptic_device_interfaces REQUIRED)

ament_target_dependencies(my_executable <-- Change this to whatever executable name you have
  # Dependencies
  rclcpp
  haptic_device_interfaces # <-- Include this dependency
  # Include all other dependencies you have for your executable
  # ...
)
```
* Open the `package.xml` file and modify it to include the following:
```xml
  <depend>haptic_device_interfaces</depend>
```


Now you can include the message types in your scripts:

* cpp:
   ```
   #include "haptic_device_interfaces/msg/Sigma7.hpp"      
   ```
* python:
   ```pycon
   from haptic_device_interfaces.msg import Sigma7  
   ```


## License

Copyright 2024-2025 [Neuromechatronics Lab], Carnegie Mellon University

Created by: Jonathan Shulgach (jshulgac@andrew.cmu.edu)

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at https://mozilla.org/MPL/2.0/.


<!------------------------------------------------------------------------------
  REFERENCES
------------------------------------------------------------------------------->


[haptics]: https://en.wikipedia.org/wiki/Haptic_technology

[ROS2 Iron]: https://docs.ros.org/en/iron/index.html

[ROS2 package]: https://docs.ros.org/en/iron/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html

[Neuromechatronics Lab]: https://www.meche.engineering.cmu.edu/faculty/neuromechatronics-lab.html
