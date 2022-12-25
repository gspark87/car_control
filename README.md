# car_control
This package is RC car control for path tracking.  
Using the Pure Pursuit algorithm.   
Keyboard control can be performed using the [following code][keyboard_code].

[keyboard_code]: https://github.com/gspark87/car_control_keyboard

## Test Hardware
* 1/8 VRX RH818 (RC Car)
* ESP32 (PWM Generator)
* Jetson Nano (Main Processor)
  * Ubuntu 20.04
  * ROS2 Galactic
## Build
    colcon build --package-select car_control
    source install/setup.bash
## Run
    #1. Main code
    ros2 run car_control pure_pursuit

    #2. Algorithm test code
    ros2 run car_control control_simulation
## Note
  Change to Serial communication due to be unstable of Micro-ROS.  
  (Low topic rate)
## Reference
https://github.com/AtsushiSakai/PythonRobotics
