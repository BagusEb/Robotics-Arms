## 4-Axis Servo Control with Joystick (Arduino)

This project demonstrates **controlling 4 servo motors using a joystick module on Arduino**, enabling **multi-axis robotic arm or gimbal movements** interactively.

---

### Features

* ✅ Control **three servos (X, Y, Z)** using analog joystick axes for smooth, precise movements.
* ✅ Control **a fourth servo (Last)** using the joystick button to toggle between positions.
* ✅ Uses **software smoothing** to avoid sudden servo jerks.
* ✅ Maps joystick analog values to servo angles effectively.
* ✅ Ready for **robotic arm or gimbal prototypes on Arduino/ESP32**.

---

### Pin Configuration

| Function        | Arduino Pin |
| --------------- | ----------- |
| Joystick X      | A0          |
| Joystick Y      | A1          |
| Joystick Z      | A2          |
| Joystick W      | A3          |
| Joystick Button | D4          |
| Servo X         | D9          |
| Servo Y         | D10         |
| Servo Z         | D11         |
| Servo Last      | D6          |

---

### How It Works

* **Joystick X and Y axes** control `posX` and `posY` angles on Servo X and Y.
* **Joystick W axis** controls `posZ` on Servo Z within 45–135°.
* **Joystick button toggles Servo Last** between 90° and 140°.
* **Smooth incremental movement** (1° steps) for stability.
* Uses `delay(15)` for consistent update timing.

---

### Usage

1. Connect servos and joystick module to your Arduino according to the pin configuration.
2. Upload the code using Arduino IDE.
3. Open Serial Monitor at `9600 baud` if you wish to debug.
4. Move the joystick to control servo angles interactively.
5. Press the joystick button to toggle the fourth servo between positions.

---

### Dependencies

* `#include <Servo.h>` (Arduino Servo library)

---

### Applications

✅ Robotic arm prototypes for student projects.
✅ Manual gimbal angle control.
✅ DIY robotics with Arduino and ESP32.
✅ Servo movement practice using joystick input.

---

### License

This project is for **educational and personal use**. Feel free to modify and adapt for your learning and experimentation.

---

If you need a **circuit diagram, schematic, or demo GIF for your GitHub**, let me know to prepare them for your repository and presentation.
