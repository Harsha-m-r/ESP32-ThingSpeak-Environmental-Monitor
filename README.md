# ESP32-ThingSpeak-Environmental-Monitor
This project uses an ESP32 to monitor temperature, humidity, and soil moisture levels, sending the data to the ThingSpeak IoT platform for real-time visualization and analysis.

## Features
- Real-time environmental data monitoring.
- Integration with ThingSpeak for data logging and visualization.
- Reads temperature and humidity using a DHT11 sensor.
- Monitors soil moisture levels using a soil moisture sensor.

## Table of Contents
- Features
- Components Required
- Wiring Diagram
- Installation and Setup
- Usage
- License

## Components Required

|       Component      |  Quantity |              Description              |
|:--------------------:|:---------:|:-------------------------------------:|
| ESP32                | 1         | Microcontroller with Wi-Fi capability |
| DHT11 Sensor         | 1         | Measures temperature and humidity     |
| Soil Moisture Sensor | 1         | Measures soil moisture levels         |
| Jumper Wires         | As needed | For connections                       |
| Breadboard           | 1         | For prototyping                       |

## Wiring Diagram
Refer to the hardware/wiring_diagram.png file for a detailed diagram.

### Summary:

**DHT11:**

- VCC → 3.3V (ESP32)
- GND → GND (ESP32)
- Data → GPIO4 (ESP32)

**Soil Moisture Sensor:**

- VCC → 3.3V (ESP32)
- GND → GND (ESP32)
- Signal → GPIO36 (ESP32 ADC Pin)

## Installation and Setup
### 1. Prerequisites
- Install the Arduino IDE (latest version).
- Install required libraries:
    1. DHT Sensor Library
    2. Adafruit Unified Sensor Library
    3. ThingSpeak Library

### 2. Clone the Repository

### 3. Configure the Code
1. Open src/esp32_thingspeak.ino in Arduino IDE.
2. Update config.h with your Wi-Fi credentials and ThingSpeak API key:

### 4. Upload the Sketch
1. Connect your ESP32 to the computer via USB.
2. Select the correct Board (ESP32 Dev Module) and Port in Arduino IDE.
3. Click Upload.

## Usage
1. Power up your ESP32.
2. Data from the DHT11 and soil moisture sensor will be sent to ThingSpeak.
3. Visit your ThingSpeak channel to view real-time graphs and data.

## License
This project is licensed under the MIT License. See the [LICENSE file](LICENSE) for details.


