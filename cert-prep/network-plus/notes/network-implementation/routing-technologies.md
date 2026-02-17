# Routing Technologies

## 1. Static vs Dynamic Routing

### Static Routing
A **static route** is manually configured by a network administrator.

- Admin defines the destination network and next-hop IP.
- Does NOT change automatically if the network changes.
- Simple, predictable, low overhead.
- Good for small or stable networks.

Example:
If Router A needs to reach 10.0.2.0/24, you manually tell it:
"Send traffic to 192.168.1.1"

Pros:
- Simple
- Secure (no route advertisements)
- No CPU overhead from routing protocols

Cons:
- Not scalable
- Must manually update if topology changes

---

### Dynamic Routing
Dynamic routing uses routing protocols to automatically exchange route information between routers.

Routers learn:
- What networks exist
- Best path to reach them
- When paths go down

Scales well for large networks.

---

## 2. Common Dynamic Routing Protocols

### OSPF (Open Shortest Path First)
- Open standard (vendor-neutral)
- Link-state protocol
- Uses cost metric (based on bandwidth)
- Fast convergence
- Common in enterprise networks

OSPF builds a map of the network and calculates shortest paths.

---

### EIGRP (Enhanced Interior Gateway Routing Protocol)
- Developed by Cisco
- Hybrid protocol (distance vector + link-state behavior)
- Fast convergence
- Uses composite metric (bandwidth + delay)

Primarily seen in Cisco environments.

---

### BGP (Border Gateway Protocol)
- Exterior Gateway Protocol (used between organizations)
- Used on the Internet
- Path-vector protocol
- Selects routes based on policies and path attributes

BGP is how the Internet decides where traffic goes between ISPs.

Key idea:
OSPF/EIGRP = inside a company  
BGP = between companies / Internet

---

## 3. Route Selection (How Routers Choose a Path)

When multiple routes exist, routers choose based on:

1. Administrative Distance (AD)
   - Trust level of route source
   - Lower AD = more preferred
   - Static route usually preferred over dynamic

2. Metric
   - Cost value assigned by routing protocol
   - Lower metric = better path

3. Longest Prefix Match
   - More specific route wins
   - Example:
     10.0.0.0/8
     10.0.1.0/24  ← more specific, preferred

Routers always choose the most specific valid route.

---

## 4. NAT and PAT

### NAT (Network Address Translation)

NAT translates private IP addresses into public IP addresses.

Purpose:
- Conserve public IP addresses
- Hide internal network structure

Example:
192.168.1.10 → 203.0.113.5

Types:
- Static NAT (1-to-1 mapping)
- Dynamic NAT (pool of public IPs)

---

### PAT (Port Address Translation)

Also called NAT overload.

- Many private IPs share one public IP.
- Differentiates sessions using port numbers.

Example:
192.168.1.10:5000 → 203.0.113.5:30001  
192.168.1.11:5001 → 203.0.113.5:30002  

PAT is what most home routers use.

---

## 5. FHRP (First Hop Redundancy Protocol)

FHRP provides gateway redundancy.

Problem:
If default gateway router fails, the network loses connectivity.

Solution:
Multiple routers share a **virtual IP (VIP)**.
Only one is active at a time.

Common FHRP protocols:
- HSRP (Cisco)
- VRRP (open standard)
- GLBP (Cisco)

---

### VIP (Virtual IP)

A VIP is a shared IP address used by redundant routers.

- Devices use VIP as their default gateway.
- If active router fails, standby router takes over.
- Users experience minimal disruption.

Think of VIP as a "floating gateway."

---

## 6. Subinterfaces

A subinterface is a logical interface created on a physical router interface.

Used mainly for:
- Inter-VLAN routing (Router-on-a-Stick)

Example:
One physical interface:
GigabitEthernet0/0

Multiple subinterfaces:
GigabitEthernet0/0.10
GigabitEthernet0/0.20
GigabitEthernet0/0.30

Each subinterface:
- Assigned to a VLAN
- Has its own IP address
- Handles tagged traffic (802.1Q)

Purpose:
Allow one physical router port to route between multiple VLANs.

---

# Big Picture Summary

Static routing = manual control  
Dynamic routing = automatic learning  
OSPF/EIGRP = inside networks  
BGP = Internet-level routing  
NAT/PAT = private-to-public translation  
FHRP/VIP = gateway redundancy  
Subinterfaces = route between VLANs using one port

Routing is about one question:

"How does a packet know where to go next?"
