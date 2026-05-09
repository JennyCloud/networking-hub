# Network Monitoring

Network monitoring is the process of observing network devices and traffic to ensure performance, availability, and security.

It helps answer:
- Is the network healthy?
- Is something failing?
- Is traffic behaving abnormally?

---

## 1. SNMP (Simple Network Management Protocol)

SNMP is used to monitor and manage network devices such as routers, switches, firewalls, and servers.

### Key Concepts:
- **SNMP Manager** → Monitoring system (polls devices)
- **SNMP Agent** → Software running on the device
- **MIB (Management Information Base)** → Database of device information
- **OIDs (Object Identifiers)** → Unique identifiers for metrics
- **Trap** → Alert sent from device to manager

### What SNMP Monitors:
- CPU usage
- Memory usage
- Interface status (up/down)
- Bandwidth usage
- Temperature

SNMP is commonly used in network monitoring platforms.

---

## 2. Flow Data (NetFlow, sFlow, IPFIX)

Flow data provides metadata about traffic without capturing full packets.

It answers:
- Who is talking to whom?
- How much data is being transferred?
- What protocol is being used?

### Flow Data Includes:
- Source IP
- Destination IP
- Source/Destination ports
- Protocol (TCP/UDP)
- Bytes transferred
- Duration of session

Flow data is useful for:
- Traffic analysis
- Capacity planning
- Detecting unusual behavior

---

## 3. Packet Capture (PCAP)

Packet capture records full packets as they travel across the network.

Tools like Wireshark analyze packet captures.

Packet capture allows deep inspection of:
- Packet headers
- Payload data
- TCP handshakes
- DNS queries
- Errors and retransmissions

Used for:
- Troubleshooting connectivity issues
- Security investigations
- Detailed protocol analysis

Packet capture provides the most detail but can consume significant storage.

---

## 4. Baseline Metrics

A baseline is a record of normal network performance.

Examples:
- Average bandwidth usage
- Normal CPU load
- Typical latency
- Expected packet loss

Why baselines matter:
- Helps detect anomalies
- Identifies performance degradation
- Assists in capacity planning

Without a baseline, you cannot determine what is “abnormal.”

---

## 5. Log Aggregation

Log aggregation collects logs from multiple devices into a centralized system.

Devices that generate logs:
- Routers
- Switches
- Firewalls
- Servers
- Applications

Common protocol: Syslog

Benefits:
- Centralized visibility
- Easier troubleshooting
- Security event detection
- Compliance auditing

---

## 6. API Integration

APIs (Application Programming Interfaces) allow monitoring tools to integrate with other systems.

Examples:
- Pulling monitoring data into dashboards
- Sending alerts to ticketing systems
- Automating configuration backups

APIs enable automation and interoperability between platforms.

---

## 7. Port Mirroring (SPAN)

Port mirroring copies traffic from one port (or VLAN) to another port.

Purpose:
- Send traffic to monitoring tools
- Perform packet analysis
- Conduct intrusion detection

Example:
Traffic from switch port 1 is mirrored to port 10 where a monitoring device is connected.

Port mirroring allows analysis without interrupting live traffic.

---

# Summary

Network monitoring methods vary in depth:

- SNMP → Device health and metrics
- Flow Data → Traffic patterns and summaries
- Packet Capture → Full packet inspection
- Baselines → Normal performance reference
- Log Aggregation → Centralized event tracking
- API Integration → Automation and integration
- Port Mirroring → Traffic duplication for analysis

Each method provides different visibility into network behavior.
