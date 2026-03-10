# Network Topologies

Network topology describes how devices are connected and how data flows between them.

## 1. Mesh Topology

In a mesh topology, devices are interconnected with multiple paths between them.

There are two types:
- Full Mesh → Every device connects to every other device.
- Partial Mesh → Some devices have multiple connections, but not all.

### Pros
- Very high redundancy
- No single point of failure
- Reliable for critical environments

### Cons
- Expensive (lots of cabling/ports)
- Complex to manage

### Common Use
- WAN connections between branch offices
- Enterprise core infrastructure

---

## 2. Star Topology (Hub-and-Spoke)

All devices connect to a central device (hub, switch, or router).

Traffic must pass through the central point.

### Pros
- Easy to install and manage
- Easy to troubleshoot
- Scalable

### Cons
- Central device is a single point of failure

### Common Use
- Most modern LANs (using switches)
- Cloud hub-and-spoke architectures

---

## 3. Hybrid Topology

A combination of two or more different topologies.

Example:
- Star topology inside each office
- Mesh connections between offices

### Pros
- Flexible
- Scalable
- Can optimize for cost and performance

### Cons
- More complex design and troubleshooting

### Common Use
- Enterprise environments

---

## 4. Point-to-Point Topology

A direct connection between two devices.

### Pros
- Simple
- High performance
- Easy to configure

### Cons
- Not scalable by itself

### Common Use
- WAN links between two routers
- Direct fiber connections

---

## 5. Three-Tier Architecture

Traditional enterprise network design divided into three layers:

1. Access Layer
   - Connects end devices (PCs, printers)
2. Distribution Layer
   - Aggregates access switches
   - Applies policies and routing
3. Core Layer
   - High-speed backbone
   - Connects distribution layers

### Pros
- Structured and scalable
- Clear separation of roles

### Cons
- More hardware required
- Higher cost

### Common Use
- Large enterprise networks

---

## 6. Collapsed Core Architecture

Combines the Distribution Layer and Core Layer into one layer.

Access Layer → Collapsed Core Layer

### Pros
- Lower cost
- Simpler design
- Easier management

### Cons
- Less scalable than full three-tier
- Potential bottleneck if overloaded

### Common Use
- Small to medium businesses

---

## 7. Spine-and-Leaf Architecture

Modern data center topology.

- Leaf switches connect to devices (servers).
- Spine switches connect all leaf switches.
- Every leaf connects to every spine.

Traffic usually flows:
Leaf → Spine → Leaf

### Pros
- High performance
- Predictable latency
- Highly scalable
- No bottlenecks at the core

### Cons
- Requires more switching hardware
- More advanced design

### Common Use
- Modern data centers
- Cloud providers

---

# Quick Comparison

- Mesh → Maximum redundancy
- Star (Hub-and-Spoke) → Centralized design
- Hybrid → Combination of multiple designs
- Point-to-Point → Direct device connection
- Three-Tier → Traditional enterprise model
- Collapsed Core → Simplified three-tier
- Spine-and-Leaf → Modern data center architecture
