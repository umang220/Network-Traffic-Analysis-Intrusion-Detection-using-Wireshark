# FTP Credential Sniffing Attack using Wireshark & Nmap

**A practical demonstration of network reconnaissance and plaintext credential capture in an unsecured FTP connection.**

![Project Banner](https://via.placeholder.com/800x200?text=Network+Security+Project)

## 🎯 Project Objective
To demonstrate how easily credentials can be captured in plain text over an unsecured network protocol (FTP) using packet sniffing tools.

---

## 🛠️ Tools Used
- **Nmap** - Network Discovery & Port Scanning
- **Wireshark** - Packet Capture & Analysis
- **FTP Server** - Vulnerable target
- **Kali Linux / Windows** - Attacker Machine

---

## 📋 Project Phases

### Phase 1: Reconnaissance
```bash
nmap -sS -A 192.168.10.4
