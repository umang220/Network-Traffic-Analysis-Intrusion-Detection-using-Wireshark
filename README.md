# 🔍 Network Traffic Analysis & Intrusion Detection using Wireshark

> A hands-on SOC lab project to simulate and detect brute-force attacks using real-time network traffic analysis.

---

## 📌 Project Overview
This project demonstrates a Security Operations Center (SOC) lab where network traffic is captured and analyzed using Wireshark.

A brute-force attack is simulated using Hydra, and the generated traffic is analyzed to detect malicious patterns.

---

## 🎯 Objectives
- Capture and analyze live network traffic  
- Simulate brute-force attack using Hydra  
- Detect suspicious behavior using packet analysis  
- Understand real-world SOC workflow  

---

## 🛠️ Tools & Technologies
- Kali Linux (Attacker Machine)  
- Ubuntu (Target Machine)  
- Wireshark  
- Hydra  
- VirtualBox  

---

## 🧪 Lab Setup
- Attacker: Kali Linux  
- Victim: Ubuntu Machine  
- Network: Same Virtual Network (VirtualBox)

---

## ⚙️ Steps Performed

### 1️⃣ Network Setup
- Configured both VMs in same network  
- Verified connectivity using ping  

### 2️⃣ Packet Capture
- Started Wireshark on Ubuntu  
- Selected active interface  
- Captured live packets  

### 3️⃣ Attack Simulation
```bash
hydra -l username -P password.txt ssh://<target-ip>
4️⃣ Traffic Analysis
Applied Wireshark filter:
tcp.port == 22
Observed repeated login attempts
Identified abnormal traffic spikes
Detected multiple SSH authentication failures
5️⃣ Detection
Multiple failed login attempts
Same IP sending repeated requests
High-frequency traffic on port 22
Suspicious brute-force attack pattern identified
