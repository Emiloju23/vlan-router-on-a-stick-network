# VLAN Router-on-a-Stick Network

## Project Overview

This project demonstrates the configuration of a VLAN-based network using Cisco Packet Tracer. The network uses router-on-a-stick to enable communication between different VLANs.

## Network Topology

The network consists of:

- 1 Cisco 2911 Router
- 2 Cisco 2960 Switches
- 8 PCs
- Multiple VLANs
- Trunk links between network devices

## VLAN Configuration

| VLAN | Department | Network |
|---|---|---|
| 10 | HR | 192.168.10.0/24 |
| 20 | Finance | 192.168.20.0/24 |
| 30 | IT | 192.168.30.0/24 |
| 40 | Sales | 192.168.40.0/24 |

## IP Addressing

| PC | Department | IP Address | Default Gateway |
|---|---|---|---|
| PC0 | HR | 192.168.10.2 | 192.168.10.1 |
| PC1 | HR | 192.168.10.3 | 192.168.10.1 |
| PC2 | Finance | 192.168.20.2 | 192.168.20.1 |
| PC3 | Finance | 192.168.20.3 | 192.168.20.1 |
| PC4 | IT | 192.168.30.2 | 192.168.30.1 |
| PC5 | IT | 192.168.30.3 | 192.168.30.1 |
| PC6 | Sales | 192.168.40.2 | 192.168.40.1 |
| PC7 | Sales | 192.168.40.3 | 192.168.40.1 |

## Router-on-a-Stick

The router uses subinterfaces on GigabitEthernet0/0/0:

- G0/0/0.10 — 192.168.10.1
- G0/0/0.20 — 192.168.20.1
- G0/0/0.30 — 192.168.30.1
- G0/0/0.40 — 192.168.40.1

Each subinterface uses IEEE 802.1Q VLAN tagging.

## Verification

The network was tested using ping commands.

Tests included:

- PC-to-default-gateway connectivity
- Same-VLAN communication
- Inter-VLAN communication
- Router and switch connectivity

The tests completed successfully with 0% packet loss.

## Technologies Used

- Cisco Packet Tracer 9.0
- Cisco 2911 Router
- Cisco 2960 Switches
- VLANs
- IEEE 802.1Q
- Router-on-a-Stick
- IPv4
- Ping

## Project File

The Cisco Packet Tracer project file is included in this repository:

`Team_Vector_VLAN_Network_Final.pkt`
AUTHOT
OMONIYI OMOTAYO ERIC
