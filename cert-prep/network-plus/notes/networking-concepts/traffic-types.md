# Traffic Types: Unicast, Broadcast, Multicast, Anycast

In networking, traffic type describes **how data is delivered from sender to receiver(s)**.

Understanding this helps explain how networks control bandwidth, efficiency, and routing behavior.

## 1. Unicast (One-to-One)

**Definition:**  
Traffic sent from one device to one specific device.

**How it works:**
- Sender knows the exact destination IP address.
- Most normal internet traffic is unicast.

**Example:**
- Opening a website
- SSH into a server
- Sending an email

**Key Point:**
Unicast is the most common traffic type on IP networks.

---

## 2. Broadcast (One-to-All in Local Network)

**Definition:**  
Traffic sent from one device to *all devices* in the same local network (broadcast domain).

**How it works:**
- Uses a broadcast address (e.g., 192.168.1.255).
- All devices on that LAN receive the packet.
- Only works within a local network (routers block broadcasts).

**Example:**
- ARP request: "Who has 192.168.1.10?"
- DHCP discovery message

**Key Point:**
Broadcast increases network traffic and does not cross routers.

---

## 3. Multicast (One-to-Many, Specific Group)

**Definition:**  
Traffic sent from one device to a selected group of devices.

**How it works:**
- Uses multicast IP range (224.0.0.0 – 239.255.255.255).
- Only devices that join the multicast group receive the traffic.
- More efficient than broadcast.

**Example:**
- Streaming video to multiple users
- Online conferencing
- IPTV

**Key Point:**
Multicast reduces unnecessary traffic compared to broadcast.

---

## 4. Anycast (One-to-Nearest)

**Definition:**  
Traffic sent to the nearest or best destination among multiple devices sharing the same IP address.

**How it works:**
- Multiple servers share the same IP.
- Routing determines the closest or most optimal destination.
- Common in global services.

**Example:**
- DNS root servers
- Content Delivery Networks (CDNs)

**Key Point:**
Anycast improves performance and redundancy.

---

# Quick Comparison

| Traffic Type | Delivery Type | Scope | Example |
|--------------|--------------|--------|----------|
| Unicast | One-to-One | Across networks | Web browsing |
| Broadcast | One-to-All | Local network only | ARP |
| Multicast | One-to-Selected-Group | Configured group members | Streaming |
| Anycast | One-to-Nearest | Across networks | DNS servers |

---

# Tips

- Broadcast traffic does NOT cross routers.
- Multicast is more bandwidth-efficient than broadcast.
- Anycast relies on routing decisions.
- Most everyday traffic is unicast.
