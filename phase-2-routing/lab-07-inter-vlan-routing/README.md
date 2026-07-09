# LAB 07 – Inter-VLAN Routing (Router-on-a-Stick)

## Overview
Enabled controlled communication between the HR and Sales VLANs
(previously fully isolated since Lab 02) using a single router with
802.1Q subinterfaces, while deliberately excluding the management
VLAN from routing.

## Scenario
Departments needed to remain logically separate (VLANs preserved)
but required controlled inter-department communication — HR to reach
shared resources, Sales to reach HR for payroll-related needs.

## Topology
See `topology.svg` in this folder.

## Addressing
| VLAN | Subnet | Gateway |
|---|---|---|
| 10 (HR) | 192.168.10.0/29 | 192.168.10.1 |
| 20 (Sales) | 192.168.20.0/28 | 192.168.20.1 |
| 99 (Management) | 192.168.99.0/30 | not routed (intentional) |

## Key Concepts
- Router-on-a-stick (subinterfaces per VLAN on a single physical link)
- 802.1Q trunk between switch and router
- Default gateway configuration on end devices
- Deliberate routing exclusion as a security boundary

## Verification Commands
