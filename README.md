# A Multifunctional Robot using Arduino UNO and Bluetooth

An Arduino-based robotic vehicle that combines **obstacle avoidance** with **Bluetooth-based wireless control**. The project uses an HC-SR04 ultrasonic sensor to detect obstacles and an HC-05 Bluetooth module to receive movement commands from an Android device.

## Problems It Solves

The project addresses common challenges in basic robotic navigation and remote control:

- **Manual navigation limitations:** Enables wireless control of the robotic vehicle through Bluetooth.
- **Obstacle detection:** Detects nearby obstacles using an ultrasonic sensor to help prevent collisions.
- **Limited autonomous movement:** Allows the robot to respond to detected obstacles and change its movement accordingly.
- **Separate control and sensing systems:** Combines Bluetooth-based manual control and ultrasonic-based obstacle detection in a single robotic vehicle.
- **Basic robotic automation:** Demonstrates the integration of sensors, wireless communication, and motor control for automated movement.

## Features

- **Obstacle Avoidance:** Detects nearby obstacles using the HC-SR04 ultrasonic sensor.
- **Bluetooth Control:** Allows wireless control of the robot using an Android device.
- **Motor Control:** Controls the movement of the robotic vehicle based on sensor input and Bluetooth commands.
- **Multiple Operating Modes:** Supports manual Bluetooth-based control and obstacle-avoidance functionality.

## Components Used

- Arduino UNO
- HC-SR04 Ultrasonic Sensor
- HC-05 Bluetooth Module
- DC Motors
- Motor Driver
- Robotic Vehicle Chassis
- Battery/Power Supply
- Connecting Wires

## Software & Technologies

- **Programming Language:** C++
- **IDE:** Arduino IDE
- **Microcontroller:** Arduino UNO
- **Communication:** Bluetooth
- **Sensor:** HC-SR04 Ultrasonic Sensor

## Working

The robot can be operated through **Bluetooth-based manual control** or **obstacle-avoidance mode**.

In Bluetooth control mode, movement commands are sent from an Android device to the **HC-05 Bluetooth module**. The Arduino UNO receives and processes these commands and controls the motors accordingly.

In obstacle-avoidance mode, the **HC-SR04 ultrasonic sensor** continuously measures the distance between the robot and nearby objects. When an obstacle is detected within a defined range, the Arduino processes the sensor input and changes the motor-control commands to help the robot avoid the obstacle.

### Basic Working Flow

```text
                  ┌─────────────────────┐
                  │     Arduino UNO     │
                  └──────────┬──────────┘
                             │
              ┌──────────────┴──────────────┐
              │                             │
              ▼                             ▼
    ┌──────────────────┐          ┌──────────────────┐
    │   HC-SR04        │          │      HC-05       │
    │ Ultrasonic Sensor│          │ Bluetooth Module │
    │ Obstacle Detection│         │ Android Control  │
    └─────────┬────────┘          └─────────┬────────┘
              │                             │
              └──────────────┬──────────────┘
                             ▼
                  ┌─────────────────────┐
                  │ Motor Driver &      │
                  │ Motor Control       │
                  └──────────┬──────────┘
                             ▼
                  ┌─────────────────────┐
                  │  Robotic Vehicle    │
                  └─────────────────────┘
```

## Project Outcome

The project successfully demonstrates a multifunctional robotic vehicle capable of **Bluetooth-based manual control and ultrasonic-sensor-based obstacle detection**. It provides practical experience in **Arduino programming, sensor interfacing, Bluetooth communication, and motor control**.

## Future Improvements

- Add additional sensors for improved obstacle detection.
- Implement more advanced autonomous navigation.
- Develop a dedicated Android application for improved robot control.
- Add camera-based monitoring.
- Integrate IoT capabilities for remote monitoring and control.
