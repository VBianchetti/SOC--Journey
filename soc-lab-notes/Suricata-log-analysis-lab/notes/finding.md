# Findings

Source IP identified:
- 192.168.0.13

Observed event types:
- alert
- flow

Primary Investigation:
- Nmap scan traffic from 192.168.0.13

Secondary Observations (noise):
- ET INFO Spotify P2P Client

Analysis performed:
- Source IP filtering
- Event correlation
- Log inspection

Lessons Learned:
- Understanding Suricata JSON logs
- Event investigation using jq
- Basic SOC workflow
