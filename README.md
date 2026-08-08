# Real-Time Smart Energy Meter with Sensor-Based Monitoring, In-Device Payment, and NILM Load Analytics



> 🏆 **Awards:** 
> * **1st Place** at the State-Level Project Exhibition (PESCE, Mandya).
> * **3rd Place** at the DSATM Hackathon (Bangalore).
> * **Best Project** at BMS College of Engineering (BMSCE, Bangalore).
> * **Presented at the 2026 International Conference on Electric Power and Renewable Energy (EPREC)** at IIT Bhilai.
> * **Filed Patent**

An end-to-end IoT-driven smart grid solution that delivers real-time energy analytics, regional slab-based automated billing, neighbor-aware fault diagnostics, dynamic UPI QR-code payments, and Machine Learning-powered **Non-Intrusive Load Monitoring (NILM)** to track individual device states from a single point of measurement.

---

## 📌 Key Features

* **Real-Time Sensing:** High-resolution AC voltage (ZMPT101B) and current (ZMCT103C) tracking computed at $\pm 5\%$ accuracy via an ESP32 microcontroller.
* **NILM Machine Learning:** Disaggregates total energy consumption using ML to identify exactly *when* specific appliances (e.g., LED, charger, heavy loads) turn ON or OFF.
* **Neighbor-Aware Outage Detection:** Cross-checks grid status against a secondary neighboring node to distinguish between a localized home blowout (e.g., blown fuse) and a wide-scale grid blackout.
* **Dynamic Slab Billing:** Automates real-time cost generation based on custom residential and commercial electricity tariffs.
* **In-Device UPI Payments:** Generates automated QR codes dynamically inside the Node-RED dashboard for instant checkout via Google Pay or PhonePe.
* **Proactive Twilio Alerts:** Dispatches instantaneous SMS text updates (< 600ms latency) during over-voltage, under-voltage, or threshold breaches.
* **Persistent Data Logging:** Saves historical consumption to CSV format for trend reviews and predictive analytics.

---


## 🏗 System Architecture

The project features a unified, multi-layered framework combining physical edge sensors, light telemetry messaging protocols, cloud computing dashboards, and Python ML pipelines.
Below is the system architecture of smart meter integrated with its core sensing subsystems:

<p align="center">
  <img src="Block Diagram" alt="Hardware Circuit Assembly" width="600">
</p>
NILM Model Device Event Analytics
The following charts illustrate the output graphs generated from the NILM model, tracing total current consumption changes and identifying exact appliance event states (ON/OFF transients):
---
<p align="center">
  <img src="NILM output1" alt="NILM Model Output Graphs" width="700">
</p>

---
<p align="center">
  <img src="NILM output2" alt="NILM Model Output Graphs" width="700">
</p>

---
<p align="center">
  <img src="Transient response of the system" alt="NILM Model Output Graphs" width="700">
</p>

---

## 🛠 Hardware Components

* **ESP32 Development Board:** Dual-core processor handling high-frequency ADC sampling and Wi-Fi transmission.
* **ZMPT101B Voltage Sensor Module:** Provides isolated, safe step-down signals proportional to AC mains voltage.
* **ZMCT103C Current Transformer:** Micro precision current tracking calibrated safely up to 5A loads.


---

## 💻 Software

* **Firmware:** C++ / Arduino IDE utilizing the optimized `EmonLib` library.
* **Broker:** HiveMQ Cloud (Lightweight, low-latency MQTT publisher/subscriber infrastructure).
* **Gateway/UI:** Node-RED flow orchestration for real-time visualization graphs and webhooks.
* **NILM Plotting Engine:** Google Collab 

---

## 📊 Performance Data & Calibration

Testing against standard industrial multimeters and commercial-grade meters shows highly reliable operational safety metrics:

| Electrical Parameter | Reference Reading | Smart Meter Reading | Error (E%) | Accuracy (A%) |
| :--- | :--- | :--- | :--- | :--- |
| **Voltage (Vrms)** | 217.49 V | 219.88 V | +1.14% | 98.86% |
| **Current (Irms)** | 0.0877 A | 0.0855 A | -2.47% | 97.53% |
| **Real Power** | 19.27 W | 18.81 W | -2.43% | 97.57% |
| **Energy (1 Hour)** | 1.392 Wh | 1.362 Wh | -2.16% | 97.84% |



## 📜 Authors & Contrubutors
* **Sumaiya MN** - *Department of ECE, DSATM, Bangalore* - drsumaiyamn@dsatm.edu.in
* **Abhishek H.J** - *Department of ECE, DSATM, Bangalore* - abhishekhj12@gmail.com
* **Hemanth Kumar M.M** - *Department of ECE, DSATM, Bangalore* - hemanthkumar.mm07@gmail.com
* **Anirudh H.S** - *Department of ECE, DSATM, Bangalore* - anirudhhs11@gmail.com
