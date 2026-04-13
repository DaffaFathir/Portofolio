# 🌊 Early Warning System (EWS) Sukapura - Final Project

A comprehensive water level monitoring and flood early warning system for the Sukapura River area. This project consists of two main components: a **Web Dashboard** for real-time data visualization and a **Telegram Bot** for automated emergency notification systems.

---

## 📖 Project Overview
**Early Warning System (EWS) Sukapura** is an **IoT (Internet of Things)** based flood mitigation solution specifically designed for residential areas and the Telkom University campus near the Sukapura River. The project integrates physical monitoring, cloud-based data processing, and instantaneous real-time information dissemination.



### 🎯 Project Objectives
The primary goal of this system is to enhance community resilience against flooding through:

* **Proactive Emergency Response**: Establishing a significant "lead time" to allow residents to execute evacuation plans and secure critical assets before floodwaters reach dangerous levels.


* **Reliable Data Transparency**: Providing a single, centralized source of truth for water level data, accessible 24/7 to ensure the community remains informed with verified information.

* **Automated Alert Precision**: Minimizing human latency and error by deploying an autonomous 24/7 bot system that delivers instantaneous, status-based emergency notifications.


* **Informed Decision Making**: Empowering authorities and residents with historical trend analysis to better understand flood patterns and improve future mitigation strategies.

---

## 🏗️ System Architecture
The project adopts a modern system architecture divided into four main layers:

| Layer | Component | Description |
| :--- | :--- | :--- |
| **1. Acquisition** | Ultrasonic Sensor | Continuously measures water surface distance at strategic points. |
| **2. Cloud Intelligence** | Supabase (PostgreSQL) | Stores historical data and streams data in real-time (zero delay). |
| **3. Presentation** | Web Dashboard | React interface to monitor water level charts and sensor health. |
| **4. Alerting** | Telegram Bot | Emergency communication channel providing automated push notifications. |

---
