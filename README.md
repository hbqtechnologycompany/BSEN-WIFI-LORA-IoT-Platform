# BSEN WIFI LORA IoT Platform

![BSEN WIFI LORA IoT Platform](https://img.shields.io/badge/Platform-IoT-blue)
![License](https://img.shields.io/badge/License-Public-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## 📋 Tổng quan dự án / Project Overview

**BSEN WIFI LORA IoT Platform** là một nền tảng IoT toàn diện kết hợp WiFi và LoRa để tạo ra một giải pháp kết nối mạng linh hoạt và mạnh mẽ. Dự án này được thiết kế để hỗ trợ các ứng dụng IoT từ cơ bản đến phức tạp, với khả năng kết nối đa dạng và quản lý dữ liệu hiệu quả.

**BSEN WIFI LORA IoT Platform** is a comprehensive IoT platform that combines WiFi and LoRa to create a flexible and powerful network connectivity solution. This project is designed to support IoT applications from basic to complex, with diverse connectivity capabilities and efficient data management.

## 🚀 Tính năng chính / Key Features

### 🌐 Kết nối đa dạng / Multi-Connectivity
- **WiFi**: Kết nối mạng không dây tốc độ cao / High-speed wireless network connection
- **LoRa**: Kết nối tầm xa, tiết kiệm năng lượng / Long-range, low-power connection
- **Dual-mode**: Hỗ trợ chuyển đổi linh hoạt giữa WiFi và LoRa / Flexible switching between WiFi and LoRa

### 📡 Giao tiếp IoT / IoT Communication
- Giao thức MQTT cho truyền thông real-time / MQTT protocol for real-time communication
- RESTful API cho quản lý thiết bị / RESTful API for device management
- WebSocket cho cập nhật dữ liệu thời gian thực / WebSocket for real-time data updates

### 🔧 Tính năng kỹ thuật / Technical Features
- **Microcontroller**: ESP32/ESP8266 tương thích / ESP32/ESP8266 compatible
- **LoRa Module**: SX1276/SX1278
- **Antenna**: Tối ưu cho cả WiFi và LoRa / Optimized for both WiFi and LoRa
- **Power Management**: Quản lý năng lượng thông minh / Smart power management
- **OTA Updates**: Cập nhật firmware từ xa / Remote firmware updates

## 📁 Cấu trúc dự án / Project Structure

```
BSEN-WIFI-LORA-IoT-Platform/
├── schematic/                    # Sơ đồ mạch điện tử / Circuit schematics
│   └── BSEN_WIFI_IoT_public.pdf # Sơ đồ chi tiết / Detailed schematics
├── firmware/                     # Mã nguồn firmware / Firmware source code
├── documentation/                # Tài liệu kỹ thuật / Technical documentation
├── examples/                     # Ví dụ sử dụng / Usage examples
└── README.md                     # Tài liệu này / This documentation
```

## 🛠️ Yêu cầu phần cứng / Hardware Requirements

### Linh kiện chính / Main Components
- **MCU**: ESP32 hoặc ESP8266 / ESP32 or ESP8266
- **LoRa Module**: SX1276/SX1278
- **Antenna**: 2.4GHz cho WiFi, 868/915MHz cho LoRa / 2.4GHz for WiFi, 868/915MHz for LoRa
- **Power Supply**: 3.3V/5V
- **Crystal**: 32.768kHz cho RTC / 32.768kHz for RTC

### Phụ kiện bổ sung / Additional Accessories
- Breadboard hoặc PCB / Breadboard or PCB
- Dây nối và connector / Wires and connectors
- Nguồn điện ổn định / Stable power supply
- Antenna ngoài (tùy chọn) / External antenna (optional)

## 📖 Hướng dẫn sử dụng / Usage Guide

### 1. Chuẩn bị phần cứng / Hardware Setup
- Tham khảo sơ đồ trong file `schematic/BSEN_WIFI_IoT_public.pdf` / Refer to schematics in `schematic/BSEN_WIFI_IoT_public.pdf`
- Lắp ráp theo hướng dẫn chi tiết / Assemble according to detailed instructions
- Kiểm tra kết nối trước khi cấp nguồn / Check connections before powering on

### 2. Cài đặt firmware / Firmware Installation
```bash
# Clone repository
git clone https://github.com/your-username/BSEN-WIFI-LORA-IoT-Platform.git

# Cài đặt Arduino IDE hoặc PlatformIO / Install Arduino IDE or PlatformIO
# Mở project và upload firmware / Open project and upload firmware
```

### 3. Cấu hình mạng / Network Configuration
- Kết nối WiFi / WiFi connection
- Cấu hình LoRa parameters / Configure LoRa parameters
- Thiết lập MQTT broker / Setup MQTT broker

## 🔧 Cấu hình / Configuration

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

## 📊 Ứng dụng / Applications

### 🏠 Smart Home
- Giám sát nhiệt độ, độ ẩm / Temperature and humidity monitoring
- Điều khiển thiết bị từ xa / Remote device control
- Báo động an ninh / Security alerts

### 🌾 Nông nghiệp thông minh / Smart Agriculture
- Giám sát đất và cây trồng / Soil and crop monitoring
- Tưới tiêu tự động / Automatic irrigation
- Dự báo thời tiết / Weather forecasting

### 🏭 Công nghiệp 4.0 / Industry 4.0
- Giám sát máy móc / Machine monitoring
- Bảo trì dự đoán / Predictive maintenance
- Quản lý kho bãi / Warehouse management

## 🛒 Mua hàng / Purchase

### 🏪 Cửa hàng chính thức / Official Store
- **Website**: [store.hbqsolution.com](https://store.hbqsolution.com)
- **Sản phẩm**: Kit phát triển BSEN WIFI LORA IoT / **Product**: BSEN WIFI LORA IoT Development Kit
- **Hỗ trợ**: Tư vấn kỹ thuật miễn phí / **Support**: Free technical consultation

### 📦 Sản phẩm có sẵn / Available Products
- ✅ Kit phát triển hoàn chỉnh / Complete development kit
- ✅ Module LoRa riêng lẻ / Individual LoRa module
- ✅ Antenna chuyên dụng / Specialized antenna
- ✅ Cáp kết nối và phụ kiện / Connection cables and accessories

## 💝 Hỗ trợ dự án / Project Support

Dự án này được phát triển bởi cộng đồng và chúng tôi rất biết ơn sự hỗ trợ của bạn! / This project is developed by the community and we greatly appreciate your support!

### 💰 Quyên góp qua GitHub / Donate via GitHub
[![GitHub Sponsors](https://img.shields.io/badge/GitHub-Sponsors-ea4aaa?logo=github&logoColor=white)](https://github.com/sponsors/hbqsolutioncompany)

### 💳 Quyên góp qua PayPal / Donate via PayPal
[![PayPal](https://img.shields.io/badge/PayPal-Donate-0070ba?logo=paypal&logoColor=white)](https://paypal.me/hbqsolutioncompany)

### 🎯 Cách hỗ trợ khác / Other Ways to Support
- ⭐ Star repository này / Star this repository
- 🐛 Báo cáo bug và đề xuất tính năng / Report bugs and suggest features
- 📝 Đóng góp tài liệu / Contribute documentation
- 🔄 Chia sẻ dự án với cộng đồng / Share project with community

## 📄 Giấy phép / License

Dự án này được phát hành dưới giấy phép **Public Domain**. Bạn có thể tự do sử dụng, chỉnh sửa và phân phối mà không cần xin phép. / This project is released under **Public Domain** license. You are free to use, modify and distribute without permission.

## 👥 Đóng góp / Contributing

Chúng tôi hoan nghênh mọi đóng góp từ cộng đồng! Hãy: / We welcome all contributions from the community! Please:

1. Fork repository này / Fork this repository
2. Tạo branch cho tính năng mới / Create branch for new feature (`git checkout -b feature/AmazingFeature`)
3. Commit thay đổi / Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push lên branch / Push to branch (`git push origin feature/AmazingFeature`)
5. Mở Pull Request / Open Pull Request

## 📞 Liên hệ / Contact

- **Website**: [hbqsolution.com](https://hbqsolution.com)
- **Email**: support@hbqsolution.com
- **GitHub**: [@hbqsolutioncompany](https://github.com/hbqsolutioncompany)
- **Store**: [store.hbqsolution.com](https://store.hbqsolution.com)

## 🙏 Lời cảm ơn / Acknowledgments

Cảm ơn tất cả các contributor và cộng đồng đã hỗ trợ dự án này. Đặc biệt cảm ơn: / Thanks to all contributors and community who supported this project. Special thanks to:

- Cộng đồng Arduino/ESP32 / Arduino/ESP32 community
- Cộng đồng LoRa / LoRa community
- Tất cả các developer đã đóng góp code / All developers who contributed code
- Các tester và người dùng beta / Testers and beta users

---

**⭐ Nếu dự án này hữu ích, hãy cho chúng tôi một star! ⭐** / **⭐ If this project is helpful, please give us a star! ⭐**

*Được phát triển với ❤️ bởi HBQ Solution Company* / *Developed with ❤️ by HBQ Solution Company*
