# Arduino Obstacle Avoiding Car

This project involves creating an Arduino-based obstacle-avoiding car using DC motors, an ultrasonic sensor, and a servo motor. The car detects obstacles in its path and maneuvers around them by making decisions based on the distance to the obstacles on its left and right.

## Components Used

- Arduino Uno
- Adafruit Motor Shield
- 4 DC Motors
- HC-SR04 Ultrasonic Sensor
- Servo Motor
- Jumper Wires
- Battery Pack

## Features

- **Obstacle Detection**: Uses an ultrasonic sensor to measure the distance to obstacles.
- **Servo Scanning**: A servo motor rotates to scan the environment for obstacles.
- **Directional Decision Making**: Compares distances to the left and right to decide the direction to turn.
- **Smooth Movement**: Gradual speed increase to protect the battery and ensure smooth movement.

## Circuit Diagram

1. Connect the DC motors to the motor shield.
2. Connect the ultrasonic sensor's TRIG pin to A0 and ECHO pin to A1.
3. Connect the servo motor to pin 10 on the Arduino.
4. Power the Arduino and motor shield using a suitable battery pack.

## Code Explanation

The code is divided into several functions to handle different tasks:

- **setup()**: Initializes the servo motor and takes initial distance readings.
- **loop()**: Continuously checks for obstacles and makes decisions on movement.
- **moveForward()**: Moves the car forward.
- **moveBackward()**: Moves the car backward.
- **turnRight()**: Turns the car to the right.
- **turnLeft()**: Turns the car to the left.
- **moveStop()**: Stops the car.
- **lookRight()**: Rotates the servo to the right and takes a distance reading.
- **lookLeft()**: Rotates the servo to the left and takes a distance reading.
- **readPing()**: Reads the distance from the ultrasonic sensor.

## How to Run

1. **Assemble the hardware** according to the circuit diagram.
2. **Upload the code** to your Arduino board using the Arduino IDE.
3. **Power the system** and place the car on the ground. The car will start moving forward, detect obstacles, and avoid them by turning left or right.


## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.


## Acknowledgments

- Arduino Community for the resources and libraries
- Adafruit for the motor shield library
