# 📡 Telecommunications Networks – Lab Series

This repository contains a set of practical labs for the *Telecommunications Networks* course, focusing on the hands-on exploration of DNS, HTTP, and TCP protocol behaviors using diagnostic tools such as `nslookup`, `Wireshark`, and browser-based packet analysis.

## 📁 Contents

The lab series is organized into three main experiments:

### 1. **Lab 1 – DNS Exploration**
- Tools used: `nslookup`, `ifconfig`, `scutil`, `traceroute`
- Objective: To understand the structure and function of the DNS hierarchy, authoritative name servers, and domain resolution.
- Activities:
  - DNS record lookups using `nslookup`
  - Authoritative server resolution
  - Reverse DNS queries and mail server lookups
  - Network interface configuration and diagnostic introspection
  - Traceroute to analyze path and latency

### 2. **Lab 2 – HTTP Protocol Analysis**
- Tools used: Web Browser, `Wireshark`
- Objective: To inspect HTTP GET/response interactions, HTTP versioning, conditional GETs, content caching, and response headers.
- Activities:
  - Capturing simple HTTP GET requests
  - Investigating HTTP headers (e.g., `If-Modified-Since`)
  - Response status code analysis
  - Understanding content-length and modification timestamps
  - Use of Wireshark filters to isolate HTTP packets

### 3. **Lab 3 – TCP Behavior with Wireshark**
- Tools used: `Wireshark`, Web Server
- Objective: To observe TCP's mechanisms for reliable data transmission including 3-way handshakes, retransmissions, flow control, and congestion control.
- Activities:
  - Uploading `alice.txt` to a remote server via HTTP POST
  - Capturing the TCP handshake and data transfer
  - Sequence and acknowledgment number tracking
  - Analyzing slow start and congestion avoidance
  - Examining timeout and fast retransmission behavior

## 🛠 Tools and Protocols Used
- **Wireshark** – Deep packet inspection and protocol analysis
- **nslookup** – DNS querying and name resolution
- **scutil/ifconfig** – System DNS and interface configuration
- **Browser** – To trigger HTTP GET/POST actions
- **TCP/IP Stack** – Underlying protocol operations

## 📘 Prerequisites
- Basic knowledge of TCP/IP networking
- Wireshark installed on your system
- Internet connection to reach test domains (e.g., `gaia.cs.umass.edu`)

## 🚀 How to Run the Labs
1. Follow the instructions in each lab's PDF/DOCX file.
2. Use the appropriate command-line tools and browser for each experiment.
3. Capture network traffic using Wireshark with filters like:
```
ip.addr == your_ip_address
http
tcp
```

4. Answer the listed questions based on your captures and observations.

## 👤 Author

**Papadopoulos Panagiotis**  
Student ID: 10697  
School of Electrical and Computer Engineering  
Aristotle University of Thessaloniki

## 📚 References

- *Computer Networking: A Top-Down Approach* – Kurose & Ross
- RFC 793, RFC 1122, RFC 2018, RFC 5681, RFC 7323
- [Wireshark Labs – UMass Amherst](http://gaia.cs.umass.edu/wireshark-labs/)

---