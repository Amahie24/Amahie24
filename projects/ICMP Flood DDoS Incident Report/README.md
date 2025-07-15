# 🛡️ Incident Response – ICMP Flood Attack (DDoS)

## Objective  
This project simulates a real-world cybersecurity incident response involving an **ICMP flood DDoS attack** that disrupted internal network services at a multimedia company. The goal was to identify the attack vector, analyze the cause of the outage, and implement appropriate countermeasures using the **NIST Cybersecurity Framework**.

---

🧠 **Skills Learned**  
- Identifying and responding to volumetric DDoS attacks  
- Analyzing ICMP packet behavior and firewall vulnerabilities  
- Applying the NIST CSF to structure a real-world incident response  
- Writing professional cybersecurity incident reports  
- Implementing technical hardening techniques and mitigation strategies  

---

🛠️ **Tools and Resources Used**  
- **Firewall and ICMP filtering rules**  
- **Network monitoring software**  
- **IDS/IPS systems**  
- **Incident response documentation framework**  
- **NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)**  

---

🪜 **Project Steps**

### Step 1: Alert Received and Initial Impact  
All internal network services became unresponsive for approximately two hours.  
An investigation revealed a flood of incoming **ICMP echo requests** overwhelming the network.  
📄 [ICMP Flood Incident Report (PDF)](./ICMP-Flood-Incident-Report.pdf)

---

### Step 2: Root Cause Analysis  
- The attack exploited a **misconfigured firewall** that failed to block ICMP packets from external sources  
- Firewall logs showed a massive spike in inbound ICMP traffic  
- The flood prevented legitimate internal traffic from reaching critical services  

---

### Step 3: Response and Mitigation  
- Blocked all incoming ICMP packets at the firewall  
- Disabled non-critical services to stabilize network load  
- Restored access to **critical systems** first  
- Implemented:
  - Rate limiting for ICMP traffic  
  - Source IP verification  
  - Network monitoring tools  
  - IDS/IPS filtering for suspicious ICMP patterns  

---

✅ **Outcome**  
- Successfully identified and mitigated an ICMP-based DDoS attack  
- Strengthened perimeter defenses and monitoring capabilities  
- Applied NIST CSF categories to structure the response and recovery process  
- Demonstrated strong practical skills in managing real-world network threats  
- Produced a detailed, portfolio-ready incident response report  

---

🔗 [Return to GitHub Profile](https://github.com/Amahie24) | [Connect on LinkedIn](https://www.linkedin.com/in/amahie-lewis-2a1288292/)

