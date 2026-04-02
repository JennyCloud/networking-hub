# Switching Technologies

## 1. VLANs (Virtual Local Area Networks)

A VLAN logically separates devices on the same physical switch into different broadcast domains.

### Why VLANs exist
- Reduce broadcast traffic
- Improve security (isolate departments)
- Organize networks logically without new hardware

Devices in different VLANs **cannot communicate directly** without a Layer 3 device (router or Layer 3 switch).

### Key Concepts
- **Access Port**: Assigned to one VLAN. Used for end devices (PCs, printers).
- **Trunk Port**: Carries multiple VLANs between switches using VLAN tagging (802.1Q).
- **Default VLAN**: Usually VLAN 1 (avoid using it for production traffic).

## 2. Interface Configuration

Switch interfaces (ports) must be configured correctly for traffic to flow properly.

### Common Settings
- Assign VLAN to access port
- Configure trunking between switches
- Set speed and duplex (auto or manual)
- Enable/disable ports
- Configure port security (limit MAC addresses)

Misconfigured interfaces often cause:
- No connectivity
- VLAN mismatch
- Duplex mismatch (causes collisions and slow performance)

---

## 3. Spanning Tree Protocol (STP)

Spanning Tree prevents **Layer 2 loops** in switched networks.

### Why loops are dangerous
Switches forward broadcast frames.
If there's a loop, broadcasts multiply endlessly.
This causes a **broadcast storm** and network failure.

### What STP Does
- Detects redundant paths
- Blocks some ports to prevent loops
- Automatically re-enables ports if a path fails

### Variants
- STP (original)
- RSTP (Rapid STP – faster convergence)

Think of STP as a traffic controller preventing infinite traffic circles.

---

## 4. MTU (Maximum Transmission Unit)

MTU is the largest packet size (in bytes) that can be transmitted over a network interface.

### Standard Ethernet MTU
- 1500 bytes

If a packet exceeds MTU:
- It must be fragmented
- Or it gets dropped (depending on settings)

MTU mismatches can cause:
- Slow performance
- Connection issues
- VPN problems
- Incomplete page loads

---

## 5. Jumbo Frames

Jumbo frames are Ethernet frames larger than 1500 bytes.

### Typical Jumbo Frame Size
- 9000 bytes

### Benefits
- Reduced CPU overhead
- Improved performance for large data transfers
- Useful in data centers and storage networks

### Important Rule
All devices along the path must support jumbo frames.
If one device does not, packets may be dropped.

---

## Troubleshooting Switching Issues

Common Problems:
- Wrong VLAN assignment
- Trunk not configured properly
- STP blocking unexpected port
- MTU mismatch
- Duplex mismatch

When troubleshooting:
1. Check VLAN membership
2. Verify trunk configuration
3. Confirm port status (up/down)
4. Check MTU consistency
5. Look for STP blocked ports

---

## Big Picture

Switching operates at Layer 2 (Data Link layer).

It forwards frames based on MAC addresses, not IP addresses.

Routing moves traffic between networks.
Switching moves traffic within networks.

Understanding switching is essential for:
- VLAN troubleshooting
- Performance optimization
- Network segmentation
- Infrastructure support roles
