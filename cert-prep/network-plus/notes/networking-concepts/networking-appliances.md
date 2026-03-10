# Networking Appliances

Networking appliances are physical or virtual devices that control, manage, secure, or optimize network traffic.

## 1. Router

A router connects different networks together and directs traffic between them.

**Main Function:**
- Operates at **Layer 3 (Network Layer)**
- Uses IP addresses to determine the best path for data

**What it does:**
- Connects LAN to WAN (e.g., home network to the Internet)
- Maintains routing tables
- Performs NAT (Network Address Translation)

**Key Idea:**
Routers move packets between networks.

---

## 2. Switch

A switch connects devices within the same network.

**Main Function:**
- Operates at **Layer 2 (Data Link Layer)**
- Uses MAC addresses to forward frames

**What it does:**
- Connects PCs, printers, servers in a LAN
- Maintains MAC address table
- Supports VLANs (Virtual LANs)

**Key Idea:**
Switches move frames within a network.

---

## 3. Firewall

A firewall filters traffic based on security rules.

**Main Function:**
- Can operate at Layer 3 and above
- Inspects traffic and allows or blocks it

**Types:**
- Packet-filtering firewall
- Stateful firewall
- Next-Generation Firewall (NGFW)

**What it does:**
- Blocks unauthorized access
- Controls inbound and outbound traffic

**Key Idea:**
Firewalls enforce security policies.

---

## 4. IDS / IPS

### IDS (Intrusion Detection System)

- Monitors network traffic
- Detects suspicious activity
- Sends alerts
- Does NOT block traffic

### IPS (Intrusion Prevention System)

- Monitors traffic
- Detects threats
- Automatically blocks malicious traffic

**Key Difference:**
IDS = Detect and alert  
IPS = Detect and stop  

---

## 5. Load Balancer

A load balancer distributes traffic across multiple servers.

**Main Function:**
- Improves performance
- Prevents server overload
- Increases availability

**Example:**
If one web server fails, traffic is redirected to another.

**Key Idea:**
Prevents single points of failure.

---

## 6. Proxy Server

A proxy acts as an intermediary between clients and servers.

**Types:**
- Forward proxy (client-side)
- Reverse proxy (server-side)

**What it does:**
- Filters requests
- Hides internal IP addresses
- Caches content
- Improves security

**Key Idea:**
Proxy = middleman for traffic.

---

## 7. NAS (Network Attached Storage)

NAS provides file storage over a network.

**Characteristics:**
- Connected via Ethernet
- Used for file sharing
- Often uses SMB or NFS protocols

**Key Idea:**
NAS = file-level storage over network.

---

## 8. SAN (Storage Area Network)

SAN provides high-speed storage access to servers.

**Characteristics:**
- Block-level storage
- Uses Fibre Channel or iSCSI
- Used in data centers

**Key Idea:**
SAN = high-performance storage network.

---

## 9. Wireless Devices

Wireless devices enable communication without physical cables.

### Access Point (AP)
- Connects wireless devices to wired network

### Wireless Router
- Combines router + switch + access point

### Wireless Controller
- Manages multiple access points centrally

**Key Idea:**
Wireless devices extend networks without cables.

---

# Summary

- Router → connects networks
- Switch → connects devices within a network
- Firewall → filters traffic
- IDS/IPS → detects/prevents attacks
- Load balancer → distributes traffic
- Proxy → traffic intermediary
- NAS → file storage
- SAN → high-speed storage network
- Wireless devices → enable Wi-Fi connectivity
