# IPv4 Addressing

## What is IPv4?

IPv4 (Internet Protocol version 4) is a 32-bit addressing system used to identify devices on a network.

- Written in dotted decimal format (e.g., 192.168.1.10)
- 32 bits total
- Divided into 4 octets (8 bits each)
- Each octet ranges from 0–255

Example:
192.168.1.10

---

# Public vs Private IP Addresses

## Public IP Address

- Globally unique
- Routable on the internet
- Assigned by ISP
- Required for communication over the public internet

Example:
8.8.8.8 (Google DNS)

---

## Private IP Address

- Used inside internal networks (LAN)
- Not routable on the public internet
- Defined by RFC1918
- Requires NAT to access the internet

---

# RFC1918 Private Address Ranges

RFC1918 defines three private IPv4 ranges:

- 10.0.0.0 – 10.255.255.255       (Class A private range)
- 172.16.0.0 – 172.31.255.255     (Class B private range)
- 192.168.0.0 – 192.168.255.255   (Class C private range)

These are commonly used in:
- Home networks
- Corporate LANs
- Cloud virtual networks

---

# APIPA (Automatic Private IP Addressing)

APIPA range:
169.254.0.0 – 169.254.255.255

- Automatically assigned when DHCP fails
- Indicates device could not reach DHCP server
- Not routable
- Used for temporary local communication only

If you see 169.254.x.x → DHCP problem.

---

# Loopback Address

Loopback range:
127.0.0.0 – 127.255.255.255

Most common:
127.0.0.1

- Refers to the local device
- Used for testing TCP/IP stack
- Never leaves the device

Command:
ping 127.0.0.1

If it fails → TCP/IP stack issue.

---

# IPv4 Address Classes (Classful Addressing)

Historically, IPv4 used classes based on first octet.

## Class A
- Range: 1.0.0.0 – 126.255.255.255
- Default subnet mask: 255.0.0.0 (/8)
- Large networks
- First octet: 1–126

## Class B
- Range: 128.0.0.0 – 191.255.255.255
- Default subnet mask: 255.255.0.0 (/16)
- Medium networks
- First octet: 128–191

## Class C
- Range: 192.0.0.0 – 223.255.255.255
- Default subnet mask: 255.255.255.0 (/24)
- Small networks
- First octet: 192–223

## Class D
- Range: 224.0.0.0 – 239.255.255.255
- Used for multicast
- Not for host assignment

## Class E
- Range: 240.0.0.0 – 255.255.255.255
- Reserved for experimental use

Note:
Classful addressing is mostly obsolete. Modern networks use CIDR.

---

# CIDR (Classless Inter-Domain Routing)

CIDR replaces classful addressing.

Format:
192.168.1.0/24

The "/24" means:
24 bits are network portion
Remaining bits are host portion

Examples:

/8  = 255.0.0.0

/16 = 255.255.0.0

/24 = 255.255.255.0

/30 = 255.255.255.252

CIDR allows flexible subnet sizes instead of fixed A/B/C classes.

---

# Subnetting

Subnetting divides a network into smaller networks.

Purpose:
- Improve performance
- Increase security
- Organize network logically
- Reduce broadcast domains

Example:
192.168.1.0/24 can be divided into:
- 192.168.1.0/26
- 192.168.1.64/26
- 192.168.1.128/26
- 192.168.1.192/26

---

# VLSM (Variable Length Subnet Mask)

VLSM allows different subnet sizes within the same network.

Example:

You need:
- 50 hosts
- 20 hosts
- 10 hosts

Instead of giving each subnet 254 hosts (/24),
you allocate:

- /26 for 50 hosts (62 usable)
- /27 for 20 hosts (30 usable)
- /28 for 10 hosts (14 usable)

VLSM increases IP address efficiency.

---

# Key Concepts

- Public = internet routable
- Private = internal only (RFC1918)
- APIPA = DHCP failure
- Loopback = local testing
- CIDR = modern subnetting
- VLSM = flexible subnet sizes
- Classes = historical concept (A, B, C, D, E)

If you understand subnetting clearly, IPv4 becomes logical instead of memorized.
