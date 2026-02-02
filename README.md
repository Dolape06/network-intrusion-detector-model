# Network Intrusion Detection System (NIDS)

### Problem Statement & Project Impact
**The Problem: Increasing Vulnerability to Cyber Attacks**
As global organizations move their operations to the cloud, the frequency and complexity of network attacks continue to rise. Traditional rule-based security systems often fail to detect novel or sophisticated patterns of intrusion. Without proactive monitoring, undetected attacks can lead to massive data breaches, financial loss, and compromised infrastructure.

**The Solution: AI-Driven Security Monitoring**
This project develops a Machine Learning classification solution to address this critical security gap. By leveraging the **cybersecurity_data_intrusion.csv** dataset, the model analyzes network traffic features—such as packet size, protocol types, login attempts, and session durations—to predict the likelihood of an intrusion (`attack_detected`). This provides an automated, intelligent layer of defense capable of identifying suspicious behavior in real-time.

### Dataset Overview
The dataset contains network traffic logs with several key technical features:
* **Network_Packet_Size**: The size of the data packets being transmitted.
* **Protocol_Type**: The communication protocol used (TCP, UDP, ICMP).
* **Login_Attempts**: Number of attempts to log into the system.
* **Session_Duration**: The length of time the connection remained active.
* **IP_Reputation_Score**: A metric determining the trustworthiness of the source IP.
* **Attack_Detected (Target)**: Binary indicator (1 for attack, 0 for normal traffic).

### Technical Stack
* **Language**: Python
* **Classification Algorithm**:Random Forest or XGBoostclassifier
* **Data Processing**: Pandas, NumPy
* **Visualization**: Matplotlib, Seaborn
* **Security Metrics**: Precision, Recall, and False Positive Rate (FPR).

###  Key Insights
* **Attack Patterns**: Higher login attempts combined with unusual session durations are strong indicators of brute-force or unauthorized access attempts.
* **Protocol Vulnerability**: Specific protocol types (like UDP) show a higher correlation with certain types of flooding attacks in this dataset.
* **Traffic Anomalies**: Significant deviations in packet size often signal data exfiltration or malicious payloads.
