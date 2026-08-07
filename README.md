# ☁️ Cloud-Connected Environmental Data Logger with Excel Reporting

## 📌 Project Overview

Environmental conditions such as temperature and gas concentration play a critical role in industries, warehouses, laboratories, hospitals, and smart agriculture. Manual monitoring of these parameters is time-consuming and may lead to delayed responses during abnormal conditions.

This project presents a **Cloud-Connected Environmental Data Logger with Excel Reporting**, developed using the **LPC2148 ARM7 Microcontroller**. The system continuously monitors **temperature and smoke levels** using the **LM35** and **MQ2** sensors, displays the readings on a **16×2 LCD**, uploads the data to the **ThingSpeak cloud** through the **ESP-01 Wi-Fi module**, and automatically stores the collected data in **Microsoft Excel** for future analysis.

The project demonstrates the integration of **Embedded Systems**, **IoT**, **Cloud Connectivity**, and **Data Logging**, providing a reliable solution for real-time environmental monitoring.

---

## 🎯 Objectives

| Objective | Description |
|------------|-------------|
| 🌡️ Temperature Monitoring | Monitor environmental temperature in real time |
| 🔥 Smoke Detection | Detect smoke using the MQ2 sensor |
| ☁️ Cloud Connectivity | Upload sensor data to ThingSpeak using the ESP-01 Wi-Fi module |
| 📊 Excel Data Logging | Store sensor data in Microsoft Excel for future analysis |
| 🖥️ LCD Display | Display live sensor readings on a 16×2 LCD |
| ⏰ Time Stamping | Record sensor data with date and time using the RTC module |
| 🚨 Alert System | Activate the buzzer when the smoke level exceeds the threshold |
| 🌐 Remote Monitoring | Enable users to monitor environmental conditions from anywhere through the cloud |

---

## 🧰 Hardware Components

| Component | Quantity | Purpose |
|-----------|:--------:|---------|
| LPC2148 ARM7 Microcontroller | 1 | Main controller that reads sensor data, processes it, and controls the system |
| LM35 Temperature Sensor | 1 | Measures ambient temperature |
| MQ2 Gas Sensor | 1 | Detects smoke and harmful gases |
| ESP-01 (ESP8266) Wi-Fi Module | 1 | Uploads sensor data to the ThingSpeak cloud |
| DS1307 RTC Module | 1 | Provides real-time date and time for data logging |
| 16×2 LCD Display | 1 | Displays real-time temperature and smoke readings. |
| Matrix Keypad | 1 | Used to configure the temperature threshold |
| Buzzer | 1 | Alerts the user when smoke exceeds the threshold |
| Crystal Oscillator | 1 | Provides the clock signal for the LPC2148 microcontroller |
| Regulated Power Supply | 1 | Supplies stable power to the complete system |

---

## 💻 Software Requirements

| Software | Purpose |
|-----------|---------|
| Keil µVision 4 | Embedded C code development and compilation |
| Flash Magic | Upload the compiled program to the LPC2148 microcontroller |
| Embedded C | Programming language used for firmware development |
| ThingSpeak | Cloud platform for remote sensor data monitoring |
| Microsoft Excel | Stores and analyzes logged sensor data |

---

## 🏗️ System Architecture

<p align="center">
  <img src="BLOCK DIAGRAM.png" alt="Cloud Connected Environmental Data Logger Block Diagram" width="1000">
</p>

The system is built around the **LPC2148 ARM7 Microcontroller**, which serves as the central controller. The **LM35 temperature sensor** and **MQ2 gas sensor** continuously monitor environmental conditions and send their readings to the microcontroller. The measured values are displayed on the **16×2 LCD** for local monitoring.

The **RTC module** provides accurate date and time information for timestamping each sensor reading. The **ESP-01 Wi-Fi module** transmits the collected data to the **ThingSpeak cloud platform**, allowing users to monitor environmental conditions remotely. The uploaded data is also recorded in **Microsoft Excel** for future analysis and reporting. Whenever the smoke level exceeds the predefined threshold, the system activates the **buzzer** to alert nearby users.

---

---

## 🔄 Working Principle

The Cloud-Connected Environmental Data Logger continuously monitors environmental conditions, displays real-time readings on the LCD, uploads the collected data to the ThingSpeak cloud, and stores the readings in Microsoft Excel for analysis.

