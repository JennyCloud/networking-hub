# Networking Functions

Networking exists to move data from one device to another reliably, efficiently, and securely.  

---

## 1. Encapsulation

Encapsulation is the process of wrapping data with protocol information as it moves down the OSI layers.

Example flow:
Application Data  
→ TCP/UDP Header added (Layer 4)  
→ IP Header added (Layer 3)  
→ Ethernet Header added (Layer 2)

Each layer adds its own header.  
At the destination, the process is reversed (decapsulation).

Why it matters:
Encapsulation allows different layers to perform specialized tasks while working together.

---

## 2. Addressing

Networks need addressing so devices know where to send data.

Types of addresses:

- MAC Address (Layer 2) → Physical hardware address
- IP Address (Layer 3) → Logical network address
- Port Number (Layer 4) → Identifies specific application/service

Without addressing, data would have no destination.

---

## 3. Routing and Forwarding

Routing determines the best path for data to travel between networks.

Routers:
- Examine the destination IP address
- Check their routing table
- Forward the packet to the next hop

Forwarding is the actual movement of the packet based on routing decisions.

---

## 4. Fragmentation

If a packet is too large for the network medium (MTU limit), it may be broken into smaller pieces.

MTU (Maximum Transmission Unit):
- Ethernet default MTU is 1500 bytes

Fragments are reassembled at the destination.

---

## 5. Error Detection

Networks must detect corruption during transmission.

Layer 2 uses:
- Frame Check Sequence (FCS)

Layer 4 (TCP) uses:
- Checksums
- Acknowledgments (ACKs)

TCP can retransmit lost or damaged data.
UDP does not guarantee delivery.

---

## 6. Flow Control

Flow control prevents a fast sender from overwhelming a slow receiver.

TCP uses:
- Window size
- Acknowledgments

This ensures stable communication.

---

## 7. Time To Live (TTL)

TTL is a field inside the IP header.

Purpose:
To prevent packets from traveling endlessly in routing loops.

How it works:
- Each router that forwards a packet reduces the TTL value by 1.
- When TTL reaches 0, the packet is dropped.
- The router sends back an ICMP "Time Exceeded" message.

Example:
If a packet starts with TTL = 64,
and passes through 5 routers,
TTL becomes 59.

If a routing loop exists,
TTL will eventually hit 0,
and the packet will be discarded.

Why TTL matters:
- Prevents infinite network loops
- Helps tools like `tracert` / `traceroute` work

Traceroute works by sending packets with increasing TTL values to discover each hop along the path.

---

## 8. Name Resolution

Humans use domain names.
Networks use IP addresses.

DNS (Domain Name System):
- Translates domain names to IP addresses

Example:
google.com → 142.250.x.x

---

## 9. Network Address Translation (NAT)

NAT allows private IP addresses to access the internet using a public IP address.

Common in home routers and firewalls.

Purpose:
- Conserves public IP addresses
- Adds a layer of basic security

---

# Summary

Core Networking Functions:

- Encapsulation
- Addressing
- Routing
- Fragmentation
- Error Detection
- Flow Control
- TTL loop prevention
- Name Resolution
- NAT

Networking is rule-based data movement.
Packets follow logic, not intention.
When something breaks, there is always a reason.
