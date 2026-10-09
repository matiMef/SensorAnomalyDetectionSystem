# IoT Sensor Anomaly Detection System

An end-to-end IoT monitoring solution leveraging multiple ESP32 edge nodes, a central server, machine learning anomaly detection models, and an interactive web HMI dashboard.

## System Architecture

- **ESP32 Nodes**: Three microcontrollers equipped with distinct sensors (Temperature, Light, Vibration) streaming environmental and operational data.
- **Central Server**: Receives incoming telemetry, handles persistence, and feeds data into the analytics engine.
- **Anomaly Detection Model**: Evaluates sensor metrics to identify deviations from normal operational baselines.
- **Web Dashboard (HMI)**: Real-time visualization of device states, anomaly alerts, logs, automated email notifications, and reporting tools.

## Data Flow

ESP32 Nodes -> Server Backend -> AI Model Inference -> Web Application Dashboard

## Methodology and Research Goal

- **Training Strategy**: Semi-supervised/unsupervised learning trained on real baseline data (normal operation) combined with simulated anomalies for robustness testing.
- **Feature Engineering**: Input vectors combine absolute sensor readings, rate of change (deltas/increments), and sensor type context.
- **Research Objective**: Comparative evaluation of different machine learning models (e.g., Isolation Forest, Autoencoders, One-Class SVM) for performance, detection latency, and accuracy in industrial anomaly detection.
