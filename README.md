# SOC-Analyst-Simulation-Minor-2
Network Traffic Analysis &amp; Incident Investigation Using PCAP
# Network Traffic Analysis & Incident Investigation Using PCAP  
### SOC Analyst Simulation – Minor 2 Project

## 📌 Project Overview
This project simulates a real-world **Security Operations Center (SOC)** investigation.  
As a **Junior SOC Analyst**, I analyzed a captured **PCAP file** using **Wireshark** to investigate a suspected system compromise within an organization.

The goal was to identify the attacker, victim system, suspicious activities, and analyze how sensitive data was exfiltrated from the network.

---

## 🎯 Objectives
- Analyze network traffic using Wireshark
- Identify the **attacker IP address**
- Identify the **victim (compromised) system**
- Detect **suspicious network activity**
- Determine the **method of data exfiltration**
- Extract a **ZIP file from PCAP**
- Retrieve the **hidden flag**

---

## 🛠️ Tools & Technologies Used
- **Wireshark**
- **PCAP file**
- Windows / Linux Operating System
- ZIP extraction utility

---

## 📂 Repository Structure

---

## 🔍 Investigation Methodology

### 1️⃣ PCAP Analysis
- Loaded the PCAP file into **Wireshark**
- Analyzed traffic patterns using:
  - Statistics → Conversations
  - Protocol hierarchy
  - Packet inspection

### 2️⃣ Attacker & Victim Identification
- Victim identified as an **internal IP address**
- Attacker identified as an **external suspicious IP**
- Multiple abnormal connections observed during the incident window

### 3️⃣ Suspicious Activity Detection
- Unauthorized communication detected
- Large data transfer observed
- Suspicious use of network protocols

### 4️⃣ Data Exfiltration Analysis
- Sensitive data transferred as a **ZIP file**
- Transfer method identified using **TCP Stream analysis**
- File extracted directly from PCAP

---

## 📦 ZIP File Extraction
- Used **Wireshark → Export Objects**
- Extracted the ZIP file from HTTP/TCP traffic
- Successfully opened and analyzed extracted files

---

## 🚩 Flag Retrieved

---

## 📊 Key Findings
| Category | Details |
|--------|--------|
| Attacker | External malicious IP |
| Victim | Internal compromised system |
| Attack Type | Data exfiltration |
| File Type | ZIP |
| Analysis Tool | Wireshark |
| Outcome | Successful flag extraction |

---

## 📸 Screenshots
All investigation screenshots are available in the **screenshots/** folder and include:
- PCAP loaded in Wireshark
- IPv4 Conversations
- TCP Stream analysis
- Exported ZIP file
- Retrieved flag

---

## 🏁 Conclusion
This project demonstrates practical SOC skills including network traffic analysis, incident investigation, and data extraction from PCAP files. The investigation successfully identified the attack source, compromised system, and recovered sensitive data.

---

## 👤 Author
**Name:** Rakhi Kumari  
**Role:** Junior SOC Analyst (Student)  
**Course:** Minor 2 – Cyber Security  

---

## 📄 License
This project is created for **academic and educational purposes only**.
