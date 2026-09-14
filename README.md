# TechFlow Network Infrastructure

## Overview

This project is a Cisco Packet Tracer enterprise network designed for a company with a Head Office and Branch Office.

The network demonstrates practical networking concepts including VLAN segmentation, inter-VLAN routing, HSRP, EtherChannel, OSPF, DHCP, NAT/PAT, ACLs, SSH, NTP, wireless networking and RADIUS authentication.

The project was developed and tested using Cisco Packet Tracer.
## Network Topology

![Network Topology](screenshots/network-topology.png)

## Network Architecture

The network consists of:

* Head Office network
* Branch Office network
* Multilayer switches
* Access switches
* Routers
* Wireless access points
* Server infrastructure
* Internet/ISP connection

### Head Office VLANs

| VLAN | Department     | Network        |
| ---- | -------------- | -------------- |
| 10   | Administration | 172.16.10.0/24 |
| 20   | Sales          | 172.16.20.0/24 |
| 30   | IT             | 172.16.30.0/24 |
| 40   | Servers        | 172.16.40.0/24 |
| 50   | Staff Wi-Fi    | 172.16.50.0/24 |
| 60   | Guest Wi-Fi    | 172.16.60.0/24 |
| 99   | Management     | 172.16.99.0/24 |

### Branch VLANs

| VLAN | Department            | Network        |
| ---- | --------------------- | -------------- |
| 110  | Branch Administration | 172.17.10.0/24 |
| 120  | Branch Sales          | 172.17.20.0/24 |
| 190  | Branch Management     | 172.17.99.0/24 |

## Technologies and Features

### Switching

* VLAN segmentation
* VTP
* 802.1Q trunking
* Rapid PVST / Spanning Tree
* EtherChannel
* Port security
* Access and trunk ports

### Routing

* Inter-VLAN routing
* OSPF
* HSRP
* Route summarisation
* Router-on-a-stick

### Network Services

* DHCP
* DNS
* NTP
* RADIUS
* Wireless networking

### Security

* VLAN-based network segmentation
* Guest network isolation
* Extended/standard ACL configuration
* SSH remote management
* Basic device security
* NAT/PAT

### Internet Connectivity

The network includes an ISP connection and uses NAT/PAT to allow internal networks to access the simulated Internet.

## WAN

The Head Office and Branch Office are connected through a point-to-point WAN link:

```text
R1 ---------------- R2
10.0.0.1/30       10.0.0.2/30
```

OSPF is used to exchange routes between the network locations.

## Network Topology

The final Packet Tracer topology contains the Head Office, Branch Office, WAN connection, ISP and supporting network services.

## Testing and Verification

The network was tested using Cisco IOS verification commands and connectivity tests.

Examples include:

```text
show ip ospf neighbor
show ip route
show standby brief
show etherchannel summary
show spanning-tree vlan 10
show ip nat translations
show port-security
show ntp status
```

Connectivity was also tested using:

```text
ping
ipconfig
nslookup
```

## Skills Demonstrated

This project demonstrates practical experience with:

* Cisco IOS configuration
* Network design
* IP addressing
* VLAN configuration
* Layer 2 switching
* Layer 3 routing
* OSPF
* Network redundancy
* Network security
* DHCP and DNS
* NAT/PAT
* Wireless networking
* Network troubleshooting
* Network verification

## Project File

The complete Cisco Packet Tracer project is available in:

`TechFlow-Network.pkt`

## Tools Used

* Cisco Packet Tracer
* Cisco IOS CLI
* GitHub
* Windows

## Author

Ronald Kadye

Information Technology Student

