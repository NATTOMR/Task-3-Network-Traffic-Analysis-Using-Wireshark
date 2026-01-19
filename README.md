# Task-3-Network-Traffic-Analysis-Using-Wireshark
# Task 3: Networking Basics for Cyber Security

## Project Title
**Network Traffic Analysis Using Wireshark**

---

## 1. Objective
The objective of this project is to understand basic networking concepts and develop the ability to analyze network traffic using packet capture tools. This includes observing TCP communication, DNS queries, and identifying encrypted versus plain-text traffic.

---

## 2. Tools Used

### Primary Tool
- Wireshark

### Alternative Tools (Optional)
- tcpdump
- Microsoft Network Monitor

---

## 3. Basic Networking Concepts
Before capturing traffic, the following networking concepts were studied:

- **IP Address**: A unique identifier assigned to a device on a network.
- **MAC Address**: A hardware address used to identify devices at the data link layer.
- **DNS (Domain Name System)**: Translates domain names into IP addresses.
- **TCP (Transmission Control Protocol)**: Reliable, connection-oriented protocol.
- **UDP (User Datagram Protocol)**: Fast, connectionless protocol.

---

## 4. Environment Setup
- Installed Wireshark on the system.
- Selected the active network interface (Wi-Fi / Ethernet).
- Started live packet capture.
- Generated network traffic by:
  - Browsing websites
  - Running `ping` commands
  - Accessing search engines

---

## 5. Packet Capture Process
- Wireshark was used to capture live network traffic.
- The capture ran for approximately **5–10 minutes**.
- Traffic included DNS queries, TCP connections, and HTTPS traffic.
- The captured file was saved as:

``text
`network_capture.pcapng`

## 6. Packet Filtering
The following filters were applied in Wireshark to analyze traffic effectively:

### 6.1 HTTP Traffic
``text
`http`
### 6.2 DNS Traffic
`dns`
### 6.3 TCP Traffic
`tcp`
## 7. TCP Three-Way Handshake Observation
The TCP three-way handshake was observed using the following steps:

1. **SYN** – Client requests a connection  
2. **SYN-ACK** – Server acknowledges and agrees  
3. **ACK** – Client confirms the connection  

This process confirms successful TCP connection establishment.

---

## 8. Plain-Text vs Encrypted Traffic

### Plain-Text Traffic
- HTTP traffic showed readable data such as URLs and headers.

### Encrypted Traffic
- HTTPS traffic (TLS) showed encrypted payloads that could not be read.

This demonstrates why HTTPS is more secure than HTTP.

---

## 9. DNS Query Analysis
- DNS requests were captured when visiting websites.
- Example domain queries observed:
  - `google.com`
  - `youtube.com`
- DNS responses returned the corresponding IP addresses.

This shows how DNS resolves domain names into IP addresses before communication begins.

---

## 10. Observations
- Most modern web traffic is encrypted using HTTPS.
- DNS traffic is usually unencrypted and easy to observe.
- TCP is widely used for reliable communication.
- Packet filtering makes traffic analysis easier and faster.
- Wireshark provides deep insight into network behavior.

---

## 11. Challenges Faced
- Understanding packet details initially was challenging.
- Identifying correct filters required practice.
- Large volumes of packets can be overwhelming without filtering.

---

## 12. Conclusion
This project helped develop a strong foundation in networking basics and traffic analysis. By using Wireshark, it became possible to observe real network communication, analyze protocols, and understand how data flows across a network. This knowledge is essential for cyber security professionals.


