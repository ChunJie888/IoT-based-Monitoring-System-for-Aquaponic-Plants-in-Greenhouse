# IoT-based-Monitoring-System-for-Aquaponic-Plants-in-Greenhouse

## Overview
This project is an IoT-based environmental monitoring system designed for aquaponic greenhouse applications. The system monitors important environmental parameters such as temperature, humidity, and water turbidity in real time using sensors connected to the Seeed Studio XIAO ESP32C3 microcontroller.
The collected data is transmitted through MQTT protocol to HiveMQ Cloud and visualized using a Node-RED dashboard. The system also provides local monitoring and warning indications through an OLED display and WS2813 RGB LED strip.

## Features
- Real-time temperature monitoring
- Real-time humidity monitoring
- Water turbidity monitoring
- MQTT cloud communication
- Node-RED dashboard visualization
- OLED local display output
- RGB LED warning indicators
- Threshold-based warning system
- Manual LED control through MQTT
- Secure WiFi and MQTT connection

## Hardware Used
- Seeed Studio XIAO ESP32C3
- Seeed Studio XIAO Expansion Board
- DHT20 Temperature & Humidity Sensor
- Turbidity Sensor
- WS2813 RGB LED Strip
- OLED Display
- Breadboard and jumper wires

## Software Used
- Arduino IDE
- Node-RED
- HiveMQ Cloud MQTT Broker
- Wokwi Simulator

## System Architecture
The system collects sensor data from:
- DHT20 sensor (temperature & humidity)
- Turbidity sensor (water quality)

The ESP32C3 processes the data and:
1. Displays values on OLED display
2. Controls RGB LED indicators
3. Publishes JSON data to HiveMQ Cloud MQTT broker
4. Sends data to Node-RED dashboard for monitoring

## MQTT Topics

### Publish Topic
```cpp
aquaponic/data
```

### Subscribe Topics
```cpp
aquaponic/lights
aquaponic/ledcolor
```

## Dashboard Functions
- Real-time sensor gauges
- Sensor charts
- Warning status monitoring
- Corrective action display
- Manual LED control

## Example JSON Payload
```json
{
  "temperature": 28.3,
  "temperature_status": "Normal",
  "humidity": 53.2,
  "humidity_status": "Normal",
  "turbidity_voltage": 1.87,
  "turbidity_status": "Normal",
  "led_mode": "auto"
}
```

## Project Members
- Ooi Chun Jie
- Poh Yu Wei
- Layla Osman Sidahmed Mohamed

## References
1. Buyya, R., & Dastjerdi, A. V. (2016). Internet of Things: Principles and paradigms.
2. Bahga, A., & Madisetti, V. (2014). Internet of Things: A hands-on approach.
3. HiveMQ Documentation: https://www.hivemq.com/
4. Node-RED Documentation: https://nodered.org/docs/

## License
This project is developed for educational and academic purposes.
