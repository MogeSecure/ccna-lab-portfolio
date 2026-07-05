# LAB 02 – VLAN Segmentation

## Overview
Segmented a single Cisco 2960 switch into separate broadcast domains
for HR and Sales departments using VLANs, and moved switch management
off the default VLAN 1 onto a dedicated management VLAN — fixing the
known limitation from Lab 01.

## Scenario
Company has two departments sharing one switch. Manager requires that
HR and Sales never see each other's broadcast traffic, and that
management access be isolated from the default VLAN.

## Topology
See `topology.svg` in this folder.

## VLANs & Addressing
| VLAN | Name | Subnet | Mask |
|---|---|---|---|
| 10 | HR | 192.168.10.0/29 | 255.255.255.248 |
| 20 | Sales | 192.168.20.0/28 | 255.255.255.240 |
| 99 | Management | 192.168.99.0/30 | 255.255.255.252 |

Subnets sized using host-count planning: HR (3 users, buffer to 6) →
/29. Sales (10 users) → /28. Management (1 device) → /30.

## Skills Practiced
- VLAN creation and naming
- Access port VLAN assignment (`switchport access vlan`)
- Dedicated management VLAN (replacing VLAN 1)
- Subnetting sized to real department headcount + growth buffer

## Verification Commands
\`\`\`
show vlan brief
show ip interface brief
\`\`\`

## Result
PCs within the same VLAN can communicate; PCs in different VLANs
cannot — confirming broadcast domain separation. No router is present
yet, so inter-VLAN communication is intentionally blocked (addressed
in Lab 07).

## Files
- `lab-02.pkt` — open in Cisco Packet Tracer
- `topology.svg` — visual topology reference

## Status
✅ Completed
