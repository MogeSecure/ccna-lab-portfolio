# Phase 1 — Switching Foundations

Six labs covering core Layer 2 switching concepts, built progressively
on a shared topology — each lab adds a new capability on top of the
last, mirroring how a real network evolves as a company grows.

## Labs in This Phase

| Lab | Topic | Status |
|---|---|---|
| [01 – Switch Deployment & Hardening](./lab-01-switch-deployment) | Basic IOS config, device hardening, subnetting fundamentals | ✅ |
| [02 – VLAN Segmentation](./lab-02-vlan-segmentation) | Broadcast domain separation, dedicated management VLAN | ✅ |
| [03 – Trunking Between Switches](./lab-03-trunking) | 802.1Q trunks, extending VLANs across multiple switches | ✅ |
| [04 – Spanning Tree Protocol](./lab-04-stp) | Loop prevention, root bridge election, redundant links | ✅ |
| [05 – STP Security](./lab-05-stp-security) | Port Security, BPDU Guard, Root Guard | ✅ |
| [06 – EtherChannel](./lab-06-etherchannel) | Link aggregation with LACP, bandwidth combining | ✅ |

## What This Phase Demonstrates
- Building a switched network from a single device up to a
  multi-switch, VLAN-segmented, loop-protected, load-balanced topology
- Subnetting sized to actual host requirements at every stage, not
  arbitrary /24s
- Progressive hardening: from basic passwords (Lab 01) to full access
  control and STP attack prevention (Lab 05)
- Real device-to-device continuity — each lab builds on the network
  design from the previous one, the way a company's network actually
  grows over time

## Topology Evolution
- Lab 01: 1 switch, 4 PCs, flat network
- Lab 02: same switch, segmented into HR/Sales/Management VLANs
- Lab 03: 2nd switch added, VLANs extended via trunk
- Lab 04: redundant link added between switches, STP prevents loop
- Lab 05: access and trunk ports hardened against unauthorized devices
- Lab 06: redundant link converted to an active-active EtherChannel

**Status: Phase 1 complete (6/6 labs)**
