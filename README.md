<!-- License

Copyright 2024-2025 Neuromechatronics Lab, Carnegie Mellon University (a.whit)

Created by: Jonathan Shulgach (jshulgac@andrew.cmu.edu)

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at https://mozilla.org/MPL/2.0/.
-->

# Haptic Device Interfaces ROS2 Package

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/ros/ros-original-wordmark.svg" />

<?xml version="1.0" ?><svg height="100px" version="1.1" viewBox="0 0 40 100" width="60px" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><title/><desc/><defs/><g fill="none" fill-rule="evenodd" id="People" stroke="none" stroke-width="1"><g fill="#000000" id="Icon-46" transform="translate(-8.000000, 0.000000)"><path d="M34,21.999 C34,19.793 32.206,17.999 30,17.999 C27.794,17.999 26,19.793 26,21.999 L26,28.328 C26.739,28.593 28.171,28.999 30,28.999 C31.845,28.999 33.266,28.596 34,28.33 L34,21.999 Z M36,21.999 L36,28.999 C36,29.378 35.786,29.724 35.447,29.894 C35.357,29.938 33.199,30.999 30,30.999 C26.801,30.999 24.643,29.938 24.553,29.894 C24.214,29.724 24,29.378 24,28.999 L24,21.999 C24,18.69 26.691,15.999 30,15.999 C33.309,15.999 36,18.69 36,21.999 L36,21.999 Z M33,53.999 L27,53.999 C26.448,53.999 26,54.446 26,54.999 C26,55.552 26.448,55.999 27,55.999 L33,55.999 C33.552,55.999 34,55.552 34,54.999 C34,54.446 33.552,53.999 33,53.999 L33,53.999 Z M33,57.999 L27,57.999 C26.448,57.999 26,58.446 26,58.999 C26,59.552 26.448,59.999 27,59.999 L33,59.999 C33.552,59.999 34,59.552 34,58.999 C34,58.446 33.552,57.999 33,57.999 L33,57.999 Z M16.725,26.457 C16.549,25.934 15.982,25.652 15.458,25.827 C14.935,26.003 14.653,26.57 14.828,27.094 C15.167,28.103 15.61,29.083 16.145,30.006 C16.33,30.326 16.666,30.505 17.011,30.505 C17.181,30.505 17.353,30.462 17.511,30.37 C17.989,30.094 18.152,29.481 17.875,29.004 C17.408,28.197 17.021,27.34 16.725,26.457 L16.725,26.457 Z M14.975,21.509 C15.008,21.512 15.041,21.514 15.074,21.514 C15.582,21.514 16.017,21.128 16.068,20.611 C16.262,18.637 16.86,16.765 17.846,15.045 C18.121,14.566 17.955,13.955 17.476,13.681 C16.997,13.406 16.386,13.572 16.111,14.051 C14.984,16.017 14.299,18.158 14.078,20.416 C14.023,20.966 14.425,21.455 14.975,21.509 L14.975,21.509 Z M26.667,6.347 C24.452,6.816 22.399,7.734 20.566,9.076 C20.12,9.402 20.023,10.027 20.349,10.474 C20.545,10.741 20.849,10.883 21.157,10.883 C21.362,10.883 21.569,10.82 21.747,10.689 C23.35,9.517 25.145,8.714 27.081,8.304 C27.622,8.189 27.967,7.658 27.853,7.118 C27.737,6.577 27.204,6.231 26.667,6.347 L26.667,6.347 Z M32.159,7.12 C32.044,7.66 32.389,8.191 32.93,8.307 C34.864,8.717 36.658,9.52 38.262,10.695 C38.44,10.826 38.646,10.889 38.852,10.889 C39.16,10.889 39.463,10.747 39.659,10.479 C39.986,10.034 39.889,9.408 39.443,9.082 C37.61,7.739 35.558,6.82 33.345,6.35 C32.803,6.235 32.273,6.58 32.159,7.12 L32.159,7.12 Z M42.531,13.69 C42.051,13.965 41.885,14.576 42.159,15.056 C43.145,16.776 43.741,18.649 43.934,20.623 C43.984,21.14 44.419,21.526 44.928,21.526 C44.96,21.526 44.993,21.524 45.026,21.521 C45.575,21.468 45.978,20.979 45.924,20.43 C45.704,18.173 45.021,16.03 43.896,14.062 C43.621,13.582 43.01,13.415 42.531,13.69 L42.531,13.69 Z M44.547,25.807 C44.024,25.632 43.458,25.915 43.282,26.437 C42.987,27.32 42.601,28.178 42.135,28.986 C41.859,29.465 42.023,30.077 42.501,30.353 C42.659,30.443 42.831,30.486 43,30.486 C43.346,30.486 43.682,30.307 43.867,29.986 C44.4,29.061 44.842,28.081 45.179,27.072 C45.354,26.548 45.071,25.981 44.547,25.807 L44.547,25.807 Z M13.059,32.615 C12.765,32.148 12.148,32.008 11.68,32.303 C11.212,32.597 11.072,33.214 11.367,33.682 C11.923,34.563 12.548,35.415 13.225,36.212 C13.423,36.444 13.705,36.564 13.988,36.564 C14.217,36.564 14.447,36.486 14.635,36.326 C15.056,35.969 15.107,35.338 14.75,34.917 C14.133,34.191 13.564,33.418 13.059,32.615 L13.059,32.615 Z M50.127,16.989 C50.222,16.989 50.318,16.976 50.413,16.947 C50.942,16.79 51.244,16.232 51.086,15.703 C50.489,13.704 49.61,11.801 48.473,10.048 C48.172,9.583 47.552,9.451 47.09,9.753 C46.627,10.054 46.495,10.673 46.795,11.136 C47.829,12.729 48.627,14.458 49.169,16.275 C49.298,16.709 49.696,16.989 50.127,16.989 L50.127,16.989 Z M52,21.858 C51.993,21.311 51.547,20.87 51,20.87 L50.988,20.87 C50.436,20.876 49.993,21.329 50,21.882 L50,21.999 C50,23.865 49.743,25.712 49.235,27.488 C49.083,28.019 49.391,28.572 49.921,28.725 C50.013,28.75 50.106,28.763 50.197,28.763 C50.632,28.763 51.032,28.477 51.158,28.037 C51.717,26.083 52,24.051 52,21.999 L52,21.858 Z M12.967,9.672 C12.506,9.37 11.886,9.499 11.583,9.961 C10.437,11.71 9.549,13.608 8.944,15.604 C8.784,16.133 9.082,16.691 9.611,16.852 C9.708,16.881 9.805,16.895 9.901,16.895 C10.33,16.895 10.727,16.616 10.858,16.185 C11.408,14.372 12.214,12.646 13.256,11.057 C13.559,10.595 13.429,9.975 12.967,9.672 L12.967,9.672 Z M38.311,3.801 C40.032,4.588 41.634,5.618 43.074,6.863 C43.263,7.026 43.496,7.106 43.728,7.106 C44.008,7.106 44.287,6.989 44.484,6.761 C44.846,6.343 44.8,5.711 44.382,5.35 C42.799,3.981 41.036,2.848 39.142,1.982 C38.639,1.753 38.045,1.974 37.816,2.476 C37.587,2.978 37.808,3.571 38.311,3.801 L38.311,3.801 Z M16.347,7.043 C16.577,7.043 16.809,6.964 16.997,6.803 C18.442,5.565 20.05,4.542 21.776,3.763 C22.279,3.535 22.503,2.943 22.275,2.439 C22.048,1.937 21.454,1.713 20.953,1.94 C19.054,2.798 17.286,3.923 15.696,5.283 C15.277,5.643 15.228,6.273 15.587,6.693 C15.785,6.925 16.065,7.043 16.347,7.043 L16.347,7.043 Z M27.214,2.19 C29.075,1.932 31.022,1.937 32.879,2.204 C32.927,2.212 32.976,2.215 33.023,2.215 C33.512,2.215 33.94,1.855 34.012,1.357 C34.091,0.812 33.711,0.304 33.165,0.226 C31.123,-0.07 28.984,-0.074 26.939,0.21 C26.392,0.286 26.01,0.791 26.086,1.338 C26.162,1.885 26.665,2.268 27.214,2.19 L27.214,2.19 Z M10,21.999 L10.001,21.784 C10.008,21.232 9.566,20.778 9.014,20.771 C8.42,20.78 8.009,21.206 8.001,21.759 L8,21.999 C8,24.015 8.274,26.013 8.814,27.938 C8.938,28.38 9.339,28.668 9.776,28.668 C9.866,28.668 9.957,28.656 10.047,28.631 C10.579,28.481 10.889,27.93 10.74,27.397 C10.249,25.648 10,23.832 10,21.999 L10,21.999 Z M48.296,32.345 C47.829,32.048 47.211,32.187 46.917,32.654 C46.41,33.455 45.839,34.228 45.221,34.952 C44.862,35.372 44.912,36.004 45.332,36.362 C45.521,36.523 45.751,36.602 45.981,36.602 C46.264,36.602 46.544,36.482 46.742,36.251 C47.422,35.454 48.049,34.604 48.606,33.725 C48.901,33.258 48.763,32.64 48.296,32.345 L48.296,32.345 Z M40,21.999 L40,58.999 C40,59.552 39.552,59.999 39,59.999 C38.448,59.999 38,59.552 38,58.999 L38,21.999 C38,17.588 34.411,13.999 30,13.999 C25.589,13.999 22,17.588 22,21.999 L22,58.999 C22,59.552 21.552,59.999 21,59.999 C20.448,59.999 20,59.552 20,58.999 L20,21.999 C20,16.485 24.486,11.999 30,11.999 C35.514,11.999 40,16.485 40,21.999 L40,21.999 Z" id="finger-click"/></g></g></svg>

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
