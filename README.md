# 🧠 MISP Integration with Wazuh SIEM

## 📌 Overview
This task focuses on integrating MISP (Malware Information Sharing Platform) with Wazuh SIEM to enrich alerts using external threat intelligence and improve detection capabilities.

📄 **Full Detailed Documentation (with screenshots & steps):** 
For PDF: ([Wazuh Integration with MISP.pdf](https://github.com/MSafwanAwan/MISP-Integration-with-Wazuh/blob/main/Wazuh%20Integration%20with%20MISP.pdf))

For Commands: ([Commands and Execution]{

## 🎯 Objective
- 🖥 Deploy MISP on Ubuntu  
- 🔗 Integrate Wazuh with MISP via API  
- 🧾 Enable IoC-based threat correlation  
- 🚨 Generate intelligence-driven alerts  

## 🏗 Architecture
- 🛡 Wazuh Manager (SIEM)  
- 💻 Wazuh Agents (Windows/Linux)  
- 🌐 MISP Server (Threat Intelligence Platform)  
- 📊 Sysmon (Advanced Event Logging)  

## ⚙️ Implementation Steps

### 1️⃣ MISP Installation
- 📦 System update & dependencies setup  
- 🗄 MySQL client configuration  
- 📥 Download & run official MISP install script  
- 🔐 Configure firewall (HTTP/HTTPS)  
- 🌍 Access web interface & initial login  
- 🏢 Create organization & admin credentials  

### 2️⃣ Threat Intelligence Feeds Setup
- 🌍 Load OSINT feeds  
- 🔄 Enable CIRCL/community feeds  
- 💾 Configure feed caching  

### 3️⃣ Sysmon Deployment (Windows Agent)
- 🧩 Install Sysmon with config  
- 📑 Enable detailed event logging  
- 🔁 Restart Wazuh agent  
- ✅ Verify log collection  

### 4️⃣ Wazuh–MISP API Integration
- 🔑 Generate MISP API key  
- 📜 Deploy integration script in Wazuh  
- ⚙️ Configure `ossec.conf` integration block  
- 🔒 Set secure script permissions  

### 5️⃣ Custom Rule Creation
- 📢 Rule for MISP event alerts  
- ⚠️ Rule for integration errors  
- 🚨 Rule for IoC match detection  

### 6️⃣ Service Restart & Validation
- 🔄 Restart Wazuh Manager  
- 📊 Verify alert enrichment from MISP  

## 🛠 Skills Demonstrated
- 🧠 Threat Intelligence Integration  
- 🔗 API-based SIEM Automation  
- 🧾 Custom Rule Development  
- 📊 Event Correlation & Analysis  
- 💻 Windows Monitoring with Sysmon  

## 🏁 Outcome
Successfully integrated MISP with Wazuh to correlate system events with real-time threat intelligence feeds and generate enriched, high-confidence security alerts.

## 📄 Documentation
📘 Full step-by-step implementation with screenshots is provided in the attached PDF.
