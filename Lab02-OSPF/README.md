Lab 02 – OSPF
## Overview

This lab demonstrates the configuration and verification of OSPF (Open Shortest Path First) as a dynamic routing protocol in a Cisco network environment.

The objective of the lab is to establish dynamic routing between multiple routers and enable communication between different networks using OSPF.

## Objectives

- Configure OSPF on Cisco routers
- Configure OSPF router IDs
- Establish OSPF neighbor adjacencies
- Advertise network prefixes using OSPF
- Verify OSPF neighbor relationships
- Verify dynamically learned routes
- Test end-to-end connectivity
- Troubleshoot OSPF connectivity issues

## Technologies

- Cisco IOS
- Cisco Packet Tracer
- OSPF
- IPv4
- Dynamic Routing
- Routing Tables

## Network Topology

The topology consists of multiple Cisco routers interconnected through routed links.

The routers use OSPF to dynamically exchange routing information and learn remote networks.

The network topology is available in the `Topology` directory.

## OSPF Configuration

OSPF is configured on the routers using a common OSPF process.

The configuration includes:

- OSPF process configuration
- Router ID configuration
- Network advertisements
- OSPF area configuration
- OSPF neighbor establishment

## Verification

The following Cisco IOS commands were used to verify the OSPF configuration:

```text
show ip ospf neighbor
show ip ospf interface
show ip ospf
show ip route
show ip route ospf
