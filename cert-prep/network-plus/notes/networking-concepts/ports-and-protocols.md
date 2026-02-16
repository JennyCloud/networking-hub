# Ports and Protocols

Ports identify specific processes or services running on a device.  
Protocols define the rules for communication between devices.

Think of an IP address as a building address, and a port number as the apartment number.

---

## FTP (File Transfer Protocol)
- **Port:** 21 (Control), 20 (Data)
- **Protocol:** TCP
- **Purpose:** Transfers files between client and server
- **Security:** Not encrypted (credentials sent in plain text)
- **Use Case:** Legacy file transfers

---

## SFTP (SSH File Transfer Protocol)
- **Port:** 22
- **Protocol:** TCP
- **Purpose:** Secure file transfer
- **Security:** Encrypted via SSH
- **Use Case:** Secure file uploads/downloads

---

## SSH (Secure Shell)
- **Port:** 22
- **Protocol:** TCP
- **Purpose:** Secure remote access to systems
- **Security:** Encrypted
- **Use Case:** Managing Linux servers remotely

---

## Telnet
- **Port:** 23
- **Protocol:** TCP
- **Purpose:** Remote command-line access
- **Security:** Not encrypted
- **Use Case:** Legacy systems (largely replaced by SSH)

---

## SMTP (Simple Mail Transfer Protocol)
- **Port:** 25 (Default)
- **Other Ports:** 587 (Secure submission), 465 (SMTPS)
- **Protocol:** TCP
- **Purpose:** Sends email between mail servers
- **Security:** Can be encrypted with TLS

---

## DNS (Domain Name System)
- **Port:** 53
- **Protocol:** UDP (mostly), TCP (zone transfers)
- **Purpose:** Resolves domain names to IP addresses
- **Use Case:** Translating example.com → 93.184.216.34

---

## DHCP (Dynamic Host Configuration Protocol)
- **Ports:** 67 (Server), 68 (Client)
- **Protocol:** UDP
- **Purpose:** Automatically assigns IP addresses and network settings
- **Process:** DORA (Discover, Offer, Request, Acknowledge)

---

## HTTP (Hypertext Transfer Protocol)
- **Port:** 80
- **Protocol:** TCP
- **Purpose:** Transfers web content
- **Security:** Not encrypted
- **Use Case:** Standard web traffic

---

## HTTPS (HTTP Secure)
- **Port:** 443
- **Protocol:** TCP
- **Purpose:** Secure web traffic
- **Security:** Encrypted using TLS/SSL
- **Use Case:** Secure websites, online banking, login pages

---

## SNMP (Simple Network Management Protocol)
- **Ports:** 161 (Agent), 162 (Traps)
- **Protocol:** UDP
- **Purpose:** Monitors and manages network devices
- **Use Case:** Network monitoring tools (routers, switches, firewalls)

---

## LDAP (Lightweight Directory Access Protocol)
- **Port:** 389
- **Secure Port:** 636 (LDAPS)
- **Protocol:** TCP/UDP
- **Purpose:** Accesses and manages directory services
- **Use Case:** Active Directory authentication

---

## RDP (Remote Desktop Protocol)
- **Port:** 3389
- **Protocol:** TCP (and UDP in newer versions)
- **Purpose:** Remote desktop access to Windows systems
- **Security:** Encrypted (can be secured further via VPN)

---

## SIP (Session Initiation Protocol)
- **Port:** 5060 (Unencrypted)
- **Secure Port:** 5061 (Encrypted)
- **Protocol:** TCP/UDP
- **Purpose:** Initiates and manages voice/video calls
- **Use Case:** VoIP systems

---

# Quick Memory Patterns

- 20/21 → FTP  
- 22 → SSH / SFTP  
- 23 → Telnet  
- 25 → SMTP  
- 53 → DNS  
- 67/68 → DHCP  
- 80 → HTTP  
- 443 → HTTPS  
- 161/162 → SNMP  
- 389 → LDAP  
- 3389 → RDP  
- 5060 → SIP  

---

Understanding ports is critical for troubleshooting.  
If traffic fails, always ask:

- Is the correct port open?
- Is the firewall blocking it?
- Is the protocol TCP or UDP?
- Is encryption required?
