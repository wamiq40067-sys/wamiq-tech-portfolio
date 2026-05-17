# Key Notes: Network Intrusion Tactics

## 1. Introduction to Network Intrusion Tactics

Network intrusion tactics refer to methods used by attackers to gain unauthorized access to systems, steal data, or disrupt services.

### Common Intrusion Techniques:
- **Packet sniffing:** Capturing network traffic to inspect sensitive data.
- **IP spoofing:** Faking source IP addresses to impersonate trusted systems.
- **On-path attacks:** Intercepting communication between two trusted devices.
- **Replay attacks:** Capturing and retransmitting valid data packets to gain access.
- **Malware-based intrusion:** Using malicious software to gain control over systems.

### Key Idea:
Attackers often exploit weak authentication, unencrypted traffic, and misconfigured networks.

---

## 2. Securing Networks Against Denial of Service (DoS) Attacks

DoS attacks aim to make systems unavailable by overwhelming them with traffic.

### Types of DoS Attacks:
- **ICMP flood:** Overloads systems using repeated ping requests.
- **SYN flood:** Exploits TCP handshake by sending repeated connection requests.
- **Ping of death:** Sends oversized ICMP packets to crash systems.
- **Smurf attack:** Uses spoofed IP and broadcast networks to amplify traffic.

### Defense Strategies:
- Use **firewalls** to filter suspicious traffic.
- Implement **rate limiting** to control request volume.
- Deploy **intrusion detection systems (IDS)**.
- Monitor traffic patterns for unusual spikes.
- Use **next-generation firewalls (NGFWs)** for anomaly detection.
- Apply **traffic filtering and blackholing** for attack mitigation.

---

## 3. Network Attack Tactics and Defense

### Attack Tactics:
- **Passive packet sniffing:** Listening to network traffic without modifying it.
- **Active packet sniffing:** Intercepting and altering network traffic.
- **Botnets:** Networks of compromised devices controlled by attackers.
- **DDoS attacks:** Coordinated attacks from multiple systems to overwhelm services.
- **IP spoofing:** Disguising attack source identity.
- **Replay attacks:** Reusing captured packets for unauthorized access.

### Defense Mechanisms:
- Encrypt data using **TLS/HTTPS** to prevent interception.
- Use **strong authentication mechanisms** (MFA, certificates).
- Segment networks to limit attack spread.
- Monitor logs and traffic using **SIEM tools**.
- Configure firewalls to block spoofed or suspicious packets.
- Keep systems patched and updated regularly.

---

