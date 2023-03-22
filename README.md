# ESP32 Temperature Sensor with BMP280 and MQTT
## Description

This program reads the temperature from a BMP280 sensor connected to an ESP32 board and publishes it to an MQTT broker. The ESP32 will go to sleep for a specified amount of time and wake up periodically to read the temperature and publish it to the broker.<br>
<b>2022</b>

## Installation

1. Install the Arduino IDE and the ESP32 core for Arduino.
2. Clone this repository.
3. Open the esp32-bmp280-mqtt.ino file in the Arduino IDE.
4. Modify the ssid, password, and mqtt_server variables to match your Wi-Fi network and MQTT broker settings.
5. Upload the sketch to your ESP32 board.

## Usage

1. Connect the BMP280 sensor to the ESP32 according to the wiring diagram in the code.
2. Power on the ESP32 board.
3. The ESP32 will connect to Wi-Fi and MQTT, collect temperature data from the BMP280 sensor, and publish it to the "esp32/temp3" topic on the MQTT broker.
4. The ESP32 will then go into deep sleep mode for the specified amount of time before waking up to collect and publish data again.

## Example

<p align="center">
<img src="https://user-images.githubusercontent.com/77733903/226798955-061d95e7-68b4-4c3e-9de3-ec0e256f5d72.jpg" width="300"><img src="https://user-images.githubusercontent.com/77733903/226799057-7f6bbdb7-3876-484a-87c1-26d8531e8f5f.jpg" width="300">
</p>

## License

This program is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.
