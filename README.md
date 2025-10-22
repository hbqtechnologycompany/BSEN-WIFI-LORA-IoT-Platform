# BSEN WIFI LORA IoT Platform

![BSEN WIFI LORA IoT Platform](https://img.shields.io/badge/Platform-IoT-blue)
![License](https://img.shields.io/badge/License-Public-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## 📋 Project Overview

**BSEN WIFI LORA IoT Platform** is a comprehensive IoT platform that combines WiFi and LoRa to create a flexible and powerful network connectivity solution. This project is designed to support IoT applications from basic to complex, with diverse connectivity capabilities and efficient data management.

## 🚀 Key Features

### 🌐 Multi-Connectivity
- **WiFi**: High-speed wireless network connection
- **LoRa**: Long-range, low-power connection
- **Dual-mode**: Flexible switching between WiFi and LoRa

### 📡 IoT Communication
- MQTT protocol for real-time communication
- RESTful API for device management
- WebSocket for real-time data updates

### 🔧 Technical Features
- **Microcontroller**: ESP32/ESP8266 compatible
- **LoRa Module**: SX1276/SX1278
- **Antenna**: Optimized for both WiFi and LoRa
- **Power Management**: Smart power management
- **OTA Updates**: Remote firmware updates

## 📁 Project Structure

```
BSEN-WIFI-LORA-IoT-Platform/
├── schematic/                    # Circuit schematics
│   └── BSEN_WIFI_IoT_public.pdf # Detailed schematics
├── firmware/                     # Firmware source code
├── documentation/                # Technical documentation
├── examples/                     # Usage examples
└── README.md                     # This documentation
```

## 🛠️ Hardware Requirements

### Main Components
- **MCU**: ESP32 or ESP8266
- **LoRa Module**: SX1276/SX1278
- **Antenna**: 2.4GHz for WiFi, 868/915MHz for LoRa
- **Power Supply**: 3.3V/5V
- **Crystal**: 32.768kHz for RTC

### Additional Accessories
- Breadboard or PCB
- Wires and connectors
- Stable power supply
- External antenna (optional)

## 📖 Usage Guide

### 1. Hardware Setup
- Refer to schematics in `schematic/BSEN_WIFI_IoT_public.pdf`
- Assemble according to detailed instructions
- Check connections before powering on

### 2. Firmware Installation
```bash
# Clone repository
git clone https://github.com/your-username/BSEN-WIFI-LORA-IoT-Platform.git

# Install Arduino IDE or PlatformIO
# Open project and upload firmware
```

### 3. Network Configuration
- WiFi connection
- Configure LoRa parameters
- Setup MQTT broker

## 🔧 Configuration

### WiFi Settings
```cpp
const char* ssid = "YOUR_WIFI_SSID";
const char* password = "YOUR_WIFI_PASSWORD";
```

### LoRa Settings
```cpp
#define LORA_FREQUENCY 868E6  // 868 MHz
#define LORA_TX_POWER 14      // 14 dBm
#define LORA_SPREADING_FACTOR 7
```

## 📊 Applications

### 🏠 Smart Home
- Temperature and humidity monitoring
- Remote device control
- Security alerts

### 🌾 Smart Agriculture
- Soil and crop monitoring
- Automatic irrigation
- Weather forecasting

### 🏭 Industry 4.0
- Machine monitoring
- Predictive maintenance
- Warehouse management

## 🛒 Purchase

### 🏪 Official Store
- **Website**: [store.hbqsolution.com](https://store.hbqsolution.com)
- **Product**: BSEN WIFI LORA IoT Development Kit
- **Support**: Free technical consultation

### 📦 Available Products
- ✅ Complete development kit
- ✅ Individual LoRa module
- ✅ Specialized antenna
- ✅ Connection cables and accessories

## 💝 Project Support

This project is developed by the community and we greatly appreciate your support!

### 💰 Donate via GitHub
[![GitHub Sponsors](https://img.shields.io/badge/GitHub-Sponsors-ea4aaa?logo=github&logoColor=white)](https://github.com/sponsors/hbqsolutioncompany)

### 💳 Donate via PayPal
[![PayPal](https://img.shields.io/badge/PayPal-Donate-0070ba?logo=paypal&logoColor=white)](https://paypal.me/hbqsolutioncompany)

### 🎯 Other Ways to Support
- ⭐ Star this repository
- 🐛 Report bugs and suggest features
- 📝 Contribute documentation
- 🔄 Share project with community

## 📄 License / Giấy phép

This project is released under **Public Domain** license. You are free to use, modify and distribute without permission. / Dự án này được phát hành dưới giấy phép **Public Domain**. Bạn có thể tự do sử dụng, chỉnh sửa và phân phối mà không cần xin phép.

## 👥 Contributing / Đóng góp

We welcome all contributions from the community! Please: / Chúng tôi hoan nghênh mọi đóng góp từ cộng đồng! Hãy:

1. Fork this repository / Fork repository này
2. Create branch for new feature / Tạo branch cho tính năng mới (`git checkout -b feature/AmazingFeature`)
3. Commit changes / Commit thay đổi (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch / Push lên branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request / Mở Pull Request

## 📞 Contact / Liên hệ

- **Website**: [hbqsolution.com](https://hbqsolution.com)
- **Email**: support@hbqsolution.com
- **GitHub**: [@hbqsolutioncompany](https://github.com/hbqsolutioncompany)
- **Store**: [store.hbqsolution.com](https://store.hbqsolution.com)

## 🙏 Acknowledgments / Lời cảm ơn

Thanks to all contributors and community who supported this project. Special thanks to: / Cảm ơn tất cả các contributor và cộng đồng đã hỗ trợ dự án này. Đặc biệt cảm ơn:

- Arduino/ESP32 community / Cộng đồng Arduino/ESP32
- LoRa community / Cộng đồng LoRa
- All developers who contributed code / Tất cả các developer đã đóng góp code
- Testers and beta users / Các tester và người dùng beta

---

**⭐ If this project is helpful, please give us a star! ⭐** / **⭐ Nếu dự án này hữu ích, hãy cho chúng tôi một star! ⭐**

*Developed with ❤️ by HBQ Solution Company* / *Được phát triển với ❤️ bởi HBQ Solution Company*
