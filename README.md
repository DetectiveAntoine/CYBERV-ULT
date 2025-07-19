L3MON — Remote Android Forensic Framework
A Secure, Cloud-Based Android Device Monitoring Suite Built for Ethical Cybersecurity Investigations

<p align="center"> <img src="https://github.com/D3VL/L3MON/raw/master/server/assets/webpublic/logo.png" height="60" alt="L3MON Logo" /> </p>
Overview
L3MON is a Node.js-based Android Remote Administration Tool (RAT) developed for ethical, educational, and internal testing purposes. It provides a powerful web interface to monitor and interact with Android devices in real time. Designed for cybersecurity professionals and digital forensic investigators, L3MON enables lawful data collection and incident response through a centralized dashboard.

⚠️ Disclaimer: This tool is strictly intended for lawful and educational use. Misuse of this software for unauthorized access or illegal surveillance is a criminal offense.

🔍 Features
Real-Time GPS Logging
Track device location and maintain historical movement data.

Microphone Activation & Audio Recording
Collect evidence through real-time or triggered recording sessions.

Comprehensive Device Visibility

Call logs

Contact lists

Installed applications

WiFi network history

Message Intelligence

View SMS history

Send authorized messages for verification/testing

Live clipboard monitoring

Live notification logging

File Management

Explore file system

Download key artifacts

Upload tools or forensic utilities if authorized

Command Queuing System
Schedule or batch forensic actions without user interruption

APK Builder
Build monitoring payloads tailored to the investigation context.

🔧 Installation Guide
✅ Prerequisites
Java Runtime Environment 8 (MANDATORY)

Node.js v14+

Linux or Termux-supported environment (Kali Linux preferred)

PM2 Process Manager (for background task management)

💻 Step-by-Step Setup (Linux)
bash
Copy
Edit
# Install required dependencies
sudo apt update && sudo apt install wget curl git npm nodejs openjdk-8-jdk openjdk-8-jre

# Clone the repository
git clone https://github.com/D3VL/L3MON.git && cd L3MON

# Install Node dependencies
npm install -g pm2
npm install

# Start the application
pm2 start index.js
pm2 startup
🔐 Setting Login Credentials
bash
Copy
Edit
# Stop the service temporarily
pm2 stop index

# Edit main DB file securely
nano maindb.json

# Generate hashed password (replace 'yourpassword')
echo -n yourpassword | openssl md5 | awk '{print $2}'
Update the JSON:

json
Copy
Edit
"admin": {
  "username": "admin",
  "password": "hashed_value_here"
}
Restart the server:

bash
Copy
Edit
pm2 restart all
Access the dashboard:

bash
Copy
Edit
http://127.0.0.1:22533
⚙️ Ethical Use & Compliance
This tool is designed to assist lawful digital investigations, incident response simulations, or academic training in:

Mobile Forensics

Remote Evidence Collection

Penetration Testing Simulations

Monitoring Device Behavior in Controlled Environments

Always ensure usage adheres to:

Organizational policy

Legal jurisdiction

Written consent or authorization

📸 UI Snapshots
Dashboard	Call Logs	GPS Logs
		

More screenshots available in the repository.

📚 Credits & Dependencies
L3MON leverages several open-source technologies:

Express.js

Socket.IO

LowDB

Leaflet & OpenStreetMap

Based on AhMyth Android RAT

🚨 Disclaimer
L3MON is provided as-is, without any warranty. The developer assumes no responsibility for misuse. It is the sole responsibility of the end-user to comply with all applicable laws.

Developed & Secured by
[Cybersecurity Professional | Digital Forensics Specialist]
antonymsafiri16@gmail.com.com | 🛡️ Kali Linux · Node.js · Android Security
