# 🛡️ SOC Lab – Network Traffic Analysis with Tcpdump (DNS + ICMPv6)

## 📌 Overview
This lab focuses on **network traffic analysis using Tcpdump in a Linux environment**, simulating real SOC (Security Operations Center) activities.

The objective is to understand how DNS resolution, traffic filtering, and ICMPv6 connectivity tests work at the packet level, and how a SOC Analyst interprets network behavior in real time.

---

## 🎯 Objective
- Analyze DNS queries and responses (A and AAAA records)
- Understand IPv4 vs IPv6 resolution behavior
- Capture and filter network traffic using Tcpdump
- Identify ICMPv6 Echo Request and Echo Reply packets
- Understand basic network connectivity at packet level
- Differentiate normal traffic from potentially suspicious behavior

---

## 🌐 Environment
- OS: Linux Mint (or similar Linux distribution)
- Tools: Tcpdump, Ping
- Network: Local Wi-Fi (IPv6 enabled)
- Protocols analyzed: DNS, TCP/IP, ICMPv6

---

## 🔧 Tools Used
- tcpdump (packet capture and filtering)
- ping (network connectivity testing)
- Linux terminal (CLI)

---

# 📡 Phase 1 – DNS Traffic Analysis

We analyzed DNS traffic to understand how domain resolution works before a connection is established.

### 🔍 Observed DNS behavior:
- `A?` → IPv4 resolution request
- `AAAA?` → IPv6 resolution request
- Multiple IP addresses returned (CDN behavior)
- Dual-stack DNS queries are standard in modern browsers

### 📌 Example:
```text
A? google.com
AAAA? google.com
