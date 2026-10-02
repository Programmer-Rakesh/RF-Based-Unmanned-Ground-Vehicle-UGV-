# 🚀 RF-Based Unmanned Ground Vehicle (UGV) | Edge IoT Project

**Individual Hardware Project – Rakesh Roy**  
B.Tech ECE | Robotics • Embedded Systems • Edge IoT

---

## 📌 Project Overview
This project documents the **iterative development of a Radio Frequency (RF)–controlled Unmanned Ground Vehicle (UGV)** designed to operate in **offline, communication-denied environments**.

Instead of relying on internet, GPS, or cellular networks, the UGV uses **direct RF communication**, making it suitable for defense, disaster response, and search-and-rescue applications.

---

## 📸 Project Visuals (Overall)

<p align="center">
  <img src="https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Photos/1.jpeg" width="650">
</p>

<p align="center">
  <img src="https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Photos/3.jpeg" width="320" height="240">
  <img src="https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Photos/4.jpeg" width="320" height="240">
</p>

---

## 🧩 Core Objective
- Build a **deployment-oriented UGV**, not a static prototype
- Ensure reliable control in **no-network zones**
- Improve range, stability, and mechanical robustness through testing
- Maintain modularity for future autonomy and sensor fusion

---

## 🧠 Core Technologies Used

### 🔧 Hardware
- Raspberry Pi 5 (4 GB RAM)
- Arduino Uno
- NRF24L01 + PA + LNA (2.4 GHz RF Transceivers) ×2
- Claw Rover Chassis
- DC Motors & Motor Driver
- External SMA Antennas

### 💻 Software & Tools
- Python (Raspberry Pi)
- Arduino IDE (Embedded C/C++)
- RF24 Library
- SSH (Offline, No-Internet)
- Serial Debugging & Monitoring

---

## 🔄 System Architecture

<!-- IMAGE PLACEHOLDER – BLOCK DIAGRAM -->

**Control Flow:**
Laptop → Raspberry Pi → NRF24L01 → Arduino → Motor Driver → Motors

---

## 🧪 Development Timeline & Progress Logs

---

### 🔹 Phase 1 – Initial RF-Based Control (Indoor / Short Range)
**Status:** Completed ✅

- Laptop-based W/A/S/D control
- Raspberry Pi used as RF transmitter
- Arduino handled motor control
- Achieved ~8 meters range (low battery)

**Observations:**
- Straight motion stable
- Turning behavior inconsistent compared to wired prototype

---

### 🔹 Phase 2 – Outdoor Testing & Turning Optimization
**Status:** Completed ✅

- Battery fully charged
- Turning logic significantly improved
- Minor drift observed under motion

**Results:**
- Reliable RF range: ~45 meters
- Line-of-sight obstruction identified as main limitation

[▶️ Watch Test Video](https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Videos/1.MP4)

---

### 🔹 Phase 3 – Extended Outdoor RF Range Testing (Day 2)
**Status:** Completed ✅

**Measured Performance:**
- Total distance traveled: ~200 meters
- Effective RF displacement range: **163–169 meters**

**Key Optimizations Applied:**
- Antenna tilted upward
- Rover height increased above ground

> RF signal considered effective at the farthest point of reception.

<p align="center">
  <img src="https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Photos/11.png" width="650">
</p>

---

### 🔹 Phase 4 – Control Interface & Latency Evaluation
**Status:** Completed ✅

**Control Mapping:**
| Key | Action |
|---|---|
| W | Forward |
| S | Reverse |
| A | Left |
| D | Right |

**Performance Insight:**
- Extremely smooth motion
- Latency nearly negligible in real-time operation

[▶️ Watch Test Video](https://github.com/Programmer-Rakesh/RF-Based-Unmanned-Ground-Vehicle-UGV-/blob/main/Media/Videos/2.MP4)

---

## 🌍 Application Domains
- 🛟 Disaster & Flood Rescue
- 🪖 Military & Defense Reconnaissance
- 🔍 Search & Rescue (SAR)
- 🏭 Industrial Inspection in Offline Zones

---

## 🔮 Planned Future Integrations
- 🧭 MPU6050 IMU (orientation & motion control)
- 📷 Camera module for live video feed
- 🛰️ GPS (hybrid navigation)
- 🏋️ Payload handling
- 🤖 Semi-autonomous navigation
- 📡 Enhanced RF reliability & range

---

## 🏆 Recognition
- 🏅 **Top 6 – Design Thinking Project Exhibition**
- Organized by GU DEECE × IEEE Industry Applications Society
- Live demo of a running UGV
- First individual participation managing pitching and troubleshooting

---

## 🧑‍💻 Author
**Rakesh Roy**  
B.Tech – Electronics & Communication Engineering  
Galgotias University  

🔗 LinkedIn: https://lnkd.in/gadwNU_k  

---

## 📜 License
This project is intended for **educational, experimental, and research purposes**.
