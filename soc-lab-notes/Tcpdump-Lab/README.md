# 🛡️ SOC Lab – ICMPv6 & Network Connectivity Analysis (Tcpdump)

## 📌 Overview
This lab focuses on analyzing **ICMPv6 traffic** using Tcpdump in a Linux environment.  
The objective is to understand how network connectivity is tested at the packet level and how a SOC Analyst interprets this type of traffic.

---

## 🎯 Objective
- Capture ICMPv6 traffic using Tcpdump
- Identify Echo Request and Echo Reply packets
- Understand how `ping` works at the network layer
- Differentiate normal network behavior from potential scanning activity
- Practice packet-level analysis for SOC investigations

---

## 🌐 Environment
- OS: Linux Mint (or similar Linux distribution)
- Tool: Tcpdump
- Network: Local Wi-Fi (IPv6 enabled)
- Protocol analyzed: ICMPv6

---

## 🔧 Tools Used
- tcpdump
- ping (IPv6 enabled via `-6` or automatic resolution)
- Terminal (Linux CLI)

---

## 📡 Phase 1 – ICMPv6 Capture Setup

```bash
sudo tcpdump -i wlo1 -nn icmp6
