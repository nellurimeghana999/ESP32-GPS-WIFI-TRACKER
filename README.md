# ESP32 WiFi GPS Tracker 🌍

This project connects an ESP32 to WiFi and reads real-time GPS coordinates using a GPS module. The latitude and longitude are displayed in the Serial Monitor.

---

## 📌 Features

- Connects ESP32 to WiFi
- Displays assigned local IP address
- Reads GPS data using TinyGPSPlus library
- Prints real-time Latitude & Longitude
- Uses UART2 (GPIO16 & GPIO17)

---

## 🛠 Hardware Required

- ESP32 Dev Board
- GPS Module (Neo-6M or similar)
- Jumper Wires
- USB Cable

---

## 🔌 Pin Connections

| GPS Module | ESP32 |
|------------|--------|
| VCC        | 3.3V or 5V |
| GND        | GND |
| TX         | GPIO16 |
| RX         | GPIO17 |

---

## 📚 Libraries Required

Install from Arduino Library Manager:

- WiFi.h (built-in for ESP32)
- TinyGPSPlus

---

## 📡 WiFi Setup

Edit these lines in the code:

```cpp
const char* ssid = "YOUR_WIFI_NAME";
const char* password = "YOUR_WIFI_PASSWORD";
```

Replace with your actual WiFi name and password.

---

## ▶️ How It Works

1. ESP32 connects to WiFi
2. Prints local IP address
3. Initializes GPS module
4. Reads NMEA data
5. Extracts and prints latitude & longitude

---

## 📷 Output Example

```
WiFi Connected!
IP Address: 192.168.1.10

Latitude: 17.385044
Longitude: 78.486671
```

---

## 🚀 Future Improvements

- Send GPS data to web server
- Create live tracking webpage
- Send location to mobile app
- Store data in cloud

---

## 👨‍💻 Author

Your Name  
ESP32 + IoT Project
