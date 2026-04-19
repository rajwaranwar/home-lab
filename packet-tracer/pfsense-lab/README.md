# pfSense Home Lab

## What is this?
A virtual network lab simulating a real company network with a head office and branch office, built on VirtualBox.

## Setup so far
- pfSense 2.8.1 installed and configured as firewall/router
- WAN interface (le0) getting IP via DHCP
- LAN interface (le1) assigned static IP 192.168.56.2/24
- DHCP server configured to hand out 192.168.56.100 - 192.168.56.200
- Windows host successfully pinging pfSense LAN IP

## In Progress
- Ubuntu-HQ (Head Office VM)
- Ubuntu-Branch (Branch Office VM)

## Planned
- VLANs, ACLs, NAT
- Site-to-site VPN
- Wazuh SIEM
- Python automation scripts
- Sigma detection rules
