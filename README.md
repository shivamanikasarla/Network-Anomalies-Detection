# Network-Anomalies-Detection
A Python-based tool that analyzes network traffic to detect suspicious or abnormal behavior such as port scans, DoS attacks, and unusual IP activity using statistical and rule-based methods.

📌 Features
🔍 Detects:

High packet rate (potential DoS)

Repeated port scans

IP flooding from single sources

Unexpected protocol usage

📊 Simple statistical thresholding and time-based monitoring

📁 Works with .pcap files (captured traffic) or live sniffing

🧠 Easily extendable for ML-based anomaly detection

📈 Logs and generates reports of suspicious events

🛠️ Technologies Used
Python

scapy – Packet sniffing

pandas – Data analysis

matplotlib – Optional visualizations

argparse – CLI support

🚀 How It Works
Capture or load network traffic.

Monitor parameters like:

Number of packets per IP

Rate of incoming/outgoing packets

Number of unique ports accessed

Compare activity against defined thresholds.

Flag and log anomalies.

🖥️ Setup Instructions
bash
Copy
Edit
git clone https://github.com/your-username/Network-Anomalies-Detection.git
cd Network-Anomalies-Detection
pip install -r requirements.txt
sudo python3 detect.py --live
You can also run it on a .pcap file:

bash
Copy
Edit
sudo python3 detect.py --file traffic.pcap
