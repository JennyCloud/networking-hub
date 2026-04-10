# Network Services Issues

Network services can experience a variety of issues that impact connectivity, performance, and overall network functionality. Key categories include:

## 1. Switching Issues

Switching problems usually occur at Layer 2 of the OSI model and affect local network communication.

- **STP (Spanning Tree Protocol) Issues**
  - Loops in the network can cause broadcast storms and network downtime.
  - Misconfigured STP may block essential ports or fail to prevent loops.
  - Symptoms: intermittent connectivity, high CPU on switches, frequent MAC table flaps.

- **VLAN Assignment Issues**
  - Devices in the wrong VLAN cannot communicate with intended peers.
  - Misconfigured VLAN trunking can prevent multiple VLANs from propagating across switches.
  - Symptoms: inability to reach certain devices, ping failures within same subnet.

- **ACLs (Access Control Lists)**
  - Incorrect ACLs on switches or routers can block legitimate traffic.
  - Can filter by IP, protocol, or port, sometimes too restrictively.
  - Symptoms: access denied errors, application failures, network segment isolation.

---

## 2. Routing Issues

Routing problems occur at Layer 3 and affect traffic between different networks or subnets.

- **Routing Table Problems**
  - Missing or incorrect routes prevent packets from reaching destinations.
  - Static routes may be misconfigured, or dynamic routing protocols may fail.
  - Symptoms: unreachable networks, routing loops, suboptimal paths.

- **Default Route Issues**
  - Default gateway not configured or incorrect.
  - Packets destined for unknown networks cannot leave the local subnet.
  - Symptoms: internet access failure, inability to reach external networks.

---

## 3. Address Pool Exhaustion

- Occurs when DHCP servers run out of available IP addresses.
- New devices cannot obtain an IP, leading to connectivity loss.
- Symptoms: clients failing to get IP addresses, APIPA addresses (169.254.x.x).

---

## 4. Incorrect Gateway/IP/Subnet Mask

- Misconfigured IP settings on hosts prevent proper network communication.
- **Incorrect IP Address**: Conflicts or wrong subnet prevent device communication.
- **Incorrect Subnet Mask**: Devices incorrectly determine which addresses are local vs remote.
- **Incorrect Default Gateway**: Packets to external networks are not routed.
- Symptoms: no connectivity outside local network, intermittent network access, communication only with local devices.

---

### Troubleshooting Tips

1. Verify switch configurations (VLANs, STP, ACLs).
2. Check routing tables and ensure default routes exist.
3. Monitor DHCP pools for available addresses.
4. Validate host IP configuration (IP, subnet mask, gateway).
