🛡️ Incident Response – SYN Flood Attack (DoS)

## Objective
This project simulates a real-world cybersecurity incident response involving a SYN flood attack that disrupted access to a travel agency’s web server. The goal was to identify the nature of the attack, analyze packet traffic using Wireshark, and report on the impact and mitigation steps taken.

---

🧠 Skills Learned
- Identifying and responding to network-based DoS attacks  
- Interpreting TCP three-way handshakes and SYN flood behavior  
- Analyzing packet capture logs (PCAP) using Wireshark  
- Writing professional cybersecurity incident reports  
- Documenting attack vectors and mitigation strategies  

---

🛠️ Tools and Resources Used
- **Wireshark / TCP Packet Logs**  
- **Firewall & IP Blocking**  
- **Incident Response Documentation Template**  
- **Guided analysis support materials**  

---

🪜 Project Steps

### Step 1: Alert Received and Initial Analysis  
Received a monitoring alert; confirmed the website was unreachable with a timeout error.  
Captured and examined network packets to find the cause.  
📄 [Cybersecurity Incident Report (PDF)](./Cybersecurity%20incident%20report.pdf)

---

### Step 2: Packet Analysis  
Used Wireshark logs to trace TCP connection attempts from multiple IPs. Discovered one source (203.0.113.0) repeatedly sending SYN packets without completing handshakes.  
📘 [How to Read a Wireshark TCP/HTTP Log (PDF)](./How%20to%20read%20a%20Wireshark%20TCP_HTTP%20log.pdf)  
📊 [Wireshark TCP/HTTP Log – Raw Packet Data (PDF)](./Wireshark%20TCP_HTTP%20log%20-%20TCP%20log.pdf)

---

### Step 3: Response and Mitigation  
- Temporarily took the web server offline to prevent further exhaustion  
- Blocked the attacker's IP using the company firewall  
- Noted that IP blocking is a short-term fix — recommended implementing SYN cookies and rate limiting for long-term resilience  

---

✅ Outcome
- Correctly identified and documented a SYN flood DoS attack  
- Used real packet logs to simulate traffic investigation  
- Demonstrated foundational skills in incident response and network forensics  
- Gained portfolio-worthy experience in documenting and mitigating network attacks  

---

🔗 [Return to GitHub Profile](https://github.com/your-username) | [Connect on LinkedIn](https://www.linkedin.com/in/amahie-lewis-2a1288292/)

