# 🛡️ Cybersecurity Key Notes

## 📄 Overview of Logs

### 🔹 What is a Log?
A **log** is a record of events that occur within systems, applications, or networks. It helps track what happened, when it happened, and where it happened.

### 🔹 Purpose of Logs
- Monitor system activity
- Detect security incidents
- Troubleshoot system issues
- Support forensic investigations

### 🔹 Types of Logs
- **System logs:** Operating system events (startup, shutdown, errors)
- **Application logs:** Events from software applications
- **Security logs:** Login attempts, access control events
- **Network logs:** Traffic and connection data

### 🔹 Key Concepts
- **Logging:** The process of generating log data
- **Log analysis:** Reviewing logs to find meaningful events
- **Log management:** Collecting, storing, and maintaining logs securely
- **Telemetry:** Automated collection and transmission of log data

---

## 🕵️ Overview of Intrusion Detection Systems (IDS)

### 🔹 What is IDS?
An **Intrusion Detection System (IDS)** is a security tool that monitors systems or networks for suspicious activity and generates alerts when potential threats are detected.

### 🔹 Types of IDS

#### 1. Network-based IDS (NIDS)
- Monitors network traffic
- Detects attacks across the entire network
- Example tool: Suricata

#### 2. Host-based IDS (HIDS)
- Installed on a specific device (endpoint)
- Monitors system files, processes, and logs
- Detects local attacks or unauthorized changes

### 🔹 Detection Methods
- **Signature-based detection:** Matches known attack patterns
- **Anomaly-based detection:** Detects unusual behavior compared to normal activity

### 🔹 Key Features
- Real-time monitoring
- Alert generation
- Threat pattern detection

### 🔹 Limitation
- IDS only alerts; it does not block attacks (unless integrated with IPS)

---

## 📊 Overview of Security Information and Event Management (SIEM)

### 🔹 What is SIEM?
A **SIEM (Security Information and Event Management)** system collects, aggregates, and analyzes log data from multiple sources to detect security threats and support incident response.

### 🔹 Core Functions
- Collect logs from endpoints, servers, and network devices
- Normalize and correlate data from different sources
- Detect suspicious patterns or anomalies
- Generate alerts and dashboards

### 🔹 Key Capabilities
- Real-time monitoring
- Event correlation across systems
- Centralized log storage
- Security reporting and dashboards
- Threat detection and alerting

### 🔹 Common SIEM Tools
- Wazuh
- Splunk
- IBM QRadar
- Microsoft Sentinel
- Elastic Security (ELK Stack)

### 🔹 SIEM Workflow
1. Data collection (logs from sources)
2. Data normalization (standard format)
3. Data correlation (pattern detection)
4. Alert generation
5. Analyst investigation

### 🔹 Benefits
- Faster threat detection
- Centralized visibility
- Improved incident response
- Better compliance and auditing

---

## 🧠 Quick Summary
- **Logs** = raw event records
- **IDS** = detects and alerts on suspicious activity
- **SIEM** = collects + analyzes logs from multiple sources to detect threats