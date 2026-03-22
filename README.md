# 💧 AquaSense — Smart Water Usage Monitoring System

> **IoT-Based Intelligent Water Conservation, Leak Detection & Fault-Tolerant Monitoring System**

[![Department](https://img.shields.io/badge/Department-Computer%20Science%20%26%20Engineering-blue)](.)
[![College](https://img.shields.io/badge/College-KMEA%20Engineering%20College-blue)](.)
[![Course](https://img.shields.io/badge/Course-Engineering%20Entrepreneurship%20%26%20IPR-teal)](.)
[![Status](https://img.shields.io/badge/Status-Business%20Plan%20Submitted-green)](.)

---

## 📌 Overview

**AquaSense** is a smart water usage monitoring platform that uses **IoT sensors**, **AI/ML algorithms**, and **cloud computing** to monitor, detect, and optimize water consumption in real time — for homes, commercial buildings, industries, and municipalities.

Unlike conventional IoT water monitors that fail silently under unknown interference, AquaSense incorporates a **four-layer Fault Tolerance & Resilience Framework** that ensures the system always detects, classifies, and communicates every disruption — even ones it has never seen before.

---

## 🚨 The Problem We Solve

Traditional IoT water systems fail in three dangerous ways when an unknown external event occurs:

- **Goes Silent** — stops receiving data and assumes everything is normal
- **Misclassifies** — confuses an unknown event with a known pattern
- **Crashes** — entire system halts with no alerts or automation

> *"A third party manually closes the external water supply valve. Flow sensors read zero. Pressure also drops. The system cannot distinguish this from 'all taps off' — so it raises no alert. The user has no water and no idea why."*

AquaSense solves this with a **four-layer fault tolerance system** that ensures the system **NEVER fails silently**.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 💧 Real-Time Monitoring | Live water flow data from every tap and zone, updated every second |
| 🚨 Instant Leak Alerts | Detects leaks as small as 0.1 L/min before damage occurs |
| 🔒 Auto Valve Shut-Off | Smart motorized valve auto-closes on severe leak or unknown event |
| 🧠 Unknown Anomaly Detection | Autoencoder Neural Network flags events that don't match any known pattern |
| ⏱️ Watchdog Heartbeat | Monitors every sensor every 30 seconds — alerts if any sensor goes silent |
| 📡 Multi-Sensor Cross-Validation | Cross-checks all sensors before any action is taken |
| 🔋 Redundant Backup | WiFi → 4G → LoRaWAN → Edge AI failover ensures zero silent failures |
| 📊 Monthly AI Reports | Personalized savings reports, conservation tips, and fault event logs |
| 🌱 Sustainability Score | Track water footprint and earn conservation badges |

---

## 🏗️ System Architecture

AquaSense operates on a **four-layer architecture**:

```
Layer 1 — SENSING
    Ultrasonic flow sensors + Pressure sensors + Smart valve
    Each sensor sends heartbeat ping every 30 seconds

Layer 2 — CONNECTIVITY (Redundant Stack)
    Primary  : WiFi + Zigbee mesh
    Backup 1 : 4G SIM (auto-activates if WiFi drops)
    Backup 2 : LoRaWAN (operates even when WiFi + 4G fail)
    Offline  : Edge AI on gateway (runs locally, syncs on reconnect)

Layer 3 — CLOUD INTELLIGENCE (AI Engine)
    Baseline Profiling    → 7-day learning of normal usage patterns
    Known Anomaly         → Isolation Forest (leaks, high usage, dry pipe)
    Unknown Anomaly       → Autoencoder Neural Network
    Watchdog Monitor      → Heartbeat tracker, 2-min timeout alert
    Cross-Validation      → Multi-sensor contradiction detection

Layer 4 — USER INTERFACE
    Mobile App (Android & iOS)
    Web Dashboard (commercial clients)
    SMS Alerts (backup for critical events)
    System Health Panel (Active / Degraded / Dead / Unknown Event)
```

---

## 🛡️ Fault Tolerance Framework (Core Innovation)

### 4 Integrated Mechanisms

#### 1. 🧠 AI Anomaly Detection for Unknown Events
- **Autoencoder Neural Network** learns normal patterns, then flags anything unrecognizable
- 5-state classification: `Normal` | `Known Leak` | `Known High Usage` | `Known Dry Pipe` | `Unknown Interference`
- Unknown events trigger: *"Unrecognized event detected — please inspect physically"*

#### 2. ⏱️ Watchdog Heartbeat System
Every sensor pings the cloud every **30 seconds** independently of data.

| State | Condition | Response |
|---|---|---|
| 🟢 Active | Heartbeat received; data normal | Continue monitoring |
| 🟡 Degraded | Heartbeat received; data suspicious | Flag + alert user |
| 🔴 Dead/Tampered | No heartbeat for 2+ minutes | **ALERT: Sensor offline** |

#### 3. 📡 Multi-Sensor Cross-Validation

| Flow | Pressure | Valve | Heartbeat | Conclusion |
|---|---|---|---|---|
| Zero | Normal | Open | Active | ⚠️ UNKNOWN: Pipe blocked |
| Zero | Zero | Open | Active | ⚠️ UNKNOWN: External supply cut |
| High | Dropping | Open | Active | 💧 Known: Leak detected |
| Zero | Zero | Closed | Active | ✅ Normal: User closed valve |
| Any | Any | Any | Dead | 🚨 CRITICAL: Sensor offline |

#### 4. 🔋 Redundant Power & Communication

| Layer | Technology | When Active |
|---|---|---|
| Primary | WiFi + Cloud AI | Normal operation |
| Backup 1 | 4G SIM | WiFi drops |
| Backup 2 | LoRaWAN | WiFi + 4G fail |
| Offline | Edge AI on Gateway | All internet down |
| Restore | Auto cloud sync | Internet restored |

---

## 🔄 How It Works

```
Client Subscribes
    ↓
Hardware Kit Shipped (48 hours)
    ↓
Sensors Installed (30 min, no pipe cutting)
    ↓
7-Day AI Baseline Learning Phase
    ↓
Active Monitoring Begins:
    ├── Watchdog heartbeat check (every 30s)
    ├── Cross-validation check (every 5 min)
    ├── Known anomaly scan (real-time)
    └── Unknown anomaly scan (every 5 min)
    ↓
Alert / Auto Valve Close / Edge AI Fallback
    ↓
Monthly AI Report: Savings + Fault Event Log
```

---

## 💰 Pricing Plans

| Plan | Target | Price | Key Features |
|---|---|---|---|
| **Home** | Households | ₹199/month | 1 zone, leak alerts, mobile app |
| **Plus** | Apartments & Villas | ₹499/month | 5 zones, auto valve, 4G backup |
| **Pro** | Hotels, Hospitals, Offices | ₹1,999/month | 20 zones, all 4 resilience layers |
| **City** | Municipalities | Custom | City-scale, full redundancy, Govt. reporting |

---

## 📈 Market Opportunity

- 🌍 Global Smart Water Management market: **USD 18B (2025) → USD 42B (2030)** at 18–22% CAGR
- 🇮🇳 India market growing at **40%+ CAGR**, driven by Jal Jeevan Mission & Smart City projects
- 🏙️ Urban water distribution losses in India: **35–50%** — directly addressable by AquaSense
- 🏠 Residential water monitoring sub-segment: **+28% CAGR**

---

## 💡 Financial Projections

| Year | Revenue | Gross Margin | Net Profit |
|---|---|---|---|
| 2026 | ₹40 Lakhs | 44% | ₹7 Lakhs |
| 2027 | ₹1.6 Crores | 57% | ₹52 Lakhs |
| 2028 | ₹6 Crores | 67% | ₹2 Crores |

**Seed Funding Required: ₹40 Lakhs**

---

## 🔐 IPR Strategy

| IP Type | Asset | Protection |
|---|---|---|
| Patent | Autoencoder unknown anomaly detection | Utility Patent (India + PCT) |
| Patent | Watchdog heartbeat protocol | Utility Patent |
| Patent | Multi-sensor cross-validation engine | Utility Patent |
| Patent | Redundant comms failover protocol | Patent / Defensive Publication |
| Trade Secret | Trained AI models + thresholds | Confidentiality + Access Controls |
| Copyright | Mobile app, dashboard, platform code | Automatic Copyright |
| Trademark | AquaSense name, logo & tagline | Registered Trademark |

---

## 👥 Team

| Member | Role |
|---|---|
| Ansil Muhammed N S | Team Member |
| Muhammed Ihsan K I | Team Member |
| Muhammed Faiz K N | Team Member |
| Muhammed Aadhil M U | Team Member |

**Department:** Computer Science and Engineering  
**Institution:** KMEA Engineering College (Autonomous), Aluva, Edathala  
**Course:** Engineering Entrepreneurship & IPR  
**Batch:** S2 CSE A  

---

## 📁 Repository Structure

```
AquaSense/
├── README.md                          # This file
├── business-plan/
│   └── AquaSense_Business_Plan.docx   # Full 30-page business plan report
├── docs/
│   ├── executive-summary.md
│   ├── technical-architecture.md
│   ├── fault-tolerance-framework.md
│   └── market-analysis.md
├── src/
│   ├── iot/                           # Sensor firmware (ESP32 / Arduino)
│   ├── ai/                            # Autoencoder + Isolation Forest models
│   ├── cloud/                         # AWS IoT Core + backend API
│   ├── mobile/                        # React Native app
│   └── dashboard/                     # Web dashboard (React)
└── hardware/
    ├── sensor-schematics/
    └── valve-circuit/
```

---

## 🔧 Tech Stack

```
IoT Hardware    : ESP32, Ultrasonic Flow Sensors, Pressure Sensors, Zigbee, LoRaWAN
Communication   : MQTT, WiFi, 4G SIM, LoRaWAN
Cloud           : AWS IoT Core, Lambda, DynamoDB
AI/ML           : Python, TensorFlow (Autoencoder), Scikit-learn (Isolation Forest)
Mobile App      : React Native (Android + iOS)
Web Dashboard   : React.js, Node.js
Edge AI         : TensorFlow Lite on ESP32 / Raspberry Pi gateway
Security        : AES-256, TLS 1.3
```

---

## 📞 Contact

**KMEA Engineering College (Autonomous)**  
Aluva, Edathala, Kerala, India  

> *"The AquaSense system NEVER fails silently. Every unknown event, sensor failure, communication drop, or power interruption is detected, classified, logged, and communicated to the user."*

---

*© 2026 AquaSense — KMEA Engineering College, CSE Department. All rights reserved.*
