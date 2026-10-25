# ESP32 to ThingSpeak: Temperature and Humidity Monitoring

## Project Overview

This project uses an ESP32 microcontroller and a DHT22 temperature and humidity sensor to collect environmental data and send it to ThingSpeak over Wi-Fi.

The sensor readings are uploaded to a ThingSpeak channel every 20 seconds and displayed using two time-series charts.

## Objectives

- Connect the ESP32 to Wi-Fi.
- Read temperature and humidity using the DHT22 sensor.
- Send sensor readings to ThingSpeak.
- Visualize temperature and humidity using cloud-based charts.
- Monitor the data through a publicly accessible ThingSpeak channel.

## Student Information

- **Full Name:** Saja Dwaikat
- **University ID:** 12325663

## Hardware and Simulation

- ESP32 DevKit
- DHT22 temperature and humidity sensor
- Wokwi online simulator
- ThingSpeak IoT analytics platform

## Circuit Connections

| DHT22 Pin | ESP32 Pin |
|---|---|
| VCC (+) | 3V3 |
| DATA | GPIO 15 |
| GND (-) | GND |

The circuit was implemented and tested using the Wokwi simulator.

## Software and Libraries

- Arduino C++
- WiFi.h
- ThingSpeak library
- DHT sensor library

## Data Collection and Cloud Integration

The ESP32 connects to the `Wokwi-GUEST` Wi-Fi network and reads temperature and humidity from the DHT22 sensor.

The readings are uploaded to ThingSpeak using the following channel fields:

- **Field 1:** Temperature (°C)
- **Field 2:** Humidity (%)

The upload interval is 20 seconds.

The program prints sensor readings and the upload status to the Serial Monitor.


## Project Links

- **Wokwi Simulation:** https://wokwi.com/projects/478878957160003585
- **ThingSpeak Public Channel:** https://thingspeak.mathworks.com/channels/3549989


## Screenshots

The `screenshots` folder contains:

1. Wokwi circuit diagram.
2. Serial Monitor showing temperature and humidity readings.
3. ThingSpeak temperature chart.
4. ThingSpeak humidity chart.

## How to Run

1. Open the Wokwi simulation using the link above.
2. Ensure the DHT22 sensor is connected to GPIO 15.
3. Configure the ThingSpeak channel ID and Write API Key in the code.
4. Start the simulation.
5. Open the Serial Monitor to view sensor readings and upload status.
6. Open the ThingSpeak channel to view the temperature and humidity charts.

## Security Note

API keys should be kept private and must not be committed to a public repository.

## Conclusion

This project demonstrates an IoT data-collection workflow using an ESP32, a DHT22 sensor, Wi-Fi connectivity, and ThingSpeak for cloud-based data visualization.
