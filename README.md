# ESP32 Ultrasonic Distance Measurement

## Project Overview
This project measures the distance of an object using the HC-SR04 ultrasonic sensor and an ESP32 development board. The measured distance is displayed on the Arduino Serial Monitor.

## Components Used
- ESP32 Development Board
- HC-SR04 Ultrasonic Sensor
- Jumper Wires
- USB Cable

## Connections

| HC-SR04 | ESP32 |
|---------|-------|
| VCC | 5V |
| GND | GND |
| TRIG | GPIO 5 |
| ECHO | GPIO 18 |

## Working
1. ESP32 sends a 10 µs pulse through the TRIG pin.
2. The ultrasonic sensor emits sound waves.
3. The ECHO pin receives the reflected signal.
4. ESP32 calculates the distance using the time taken by the echo.
5. The distance is displayed on the Serial Monitor.

## Formula

Distance (cm) = (Duration × 0.0343) / 2

## Output

Example:

Distance: 18.03 cm
Distance: 17.70 cm
Distance: 19.11 cm

## Software Used
- Arduino IDE
- ESP32 Board Package
