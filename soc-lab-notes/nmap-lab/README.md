# 🛡️ SOC Lab – Network Security Assessment with Nmap

## 📌 Overview

This laboratory documents the use of **Nmap** to perform network reconnaissance and attack surface analysis in a controlled home lab environment.

The objective is to identify active hosts, enumerate exposed services, analyze firewall behavior, and document security findings from a Blue Team perspective.

---

## 🎯 Objectives

- Discover active hosts on the local network
- Identify open, closed, and filtered ports
- Enumerate running services
- Analyze firewall behavior
- Identify potential security risks
- Practice attack surface assessment techniques

---

## 🌐 Environment

- **Operating System:** Linux Mint 22.3
- **Tool:** Nmap v7.x
- **Network:** 192.168.0.0/24
- **Environment:** Authorized Home Lab

---

# 🔎 Phase 1 – Host Discovery

```bash
nmap -sn 192.168.0.0/24
```

### Findings

- Gateway detected (`192.168.0.1`)
- Active endpoint detected
- Linux workstation detected

This scan was used to identify active assets connected to the local network.

---

# 🔍 Phase 2 – Service Enumeration

```bash
nmap -sV 192.168.0.1
```

### Findings

- HTTP service detected (TCP/80)
- UPnP service detected (TCP/5431)
- Multiple filtered ports identified

The enumeration revealed services exposed by the router and provided visibility into the local attack surface.

---

# 🛡️ Phase 3 – Firewall Assessment

Additional scans were performed to verify filtered and open ports.

Observed behavior indicates that the firewall blocks several services while allowing only essential management services.

---

# ⚠️ Security Observations

- HTTP management interface exposed on port 80
- UPnP service enabled
- Several ports filtered by firewall
- Limited external exposure observed

---

# 🔐 Hardening Recommendations

- Disable UPnP if not required
- Enable HTTPS management if supported
- Keep router firmware updated
- Restrict management access to trusted hosts
- Continuously monitor network assets

---

# 📚 Conclusion

This laboratory demonstrates practical use of Nmap for host discovery, service enumeration, and attack surface assessment in a home lab environment.

The exercise reinforces Blue Team concepts related to asset visibility, exposure analysis, and network hardening.

---

## 🚀 Skills Demonstrated

- Network Discovery
- Service Enumeration
- Attack Surface Mapping
- Firewall Analysis
- Security Assessment
- Blue Team Fundamentals

---

## ⚠️ Disclaimer

This project was performed in a controlled and authorized home lab environment for educational purposes only.
