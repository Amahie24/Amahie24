# Incident Response: SYN Flood Attack (DoS)

This project documents a simulated cybersecurity incident involving a Denial-of-Service (DoS) attack on a travel agency’s web server. The attack analysis, written report, and packet capture logs illustrate how SYN flooding impacts system availability and what steps can be taken to mitigate it.

---

## 🧠 Scenario Overview

An alert from the network monitoring system revealed that the company’s website was unreachable. A packet capture showed an abnormal number of TCP SYN requests from a single IP address, suggesting a SYN flood attack. This prevented legitimate users from completing the TCP three-way handshake and accessing the site.

---

## 🔍 Key Findings

- **Attack Type**: Denial-of-Service (DoS) via SYN Flood  
- **Symptoms**: Connection timeout errors for legitimate users  
- **Cause**: Excessive SYN packets overwhelmed the server’s ability to process TCP handshakes  
- **Logs**: Highlighted packet activity from IP `203.0.113.0` continuously sending SYN packets  
- **Impact**: Server performance degraded; access to the website became unavailable for employees and customers  
- **Mitigation**: IP temporarily blocked, server taken offline to recover

---

## 📁 Files Included

- `Cybersecurity incident report.pdf`: Completed template identifying the attack and explaining its effect
- `Wireshark TCP_HTTP log - TCP log.pdf`: Raw packet capture log showing SYN flood traffic
- `How to read a Wireshark TCP_HTTP log.pdf`: Guide for interpreting the captured packets

---

## 📈 How SYN Flood Works

The TCP three-way handshake:
1. **SYN**: Client requests connection
2. **SYN-ACK**: Server acknowledges and allocates resources
3. **ACK**: Client confirms connection

In a SYN flood:
- The attacker sends numerous SYN packets but doesn’t complete the handshake.
- Server keeps resources open, waiting for ACKs that never arrive.
- Server becomes overwhelmed and eventually drops legitimate requests.

---

## 🛡️ Lessons Learned

- Always monitor abnormal traffic patterns
- SYN flood attacks can be launched from a single IP (DoS) or multiple IPs (DDoS)
- Packet analysis with tools like Wireshark is critical in identifying and understanding threats
- Firewalls and SYN cookies can help mitigate this type of attack

---

## 🔧 Tools Used

- Wireshark (or similar packet sniffer)
- Network monitoring system
- Linux shell / CLI (for packet analysis and server management)

---

## 🗂️ Project Purpose

This hands-on lab was completed as part of a cybersecurity training program. It demonstrates the importance of packet-level analysis in identifying denial-of-service attacks and preparing effective incident responses.

