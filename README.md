# Smart Healthcare Monitoring and Medication Management System

An IoT-based healthcare monitoring system built using **ESP32**, **FreeRTOS**, **MQTT**, and **Adafruit IO** for real-time patient health monitoring, environmental sensing, alert generation, and role-based dashboards.

##  Overview

This project simulates a smart hospital environment where patient vital signs and healthcare facility conditions are monitored continuously. The system uses concurrent FreeRTOS tasks to collect sensor data, process alerts, publish information to cloud dashboards, and provide real-time visualization.

##  Features

- Real-time patient health monitoring
- Environmental monitoring for healthcare facilities
- Medical and facility alert generation
- MQTT-based cloud communication using Adafruit IO
- Role-based dashboards for medical staff and facility management
- FreeRTOS-based concurrent task execution
- Data aggregation for simplified monitoring
- Watchdog timer for improved system reliability

##  Technologies Used

- ESP32
- FreeRTOS
- MQTT
- Adafruit IO
- Arduino IDE
- OLED Display
- Wokwi Simulator

##  Parameters Monitored

### Patient Monitoring
- Body Temperature
- Heart Rate
- SpO₂
- Blood Pressure
- ECG

### Facility Monitoring
- Room Temperature
- Oxygen Level
- Air Quality Index (AQI)
- Motion Detection

##  System Architecture

The system is divided into multiple FreeRTOS tasks responsible for:

- Patient vital monitoring
- Environmental monitoring
- MQTT communication
- Alert handling
- OLED display updates
- Data aggregation
- Watchdog monitoring

Inter-task communication is implemented using:

- Queues
- Semaphores
- Mutexes

##  Cloud Dashboard

Sensor data and alerts are published to **Adafruit IO** using MQTT.

Two separate dashboards are implemented:

- **Medical Staff Dashboard**
  - Heart Rate
  - SpO₂
  - Body Temperature
  - Medical Alerts

- **Facility Management Dashboard**
  - Room Temperature
  - Oxygen Level
  - AQI
  - Motion Detection
  - Facility Alerts

##  Alert System

The system generates alerts whenever sensor readings exceed predefined thresholds.

Examples include:

- High/Low Body Temperature
- High/Low Heart Rate
- Low SpO₂
- High Blood Pressure
- Abnormal ECG
- Poor Air Quality
- Low Oxygen Levels
- Motion Detection Alerts

##  Project Structure

```
├── Code/
│   ├── ESP32 Source Code
│   ├── FreeRTOS Tasks
│   └── MQTT Configuration
│
├── Images/
│   ├── Circuit Diagram
│   ├── OLED Output
│   ├── Medical Dashboard
│   └── Facility Dashboard
│
├── Report/
│   └── Project Report.pdf
│
└── README.md
```


##  Future Improvements

- Integration with real hardware sensors
- Secure MQTT communication (TLS)
- Patient history database
- Mobile application support
- AI-based health anomaly detection
- SMS/Email emergency notifications

##  Author

**Ardra P**

B.Tech Electronics and Communication Engineering  
International Institute of Information Technology Hyderabad (IIIT Hyderabad)
