# Lab 03 – STP and EtherChannel

## Overview

This lab demonstrates the configuration and verification of Spanning Tree Protocol (STP) and EtherChannel in a Cisco switched network environment.

The purpose of the lab is to prevent Layer 2 loops using STP and to provide link redundancy and increased bandwidth by combining multiple physical links into a single logical EtherChannel.

## Objectives

- Configure and verify VLANs
- Configure trunk links between switches
- Configure Spanning Tree Protocol
- Understand root bridge election
- Configure STP priority
- Verify STP port roles and states
- Configure EtherChannel
- Combine multiple physical links into a logical Port-Channel
- Verify EtherChannel operation
- Test network connectivity and redundancy

## Technologies

- Cisco IOS
- Cisco Packet Tracer
- VLAN
- IEEE 802.1Q Trunking
- Spanning Tree Protocol (STP)
- EtherChannel
- Port-Channel
- Layer 2 Switching

## Network Topology

The topology consists of multiple Cisco switches connected using redundant links.

STP is used to prevent Layer 2 loops, while EtherChannel is used to combine multiple physical links into a single logical connection between switches.

The network topology is available in the `Topology` directory.

## Spanning Tree Protocol

STP is used to prevent Layer 2 switching loops in a redundant switched network.

The lab demonstrates:

- Root Bridge election
- Bridge ID
- STP priority
- Root ports
- Designated ports
- Blocking/forwarding states
- STP convergence

STP verification commands:

```text
show spanning-tree
show spanning-tree vlan 10
show spanning-tree root
