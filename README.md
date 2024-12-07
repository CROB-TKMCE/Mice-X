# Ultrasonic Sensor-Based Obstacle Avoidance Robot

This project involves a simple robot that uses ultrasonic sensors to detect obstacles and navigate its surroundings. It can move forward, turn left, or turn right based on sensor inputs, making decisions to avoid obstacles in its path.

## Features

- **Obstacle Detection**: Uses 3 ultrasonic sensors (front, left, right) to detect obstacles.
- **Autonomous Navigation**: The robot avoids obstacles by moving forward, turning left, or turning right.
- **Arduino Powered**: The code is designed to work with an Arduino or compatible microcontroller.

## Hardware

- **3 Ultrasonic Sensors**: For detecting objects at the front, left, and right.
- **Motor Driver (L298N)**: To control the movement of the robot using DC motors.
- **Arduino Board**: To run the code and process sensor data.
- **DC Motors**: For the movement of the robot.

## Wiring

Refer to the wiring diagram for connecting the ultrasonic sensors and motor driver to the Arduino. Make sure the motor driver and sensors are connected to the correct pins as defined in the code.

## Code

The code is written in Arduino C++ and uses the `NewPing` library to interface with the ultrasonic sensors. The robot uses basic logic to detect obstacles and make decisions about its movement.

### Main Functions:

- `moveForward()`: Moves the robot forward.
- `moveLeft()`: Turns the robot left.
- `moveRight()`: Turns the robot right.
- `stopMotors()`: Stops the robot.
- `checkObjectInRange()`: Checks if an object is within the defined detection range (3 cm).

### Code Walkthrough:

1. **Setup Sensors**: The ultrasonic sensors are initialized with defined trigger and echo pins.
2. **Obstacle Avoidance Logic**: The robot checks the sensor readings and avoids obstacles by either turning left or right when an obstacle is detected in front.

## How to Use

1. **Hardware Setup**: Connect the ultrasonic sensors and motor driver to your Arduino according to the wiring diagram.
2. **Software Setup**: Install the required libraries in Arduino IDE (`NewPing` library).
3. **Upload Code**: Upload the provided code to your Arduino board.
4. **Power the Robot**: Power your robot and observe it in action as it detects obstacles and avoids them autonomously.

## License

This project is licensed under the MIT License.
