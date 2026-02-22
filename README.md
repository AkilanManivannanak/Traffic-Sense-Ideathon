# TrafficSense — ML-Based Traffic Congestion Prediction & Signal Optimization (Ideathon)

TrafficSense is an ideathon concept project that proposes a **Smart City Machine Learning system** to **predict short-horizon traffic congestion** and recommend **constraint-aware adaptive signal timing** to reduce queues and prevent gridlock.

This repository contains the **pitch deck (PPT)** and supporting project description.

---

## 📌 Project Overview

Urban congestion changes rapidly due to **time-of-day**, **incidents**, **weather**, and **local events**. Fixed-time signal plans often cannot react to real-time demand at each intersection, leading to queue spillback and corridor-level bottlenecks.

TrafficSense is designed as a **two-stage pipeline**:

1. **Prediction (ML):** Forecast congestion 5–15 minutes ahead per road segment / intersection approach  
2. **Optimization (Control):** Convert forecasts into recommended signal timings under strict constraints

---

## 🎯 Problem Statement

Cities need a solution that can **predict congestion before queues become severe** and translate predictions into **safe, constraint-aware signal timing recommendations**.

The system must operate under real-world constraints such as:
- Minimum/maximum green times  
- Pedestrian crossing phases  
- Fairness across approaches (no starvation)  
- Coordination across adjacent intersections  
- Robustness to noisy/missing sensor inputs  

---

## ✅ Benefits & Impact

- **Proactive congestion control:** Mitigate congestion *before* it peaks (short-horizon forecasting).
- **Reduced waiting time:** Better green-time allocation improves traffic flow at intersections.
- **Incident/event awareness:** Alerts for unusual spikes, road closures, and event-driven surges.
- **Safety-first actuation:** Recommendations respect operational constraints and pedestrian phases.
- **Emergency priority support (optional):** Can integrate priority routing/preemption logic.
- **Scalable rollout:** Start with one corridor → expand city-wide with more data sources.
- **Lower emissions & fuel waste:** Smoother flow reduces stop-and-go traffic.

---

## 🧠 ML Approach 

**Inputs (examples):**
- Timestamp, day type (weekday/holiday)
- Intersection / road segment ID
- Vehicle count, estimated queue length, average speed
- Recent trends (moving averages)
- Optional: weather, event schedule, incident signals

**Model (examples):**
- Baseline regression
- Gradient Boosting (XGBoost/LightGBM)
- Time-series models (optional extension)

**Outputs:**
- Congestion score / predicted density
- Recommended signal plan parameters:
  - Green split ratios
  - Cycle length adjustments
  - Phase scheduling suggestions

**Evaluation (suggested):**
- Forecasting: MAE / RMSE
- Classification framing (optional): Precision / Recall for congestion levels
- System-level: reduced queue length, improved throughput, reduced travel time

---

## 📂 Repository Contents

- `[TrafficSense_Ideathon_2022_AKAKN.pptx](https://github.com/AkilanManivannanak/Traffic-Sense-Ideathon/blob/main/IDEATHON%202022%20_AKAKN.pptx) 
---

## 🏫 Event

**Ideathon | Panimalar Engineering College**  
**Date:** 08/2023  
**Theme:** Smart City / Urban Traffic (ML-inspired 2022 topic)

---

## 👤 Author

**Akilan Manivannan**  
GitHub: https://github.com/AkilanManivannanak

---

