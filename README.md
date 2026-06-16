# 🎯 Lightweight Target Body Stabilizer & Damage Overrider (Lua)

An optimized, lightweight Lua configuration framework engineered to demonstrate **real-time input pooling, dynamic dynamic centroid shifting, and algorithmic damage evaluation overrides** within 3D physics environments.

This repository serves as a clear, structural code reference for developers studying input state listening, conditional execution pipelines, and matrix calculations.

---

## ⚠️ Academic & Research Disclaimer
This repository is published strictly for **educational, analytical, and historical research purposes**. It explores how input hooks interact with simulation data structures to prioritize specific telemetry nodes over standard precision vectors. The author does not condone, promote, or support the deployment of this configuration in live, competitive gaming matchmaking environments.

---

## 🚀 Core Mechanical Insights

### 1. Centroid Target Modification (Force Body Aim)
The script intercepts execution cycles via `on_createmove_start`. When the primary interaction key (`button 1`) is registered, it commands the tracking logic to bypass standard point filters, dynamically locking the calculation grid onto the center mass of the target matrix to minimize packet registration failure.

### 2. Runtime Threshold Bypass (Damage Override)
Under baseline operations, the system filters calculations through high-precision metrics. This routine demonstrates how to bypass those delay loops on demand, forcing instantaneous evaluation cycles based on the real-time slider value selected by the user.

### 3. Automated State Restorer
Features an asynchronous rollback safety routine. The moment input polling registers a release state, the script instantly relinquishes override controls, reverting the entire system core to default, nominal operational baselines.

---

## 🎨 Interactive Calibration Panel
The module implements a clean, native graphical user interface container titled **"Lua Rage Booster"**:

* **Master Operational Switch:** A global checkbox to safely engage or disengage the monitoring logic from the active cycle thread.
* **Damage Metric Slider:** An integer calibration node (1 to 100) allowing users to dynamically modify structural thresholds with immediate effect.

---

## 📦 Repository Components
* `rage_body_booster.lua` — Core standalone calculation script with integrated UI components.
* `README.md` — Technical system manual, behavioral explanations, and structural guidelines.

---

## 📄 License
This module is fully open-source and officially distributed under the permissive terms of the **MIT License**.
