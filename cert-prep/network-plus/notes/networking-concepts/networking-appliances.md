# Networking Appliances

Networking appliances are dedicated devices designed to perform specific network functions such as routing, switching, filtering, monitoring, or securing traffic.

They are optimized for reliability, performance, and security within a network environment.

---

## 1. Router

A router connects different networks together and forwards traffic between them.

- Operates at **Layer 3 (Network layer)** of the OSI model
- Uses IP addresses to determine the best path for data
- Commonly connects internal networks to the internet
- Can perform NAT (Network Address Translation)

Example: Home internet router connecting LAN to ISP.

---

## 2. Switch

A switch connects devices within the same local network (LAN).

- Operates at **Layer 2 (Data Link layer)**
- Uses MAC addresses to forward traffic
- Reduces network collisions
- Supports VLAN segmentation

Example: Office switch connecting computers and printers.

---

## 3. Firewall

A firewall filters network traffic based on security rules.

- Can operate at Layer 3 and above
- Blocks or allows traffic based on IP, port, protocol
- Can be stateful (tracks active connections)

Purpose: Protect internal network from unauthorized access.

---

## 4. IDS / IPS

### IDS (Intrusion Detection System)
- Monitors traffic
- Detects suspicious activity
- Sends alerts

### IPS (Intrusion Prevention System)
- Detects and actively blocks malicious traffic

These help protect networks from attacks.

---

## 5. Load Balancer

Distributes incoming traffic across multiple servers.

- Prevents overload on a single server
- Improves performance and availability
- Common in web applications and cloud environments

---

## 6. Proxy Server

Acts as an intermediary between clients and external servers.

- Can filter content
- Improves security
- May cache content to improve performance

---

## 7. Wireless Access Point (WAP)

Provides wireless connectivity to a wired network.

- Extends network access via Wi-Fi
- Often connected to a switch

---

## 8. VPN Concentrator

Manages multiple VPN connections.

- Allows secure remote access
- Encrypts traffic between remote users and the network

---

# Key Concept

Networking appliances control how traffic flows, is filtered, secured, and monitored.

In troubleshooting, always ask:
- Where is the traffic flowing?
- Which appliance handles that traffic?
- Could that device be blocking or misrouting it?
