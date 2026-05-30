# Understand Network Traffic

## Network Traffic Fundamentals

* Network traffic is the flow of data between devices connected to a network.
* Network data refers to the actual information being transmitted.
* Monitoring network traffic helps organizations maintain visibility into network activity.
* Establishing a baseline of normal network behavior helps identify anomalies and potential threats.
* Security analysts use network monitoring to detect suspicious activity and indicators of compromise (IoCs).

## Components of Network Monitoring

### Flow Analysis

* Examines the movement of packets across protocols and ports.
* Helps identify unusual communication patterns.
* Detects unauthorized command and control (C2) communications.
* Monitors mismatches between protocols and commonly associated ports.

### Packet Payload Analysis

* Focuses on the actual data contained within packets.
* Can reveal unauthorized transmission of sensitive information.
* Useful for detecting data exfiltration attempts.
* Often requires decryption if traffic is encrypted.

### Temporal Analysis

* Examines network activity over time.
* Compares traffic patterns against established baselines.
* Identifies unusual activity occurring outside normal operating hours.
* Helps detect suspicious spikes in network usage.

## Network Monitoring Tools

### Intrusion Detection Systems (IDS)

* Monitor systems and networks for malicious activity.
* Generate alerts when suspicious behavior is detected.
* Analyze packet contents for known attack patterns.

### Network Protocol Analyzers

* Capture and inspect network traffic.
* Used for troubleshooting, investigations, and threat detection.
* Examples include Wireshark, tcpdump, and TShark.

---

# Capture and View Network Traffic

## Network Protocol Analyzers

* Also called packet sniffers.
* Capture, inspect, and analyze network communications.
* Convert raw packet data into a human-readable format.
* Help security analysts investigate network events.

## Network Interface Card (NIC)

* Hardware component that connects a device to a network.
* Receives and transmits network traffic.
* Must operate in monitoring mode or promiscuous mode to capture all visible traffic.

## Packet Sniffing

* Process of intercepting and examining packets moving across a network.
* Provides visibility into communications between devices.
* Useful for security investigations and network troubleshooting.

## Packet Capture (P-CAP)

* A file containing captured network packets.
* Allows analysts to save and review traffic later.
* Common file formats:

  * Libpcap
  * WinPcap
  * Npcap
  * PCAPng

## tcpdump Basics

### Purpose

* Command-line network protocol analyzer.
* Captures and analyzes network traffic.
* Commonly available on Linux and Unix-based systems.

### Common Commands

```bash
sudo tcpdump -i any
```

Captures traffic from all interfaces.

```bash
sudo tcpdump -i any -w capture.pcap
```

Saves captured traffic to a file.

```bash
sudo tcpdump -r capture.pcap
```

Reads a packet capture file.

### Useful Options

* `-i` : Specify network interface.
* `-w` : Write packets to a file.
* `-r` : Read packets from a file.
* `-v`, `-vv`, `-vvv` : Increase output detail.
* `-c` : Limit packet count.
* `-n` : Disable hostname resolution.
* `-nn` : Disable hostname and port resolution.

## Filtering Traffic

### Protocol Filters

```bash
ip6
```

Displays IPv6 traffic.

### Port Filters

```bash
port 80
```

Displays traffic using port 80.

### Boolean Operators

* `and`
* `or`
* `not`

Example:

```bash
ip and (port 80 or port 443)
```

---

# Packet Inspection

## Data Packet Structure

Packets consist of three primary components:

### Header

* Contains routing and addressing information.
* Includes source and destination addresses.
* Specifies protocol information.
* Used by network devices to deliver packets.

### Payload

* Contains the actual data being transmitted.
* May include files, messages, images, or application data.

### Footer (Trailer)

* Used primarily for error detection.
* Helps verify packet integrity during transmission.
* Commonly found in Ethernet frames.

## Internet Protocol (IP)

### IPv4 Header Fields

* Version
* Internet Header Length (IHL)
* Type of Service (ToS)
* Total Length
* Identification
* Flags
* Fragment Offset
* Time to Live (TTL)
* Protocol
* Header Checksum
* Source Address
* Destination Address
* Options

### IPv6 Header Fields

* Version
* Traffic Class
* Flow Label
* Payload Length
* Next Header
* Hop Limit
* Source Address
* Destination Address

## Wireshark Packet Inspection

### Wireshark Features

* Open-source graphical packet analyzer.
* Displays packet information in a readable format.
* Supports advanced filtering and stream analysis.

### Display Filters

#### Protocol Filters

```text
dns
http
ftp
ssh
icmp
arp
telnet
```

#### IP Address Filters

```text
ip.addr == 192.168.1.10
ip.src == 10.10.10.10
ip.dst == 8.8.8.8
```

#### MAC Address Filter

```text
eth.addr == 00:70:f4:23:18:c4
```

#### Port Filters

```text
udp.port == 53
tcp.port == 25
```

### Comparison Operators

| Operator              | Symbol | Abbreviation |
| --------------------- | ------ | ------------ |
| Equal                 | ==     | eq           |
| Not Equal             | !=     | ne           |
| Greater Than          | >      | gt           |
| Less Than             | <      | lt           |
| Greater Than or Equal | >=     | ge           |
| Less Than or Equal    | <=     | le           |

### Stream Analysis

* Reassembles communication sessions between devices.
* Displays complete protocol conversations.
* Helps analysts understand requests and responses.
* Useful for HTTP, TCP, and other protocol investigations.

## Importance of Packet Inspection

* Detects malicious network activity.
* Identifies indicators of compromise (IoCs).
* Investigates security incidents.
* Supports threat hunting and forensic analysis.
* Improves overall network visibility and security posture.
