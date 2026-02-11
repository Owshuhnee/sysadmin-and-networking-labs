# NetAcad Networking Basics - Terms by Module

This document contains brief definitions of key terms from the
**Cisco Networking Academy – Networking Basics** course.

---

## Module 1 — Communication in a Connected World
- **Network** – Devices connected to share data  
- **Protocol** – Rules that define how devices communicate  
- **Bandwidth** – Maximum data capacity of a network connection  
- **Latency** – Delay before data begins to transfer  
- **Throughput** – Actual amount of data successfully transferred  
- **Packet** – Small unit of data sent across a network  

---

## Module 2 — Network Components, Types, and Connections
- **ISP (Internet Service Provider)** – Company that provides internet access  
- **Client** – Device that requests services or data from another device  
- **Server** – Device that provides services or data to clients  
- **P2P (Peer-to-Peer) Network** – Network where devices share resources directly  
- **Network Infrastructure** – Components that support network communication  
  - End devices  
  - Intermediate devices  
  - Network media  
- **Cable** – Physical medium used to transmit data  
- **DSL (Digital Subscriber Line)** – Internet connection using telephone lines  
- **Satellite Connection** – Internet access delivered via satellite links  

---

## Module 3 — Wireless and Mobile Networks
- **Wireless Networks** – Networks that transmit data without cables  
- **Wi-Fi** – Wireless LAN technology based on IEEE 802.11 standards  
- **GPS (Global Positioning System)** – Satellite system used for location tracking  
- **Cellular Data** – Mobile network data provided by cellular carriers  
- **Bluetooth** – Short-range wireless communication technology  
- **NFC (Near Field Communication)** – Very short-range wireless communication  

---

## Module 4 — Build a Home Network
- **WLAN (Wireless Local Area Network)** – Local network using wireless connections  
- **Network Router** – Device that forwards data between different networks  
- **SSID (Service Set Identifier)** – Name of a wireless network  
- **IEEE** – Organization that defines networking standards  

---

## Module 5 — Communication Principles
- **Protocols** – Defined rules for data format, transmission, and delivery  
- **Network Standards Organizations** – Groups that create networking standards  
- **IANA (Internet Assigned Numbers Authority)** – Manages IP addresses and ports  
- **IETF (Internet Engineering Task Force)** – Develops internet standards  
- **TCP/IP Model** – Four-layer model used for internet communication  
- **OSI Model** – Seven-layer model used to understand networking concepts  

---

## Module 6 — Network Media
- **Data** – Information transmitted across a network  
- **Twisted-Pair Cable** – Common copper cabling used in Ethernet networks  
- **Coaxial Cable** – Shielded cable used for broadband and legacy networks  
- **Fiber-Optic Cable** – Cable that transmits data using light  
- **Network Media Types** – Physical or wireless methods used to carry data  

---

## Module 7 — The Access Layer
- **NIC (Network Interface Card)** – Hardware that connects a device to a network  
- **MAC (Media Access Control)** – Physical Layer 2 address used on a local network  
- **Encapsulation** – Wrapping data with headers as it moves down the network stack  
- **Internet Protocol (IP)** – Logical Layer 3 address used to route data  
- **Preamble** – Bits sent before a frame to synchronize sender and receiver  
- **Start Frame Delimiter (SFD)** – Marks the exact start of an Ethernet frame  
- **Ethernet Frame** – Layer 2 data unit used to transmit data on a LAN  
- **Access Layer** – Network layer where end devices connect to switches  
- **Frame Check Sequence (FCS)** – Error-checking field used to detect corrupted frames  

---

## Module 8 — The Internet Protocol
- **IPv4** – Logical network address that identifies a host; 32-bit (4 octets)  
- **Subnet Mask** – Determines which part of an IP address is network vs host 


---
## Module 9 - IPV4 and Network Segmentation
- **Unicast Transmission** -  Refers to one device sending a message to one other device in one-to-one communications.

- **Broadcast Transmission** - Refers to a device sending a message to all the devices on a network in one-to-all communications.

- **Multicast Transmission** - 
- **Private IPv4 addresses** - 
- **Loopback addresses** -
- **Link-Local addresses** -
- **Automatic Private IP Addressing (APIPA)** -
- **Regional Internet Registries** -


## Miscellaneous
### OSI Model (7 Layers)
1. **Application** – User-facing network services (HTTP, FTP, SMTP)
2. **Presentation** – Formatting, encryption, and compression
3. **Session** – Session setup, management, and termination
4. **Transport** – End-to-end communication and reliability (TCP/UDP)
5. **Network** – Logical addressing and routing (IP)
6. **Data Link** – Framing, MAC addressing, and error detection
7. **Physical** – Transmission of raw bits over media

---

### TCP/IP Model (4 Layers)
1. **Application** – Network services and applications
2. **Transport** – Host-to-host communication (TCP/UDP)
3. **Internet** – Logical addressing and routing (IP)
4. **Network Access** – Physical transmission and local delivery

---

### OSI vs TCP/IP Layer Mapping
- **OSI Layers 7–5** → TCP/IP **Application**
- **OSI Layer 4** → TCP/IP **Transport**
- **OSI Layer 3** → TCP/IP **Internet**
- **OSI Layers 2–1** → TCP/IP **Network Access**

---

![RFC 1918](./screenshots/RFC%201918%20Private%20address%20Range.png)

## Resources
- [Network Access Layer: Introduction — Rick Graziani](https://www.youtube.com/watch?v=k1AC96Ppuzc&list=PLMLm7-g0V0ke_dSguEQfz-ZSHrSUikTJ7)
