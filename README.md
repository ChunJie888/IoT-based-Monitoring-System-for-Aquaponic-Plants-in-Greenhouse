# IoT-based-Monitoring-System-for-Aquaponic-Plants-in-Greenhouse

# Overview
This project is an IoT-based environmental monitoring system designed for aquaponic greenhouse applications. The system monitors important environmental parameters such as temperature, humidity, and water turbidity in real time using sensors connected to the Seeed Studio XIAO ESP32C3 microcontroller.
The collected data is transmitted through MQTT protocol to HiveMQ Cloud and visualized using a Node-RED dashboard. The system also provides local monitoring and warning indications through an OLED display and WS2813 RGB LED strip.

# Features
1. Real-time temperature monitoring
2. Real-time humidity monitoring
3. Water turbidity monitoring
4. MQTT cloud communication
5. Node-RED dashboard visualization
6. OLED local display output
7. RGB LED warning indicators
8. Threshold-based warning system
9. Manual LED control through MQTT
10. Secure WiFi and MQTT connection

# Hardware Used
1. Seeed Studio XIAO ESP32C3
2. Seeed Studio XIAO Expansion Board
3. DHT20 Temperature & Humidity Sensor
4. Turbidity Sensor
5. WS2813 RGB LED Strip
6. OLED Display
7. Breadboard and jumper wires

# Software Used
1. Arduino IDE
2. Node-RED
3. HiveMQ Cloud MQTT Broker
4. Wokwi Simulator

# System Architecture
The system collects sensor data from:
DHT20 sensor (temperature & humidity) & Turbidity sensor (water quality)

The ESP32C3 processes the data and:
1. Displays values on OLED display
2. Controls RGB LED indicators
3. Publishes JSON data to HiveMQ Cloud MQTT broker
4. Sends data to Node-RED dashboard for monitoring

# Dashboard Functions
1. Real-time sensor gauges
2. Sensor charts
3. Warning status monitoring
4. Corrective action display
5. Manual LED control

# Project Members
1. Ooi Chun Jie
2. Poh Yu Wei
3. Layla Osman Sidahmed Mohamed

## References
1. Buyya, R., & Dastjerdi, A. V. (2016). Internet of Things: Principles and paradigms.
2. Bahga, A., & Madisetti, V. (2014). Internet of Things: A hands-on approach.
3. HiveMQ Documentation: https://www.hivemq.com/
4. Node-RED Documentation: https://nodered.org/docs/

# License
This project is developed for educational and academic purposes.
