4-Axis Servo Control with Joystick (Arduino)
This project demonstrates controlling 4 servo motors using a joystick module on Arduino, enabling multi-axis robotic arm or gimbal movements interactively.

Features
✅ Controls three servos (X, Y, Z) smoothly using analog joystick axes.
✅ Controls an additional servo (W/Last) using a button toggle for locking/releasing position.
✅ Includes software smoothing to prevent sudden jerks on servos.
✅ Uses analogRead with mapping to convert joystick values to servo angles.
✅ Serial debug ready at 9600 baud for monitoring.
✅ Suitable for robotic arm prototypes, camera gimbal control, or ESP32/Arduino robotics practice.

Pin Configuration
Joystick:

X-axis: A0

Y-axis: A1

Z-axis: A2 (currently unused, mapped separately)

W-axis: A3

Button: D4

Servos:

X Servo: D9

Y Servo: D10

Z Servo: D11

Last Servo: D6 (controlled via button toggle)

How it works
Moving the joystick on X and Y changes posX and posY angles on the respective servos.

Moving the joystick on W-axis changes posZ within 45–135°.

Pressing the joystick button toggles the fourth servo (Last) between 90° and 140°.

The servos increment or decrement gradually (step of 1°) for smooth movement.

A delay(15) is used for stability between updates.

Usage
1️⃣ Connect the servos and joystick module to your Arduino as per the pin configuration.
2️⃣ Upload the sketch using the Arduino IDE.
3️⃣ Open the Serial Monitor at 9600 baud for debug if needed.
4️⃣ Move the joystick to control servo positions in real-time.
5️⃣ Press the joystick button to toggle the fourth servo position.
