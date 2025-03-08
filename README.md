# Obstacle Avoidance Robot

This project is an obstacle avoidance robot using an Arduino. The robot uses an ultrasonic sensor to detect obstacles and a servo motor to navigate around them.

## Components

- Arduino Uno
- Ultrasonic Sensor (HC-SR04)
- Servo Motor
- DC Motors
- Motor Driver (L298N)
- Breadboard and Jumper Wires

## Pin Configuration

- **Ultrasonic Sensor**
  - Trig: A0
  - Echo: A1
- **Servo Motor**
  - Signal: 11
- **DC Motors**
  - Right Motor MA1: 7
  - Right Motor MA2: 6
  - Left Motor MB1: 5
  - Left Motor MB2: 4
  - Right Motor Enable Pin EA: 9
  - Left Motor Enable Pin EB: 10

## Installation

1. Install the Arduino IDE from [here](https://www.arduino.cc/en/software).
2. Open the Arduino IDE and go to **Sketch** > **Include Library** > **Manage Libraries**.
3. Search for `Servo` and install it.

## Usage

1. Connect the components as per the pin configuration.
2. Open the `main.ino` file in the Arduino IDE.
3. Upload the code to the Arduino board.
4. Power the Arduino and observe the robot avoiding obstacles.

## Code Explanation

- The `setup()` function initializes the pins and the servo motor.
- The `loop()` function continuously checks the distance to obstacles and decides the movement of the robot.
- The `forward()`, `backward()`, `turnleft()`, `turnright()`, and `Stop()` functions control the movement of the robot.
- The `leftsee()` and `rightsee()` functions check for obstacles on the left and right sides.
- The `ultrasonic()` function calculates the distance to an obstacle using the ultrasonic sensor.
- The `start()` function initializes the servo motor position.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
