#  IoT-Based Multi-Gas Monitoring System with ESP32-CAM

An open-source IoT project for real-time multi-gas monitoring using **XIAO ESP32C3** and **ESP32-CAM**.

---

##  Features

-  4-channel gas monitoring
-  Live ESP32-CAM video streaming
-  Real-time web dashboard
-  JSON API support
-  LED alert system
-  WiFi-enabled monitoring
-  Custom EasyEDA PCB

---

##  Hardware Components

| Component | Purpose |
|---|---|
| XIAO ESP32C3 | Main controller |
| ESP32-CAM | Video streaming |
| MQ2 | LPG / Smoke |
| MQ3 | Alcohol detection |
| MQ5 | Natural Gas |
| MQ9 | Carbon Monoxide |
| LEDs + Resistors | Alert indicators |
| ZTX450STZ | LED driver transistor |

---

## 🔌 Pin Connections

| Pin | Device |
|---|---|
| D0 | MQ2 |
| D1 | MQ3 |
| D2 | MQ5 |
| D3 | MQ9 |
| D4 | LED Driver |

---

##  Project Structure

```text
ESP32C3_GasMonitor/
├── src/main.ino
└── include/config.h

ESP32CAM_Stream/
└── src/ESP32CAM_Stream.ino
```

---

## Gas Thresholds

| Sensor | Threshold |
|---|---|
| MQ2 | 1500 |
| MQ3 | 1200 |
| MQ5 | 1300 |
| MQ9 | 1400 |

---

##  Setup

1. Install Arduino IDE  
2. Install ESP32 board package  
3. Configure WiFi in `config.h`
4. Upload firmware to:
   - XIAO ESP32C3
   - ESP32-CAM

---

##  JSON API Example

```json
{
  "mq2": 1320,
  "mq3": 980,
  "mq5": 1105,
  "mq9": 870,
  "alert": false
}
```

---

##  PCB Details

- Designed in **EasyEDA**
- REV 1.0
- 5V Powered
- Grove XH2.54-4PIN connectors

---

##  Services

If you want to scale your IoT product with professional<a href="https://digitalmonk.biz/electronics-embedded-software-development-services/"> Embedded Software Development Services</a>, feel free to connect for custom firmware, PCB design, and hardware solutions.

---

##  License

Licensed under **MIT License**




