# 🛰️ DNS Traffic Analysis Incident Report
**Course-Based Simulation**

Analyzed DNS and ICMP network traffic to investigate a website access issue for a client’s customers. Captured and examined data using `tcpdump` to identify root causes of a service outage.

---

## 📖 Scenario

Several customers reported they were unable to access the client company website, **www.yummyrecipesforme.com**, seeing the error **“destination port unreachable.”**

As a cybersecurity analyst, I attempted to replicate the issue. When trying to visit the website, I received the same error. Using `tcpdump`, I captured network traffic and discovered the browser’s DNS query was sent over **UDP port 53**, but received **ICMP “udp port 53 unreachable”** error messages from the DNS server.

---

## 🔎 Key Analysis Findings

- **Network protocol affected:** UDP traffic on port 53 (DNS).
- **Service impacted:** DNS resolution — preventing clients from accessing the website.
- **Evidence:** tcpdump logs showed repeated ICMP errors in response to DNS queries.
- **Time of incident:** Approximately **1:24 p.m.** as recorded in packet timestamps.
- **Likely causes:**  
  - The DNS server was down or unresponsive.
  - A firewall misconfiguration was blocking port 53.
  - A potential Denial of Service attack on the DNS server.

---

## 🛠️ Skills Demonstrated

✅ Captured and analyzed network traffic using `tcpdump`  
✅ Identified protocol-specific failures and interpreted ICMP error messages  
✅ Documented incidents clearly and professionally for escalation  
✅ Understood the relationship between DNS resolution, UDP, and ICMP protocols  

---

## 📄 Full Report

[Download the PDF version of this incident report](Cybersecurity%20incident%20report%20network%20traffic%20analysis.pdf)

---

📌 *This simulation demonstrates hands-on ability to troubleshoot real-world DNS and network-related issues as part of a cybersecurity incident response process.*
