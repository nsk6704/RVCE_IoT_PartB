This is a repository consisting of the codes for Part B of IoT Lab at RVCE - Semester 4
# ESP32 IoT Projects with Blynk Integration

This repository contains a collection of IoT projects using the ESP32 microcontroller. Each project is designed to monitor or control a specific environment or system using various sensors, with real-time data visualization on Blynk.

## Projects

1. **Smart Lighting - LDR and LED**
2. **Smart Parking - 2 IR Sensors**
3. **Weather Monitoring - DHT11**
4. **Smart Irrigation - Soil Moisture and LED**
5. **Forest Fire Detection - DHT11**

### 1. Smart Lighting - LDR and LED

This project uses an LDR (Light Dependent Resistor) to monitor ambient light levels and control an LED accordingly. If the light level falls below a specified threshold, the LED turns on. The current light level is displayed on Blynk.

- **Hardware Used**: 
  - ESP32
  - LDR (connected to GPIO 34)
  - LED (connected to GPIO 2)

- **Blynk Virtual Pins**:
  - V1: Light level

### 2. Smart Parking - 2 IR Sensors

This project uses two IR sensors to detect the presence of a vehicle in a parking spot. The state of each sensor is displayed on Blynk.

- **Hardware Used**:
  - ESP32
  - 2 IR Sensors (connected to GPIO 32 and GPIO 33)

- **Blynk Virtual Pins**:
  - V1: Sensor 1 state
  - V2: Sensor 2 state

### 3. Weather Monitoring - DHT11

This project uses a DHT11 sensor to monitor the temperature and humidity of the environment. The readings are sent to Blynk for real-time monitoring.

- **Hardware Used**:
  - ESP32
  - DHT11 Sensor (connected to GPIO 4)

- **Blynk Virtual Pins**:
  - V5: Temperature
  - V6: Humidity

### 4. Smart Irrigation - Soil Moisture and LED

This project uses a soil moisture sensor to monitor the moisture level in the soil. If the moisture falls below a certain threshold, an LED (simulating a water pump) is activated. The moisture level is displayed on Blynk.

- **Hardware Used**:
  - ESP32
  - Soil Moisture Sensor (connected to GPIO 35)
  - LED (connected to GPIO 2)

- **Blynk Virtual Pins**:
  - V3: Soil moisture level

### 5. Forest Fire Detection - DHT11 and Smoke Sensor

This project uses a DHT11 sensor to monitor the temperature and humidity of an environment, combined with a smoke sensor to detect the presence of smoke. If the temperature exceeds a critical threshold or smoke is detected, it triggers a warning, indicating a potential fire risk. The data is displayed on Blynk for real-time monitoring.

- **Hardware Used**:
  - ESP32
  - DHT11 Sensor (connected to GPIO 4)
  - Smoke Sensor (e.g., MQ-2, connected to GPIO 34)

- **Blynk Virtual Pins**:
  - V5: Temperature
  - V6: Humidity
  - V7: Smoke level

## Getting Started

### Prerequisites

- [Arduino IDE](https://www.arduino.cc/en/software)
- [Blynk Library](https://github.com/blynkkk/blynk-library)
- ESP32 board setup in Arduino IDE ([Installation Guide](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/))

### Installation

1. **Clone this repository:**
    ```bash
    git clone https://github.com/your-username/esp32-iot-projects.git
    cd esp32-iot-projects
    ```

2. **Open each project in Arduino IDE:**
    * Navigate to the specific project directory.
    * Open the `.ino` file in Arduino IDE.

3. **Set up Blynk:**
    * Replace `"YourAuthToken"`, `"YourNetworkName"`, and `"YourPassword"` with your Blynk authentication token, Wi-Fi network name, and password in the Arduino sketch.

4. **Upload the code to ESP32:**
    * Connect your ESP32 to your computer.
    * Select the correct board and port in Arduino IDE.
    * Click on the Upload button.

### Usage

* Open the Blynk app on your smartphone.
* Create a new project and use the same auth token as in your code.
* Add widgets corresponding to the virtual pins specified in the project.
* Monitor the sensor values and control the devices in real-time.

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. Please ensure your contributions are well-documented and tested.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* [Blynk](https://blynk.io) for providing a versatile platform for IoT projects.
* [Espressif Systems](https://www.espressif.com) for the ESP32 microcontroller.

