Temperature-monitoring-system
Arduino-based temperature monitoring system using an LM35 sensor. Measures ambient temperature in real time, displays readings on the Serial Monitor, and indicates normal and high-temperature conditions using LED indicators.

Temperature Monitoring System

Overview
This project is an Arduino-based Temperature Monitoring System that uses an LM35 temperature sensor to measure ambient temperature in real time. The measured temperature is displayed on the Arduino Serial Monitor, while LEDs provide a visual indication of normal and high-temperature conditions.

 Features
- Real-time temperature monitoring
- Displays temperature in degrees Celsius
- Green LED indicates normal temperature
- Red LED indicates high temperature (60°C or above)
- Simple and low-cost Arduino project

Components Required
- Arduino Uno
- LM35 Temperature Sensor
- Red LED
- Green LED
- 220 Ω Resistors
- Breadboard
- Jumper Wires
- USB Cable

Pin Connections

| Component | Arduino Pin |
|----------|-------------|
| LM35 Output | A0 |
| Red LED | D7 |
| Green LED | D6 |

Working Principle
1. The LM35 continuously measures the surrounding temperature.
2. The Arduino converts the sensor output into degrees Celsius.
3. The temperature is displayed on the Serial Monitor.
4. If the temperature is below 60°C, the Green LED turns ON.
5. If the temperature reaches or exceeds 60°C, the Red LED turns ON to indicate a high-temperature condition.

Programming Language
- Arduino C/C++

Applications
- Room temperature monitoring
- Laboratory temperature monitoring
- Educational Arduino projects
- Basic industrial temperature indication
