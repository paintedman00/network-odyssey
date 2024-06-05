# Networking

## Table of Contents
1. [Beginner Topics](#beginner-topics)
    - [What is Networking?](#what-is-networking)
    - [TCP/IP Five-Layer Model](#tcpip-five-layer-model)
    - [Basic Networking Devices](#basic-networking-devices)
    - [Name Resolution](#name-resolution)
2. [Intermediate Topics](#intermediate-topics)
    - [OSI Model](#osi-model)
    - [IP Addresses](#ip-addresses)
    - [Subnetting](#subnetting)
    - [The Transport Layer](#the-transport-layer)
    - [Routing](#routing)
    - [Firewalls](#firewalls)
3. [Advanced Topics](#advanced-topics)
    - [Advanced DNS Concepts](#advanced-dns-concepts)
    - [TCP Details](#tcp-details)
    - [Advanced Routing Concepts](#advanced-routing-concepts)
    - [Network Address Translation (NAT)](#network-address-translation-nat)
    - [IPv6 Addressing and Subnetting](#ipv6-addressing-and-subnetting)
    - [Network Troubleshooting Tools](#network-troubleshooting-tools)
    - [Cloud Computing](#cloud-computing)
    - [Firewalls and Security](#firewalls-and-security)

## Beginner Topics

### What is Networking?
- **Protocol**: A defined set of standards that computers must follow to communicate properly.
- **Computer Networking**: The full scope of how computers communicate with each other.

### TCP/IP Five-Layer Model
| Layer | Name         | Protocols        | Protocol Data Unit | Addressing     |
|-------|--------------|------------------|--------------------|----------------|
| 5     | Application  | HTTP, SMTP, etc. | Messages           | n/a            |
| 4     | Transport    | TCP/UDP          | Segment            | Port #'s       |
| 3     | Network      | IP               | Datagram           | IP Address     |
| 2     | Data Link    | Ethernet, Wi-Fi  | Frames             | MAC Address    |
| 1     | Physical     | 10 Base T, 802.11| Bits               | n/a            |

#### Physical Layer
Represents physical devices that interconnect computers, specifications, joiners, signals, cabling, connectors, and sending signals.

#### Data Link Layer (Network Interface / Network Access Layer)
Defines a common way of interpreting signals so network devices can communicate.
- Common protocols: Ethernet, Wi-Fi.
- Responsible for getting data across a single link.

### Basic Networking Devices
#### Cables
- **Types**: Copper or fiber.
- **Common Forms**: Cat5, Cat5e, Cat6.
- **Fiber Optic**: Pulses of light, used in places with electromagnetic interference.

#### Hubs and Switches
- **Hub**: Physical layer device allowing connections from many computers.
- **Switch**: Data-link layer device, eliminates collision domains.

#### Routers
- Connects different networks (LAN, WAN).
- **Function**: Forward data between networks, operates at the Network Layer.
- **BGP**: Border Gateway Protocol, lets routers learn optimal paths for traffic.

### Name Resolution
- **DNS**: Domain Name System, resolves domain names to IP addresses.
- **MAC Address**: 48-bit binary numbers.
- **IP Address**: Addresses used in DNS can change frequently.

## Intermediate Topics

### OSI Model
| Layer       | Protocol Data Unit (PDU) | Function                                           |
|-------------|--------------------------|----------------------------------------------------|
| 7. Application | High-level APIs            | Resource sharing, remote file access                |
| 6. Presentation| Data                     | Translation between networking service and application|
| 5. Session    |                        | Managing communication sessions                     |
| 4. Transport  | Segment (TCP)/Datagram (UDP) | Reliable transmission, segmentation, acknowledgement |
| 3. Network    | Packet                   | Structuring and managing a multi-node network       |
| 2. Data Link  | Frame                    | Reliable transmission between two nodes             |
| 1. Physical   | Bit                      | Transmission of raw bit streams                     |

### IP Addresses
- **IPv4**: 32-bit addresses.
- **IPv6**: 128-bit addresses, uses hexadecimal notation.

### Subnetting
- **Subnet Mask**: Defines the network and host portions of an IP address.
- **CIDR**: Classless Inter-Domain Routing, provides flexible addressing.

### The Transport Layer
- **TCP**: Transmission Control Protocol, reliable transmission.
- **UDP**: User Datagram Protocol, connectionless and faster but less reliable.

### Routing
- **Routing Table**: Used by routers to determine the next hop for packet forwarding.
- **Interior Gateway Protocols**: RIP, EIGRP.
- **Exterior Gateway Protocols**: BGP.

### Firewalls
- **Function**: Block traffic that meets certain criteria.
- **Implementation**: Can operate at various network layers, often integrated with routers.

## Advanced Topics

### Advanced DNS Concepts
- **Resource Record Types**: A, AAAA, CNAME, MX, SRV, TXT, NS, SOA.
- **Name Resolution Process**: Steps for converting domain names to IP addresses.

### TCP Details
- **TCP Segment Structure**: Header, data section, and control flags.
- **Three-Way Handshake**: SYN, SYN-ACK, ACK.

### Advanced Routing Concepts
- **Mesh Network**: Ensures multiple paths for packet delivery.
- **Non-Routable Address Space**: IP ranges reserved for internal use (RFC 1918).

### Network Address Translation (NAT)
- **Purpose**: Allows internal devices to communicate with external networks.
- **Types**: Static, dynamic, PAT (Port Address Translation).

### IPv6 Addressing and Subnetting
- **Structure**: 128-bit addresses, divided into network and host portions.
- **IPv6 Header**: Contains fields like version, traffic class, flow label, and hop limit.

### Network Troubleshooting Tools
- **ICMP**: Used for error reporting and diagnostics (e.g., ping).
- **Traceroute**: Discovers the path between two nodes.
- **Netcat**: Tests port connectivity.

### Cloud Computing
- **Services**: IaaS, PaaS, SaaS.
- **Cloud Types**: Public, private, hybrid.
- **Virtualization**: Use of hypervisors to manage virtual machines.

### Firewalls and Security
- **Types**: Network-based, host-based.
- **Functions**: Blocking unauthorized access, logging, and auditing traffic.

