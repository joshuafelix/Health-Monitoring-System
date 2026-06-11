# IoT-Based Health Monitoring System

An IoT-enabled health monitoring system that collects physiological parameters from sensors connected to an ESP32 microcontroller, transmits data to the cloud using HTTP protocol, and visualizes the information through ThingSpeak and a custom web dashboard.

## Project Highlights

- Real-time temperature monitoring
- Real-time heart rate monitoring
- ESP32-based IoT architecture
- HTTP protocol for cloud communication
- ThingSpeak cloud integration
- Custom HTML dashboard
- Threshold-based health alerts
- Multi-platform simulation and validation
- Professional development workflow using PlatformIO

## Technologies Used

### Hardware
- ESP32-WROOM
- LM35 Temperature Sensor
- Heartbeat Sensor
- 16x2 LCD Display

### Software & Tools
- Visual Studio Code
- PlatformIO IDE
- Wokwi Simulator
- Proteus Professional
- ThingSpeak Cloud
- HTML
- CSS
- JavaScript
- GitHub

## Development Workflow

### Wokwi Simulation
The project logic and ESP32 firmware were initially developed and tested in Wokwi to verify sensor acquisition, LCD operation, WiFi connectivity, and cloud communication.

### PlatformIO Development
Firmware was developed using PlatformIO in Visual Studio Code, enabling structured project management, library handling, and easier debugging.

### Proteus Validation
The complete hardware circuit was recreated in Proteus to validate component connections and system behavior before physical implementation.

### Cloud Integration
Sensor readings are transmitted to ThingSpeak using HTTP requests, allowing remote monitoring and historical data analysis.

### Custom Dashboard
A custom HTML dashboard fetches data from ThingSpeak APIs and displays:
- Temperature
- Heart Rate
- Alert Status
- Real-time updates

## System Architecture

Sensors
↓
ESP32
↓
HTTP Protocol
↓
ThingSpeak Cloud
↓
Custom Web Dashboard
↓
Threshold-Based Alerts

## Alert Conditions

### Temperature
| Status | Range |
|----------|----------|
| Normal | 35°C – 38°C |
| High Alert | > 38°C |
| Low Alert | < 35°C |

### Heart Rate
| Status | Range |
|----------|----------|
| Normal | 60–100 BPM |
| High Alert | > 100 BPM |
| Low Alert | < 60 BPM |

## Repository Structure

```text
.
├── src/
│   └── main.cpp
├── dashboard/
│   └── dashboard.html
├── proteus/
│   └── circuit_design
├── screenshots/
└── README.md
```
```markdown
## Screenshots

### Wokwi Simulation
![Wokwi](screenshots/wokwi.png)

### Proteus Circuit
![Proteus](screenshots/proteus.png)

### ThingSpeak Dashboard
![ThingSpeak](screenshots/thingspeak.png)

### Custom Dashboard
![Dashboard](screenshots/dashboard.png)
