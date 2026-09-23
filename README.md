# Industry 4.0 Predictive Asset Condition Monitor (Advanced Tier)

## System Overview
This project simulates an industrial Predictive Maintenance (PdM) ecosystem designed for automated rotary assets. It processes edge-layer telemetry arrays to actively evaluate operational health metrics, isolate stress-induced anomalies, and log safety intervention metrics before hardware damage occurs.

## System Architecture & Data Flow
1. **Edge Telemetry Ingestion (C++/Arduino):** An Arduino node evaluates dual analog and digital signals capturing motor load characteristics (RPM via Potentiometer mapping), ambient bearing temperatures (DHT22 sensor processing), and factory safety kill-switch configurations.
2. **Cloud Statistical Analysis (Python/Colab):** The cloud script functions as a localized Digital Twin. It ingests the telemetry matrix, checks variables using logical anomaly bounds, flags conditions, and maps variables side-by-side using double-scaled graphical plots (`matplotlib`).

## Engineering Competencies Highlighted
* **Advanced Embedded Systems:** Variable conversion math formulas and multi-sensor conditional scheduling protocols.
* **Algorithmic Data Classification:** Conditional array scanning loops mimicking industrial machine learning structures.
* **Industrial UI Design:** Generating dual-axis parametric tracking charts mapping distinct engineering physical constraints simultaneously.

## Digital System Links
* **Wokwi Core Circuit Simulation:** [https://wokwi.com/projects/475941984302170113]
* **Google Colab Cloud Execution Code:** [https://colab.research.google.com/drive/1JserWZxVMuBNhcCb9ftiI7ahtycH8xsg?usp=sharing]
