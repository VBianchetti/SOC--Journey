# Suricata IDS Lab - Log Analysis and Event Investigation

## Objective

This project demonstrates the deployment of Suricata IDS and the analysis of network events using JSON logs and jq filters.

## Environment

### Monitoring Machine

* Linux Mint
* Suricata IDS
* jq

### Traffic Generation

* macOS (Apple Silicon)
* Nmap

### Network

* Local Network (192.168.0.0/24)

## Tools Used

* Suricata
* jq
* Nmap
* Linux Mint

## Evidence

### 1. Suricata Running

![Suricata Status](screenshots/01-suricata-status.png)

Suricata service running and monitoring network traffic.

### 2. Traffic Generation

![Nmap Scan](screenshots/02-nmap-scan-mac.png)

Traffic generated from a separate host using Nmap.

### 3. Event Investigation

![Log Analysis](screenshots/03-jq-filter-src-ip.png)

Filtering events by source IP using jq.

### 4. Alert Analysis

![Alert Event](screenshots/04-alert-log.png)

Reviewing Suricata alerts stored in eve.json.

### 5. Additional Event Investigation

![Additional Analysis](screenshots/05-event-analysis.png)

Analysis of captured network events.

## Findings

* Successfully deployed Suricata IDS.
* Generated and monitored network traffic.
* Investigated events using jq.
* Identified source IP activity through log filtering.
* Learned basic SOC investigation workflow.

## Skills Demonstrated

* Network Monitoring
* IDS Analysis
* Log Investigation
* JSON Parsing
* Linux Administration
* Basic SOC Operations
