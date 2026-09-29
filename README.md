# 🏭 Predictive Asset Condition Monitor

An Industry 4.0 learning project simulating how automated systems detect machine wear and tear before breakdowns happen.

## 💡 The Motivation
Having spent time on the shop floor operating CNC machines, I know how devastating unexpected machine downtime can be. I built this simulation to understand the coding logic behind "Predictive Maintenance",using real-time data data spikes (like heat and motor strain) to catch tool wear early.

## 🛠️ How the System Works
1. **The Simulated Machine (Wokwi):** An Arduino node acts as an industrial motor. It tracks motor speed using a dial (potentiometer), monitors bearing temperature with a DHT22 sensor, and includes an emergency stop kill-switch circuit.
2. **The Smart Monitor (Google Colab):** A Python script acts as a basic "digital twin." It reads this machine data, scans it against safe operating limits, flags any dangerous spikes, and plots the speed and temperature side-by-side on a graph.

## 🔗 Live Interactive Links
* **Interactive Circuit Simulator:** [Launch the Wokwi Simulation](https://wokwi.com/projects/475941984302170113)
* **Cloud Analytics Execution Script:** [Open the Google Colab Notebook](https://colab.research.google.com/drive/1Kfl2ENKIdIyjaqrp2857afsuD3OqTPbQ?usp=sharing)

## 🧠 What I Learned & Practised
* **Industrial Logic**: Translated physical machine concepts (motor strain, bearing friction, overheating) into digital thresholds (`if speed > safe_limit`).
* **Multi-Sensor Integration**: Programmed C++ code to read and scale both analog dials and digital environment sensors simultaneously.
* **Data Visualization**: Used Python's `matplotlib` to plot two different physical properties (temperature and RPM) on a dual-axis chart to visually track how they affect each other.
* **Safety Circuits**: Practised integrating a physical hardware override (kill-switch) into code loops to ensure immediate safety shutdowns.

---

### 🚨 Core Project Highlight
This project directly connects my college workshop machinery training with software logic, proving how writing code can protect expensive industrial hardware from mechanical failure.
