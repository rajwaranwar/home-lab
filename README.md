

# Home Lab Portfolio

## About
Virtual network lab simulating a real enterprise environment, 
built to develop practical skills for NOC and network support roles.

## Labs

### 1. Cisco Packet Tracer
Foundational networking concepts simulated in Packet Tracer.
See packet-tracer/ folder.

### 2. pfSense Virtual Lab
Real firewall/router setup using pfSense on hyper-V 
with Ubuntu Server VMs.
See pfsense-lab/ folder.

## Skills Being Developed
- Network configuration and troubleshooting
- Firewall management (pfSense)
- Linux Server administration
- SIEM and security monitoring (Wazuh) - upcoming
- Python automation - upcoming
- Sigma detection rules - upcoming

##  Project Overview
I built a complete corporate network inside my laptop using Hyper‑V, pfSense, and Ubuntu Server — with two isolated offices, firewall rules, and SSH access. This project proves I can build, secure, and monitor a real network from scratch.

##  Topology
INTERNET
    │
    ▼
WAN-SWITCH
    │
    ▼
pfSense (192.168.10.1 / 192.168.20.1)
    │
    ├── HQ-SWITCH (192.168.10.0/24)
    │       └── Ubuntu-HQ (192.168.10.103)
    │
    └── BRANCH-SWITCH (192.168.20.0/24)
            └── Ubuntu-Branch (192.168.20.106)

## Phases
- **Phase 1**: Hyper‑V switches, pfSense, Ubuntu-HQ, Ubuntu-Branch
- **Phase 2**: Internet, DHCP, static IPs, cross‑VM connectivity
- **Phase 3**: Firewall rules (block all, allow SSH), permanent rules

##  Tests
| Test | Result |
|------|--------|
| HQ → Branch ping | ❌ Blocked |
| Branch → HQ ping | ✅ Allowed |
| HQ → Branch SSH | ✅ Allowed |

## 📸 Screenshots
[Add pfSense rules, ping results, SSH logs]

##  Credentials (redacted)
- pfSense: `admin` / `[REDACTED]`
- Ubuntu-HQ: `ubuntu-hq` / `[REDACTED]`
- Ubuntu-Branch: `branch` / `[REDACTED]`

## 📄 Configuration Files
- `ubuntu-hq-netplan.yaml`
- `ubuntu-branch-netplan.yaml`
- `pfSense-rules.txt`

##  Next Steps
- Phase 4: Wazuh SIEM (monitoring and detection)
- Phase 5: Kali Linux (offensive testing)
## Status
 In Progress — Started April 2026
