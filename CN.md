Here’s a **Last Minute Revision** in the same format for **Computer Networks** as a README file:

---

# Computer Networks - Last Minute Revision

## Table of Contents

1. [OSI and TCP/IP Models](#1-osi-and-tcpip-models)
2. [Transmission Media](#2-transmission-media)
3. [IP Addressing](#3-ip-addressing)
4. [Subnetting](#4-subnetting)
5. [Routing Protocols](#5-routing-protocols)
6. [DNS (Domain Name System)](#6-dns-domain-name-system)
7. [HTTP, HTTPS, and FTP](#7-http-https-and-ftp)
8. [Firewalls and NAT](#8-firewalls-and-nat)
9. [TCP vs UDP](#9-tcp-vs-udp)
10. [Network Devices](#10-network-devices)
11. [Network Topologies](#11-network-topologies)
12. [Error Detection & Correction](#12-error-detection-correction)

---

## 1. OSI and TCP/IP Models

### OSI Model:
1. **Layer 1: Physical Layer** – Deals with hardware transmission (cables, switches, etc.)
2. **Layer 2: Data Link Layer** – Manages data transfer between devices on the same network (e.g., MAC addresses).
3. **Layer 3: Network Layer** – Handles logical addressing and routing (e.g., IP addresses).
4. **Layer 4: Transport Layer** – Manages end-to-end communication (TCP/UDP protocols).
5. **Layer 5: Session Layer** – Controls dialogues and sessions between computers.
6. **Layer 6: Presentation Layer** – Translates data formats, encryption, compression.
7. **Layer 7: Application Layer** – Interfaces for network services (e.g., HTTP, FTP, SMTP).

### TCP/IP Model:
1. **Network Interface Layer** – Corresponds to Physical and Data Link layers.
2. **Internet Layer** – Corresponds to Network layer (IP addressing, routing).
3. **Transport Layer** – Corresponds to Transport layer (TCP/UDP).
4. **Application Layer** – Corresponds to Session, Presentation, and Application layers (HTTP, FTP, etc.).

---

## 2. Transmission Media

1. **Wired Media**:
   - **Twisted Pair Cable**: Used for telephones, Ethernet (e.g., Cat5, Cat6).
   - **Coaxial Cable**: Used for cable TV.
   - **Fiber Optic Cable**: High-speed, long-distance transmission using light.

2. **Wireless Media**:
   - **Radio Waves**: Used in WiFi, AM/FM.
   - **Microwaves**: Used in satellite communication.
   - **Infrared**: Short-distance communication (e.g., TV remotes).

---

## 3. IP Addressing

### IPv4:
- **Format**: 32-bit address, divided into 4 octets (e.g., 192.168.0.1).
- **Classes**:
  - **Class A**: 0.0.0.0 to 127.255.255.255 (for large networks).
  - **Class B**: 128.0.0.0 to 191.255.255.255 (for medium-sized networks).
  - **Class C**: 192.0.0.0 to 223.255.255.255 (for small networks).

### IPv6:
- **Format**: 128-bit address, written in hexadecimal (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
- Allows a vastly larger number of unique addresses compared to IPv4.

---

## 4. Subnetting

### Purpose:
- **Subnetting** divides a larger network into smaller, more manageable sub-networks (subnets), improving performance and security.

### Subnet Mask:
- Helps determine the network and host portions of an IP address (e.g., 255.255.255.0).

### Example:
- **Network Address**: 192.168.1.0
- **Subnet Mask**: 255.255.255.0
  - Network: First 3 octets (192.168.1), Host: Last octet (.0 to .255).

---

## 5. Routing Protocols

1. **Static Routing**: Manually configured routes, suitable for small networks.
2. **Dynamic Routing**: Uses algorithms to find the best route automatically.
   - **RIP (Routing Information Protocol)**: Distance vector protocol, limited by hop count (max 15 hops).
   - **OSPF (Open Shortest Path First)**: Link-state protocol, uses the shortest path first algorithm.
   - **BGP (Border Gateway Protocol)**: Used for routing between ISPs, the protocol of the internet.

---

## 6. DNS (Domain Name System)

### Function:
- Translates human-readable domain names (e.g., `www.example.com`) into IP addresses (e.g., `93.184.216.34`).

### Components:
1. **DNS Server**: Resolves domain names to IP addresses.
2. **Resolver**: Client-side function that requests DNS resolution.

---

## 7. HTTP, HTTPS, and FTP

1. **HTTP (HyperText Transfer Protocol)**:
   - Protocol for transmitting web pages.
   - Uses port 80.
   
2. **HTTPS (HTTP Secure)**:
   - Encrypted version of HTTP, using SSL/TLS.
   - Uses port 443.

3. **FTP (File Transfer Protocol)**:
   - Used for transferring files between computers.
   - Uses ports 20 (data) and 21 (control).

---

## 8. Firewalls and NAT

1. **Firewall**: 
   - A network security device that monitors and filters incoming and outgoing traffic based on predetermined security rules.
   
2. **NAT (Network Address Translation)**:
   - Translates private IP addresses into a public IP address for accessing the internet.
   - Helps conserve public IP addresses and provides security by masking internal IP addresses.

---

## 9. TCP vs UDP

1. **TCP (Transmission Control Protocol)**:
   - Connection-oriented protocol.
   - Provides reliability with error-checking and guarantees data delivery.
   - Slower but ensures data integrity.
   - Use cases: Web browsing (HTTP), file transfer (FTP).

2. **UDP (User Datagram Protocol)**:
   - Connectionless protocol.
   - No error-checking or guaranteed delivery.
   - Faster but less reliable.
   - Use cases: Video streaming, VoIP, DNS queries.

---

## 10. Network Devices

1. **Hub**: Broadcasts data to all devices in a network.
2. **Switch**: Forwards data to specific devices based on MAC addresses.
3. **Router**: Routes data between different networks based on IP addresses.
4. **Modem**: Converts digital data to analog signals (and vice versa) for transmission over telephone lines.
5. **Access Point**: Provides wireless connectivity for devices in a network.

---

## 11. Network Topologies

1. **Star Topology**: All devices connected to a central switch/hub. Failure of the hub disrupts the network.
2. **Bus Topology**: All devices share a single communication line. Failure of the backbone line affects the entire network.
3. **Ring Topology**: Devices are connected in a circular loop. Data travels in one direction (or both directions in a dual ring).
4. **Mesh Topology**: Every device is connected to every other device. Provides redundancy and fault tolerance.
5. **Hybrid Topology**: A combination of two or more topologies (e.g., Star-Bus).

---

## 12. Error Detection & Correction

### Error Detection Techniques:
1. **Parity Bit**: Adds a bit to ensure the number of 1s is even or odd.
2. **Checksum**: Sums up the data segments to detect errors.
3. **CRC (Cyclic Redundancy Check)**: A polynomial division-based method for error detection.

### Error Correction Techniques:
1. **Hamming Code**: Adds redundancy bits to enable both error detection and correction.
2. **Forward Error Correction (FEC)**: Transmits additional data to allow the receiver to detect and correct errors without needing retransmission.

---

This file summarizes the key concepts in **Computer Networks** for quick last-minute revisions, particularly for interviews. Make sure to understand the practical examples and the importance of each topic, as they are often asked in both theoretical and practical interview rounds.
