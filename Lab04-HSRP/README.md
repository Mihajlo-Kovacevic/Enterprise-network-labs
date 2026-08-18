# Lab 04 – HSRP

## Overview

This lab demonstrates the configuration and verification of Hot Standby Router Protocol (HSRP) in a Cisco network environment.

HSRP provides first-hop redundancy by allowing multiple routers or Layer 3 switches to share a virtual IP address that is used as the default gateway by end devices.

The purpose of the lab is to provide gateway redundancy and maintain network connectivity if the active gateway becomes unavailable.

## Objectives

- Configure HSRP between two Layer 3 devices
- Configure a virtual IP address
- Configure HSRP priority
- Configure the Active and Standby routers
- Understand HSRP gateway redundancy
- Verify HSRP status
- Test gateway failover
- Verify network connectivity after failover

## Technologies

- Cisco IOS
- Cisco Packet Tracer
- HSRP
- First-Hop Redundancy Protocol
- VLAN
- Inter-VLAN Routing
- Layer 3 Switching

## Network Topology

The topology uses two Layer 3 devices that provide redundant default gateway services for the connected hosts.

Both devices participate in HSRP and share a virtual IP address.

The network topology is available in the `Topology` directory.

## HSRP Configuration

HSRP provides a virtual default gateway for end devices.

The HSRP configuration includes:

- HSRP group
- Virtual IP address
- HSRP priority
- Active router
- Standby router

The device with the higher HSRP priority becomes the Active router, while the other device operates as the Standby router.

## HSRP Failover

One of the main objectives of the lab is to test gateway redundancy.

The Active device was intentionally taken offline to simulate a failure.

The Standby device then takes over the Active role and continues providing the virtual gateway.

This allows end devices to maintain connectivity without changing their configured default gateway.

## Verification

The following Cisco IOS commands were used to verify HSRP:

```text
show standby
show standby brief
show ip interface brief
