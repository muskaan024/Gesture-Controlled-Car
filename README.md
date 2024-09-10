# GestureControlledCar
This repository contains code and diagram for hand gesture controlled car using Arduino


# Gesture Controlled Car with MPU6050

Welcome to the Gesture Controlled Car project! This repository includes code and documentation for controlling a car using hand gestures, facilitated by the MPU6050 sensor.

## Overview

This project enables you to navigate a car using hand gestures by interpreting data from the MPU6050 sensor, which integrates both a gyroscope and accelerometer. The data is processed by an Arduino Nano, which sends control signals to the car’s motors via a motor driver.

## Materials Used

- **Microcontroller**: [Arduino Nano](https://www.arduino.cc/en/Guide/ArduinoNano)
  - The microcontroller processes sensor data and controls the car.

- **IMU Sensor**: [MPU6050](https://www.invensense.com/wp-content/uploads/2015/02/MPU-6000-Register-Map1.pdf)
  - A 6-axis motion-tracking device that combines a 3-axis gyroscope and a 3-axis accelerometer to detect orientation and movement.

- **Motor Driver**: [L298N](https://www.electronicwings.com/nodemcu/l298n-motor-driver-module)
  - Controls the car's DC motors based on commands from the microcontroller.

- **DC Motors**: [Generic DC Motors](https://www.robotshop.com/en/dc-motors.html)
  - Drive the car’s wheels.

- **Power Supply**: [LiPo Battery](https://www.hobbyking.com/hobbyking/store/__67114__Turnigy_2200mAh_3S_25C_Lipo_Pack.html)
  - Provides power to the car and its components.

- **Chassis**: [RC Car Chassis Kit](https://www.amazon.com/Remote-Controlled-Children-Construction-Toys/dp/B07PHFRFY5)
  - The physical body of the car.

## Basic Description

The Gesture Controlled Car uses the MPU6050 sensor to detect changes in orientation and movement of the car. The sensor data is processed by the Arduino Nano, which interprets gestures to control the car's movements. The L298N motor driver translates these commands into physical motion, allowing the car to move forward, backward, left, or right.

### How It Works

1. **Sensor Data Acquisition**: The MPU6050 measures acceleration and angular velocity, providing data on the car's orientation.
2. **Gesture Recognition**: The Arduino Nano processes this sensor data to recognize specific hand gestures or movements.
3. **Motor Control**: Based on recognized gestures, the Arduino sends control signals to the L298N motor driver to actuate the car's motors.

## Getting Started

1. **Assemble the Car**: Follow the assembly instructions for the chassis and attach the DC motors.
2. **Connect the Electronics**: Wire the MPU6050 sensor, motor driver, and Arduino Nano according to the wiring diagram in `wiring_diagram.pdf`.
3. **Upload the Code**: Use the Arduino IDE to upload the provided sketch to the Arduino Nano. The sketch includes code for reading the MPU6050 data and controlling the motors based on detected gestures.
4. **Power Up**: Connect the LiPo battery to the car and start testing the gesture controls.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
