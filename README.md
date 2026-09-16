# Drishti: Intelligent Border Video Analytics Platform (Frontend Showcase)

[![Live Status](https://img.shields.io/badge/Status-Static%20Showcase-blue?style=for-the-badge)](https://github.com/ishanyatripathi/Drishti)
[![Main Codebase](https://img.shields.io/badge/Core%20Repository-ShreyaB002%2FDrishti--orange?style=for-the-badge&logo=github)](https://github.com/ShreyaB002/Drishti-)
[![Platform](https://img.shields.io/badge/Target-Offline%20Edge%20Devices-darkgreen?style=for-the-badge)](https://github.com/ShreyaB002/Drishti-)

---

> [!IMPORTANT]
> ### 🛡️ Architecture & Deployment Notice
> **This repository hosts strictly the static frontend demonstration of Drishti.**
> 
> In real-world security and border monitoring operations:
> - The Drishti software is engineered to run **completely offline on edge / end devices** (forward operating bases, air-gapped border surveillance command centers, and tactical vehicles).
> - All heavy AI computation—including YOLOv11 computer vision, Optical Flow tracking, ANPR OCR engines, and biometric facial matching—executes **100% locally on local GPUs/NPUs without any cloud or internet dependency**.
> - For online evaluation, review, and demonstration purposes, we have hosted this lightweight static interface showcasing pre-recorded, GPU-annotated surveillance streams from our core system.
> 
> 👉 **The complete, full-stack core repository**—containing the FastAPI backend server, YOLOv11/ResNet models, ANPR OCR engines, Virtual Fence intrusion algorithms, tracking pipelines, and dataset utilities—is located at:
> 
> ### 🔗 **[https://github.com/ShreyaB002/Drishti-](https://github.com/ShreyaB002/Drishti-)**

---

## 🖥️ What this Static Showcase Demonstrates

This static frontend mirrors the exact production user interface of the Drishti command center:

1. **6-Channel Tactical Surveillance Grid**:
   - **Cam 1 (Virtual Fence)**: Polygon-restricted perimeter boundary monitoring with real-time intrusion alarms.
   - **Cam 2 (Vehicle Tracking)**: Multi-class vehicle tracking (cars, trucks, buses, motorcycles) with unique trajectory tracking IDs.
   - **Cam 3 (Human Detection)**: Perimeter pedestrian movement surveillance and patrol tracking.
   - **Cam 4 (ANPR Engine)**: Automatic Number Plate Recognition featuring tactical HUD overlays and license plate readouts.
   - **Cam 5 (Suspicious Activity)**: Nighttime loitering and curfew intrusion detection in critical blind spots.
   - **Cam 6 (Facial Recognition)**: Edge-based biometric face matching against verified security watchlists.

2. **Forensic Evidence Drawer**:
   - Slide-out incident log containing timestamped event cards, severity indicators (High/Medium/Low), and captured forensic snapshots.
   - Clicking any snapshot immediately expands and inspects that camera channel.

3. **Client-Side CSV Audit Export**:
   - The **"Export Log"** button dynamically generates and downloads a formal audit CSV report (`Drishti_Incident_Log_<timestamp>.csv`) directly in your browser.

4. **Enlarged High-Resolution Modal View**:
   - Interactive zoom view allowing security operators to focus on any single camera channel.

5. **Government of India / MHA Command Identity**:
   - Official national identity banner, live status badges, and threat notification banners.

---

## 🚀 Running Locally

You can preview this static showcase on any machine with zero external dependencies:

```bash
# Using Python
python -m http.server 8080

# Or using Node.js
npx serve .
```

Then visit `http://localhost:8080` in your web browser.

---

## 📂 Repository Contents

```
├── index.html                  # Main responsive command dashboard
├── README.md                   # Repository documentation & architecture notice
├── .gitignore                  # Git ignore file for OS artifacts
└── assets/                     # High-efficiency H.264 annotated surveillance feeds & branding
    ├── Cam1.mp4                # Virtual Fence Restricted Zone Intrusion (H.264)
    ├── Cam2.mp4                # Multi-Class Vehicle Detection & Tracking (H.264)
    ├── Cam3.mp4                # Perimeter Human Detection (H.264)
    ├── Cam4.mp4                # ANPR License Plate Recognition & HUD (H.264)
    ├── Cam5.mp4                # Suspicious Activity Detection (H.264)
    ├── Cam6.mp4                # Facial Recognition & Verification (H.264)
    ├── product_logo.png        # Drishti product logo
    ├── favion.png              # Favicon
    └── team_logo.png           # Team brand logo
```

---

## 🔗 Full Project & Backend Repository

To explore the backend architecture, computer vision models, training notebooks, and setup guides for offline edge deployment, visit the primary repository:
**[https://github.com/ShreyaB002/Drishti-](https://github.com/ShreyaB002/Drishti-)**
