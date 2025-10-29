# SENTRY-AI
SENTRY-AI is an intelligent system that monitors network traffic in real time and uses Artificial Intelligence to detect abnormal or suspicious activities such as intrusions, malware communication, or data theft. It automatically alerts the administrator and can block malicious connections to ensure network safety.

# SENTRY-AI: Sprint 1 README

## Sprint 1 Objective
Build the **frontend interface** and foundational architecture for the real-time network monitoring system. This sprint focuses on creating a behavioral dashboard that simulates live traffic, visualizes anomalies, and provides admin controls for monitoring and blocking suspicious activity.

---

## Deliverables

### 1. Streamlit Frontend Dashboard
- Developed a real-time **interactive dashboard** using Streamlit.
- Displays live simulated network traffic with columns for Source IP, Destination IP, Protocol, Bytes Sent, and Anomaly Score.
- Color-coded alerts to highlight suspicious activity exceeding a configurable threshold.
- Metrics section showing total connections, blocked IPs, and alerts raised.
- Sidebar control panel with:
  - Mode selection: *Monitor Only*, *Alert Only*, *Alert + Block*
  - Adjustable anomaly threshold slider
  - Start/Stop monitoring buttons

### 2. Behavioral Visualization
- Created dynamic tables to show **normal vs suspicious behavior**.
- Integrated time-based anomaly charts using Streamlit’s line chart module.
- Added a model summary block for quick insight into AI status.

### 3. Backend Simulation
- Simulated network packet data generation using random values.
- Emulated AI anomaly scores for visualization purposes.
- Live updates every 2 seconds to mimic real-time packet flow.

### 4. Repository Structure
```
SENTRY-AI/
  ├── app/
  │   └── streamlit_app.py        # Sprint 1 Frontend
  ├── models/                     # (Placeholder for future AI models)
  ├── scripts/                    # (Placeholder for backend and packet capture logic)
  ├── data/                       # (Placeholder for training and test data)
  ├── tests/                      # (Unit test directory)
  ├── requirements.txt
  └── README.md (Sprint 1)
```

### 5. Technology Stack
- **Python 3.8+**
- **Streamlit** for dashboard and visualization
- **NumPy & Pandas** for data simulation
- **Matplotlib/Altair** (future integration for advanced graphs)

---

## Sprint 1 Outcome
✅ Successfully created an interactive UI that visualizes simulated traffic and alerts.
✅ Established real-time dashboard logic and control mechanisms.
✅ Prepared a base to integrate backend detection and AI model in Sprint 2.

---

## Next Sprint Goals (Sprint 2 Preview)
- Integrate **real packet capture** using Scapy or PyShark.
- Connect trained **Autoencoder/LSTM model** for anomaly detection.
- Implement **database (SQLite)** for storing alerts and logs.
- Develop **Telegram/email alerting** system.
- Begin implementing **firewall auto-blocking** via iptables (Linux).

---

## How to Run the Frontend
```bash
git clone https://github.com/<your-username>/sentry-ai.git
cd sentry-ai
pip install -r requirements.txt
streamlit run app/streamlit_app.py
```

---

## Contributors
- **Augustus Mathew** – Lead Developer & Cybersecurity Engineer

---

## Version
**Sprint 1 – Frontend Implementation**

---

## License
Licensed under the MIT License. See LICENSE file for details.
