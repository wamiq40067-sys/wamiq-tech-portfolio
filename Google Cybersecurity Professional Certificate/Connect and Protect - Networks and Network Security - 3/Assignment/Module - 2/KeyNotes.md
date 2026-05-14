# Key Notes: Introduction to Network Protocols

## What are Network Protocols?
- Network protocols are standardized rules that allow devices to communicate over a network.
- They define how data is formatted, transmitted, received, and processed.
- Protocols ensure compatibility between different devices and systems.

---

# Importance of Network Protocols
- Enable reliable communication between devices.
- Ensure proper delivery of data packets.
- Help organize and manage network traffic.
- Support security, error handling, and data recovery.
- Allow devices worldwide to communicate using common standards.

---

# Main Categories of Network Protocols

## 1. Communication Protocols
- Handle the exchange of data between devices.
- Manage data transmission and connectivity.

### Examples:
- **TCP (Transmission Control Protocol)**  
  - Reliable and connection-oriented.
  - Ensures accurate delivery of data.

- **UDP (User Datagram Protocol)**  
  - Faster but less reliable than TCP.
  - Commonly used for streaming and real-time applications.

- **HTTP/HTTPS**  
  - Used for web communication between browsers and servers.

- **SMTP**  
  - Used for sending emails.

---

## 2. Management Protocols
- Used to monitor, configure, and troubleshoot networks.

### Examples:
- **SNMP (Simple Network Management Protocol)**  
  - Monitors and manages network devices.

- **ICMP (Internet Control Message Protocol)**  
  - Reports network errors and supports troubleshooting tools like ping.

---

## 3. Security Protocols
- Protect data transmitted across networks.
- Use encryption and authentication methods.

### Examples:
- **HTTPS**
- **SSH**
- **SFTP**
- **IPSec**
- **SSL/TLS**

---

# Common Network Protocols

## DNS (Domain Name System)
- Converts domain names into IP addresses.
- Helps users access websites without remembering numeric IP addresses.

## ARP (Address Resolution Protocol)
- Maps IP addresses to MAC addresses on local networks.

## DHCP (Dynamic Host Configuration Protocol)
- Automatically assigns IP addresses to devices on a network.

---

# Ports and Protocols
- Port numbers identify specific services on a device.
- Firewalls use port numbers to allow or block traffic.

### Common Ports:
| Protocol | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| DNS | 53 |
| SMTP | 25 |

---

# Wireless Network Protocols
- Wireless communication commonly uses Wi-Fi standards (IEEE 802.11).
- Wireless security protocols include:
  - WEP
  - WPA
  - WPA2
  - WPA3

- WPA2 and WPA3 provide stronger encryption and security.

---

# Key Security Concerns
- Some protocols are outdated and vulnerable.
- Unencrypted protocols can expose sensitive data.
- Security analysts must understand protocol weaknesses and secure alternatives.

---


# Key Notes: System Identification

## What is System Identification?
- System identification refers to recognizing and distinguishing devices, systems, and services on a network.
- It helps administrators and security analysts understand what devices are connected and how they communicate.

---

# Importance of System Identification
- Helps track authorized and unauthorized devices.
- Supports network management and troubleshooting.
- Assists in detecting suspicious or malicious activity.
- Improves security monitoring and access control.

---

# Methods of Identifying Systems

## IP Address
- A unique logical address assigned to a device on a network.
- Used for routing and communication between systems.

### Types:
- Private IP addresses
- Public IP addresses

---

## MAC Address
- A unique physical identifier assigned to a network interface card (NIC).
- Used for communication within the same local network.

### Characteristics:
- Permanent hardware address
- Helps identify specific devices on a LAN

---

## Hostname
- A human-readable name assigned to a device.
- Makes devices easier to identify on a network.

Example:
- `server01`
- `office-printer`

---

## Port Numbers
- Identify services and applications running on a system.
- Help determine what type of communication is occurring.

Example:
- Port 80 → HTTP
- Port 22 → SSH

---

# Role of DNS in System Identification
- DNS maps hostnames to IP addresses.
- Helps users and applications locate systems on a network.

---

# ARP and System Identification
- ARP translates IP addresses into MAC addresses.
- Helps devices identify hardware destinations on local networks.

---

# Device Identification in Cybersecurity
Security analysts use system identification to:
- Monitor endpoints
- Detect unauthorized devices
- Investigate suspicious traffic
- Track communication sources
- Analyze network behavior

---

# Endpoint Devices
Examples of endpoints include:
- Computers
- Smartphones
- Tablets
- Servers
- Printers
- IoT devices

Each endpoint has identifying information such as:
- IP address
- MAC address
- Hostname

---

# System Identification Tools
Common tools used for system identification include:
- Ping
- ARP tables
- DNS lookup tools
- Network scanners
- SNMP monitoring tools

---

# Security Considerations
- Attackers may spoof IP or MAC addresses.
- Unknown devices on a network can indicate security risks.
- Proper identification improves incident detection and response.

---

