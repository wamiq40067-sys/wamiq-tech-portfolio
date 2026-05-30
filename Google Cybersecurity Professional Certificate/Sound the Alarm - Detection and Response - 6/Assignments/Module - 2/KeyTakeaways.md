# Key Takeaways: Understand Network Traffic, Capture and View Network Traffic, Packet Inspection

## Understand Network Traffic

* Network traffic represents the movement of data between devices across a network.
* Network data is the actual information transmitted during communication.
* Establishing a network baseline helps identify abnormal or suspicious activity.
* Monitoring network traffic improves visibility into network operations and security events.
* Flow analysis helps detect unusual protocol and port usage, including potential Command and Control (C2) communications.
* Packet payload analysis can reveal unauthorized transfers of sensitive information and data exfiltration attempts.
* Temporal analysis compares network activity against expected usage patterns to identify anomalies.
* Security analysts use Indicators of Compromise (IoCs) to detect potential security incidents.
* Intrusion Detection Systems (IDS) help identify and alert on suspicious network behavior.
* Effective network monitoring is essential for threat detection, investigation, and incident response.

## Capture and View Network Traffic

* Network protocol analyzers (packet sniffers) capture and analyze network communications.
* Packet sniffing involves intercepting and inspecting packets traveling across a network.
* Packet captures (P-CAPs) store network traffic for future analysis and investigation.
* Network Interface Cards (NICs) must operate in monitoring or promiscuous mode to capture all visible traffic.
* Tcpdump is a command-line packet analyzer commonly used on Linux and Unix-based systems.
* Captured traffic can be saved, shared, and reexamined using packet capture files.
* Tcpdump supports filtering traffic by protocols, ports, IP addresses, and other criteria.
* Common tcpdump options include:

  * `-i` for selecting interfaces
  * `-w` for saving captures
  * `-r` for reading captures
  * `-v` for verbose output
  * `-c` for limiting packet count
  * `-n` for disabling name resolution
* Filtering reduces noise and helps analysts focus on relevant traffic.
* Capturing and reviewing network traffic is a critical skill for security investigations and troubleshooting.

## Packet Inspection

* Packets are the fundamental units of network communication.
* Every packet consists of a header, payload, and sometimes a footer.
* Headers contain routing, addressing, and protocol information.
* Payloads contain the actual transmitted data.
* Footers provide error-checking information in some protocols, such as Ethernet.
* Internet Protocol (IP) is responsible for addressing and routing packets across networks.
* IPv4 and IPv6 use different header structures to manage packet delivery.
* Packet inspection helps analysts understand communication patterns and identify threats.
* Wireshark is a graphical packet analyzer used to inspect packet captures in detail.
* Display filters in Wireshark help isolate traffic based on protocols, IP addresses, MAC addresses, and ports.
* Comparison operators and logical expressions make packet filtering more precise.
* Stream analysis reconstructs conversations between devices, making communications easier to understand.
* Packet inspection supports threat hunting, incident response, forensic analysis, and network troubleshooting.
* Understanding packet structure and analysis tools is essential for identifying malicious network activity.
