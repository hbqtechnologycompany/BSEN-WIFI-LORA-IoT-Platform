# BSEN WIFI LORA IoT Platform

![BSEN WIFI LORA IoT Platform](https://img.shields.io/badge/Platform-IoT-blue)
![License](https://img.shields.io/badge/License-Public-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## 📋 Hardware Overview

**BSEN WIFI LORA IoT Platform** is a professional-grade development board designed for IoT applications requiring both WiFi and LoRa connectivity. This hardware platform features a dual-radio architecture with ESP32-S3/ESP32-C6 microcontroller and SX1276/SX1278 LoRa transceiver, providing flexible connectivity options for various IoT scenarios.

![BSEN_3D](https://github.com/user-attachments/assets/4914a530-e1f3-4469-9229-12d4f3110b18)

### 🔧 Hardware Specifications
- **Microcontroller**: ESP32-S3 or ESP32-C6 (factory option)
- **LoRa Module**: SX1276 (868MHz)
- **WiFi**: 2.4GHz IEEE 802.11 b/g/n (ESP32-S3) / WiFi 6 (ESP32-C6)
- **Bluetooth**: Bluetooth 5.0 LE (ESP32-S3) / Bluetooth 5.2 LE (ESP32-C6)
- **Power Supply**: 3.3V/5V DC input
- **Operating Temperature**: -40°C to +85°C
- **Dimensions**: 65mm x 45mm (standard form factor)
- **Interface**: UART, SPI, I2C, GPIO, USB

## 🚀 Hardware Features

### 🌐 Dual Radio Architecture
- **WiFi Radio**: 2.4GHz IEEE 802.11 b/g/n (ESP32-S3) / WiFi 6 (ESP32-C6)
- **LoRa Radio**: SX1276 transceiver (868MHz)
- **Bluetooth**: Bluetooth 5.0 LE (ESP32-S3) / Bluetooth 5.2 LE (ESP32-C6)
- **Antenna Design**: Optimized dual-band antenna system
- **Radio Switching**: Hardware-controlled radio selection

### ⚡ Power Management
- **Input Voltage**: 5V-36VDC DC (wide input range)
- **Power Consumption**: 
  - Active mode: 70mA (WiFi), 45mA (LoRa)
  - Deep sleep: 2.5μA (ESP32-S3) / 1.5μA (ESP32-C6)
- **Battery Support**: Li-ion/Li-Po battery connector
- **Power Monitoring**: Built-in voltage monitoring
- **USB Power**: USB-C connector for development

### 🔌 Interface & Connectivity
- **USB-C**: USB-C connector for programming, power, and debugging
- **UART**: 3.3V TTL UART for serial communication
- **SPI**: High-speed SPI interface for LoRa module
- **I2C**: I2C bus for sensor integration
- **RS485**: Industrial communication interface for Modbus sensors
- **ADC**: 4-channel 12-bit ADC
- **Relay Outputs**: 2x NO/NC relay outputs for device control
- **Analog Inputs**: 4x 4-20mA/0-5V analog input channels
- **Pulse Counter**: 2x pulse counter inputs

### 🛡️ Protection & Reliability
- **ESD Protection**: ±8kV ESD protection on all I/O pins
- **Overvoltage Protection**: Input voltage protection up to 36V
- **Reverse Polarity Protection**: Built-in reverse polarity protection

## 📁 Hardware Documentation

```
BSEN-WIFI-LORA-IoT-Platform/
├── schematic/                    # Hardware schematics
│   └── BSEN_WIFI_IoT_public.pdf # Complete circuit schematics
├── firmware/                     # Firmware source code
├── documentation/                # Hardware documentation
│   ├── datasheet/               # Component datasheets
│   ├── pinout/                  # Pinout diagrams
└── README.md                     # This documentation
```

## 🛠️ Hardware Components

### Core Components
- **Microcontroller**: ESP32-S3 (240MHz dual-core) or ESP32-C6 (160MHz single-core)
- **LoRa Transceiver**: SX1276 (868MHz, 14dBm output power)
- **Crystal Oscillators**: 40MHz (main), 32.768kHz (RTC)
- **Voltage Regulators**: 3.3V LDO, 5V switching regulator
- **Antenna System**: Dual-band integrated antenna
- **USB-C Controller**: USB-C interface for programming and power

### Supporting Components
- **Flash Memory**: 8MB/16MB SPI Flash
- **SRAM**: 512KB (ESP32-S3) / 512KB (ESP32-C6)
- **PSRAM**: 8MB external PSRAM (ESP32-S3 only)
- **Real-time Clock**: Built-in RTC with battery backup
- **LED Indicators**: Power, WiFi, LoRa status LEDs
- **Reset Circuit**: Hardware reset with debouncing
- **USB-C Connector**: USB-C for programming and power

### Connectors & Interfaces
- **USB-C Connector**: USB-C for programming, power, and debugging
- **Power Connector**: 6-36V DC input + screw terminal
- **UART Connector**: 6-pin header (3.3V TTL)
- **RS485 Connector**: 3-pin terminal block (A, B, GND)
- **Relay Outputs**: 2x 3-pin terminal blocks (NO, NC, COM)
- **Analog Inputs**: 4x 3-pin terminal blocks (4-20mA/0-5V)
- **Pulse Counter**: 2x 2-pin terminal blocks
- **I2C Sensor**: 4-pin header (VCC, GND, SDA, SCL)
- **Antenna Connector**: SMA connector for external antenna
- **Battery Connector**: 2-pin JST connector

## 📖 Hardware Setup Guide

### 1. Initial Hardware Setup
- Review complete schematics in `schematic/BSEN_WIFI_IoT_public.pdf`
- Verify all components are properly soldered
- Check power supply voltage (5V-36V DC)
- Ensure proper antenna connection

### 2. Power Supply Configuration
- **USB-C Power**: 5V via USB-C connector (development)
- **DC Input**: 6-36V DC via screw terminal (industrial applications)
- **Battery Backup**: 3.7V Li-ion/Li-Po via JST connector
- **Power LED**: Green LED indicates power on
- **Status LED**: LED for system status indication
- **Voltage Monitoring**: Built-in voltage divider for monitoring

### 3. Interface Connections
- **USB-C**: Direct connection to PC for programming and debugging
- **UART**: Connect to PC via USB-to-Serial adapter (backup)
- **GPIO**: Use 20-pin header for sensor connections
- **I2C Sensors**: Connect digital sensors to I2C header (VCC, GND, SDA, SCL)
- **RS485 Sensors**: Connect Modbus sensors to RS485 terminal block
- **Analog Sensors**: Connect 4-20mA/0-5V sensors to analog input terminals
- **Relay Outputs**: Connect devices to relay terminal blocks (NO, NC, COM)
- **Pulse Counter**: Connect pulse-generating sensors to pulse counter terminals
- **SPI**: LoRa module uses dedicated SPI interface
- **JTAG**: Connect JTAG debugger for advanced debugging

### 4. Antenna Configuration
- **WiFi Antenna**: Integrated 2.4GHz antenna( or external antenna IPEX connector)
- **LoRa Antenna**: 8685MHz external antenna (IPEX connector)

## 🔧 Hardware Configuration

### Pin Configuration
```cpp
// WiFi Pins (ESP32-S3/ESP32-C6)
#define WIFI_EN_PIN    2
#define WIFI_RST_PIN    4

// LoRa Pins (SX1276/SX1278)
#define LORA_CS_PIN    15
#define LORA_RST_PIN   16
#define LORA_DIO0_PIN  5
#define LORA_DIO1_PIN  6
#define LORA_DIO2_PIN  7

// USB-C Pins (ESP32-S3/ESP32-C6)
#define USB_DM_PIN     19
#define USB_DP_PIN     20

// Relay Outputs
#define RELAY1_PIN     8
#define RELAY2_PIN     9

// RS485 Interface
#define RS485_TX_PIN   10
#define RS485_RX_PIN   11
#define RS485_EN_PIN   12

// Analog Inputs (4-20mA/0-5V)
#define ADC1_PIN       A0
#define ADC2_PIN       A1
#define ADC3_PIN       A2
#define ADC4_PIN       A3

// Pulse Counter Inputs
#define PULSE1_PIN     13
#define PULSE2_PIN     14

// I2C Interface
#define I2C_SDA_PIN    21
#define I2C_SCL_PIN    22
```


## 📊 Applications

### 🏠 Smart Home Applications
- **Sensor Nodes**: Temperature, humidity, motion sensors via I2C
- **Gateway Device**: WiFi-LoRa bridge for home automation
- **Security Systems**: Door/window sensors with LoRa backhaul
- **Device Control**: Relay outputs for lights, fans, appliances
- **Energy Monitoring**: Power consumption monitoring via RS485

### 🌾 Agricultural IoT
- **Soil Monitoring**: pH, moisture, nutrient sensors via analog inputs
- **Weather Stations**: Temperature, humidity, pressure monitoring
- **Irrigation Control**: Automated watering systems via relay outputs
- **Flow Monitoring**: Water flow sensors via pulse counter inputs
- **Crop Health**: Plant monitoring with LoRa mesh network

### 🏭 Industrial Applications
- **Machine Monitoring**: Vibration, temperature, pressure sensors via analog inputs
- **Process Control**: Relay outputs for pumps, valves, motors
- **Modbus Integration**: Industrial sensors via RS485 interface
- **Flow Measurement**: Flow sensors via pulse counter inputs
- **Environmental Monitoring**: Air quality, noise level monitoring
- **Predictive Maintenance**: Vibration analysis with LoRa transmission

### 🔬 Research & Development
- **Sensor Networks**: Distributed sensing applications
- **Prototyping**: Rapid IoT prototype development
- **Testing**: Radio frequency testing and validation
- **Education**: IoT and wireless communication learning

## 🛒 Hardware Purchase

### 🏪 Official Store
- **Website**: [store.hbqsolution.com](https://store.hbqsolution.com)
- **Product**: BSEN WIFI LORA IoT Development Board
- **Support**: Free technical consultation and hardware support

### 📦 Available Hardware
- ✅ **Complete Development Kit**: Board + antennas + cables + documentation
- ✅ **Accessory Kit**: Cables,antennas, and enclosure

### 🔧 Hardware Specifications
- **PCB Layers**: 2-layer FR4.
- **Surface Finish**: HASL (Hot Air Solder Leveling)
- **Testing**: 100% functional testing before shipment
- **Warranty**: 1-year hardware warranty

## 💝 Project Support

This project is developed by the community and we greatly appreciate your support!

### Support the Project
- PayPal Donate: [![PayPal Donate](https://img.shields.io/badge/PayPal-Donate-0070ba?logo=paypal&logoColor=white)](https://paypal.me/hbqtechnology)
- GitHub Sponsors : [![GitHub Sponsors](https://img.shields.io/badge/GitHub-Sponsors-ea4aaa?logo=github&logoColor=white)](https://github.com/sponsors/hbqtechnologycompany)

### 🎯 Other Ways to Support
- ⭐ Star this repository
- 🐛 Report bugs and suggest features
- 📝 Contribute documentation
- 🔄 Share project with community

## 📄 License

This project is released under **Public Domain** license. You are free to use, modify and distribute without permission.

## 👥 Contributing

We welcome all contributions from the community! Please:

1. Fork this repository
2. Create branch for new feature (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📞 Contact

- **Website**: [web.hbqsolution.com](www.web.hbqsolution.com)
- **Email**: support@hbqsolution.com / hbqsolution@gmail.com
- **GitHub**: [@hbqsolutioncompany](https://github.com/hbqsolutioncompany)
- **Store**: [store.hbqsolution.com](https://store.hbqsolution.com)

## 🙏 Acknowledgments

Thanks to all contributors and community who supported this project. Special thanks to:

- Arduino/ESP32 community
- LoRa community
- All developers who contributed code
- Testers and beta users

---

**⭐ If this project is helpful, please give us a star! ⭐**

*Developed with ❤️ by HBQ Solution Company*
