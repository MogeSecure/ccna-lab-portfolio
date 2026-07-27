# Phase 3 — Services

Labs covering the network services that make a company network
actually usable day-to-day — automatic addressing, address
translation, traffic filtering, and secure remote management.

## Labs in This Phase

| Lab | Topic | Status |
|---|---|---|
| [13 – DHCP (Server & Relay)](./lab-13-dhcp) | Centralized DHCP server, ip helper-address relay across a WAN | ✅ |
| 14 – NAT | Translating private addresses for internet access | ⏳ Planned |
| 15 – ACLs | Standard and extended access control lists | ⏳ Planned |
| 16 – SSH | Replacing Telnet with encrypted remote management | ⏳ Planned |
| 17 – Security Hardening Review | Consolidating security practices across the network | ⏳ Planned |

## What This Phase Demonstrates
- Moving from manually configured end devices to centralized,
  automatic network services
- Understanding why certain traffic (like DHCP broadcasts) needs
  special handling to cross routed boundaries
- Building toward a network that's not just functional, but
  operationally practical at scale

## Building on Phases 1 and 2
This phase reuses the exact switching and routing topology from
Phases 1-2 — DHCP, NAT, ACLs, and SSH are layered on top of an
already-functioning network, the way real services get added to
existing infrastructure rather than rebuilt from scratch each time.

**Status: 1 of 5 labs complete**
