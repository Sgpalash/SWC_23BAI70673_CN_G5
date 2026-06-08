# Introduction to Computer Networks

## What is a Computer Network?

A Computer Network is a collection of interconnected devices that communicate and share resources such as data, files, printers, and internet connections.

### Advantages of Networking
- Resource Sharing
- Fast Communication
- Data Sharing
- Centralized Management
- Internet Access

---

# Networking Devices

## 1. Router

A Router connects different networks and forwards data packets between them.

### Functions
- Connects LAN to the Internet
- Finds the best path for data transmission
- Uses IP Addresses to route packets

### Example
Home Wi-Fi routers connect your devices to the Internet.

---

## 2. Switch

A Switch connects devices within the same network.

### Functions
- Transfers data between devices
- Uses MAC Addresses
- Reduces network traffic

### Example
Computers connected in a laboratory through a switch.

---

# Data Units in Networking

## 1. Segment

- Data unit at the Transport Layer.
- Created by TCP before transmission.

### Example
A large file is divided into smaller segments.

---

## 2. Packet

- Data unit at the Network Layer.
- Contains source and destination IP addresses.

### Example
Routers forward packets through the Internet.

---

# Addressing

## 1. IP Address

An IP Address uniquely identifies a device on a network.

### Example
- IPv4: 192.168.1.1
- IPv6: 2001:db8::1

### Types
- Public IP
- Private IP

---

## 2. MAC Address

A MAC Address is a unique hardware address assigned to a network interface card (NIC).

### Example
00:1A:2B:3C:4D:5E

### Characteristics
- Permanent address
- Used within local networks

---

# Flow of Data on Google/Internet

When a user enters www.google.com in a browser:

1. Browser sends a DNS request.
2. DNS converts the domain name into an IP address.
3. Data is divided into segments and packets.
4. Packets travel through switches and routers.
5. Google server receives the request.
6. Server processes the request.
7. Response packets are sent back.
8. Browser displays the webpage.

### Flow Diagram

User Device
→ Switch
→ Router
→ ISP
→ Internet
→ Google Server
→ Internet
→ ISP
→ Router
→ Switch
→ User Device

---

# OSI Model

OSI (Open Systems Interconnection) Model consists of 7 layers.

| Layer Number | Layer Name |
|-------------|-----------|
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

---

## Layer 7: Application Layer

### Functions
- Provides network services to users
- Supports applications like browsers and email

### Examples
- HTTP
- FTP
- DNS

---

## Layer 6: Presentation Layer

### Functions
- Data Translation
- Encryption
- Compression

### Example
Converting data formats between systems.

---

## Layer 5: Session Layer

### Functions
- Establishes sessions
- Maintains sessions
- Terminates sessions

### Example
Video conferencing sessions.

---

## Layer 4: Transport Layer

### Functions
- Reliable data transfer
- Error checking
- Flow control

### Protocols
- TCP
- UDP

---

## Layer 3: Network Layer

### Functions
- Logical Addressing
- Routing

### Device
- Router

### Protocol
- IP

---

## Layer 2: Data Link Layer

### Functions
- MAC Addressing
- Error Detection

### Device
- Switch

---

## Layer 1: Physical Layer

### Functions
- Transmission of bits
- Electrical and mechanical specifications

### Examples
- Cables
- Connectors
- Wireless Signals

---

# Cryptography Basics

## 1. Symmetric Key Cryptography

Uses the same key for encryption and decryption.

### Advantages
- Fast
- Efficient

### Disadvantages
- Key distribution is difficult

### Example
AES (Advanced Encryption Standard)

---

## 2. Asymmetric Key Cryptography

Uses two keys:
- Public Key
- Private Key

### Advantages
- More secure key exchange

### Disadvantages
- Slower than symmetric encryption

### Examples
- RSA
- ECC

---

# Networking Protocols and Concepts

## 1. MAC (Media Access Control)

### Purpose
- Identifies devices in a local network
- Uses MAC Addresses

### Example
Switches use MAC addresses for forwarding frames.

---

## 2. TCP (Transmission Control Protocol)

### Features
- Connection-oriented
- Reliable
- Error checking
- Ordered delivery

### Uses
- Web browsing
- Email
- File transfer

---

## 3. UDP (User Datagram Protocol)

### Features
- Connectionless
- Faster
- No guarantee of delivery

### Uses
- Video Streaming
- Online Gaming
- VoIP

---

## 4. DNS (Domain Name System)

### Purpose
Converts domain names into IP addresses.

### Example
www.google.com → 142.250.xxx.xxx

---

## 5. FTP (File Transfer Protocol)

### Purpose
Transfers files between client and server.

### Features
- Upload files
- Download files

---

## 6. HTTP (HyperText Transfer Protocol)

### Purpose
Transfers web pages over the Internet.

### Characteristics
- Stateless protocol
- Used for websites

---

## 7. TLS (Transport Layer Security)

### Purpose
Provides encryption and security for data transmission.

### Features
- Authentication
- Encryption
- Data Integrity

---

## 8. HTTPS (HyperText Transfer Protocol Secure)

### Purpose
Secure version of HTTP.

### Features
- Uses TLS encryption
- Protects user data
- Secure web communication

### Example
https://www.google.com

---

# Remote Access and Connectivity Tools

## 1. PuTTY

### Definition
PuTTY is a free terminal emulator used for remote access.

### Features
- SSH support
- Telnet support
- Serial communication

### Uses
- Remote server management

---

## 2. SSH (Secure Shell)

### Definition
A secure protocol for remote login and command execution.

### Features
- Encryption
- Authentication
- Secure communication

### Default Port
22

### Example
Remote administration of Linux servers.

---

## 3. TELNET

### Definition
A protocol for remote login over a network.

### Features
- Text-based communication
- No encryption

### Default Port
23

### Disadvantages
- Insecure because data is transmitted in plain text

### Modern Alternative
SSH

---

# Conclusion

Computer Networks enable communication between devices and provide access to shared resources and the Internet. Understanding networking devices, addressing, protocols, OSI layers, cryptography, and remote access tools forms the foundation of modern networking.
