# Networking Functions

Networking functions describe what a network is responsible for doing in order to allow devices to communicate reliably and securely.

---

## 1. Device Identification (Addressing)

Every device on a network must have a unique identifier.

- **MAC Address** → Physical address (Layer 2)
- **IP Address** → Logical address (Layer 3)

Without addressing, devices would not know where to send data.

---

## 2. Encapsulation

Encapsulation is the process of wrapping data with protocol information as it moves down the OSI model layers.

Example:
Application Data → TCP Segment → IP Packet → Ethernet Frame

Each layer adds its own header information.

Purpose:
- Identifies source and destination
- Tracks sessions
- Ensures proper delivery

---

## 3. Segmentation and Reassembly

Large pieces of data are broken into smaller segments for transmission.

- TCP divides data into segments
- Receiver reassembles segments in the correct order

This improves reliability and efficiency.

---

## 4. Routing and Switching

### Switching (Layer 2)
- Moves data within the same local network (LAN)
- Uses MAC addresses

### Routing (Layer 3)
- Moves data between different networks
- Uses IP addresses

Routers determine the best path for data to reach its destination.

---

## 5. Name Resolution

Humans use names.
Computers use IP addresses.

**DNS (Domain Name System)** translates domain names into IP addresses.

Example:
google.com → 142.250.x.x

---

## 6. DHCP (Dynamic Host Configuration Protocol)

Automatically assigns:
- IP address
- Subnet mask
- Default gateway
- DNS server

Prevents manual configuration errors.

---

## 7. Network Security

Networks must protect data and control access.

Common functions:
- Firewalls (traffic filtering)
- Access Control Lists (ACLs)
- VPNs (encrypted tunnels)
- Authentication systems

---

## 8. Monitoring and Management

Networks must be observed and maintained.

Examples:
- SNMP (Simple Network Management Protocol)
- Logging and alerting
- Configuration backups

Monitoring tools detect failures, performance issues, and security threats.

---

## 9. Fault Tolerance and Redundancy

Networks are designed to avoid single points of failure.

Examples:
- Redundant links
- Failover routers
- Load balancing

Goal: Maintain uptime and availability.

---

## Summary

Networking functions allow devices to:

- Identify each other
- Send and receive data
- Resolve names
- Route traffic correctly
- Maintain security
- Monitor health
- Recover from failures

A network is not just cables and devices — it is a system that manages communication from end to end.
