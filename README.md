# Water-Quality-Analysis-using-IOT
# 💧 Real-Time Water Quality Analysis using IoT

![Project Banner](https://img.shields.io/badge/IoT-Water--Quality--Monitoring-blue?style=for-the-badge)
  
This project is a **real-time IoT system for monitoring water quality** using sensors and cloud integration. Built using ESP8266, TDS sensor, and Firebase, this system helps analyze water quality parameters and alerts users in real time.

---

## 📸 Project Images

### 1. IoT Device Setup
![WhatsApp Image 2025-05-24 at 11 56 43_185b3981](https://github.com/user-attachments/assets/86f7bf5c-c6bf-42a2-8057-86c75c2d2428)


### 2. Firebase Realtime Database
![WhatsApp Image 2025-05-24 at 11 56 43_5b71f1b3](https://github.com/user-attachments/assets/8411614b-8bf1-4d63-a845-8a71f6484427)


---

## 🔧 Components Used

| Component        | Description                            |
|------------------|----------------------------------------|
| ESP8266 NodeMCU  | Microcontroller with WiFi capability   |
| TDS Sensor       | Measures Total Dissolved Solids        |
| pH Sensor (Optional) | Measures pH level of water         |
| DHT11 Sensor     | Temperature and Humidity readings      |
| Jumper Wires     | For circuit connection                 |
| Firebase         | For real-time cloud data storage       |

---

## ⚙️ How It Works

1. Sensors collect water data (e.g., TDS, temperature).
2. ESP8266 reads the data and sends it to Firebase in real-time.
3. Data is stored in Firebase Realtime Database.
4. A front-end dashboard (optional) or LCD can be used to visualize readings.
5. Alerts can be configured based on thresholds.

---

## 🚀 How to Recreate This Project

### 🔌 Hardware Setup

1. Connect TDS sensor → A0 pin of ESP8266  
2. Connect DHT11 → Digital pin (e.g., D2)  
3. Power up using USB or battery module  
4. Install Arduino IDE + add ESP8266 board package

### 💻 Arduino Code Setup

1. Install libraries:
   - `FirebaseESP8266.h`
   - `DHT.h`

2. Update your Firebase credentials and WiFi SSID/password in the code.

3. Upload the code using Arduino IDE.

### ☁️ Firebase Configuration

1. Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com/)
2. Enable Realtime Database
3. Set rules to:
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}

