# LAB 13 – DHCP (Server & Relay)

## Overview
Converted all PCs across HQ and the branch office from static IP
addressing to DHCP, with HQ-R1 acting as a centralized DHCP server
for all three subnets, and BRANCH-R1 relaying DHCP broadcasts across
the WAN using ip helper-address.

## Scenario
Manually assigning static IPs to every new employee's PC was slow
and error-prone — a duplicate IP assignment had already caused a
conflict. DHCP automates address assignment, eliminating both
problems.

## Topology
See `topology.svg` in this folder.

## Addressing
| Network | Subnet | Gateway (excluded from pool) |
|---|---|---|
| VLAN 10 (HR) | 192.168.10.0/29 | 192.168.10.1 |
| VLAN 20 (Sales) | 192.168.20.0/28 | 192.168.20.1 |
| Branch LAN (VLAN 30) | 192.168.30.0/29 | 192.168.30.1 |

## Key Concepts
- Why DHCP broadcasts don't cross routers by default (broadcasts
  never leave the originating network segment)
- `ip helper-address` as a broadcast-to-unicast relay mechanism,
  configured on the router interface actually facing the requesting
  clients
- Excluding gateway addresses from DHCP pools to prevent IP conflicts
  with router interfaces
- Centralized (single DHCP server) vs distributed (per-site DHCP
  server) design tradeoffs

## Verification Commands
