This is an ESP32-based earthquake early warning system that detects ground shaking using an accelerometer and alerts you with LED and buzzer warnings at two different sensitivity levels.

The project uses an MPU6050 accelerometer to monitor vibration on all three axes. A digital filter removes gravity noise so we can detect actual shaking. When acceleration crosses a low threshold, a blinking LED activates as an early warning. If shaking gets stronger and crosses a high threshold, a passive buzzer kicks in with a sweeping alarm tone. A backup KY-002 vibration switch provides secondary confirmation of shaking.

This teaches I2C sensor communication, digital filtering, and two-stage alert logic — the same principles used in real earthquake early warning systems.

Supplies
ESP32 development board (with USB cable)
MPU6050 accelerometer module (I2C sensor)
Passive buzzer module (PWM-driven, not active buzzer)
LED (any color)
220Ω current-limiting resistor
Breadboard and jumper wires
Arduino IDE with ESP32 board support
