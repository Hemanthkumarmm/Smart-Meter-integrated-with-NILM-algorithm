# 📡 Real-time Cloud-based Smart Energy Meter

A smart IoT-based energy monitoring system that measures real-time energy usage and sends data to the cloud for live monitoring, visualization, and analysis.

---

## 🚀 Project Overview
This project implements a **Real-time Smart Energy Meter** using IoT technologies.  
It measures:

- Voltage  
- Current  
- Power  
- Energy consumption  

The system uploads all measurements to the cloud and helps users:

- Track their energy usage  
- Detect abnormalities  
- Optimize power consumption  

---

## 🧩 Features

### 📊 Real-time measurement of:
- Voltage  
- Current  
- Power  
- Energy consumption  

### Additional Features
- ☁️ Cloud integration for live data logging  
- 📱 Web / mobile dashboard for visualization  
- ⚡ Alerts for abnormal readings  
- 📶 Wireless data transfer (Wi-Fi / ESP32)  
- 🔐 Secure and scalable cloud storage  
- 💡 Low-cost, easy-to-build hardware  

---

## 🛠️ Hardware Components

| Component | Description |
|----------|-------------|
| **ESP32 / ESP8266** | Main microcontroller with Wi-Fi |
| **Current Sensor (ACS712 / SCT-013)** | Measures current |
| **Voltage Sensor (ZMPT101B)** | Measures line voltage |
| **LCD / OLED Display** | Optional local display |
| **Power Supply** | 5V / 12V |
| **Wires, Resistors, PCB** | Circuit setup |

---

## 🧪 Software & Cloud Requirements

- **Arduino IDE**  
- **MQTT Broker (HiveMQ)**  
- **Node-RED Dashboard**  

---

## 🔧 System Architecture

1. Sensors collect real-time voltage and current values.  
2. Microcontroller calculates **power** and **energy usage**.  
3. Data is sent to the **cloud** using Wi-Fi and MQTT.  
4. Node-RED dashboard visualizes the readings.  
5. Users can detect overloads, monitor trends, and track consumption.  
6. Optional:  
   - Machine-learning-based load forecasting  
   - Billing and cost estimation  

---

## 📷 Circuit Diagram

<img width="430" height="290" alt="Circuit Diagram" src="https://github.com/user-attachments/assets/9da932cb-3450-4fd9-ba3a-1faac306a1ce" />

---

## 📈 Results

- Accurate real-time energy monitoring  
- Smooth cloud integration  
- Visualization of power usage trends  
- Alerts for abnormal spikes  

---

## 🧭 Future Improvements

- Predictive maintenance  
- Integration with home automation systems  
- Mobile app support  

---
