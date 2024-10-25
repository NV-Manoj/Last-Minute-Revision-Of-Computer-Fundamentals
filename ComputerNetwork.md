Here's an updated and refined last-minute revision guide for Computer Networks, optimized for interview preparation:

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
12. [Error Detection & Correction](#12-error-detection-and-correction)

---

## 1. OSI and TCP/IP Models

### OSI Model:
- **Physical Layer (1)**: Transmits raw bitstream over physical hardware.
- **Data Link Layer (2)**: Handles MAC addresses, framing, and error detection.
- **Network Layer (3)**: Manages IP addressing and routing between devices.
- **Transport Layer (4)**: Controls end-to-end data delivery (TCP/UDP).
- **Session Layer (5)**: Manages sessions and connection control.
- **Presentation Layer (6)**: Translates data formats and handles encryption.
- **Application Layer (7)**: Provides network services (e.g., HTTP, SMTP).

### TCP/IP Model:
- **Network Interface**: Physical and Data Link layers.
- **Internet**: IP addressing and routing (Network layer).
- **Transport**: End-to-end communication (TCP/UDP).
- **Application**: Includes Session, Presentation, Application layers.

---

## 2. Transmission Media

1. **Wired Media**:
   - **Twisted Pair**: Common for Ethernet networks.
   - **Coaxial Cable**: Used in cable TV, supports higher bandwidth.
   - **Fiber Optic**: Transmits data using light, high speed, and secure.

2. **Wireless Media**:
   - **Radio Waves**: Used for WiFi, broad coverage.
   - **Microwaves**: Satellite and long-distance communication.
   - **Infrared**: Short range, used in remotes.

---

## 3. IP Addressing

### IPv4:
- **32-bit Address**: Four octets (e.g., 192.168.1.1).
- **Classes**:
  - **A**: Large networks, 0.0.0.0 - 127.255.255.255.
  - **B**: Medium networks, 128.0.0.0 - 191.255.255.255.
  - **C**: Small networks, 192.0.0.0 - 223.255.255.255.

### IPv6:
- **128-bit Address**: Hexadecimal notation, e.g., 2001:0db8::1.
- Vast address space, includes features for auto-configuration and security.

---

## 4. Subnetting

- **Purpose**: Divides networks to manage traffic and enhance security.
- **Subnet Mask**: Defines network and host parts of an IP (e.g., 255.255.255.0).
- **Example**:
  - **Network Address**: 192.168.1.0/24.
  - Hosts: 192.168.1.1 - 192.168.1.254.

---

## 5. Routing Protocols

1. **Static Routing**: Manually configured, good for small networks.
2. **Dynamic Routing**:
   - **RIP**: Simple, max 15 hops.
   - **OSPF**: Link-state, faster convergence, suitable for large networks.
   - **BGP**: Path-vector, backbone of the internet, connects ISPs.

---

## 6. DNS (Domain Name System)

- **Function**: Converts domain names to IP addresses.
- **Records**:
  - **A**: IPv4 address.
  - **AAAA**: IPv6 address.
  - **CNAME**: Alias for a domain.
  - **MX**: Mail server.

---

## 7. HTTP, HTTPS, and FTP

1. **HTTP**: Used for web browsing (port 80), not secure.
2. **HTTPS**: Encrypted HTTP using SSL/TLS (port 443).
3. **FTP**: Transfers files over a network (ports 20 and 21).

---

## 8. Firewalls and NAT

1. **Firewalls**: Control incoming/outgoing traffic based on security rules (packet filtering, stateful inspection).
2. **NAT**: Translates private IPs to a public IP, masks internal addresses from external networks.

---

## 9. TCP vs UDP

1. **TCP**:
   - Reliable, connection-oriented.
   - Uses handshaking (SYN-ACK).
   - Ideal for HTTP, FTP.

2. **UDP**:
   - Connectionless, faster.
   - No reliability (packet loss possible).
   - Used for DNS, video streaming.

---

## 10. Network Devices

- **Hub**: Broadcasts data to all devices.
- **Switch**: Connects devices and forwards based on MAC.
- **Router**: Routes data between different networks.
- **Modem**: Converts signals for transmission over phone lines.
- **Access Point**: Allows wireless connections to a network.

---

## 11. Network Topologies

1. **Star**: Centralized, failure at hub affects network.
2. **Bus**: Shared backbone, prone to congestion.
3. **Ring**: Circular, data travels in one direction.
4. **Mesh**: High redundancy, resilient.
5. **Hybrid**: Mix of multiple topologies.

---

## 12. Error Detection and Correction

1. **Detection**:
   - **Parity Check**: Adds a parity bit for error detection.
   - **Checksum**: Sum of data for integrity.
   - **CRC**: Polynomial-based error detection.

2. **Correction**:
   - **Hamming Code**: Adds redundancy for single-bit correction.
   - **FEC**: Adds extra data to correct errors on the receiver's end.

---

This summary should help you with a quick review of **Computer Networks** concepts for interviews. Make sure you grasp the practical applications and use cases for each concept as they’re commonly asked in interviews.
