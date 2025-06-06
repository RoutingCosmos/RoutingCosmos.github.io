# OSPF Dynamic Routing Lab – Three-Router Mesh Network

## Overview

This project demonstrates the configuration and implementation of the OSPFv2 dynamic routing protocol across a three-router mesh network using Cisco Packet Tracer. 
The goal was to establish full neighbor adjacency, dynamic route propagation, and redundancy within the network.

## Topology

- Three Cisco routers connected in a triangular mesh topology.
- Each router advertises directly connected networks using OSPF in Area 0.
- FastEthernet interfaces configured with subnetted private IP ranges (10.0.x.x/24).

## Objectives

- Configure OSPFv2 on all routers to enable dynamic routing.
- Verify OSPF neighbor relationships and full adjacency.
- Validate routing table convergence and equal-cost multipath routing.
- Test network connectivity using ICMP ping between all routers.
- Observe Designated Router (DR) and Backup Designated Router (BDR) election on shared Ethernet links.

## Configuration Highlights

- OSPF Process ID: 1
- Area: 0 (Backbone)
- Network statements advertising all directly connected subnets.
- Interface IP addressing using 10.0.x.x/24 subnets.
- Interfaces brought up with `no shutdown`.
- Verification commands used:
  - `show ip ospf neighbor`
  - `show ip route ospf`
  - `ping`
