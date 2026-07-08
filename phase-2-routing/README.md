
# Phase 2 — Routing

Labs covering how traffic moves between networks — starting with
getting isolated VLANs to communicate, then building up to dynamic
routing protocols and real troubleshooting scenarios.

## Labs in This Phase

| Lab | Topic | Status |
|---|---|---|
| [07 – Inter-VLAN Routing](./lab-07-inter-vlan-routing) | Router-on-a-stick, subinterfaces, controlled inter-VLAN communication | ✅ |
| 08 – Static Routing | Manually defined routes between networks | ⏳ Planned |
| 09 – Default Routing & Routing Tables | Deep dive into how routers choose paths | ⏳ Planned |
| 10 – OSPF Single-Area | Dynamic routing basics | ⏳ Planned |
| 11 – OSPF Multi-Area | Scaling dynamic routing | ⏳ Planned |
| 12 – Routing Troubleshooting | Diagnosing a broken routing scenario from scratch | ⏳ Planned |

## What This Phase Demonstrates
- Moving from fully isolated VLANs (Phase 1) to controlled,
  deliberate communication between networks
- Manual routing logic before introducing dynamic protocols
- Realistic network design decisions — such as deliberately keeping
  the management VLAN unroutable for security

## Building on Phase 1
This phase reuses the exact switching topology from Phase 1 (VLANs,
trunking, EtherChannel, STP) rather than starting over — routing is
added on top of an already-functioning switched network, the way it
would be in a real company.

**Status: 1 of 6 labs complete**
