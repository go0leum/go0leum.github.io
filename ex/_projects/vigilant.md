---
layout: page
title: Vigilant-Construction Worker Safety Monitoring System
description: 
img: assets/img/vigilant.png
importance: 6
category: project
giscus_comments: false
---

[GitHub Repository](https://github.com/go0leum/vigilant_demo.git)

**Collaborators:**  
[Euna Cho](https://www.linkedin.com/in/euna-cho-b80707297/)

# 🛠️ Vigilant: Real-time Construction Safety System Powered by IoT and AI

### 📌 Enhancing Safety in Construction Sites with Technology


<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant.png" title="Thumnail" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

Construction sites remain one of the most dangerous working environments, accounting for nearly **44% of workplace fatalities in 2023**, with **falling accidents** being the leading cause. Despite policy efforts like the Serious Accidents Punishment Act in Korea, traditional monitoring methods still rely heavily on manual and visual checks.

This is where **Vigilant** comes in—a real-time safety monitoring system that integrates **wearable sensors, CCTV, AI fire detection, and a live dashboard** to help site managers detect accidents as they happen and respond immediately.

---

## 🎯 Project Objectives

Vigilant aims to build a smart, data-driven safety management system that can:

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant_accident.png" title="vigilant_accident detection description" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant_fire.png" title="vigilant_fire detection description" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

* **Monitor workers' vital signs and location** in real time using wearable devices
* **Detect fire hazards** via AI-powered CCTV analysis
* **Alert site managers immediately** when a fall, abnormal heart rate, or fire is detected
* **Visualize live worker data** on an interactive React dashboard

---

## 🧱 System Architecture

### 🧠 Hardware

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant_hardware.jpg" title="vigilant hardware design description" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

| Component          | Description                  |
| ------------------ | ---------------------------- |
| MCU                | Heltec Wireless Tracker v1.1 |
| Heart Rate Sensor  | SZH-HWS001                   |
| Accelerometer/Gyro | MPU6050                      |
| Camera             | ESP32-CAM                    |

### 🖥️ Software

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant_web_map.png" title="vigilant_web map description" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/vigilant_web_dashboard.png" title="vigilant_web dashboard detection description" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

| Layer          | Technology                    |
| -------------- | ----------------------------- |
| Frontend       | React.js (WebSocket-based)    |
| Backend        | Django, Django REST Framework |
| DB             | PostgreSQL                    |
| AI             | YOLOv8 Nano (PyTorch), OpenCV |
| Infrastructure | Docker, Nginx, HTTPS          |

---

## ⚙️ Key Features

### 🔹 Real-time Fall and Health Monitoring

* Detects **sudden falls** using accelerometer and gyroscope data
* Analyzes **heart rate anomalies** using physiological metrics like OI (Overwork Index)
* Local processing on ESP32 for fast decision-making using **Decision Tree algorithms**

### 🔹 AI-based Fire Detection

* Streams CCTV footage to YOLOv8 model for **flame and smoke detection**
* Sends alert to the dashboard within **1 second of detection**

### 🔹 Centralized Live Dashboard

* React-based UI showing **worker locations, health stats, and camera feeds**
* Admins receive **WebSocket push notifications** for emergencies
* All events are logged for **later review and accountability**

---

## 🔐 Security & Reliability

* **HTTPS encryption** with SSL/TLS
* **Role-based access control** (managers vs workers)
* **CSRF protection and session-based auth** via Django
* Real-time system designed to maintain **<1 sec latency**
* Offline detection and reconnection logic for unstable networks

---

## ✅ Expected Impact

* **Prevents accidents** by detecting early signs of fatigue, falls, and fire
* **Improves site management** by centralizing real-time data
* **Provides forensic data** in the event of a serious incident
* **Scalable** to other high-risk environments like logistics hubs, factories, and disaster response zones

---

## 🧩 Technical Challenges & Solutions

> “We didn’t just collect data. We built a real-time, event-driven platform to act on it.”

* Developed **low-latency WebSocket communication**
* Designed **lightweight AI and sensor-side analysis** suitable for low-power devices
* Tuned YOLOv8 to perform **fire detection** with >90% accuracy under 1 second
* Built **fully containerized infrastructure** with Docker & Nginx

---

## 👩‍💻 Why We Built This

Our team consists of students from **Construction Engineering** and **Applied Statistics**. We wanted to combine our disciplines and apply cutting-edge tech—**IoT, AI, and full-stack web development**—to a real-world problem with societal impact.

Vigilant is our response to the need for **smarter, faster, and more reliable safety solutions** on-site.

---

## 🔗 Conclusion

Construction work will always involve risks. But with systems like **Vigilant**, we can make those risks more manageable, measurable, and actionable.

> Tech doesn’t just automate tasks—it **saves lives**.

---