# Network Notes

## Table of Contents
1. [What is Networking?](#what-is-networking)
2. [TCP/IP Five-Layer Model](#tcpip-five-layer-model)
3. [Basic Networking Devices](#basic-networking-devices)
4. [Name Resolution](#name-resolution)
5. [OSI Model](#osi-model)
6. [IP Addresses](#ip-addresses)
7. [Subnetting](#subnetting)
8. [The Transport Layer](#the-transport-layer)
9. [Routing](#routing)
10. [Firewalls](#firewalls)
11. [Advanced DNS Concepts](#advanced-dns-concepts)
12. [TCP Details](#tcp-details)
13. [Advanced Routing Concepts](#advanced-routing-concepts)
14. [Network Address Translation (NAT)](#network-address-translation-nat)
15. [IPv6 Addressing and Subnetting](#ipv6-addressing-and-subnetting)
16. [Network Troubleshooting Tools](#network-troubleshooting-tools)
17. [Cloud Computing](#cloud-computing)
18. [Firewalls and Security](#firewalls-and-security)
19. [CCNA Topics](#ccna-topics)
    - [Network Fundamentals](#network-fundamentals)
    - [LAN Switching Technologies](#lan-switching-technologies)
    - [Routing Technologies](#routing-technologies)
    - [WAN Technologies](#wan-technologies)
20. [MCSA Topics](#mcsa-topics)
    - [Active Directory](#active-directory)
    - [Windows Server](#windows-server)
    - [Networking with Windows Server](#networking-with-windows-server)

## What is Networking?
- **Protocol**: A defined set of standards that computers must follow to communicate properly.
- **Computer Networking**: The full scope of how computers communicate with each other.

## TCP/IP Five-Layer Model
| Layer | Name         | Protocols        | Protocol Data Unit | Addressing     |
|-------|--------------|------------------|--------------------|----------------|
| 5     | Application  | HTTP, SMTP, etc. | Messages           | n/a            |
| 4     | Transport    | TCP/UDP          | Segment            | Port #'s       |
| 3     | Network      | IP               | Datagram           | IP Address     |
| 2     | Data Link    | Ethernet, Wi-Fi  | Frames             | MAC Address    |
| 1     | Physical     | 10 Base T, 802.11| Bits               | n/a            |

### Physical Layer
Represents physical devices that interconnect computers, specifications, joiners, signals, cabling, connectors, and sending signals.

### Data Link Layer (Network Interface / Network Access Layer)
Defines a common way of interpreting signals so network devices can communicate.
- Common protocols: Ethernet, Wi-Fi.
- Responsible for getting data across a single link.

## Basic Networking Devices
### Cables
- **Types**: Copper or fiber.
- **Common Forms**: Cat5, Cat5e, Cat6.
- **Fiber Optic**: Pulses of light, used in places with electromagnetic interference.

### Hubs and Switches
- **Hub**: Physical layer device allowing connections from many computers.
- **Switch**: Data-link layer device, eliminates collision domains.

### Routers
- Connects different networks (LAN, WAN).
- **Function**: Forward data between networks, operates at the Network Layer.
- **BGP**: Border Gateway Protocol, lets routers learn optimal paths for traffic.

## Name Resolution
- **DNS**: Domain Name System, resolves domain names to IP addresses.
- **MAC Address**: 48-bit binary numbers.
- **IP Address**: Addresses used in DNS can change frequently.

## OSI Model
| Layer       | Protocol Data Unit (PDU) | Function                                           |
|-------------|--------------------------|----------------------------------------------------|
| 7. Application | High-level APIs            | Resource sharing, remote file access                |
| 6. Presentation| Data                     | Translation between networking service and application|
| 5. Session    |                        | Managing communication sessions                     |
| 4. Transport  | Segment (TCP)/Datagram (UDP) | Reliable transmission, segmentation, acknowledgement |
| 3. Network    | Packet                   | Structuring and managing a multi-node network       |
| 2. Data Link  | Frame                    | Reliable transmission between two nodes             |
| 1. Physical   | Bit                      | Transmission of raw bit streams                     |

## IP Addresses
- **IPv4**: 32-bit addresses.
- **IPv6**: 128-bit addresses, uses hexadecimal notation.

## Subnetting
- **Subnet Mask**: Defines the network and host portions of an IP address.
- **CIDR**: Classless Inter-Domain Routing, provides flexible addressing.

## The Transport Layer
- **TCP**: Transmission Control Protocol, reliable transmission.
- **UDP**: User Datagram Protocol, connectionless and faster but less reliable.

## Routing
- **Routing Table**: Used by routers to determine the next hop for packet forwarding.
- **Interior Gateway Protocols**: RIP, EIGRP.
- **Exterior Gateway Protocols**: BGP.

## Firewalls
- **Function**: Block traffic that meets certain criteria.
- **Implementation**: Can operate at various network layers, often integrated with routers.

## Advanced DNS Concepts
- **Resource Record Types**: A, AAAA, CNAME, MX, SRV, TXT, NS, SOA.
- **Name Resolution Process**: Steps for converting domain names to IP addresses.

## TCP Details
- **TCP Segment Structure**: Header, data section, and control flags.
- **Three-Way Handshake**: SYN, SYN-ACK, ACK.

## Advanced Routing Concepts
- **Mesh Network**: Ensures multiple paths for packet delivery.
- **Non-Routable Address Space**: IP ranges reserved for internal use (RFC 1918).

## Network Address Translation (NAT)
- **Purpose**: Allows internal devices to communicate with external networks.
- **Types**: Static, dynamic, PAT (Port Address Translation).

## IPv6 Addressing and Subnetting
- **Structure**: 128-bit addresses, divided into network and host portions.
- **IPv6 Header**: Contains fields like version, traffic class, flow label, and hop limit.

## Network Troubleshooting Tools
- **ICMP**: Used for error reporting and diagnostics (e.g., ping).
- **Traceroute**: Discovers the path between two nodes.
- **Netcat**: Tests port connectivity.

## Cloud Computing
- **Services**: IaaS, PaaS, SaaS.
- **Cloud Types**: Public, private, hybrid.
- **Virtualization**: Use of hypervisors to manage virtual machines.

## Firewalls and Security
- **Types**: Network-based, host-based.
- **Functions**: Blocking unauthorized access, logging, and auditing traffic.

## CCNA Topics

### Network Fundamentals
- **Basic Concepts**: Network topologies, types of networks (LAN, WAN, MAN), and the role of network components.
- **IP Addressing**: Subnetting, VLSM (Variable Length Subnet Mask), IPv4 vs IPv6.
- **Cabling and Media**: UTP, STP, Fiber Optic, Coaxial, and cable standards (e.g., TIA/EIA-568-B).

### LAN Switching Technologies
- **Switching Concepts**: MAC address tables, VLANs, trunking (802.1Q), inter-VLAN routing.
- **Spanning Tree Protocol (STP)**: Purpose and operation, types of STP (e.g., RSTP).
- **EtherChannel**: Bundling multiple physical links for increased bandwidth.

### Routing Technologies
- **Routing Basics**: Static vs dynamic routing, routing tables.
- **Routing Protocols**: OSPF, EIGRP, RIP.
- **First Hop Redundancy Protocols (FHRPs)**: HSRP, VRRP, GLBP.

### WAN Technologies
- **WAN Protocols**: PPP, Frame Relay, MPLS.
- **VPNs**: Site-to-site and remote-access VPNs.
- **GRE Tunnels**: Use and configuration.

## MCSA Topics

### Active Directory
- **AD Concepts**: Forests, domains, OUs (Organizational Units), schema.
- **AD DS (Active Directory Domain Services)**: Installation, configuration, and management.
- **Group Policy**: Creating and managing GPOs, applying GPOs to OUs.

### Windows Server
- **Installation and Configuration**: Server roles and features, Windows Server installation options.
- **Storage Solutions**: Disk management, RAID configurations, file systems (NTFS, ReFS).
- **Networking Services**: DHCP, DNS, VPN, DirectAccess.

### Networking with Windows Server
- **IP Address Management (IPAM)**: IP address tracking, management, and auditing.
- **Network Access Protection (NAP)**: Health policies, NAP enforcement.
- **Remote Access**: RADIUS, NPS (Network Policy Server), configuring remote access solutions.

