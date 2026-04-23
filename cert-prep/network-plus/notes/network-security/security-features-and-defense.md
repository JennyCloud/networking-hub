# Security Features and Defense

---

## Device Hardening
Device hardening is the process of securing a device by reducing its attack surface.  
**Methods include:**
- Disabling unnecessary services and ports
- Applying the latest security patches and updates
- Enforcing strong authentication and passwords
- Implementing endpoint protection (antivirus/antimalware)

## Network Access Control (NAC)
NAC restricts device access to a network based on compliance with security policies.  
**Key points:**
- Devices must meet predefined requirements (e.g., antivirus installed, OS up-to-date) before granting access
- Helps prevent compromised or unauthorized devices from connecting
- Can enforce access via VLAN assignment or quarantined network segments

## Key Management
Key management involves creating, distributing, storing, and rotating cryptographic keys securely.  
**Essential practices:**
- Use strong encryption keys for data in transit and at rest
- Regularly rotate keys to reduce exposure
- Protect keys in hardware security modules (HSMs) or secure storage

## Access Control Lists (ACL)
ACLs define rules to allow or deny traffic based on IP addresses, protocols, or ports.  
**Example uses:**
- Restricting which devices can access specific servers
- Filtering traffic at routers, firewalls, or switches
- Implementing least-privilege network access

## URL/Content Filtering
URL/content filtering blocks access to malicious or unwanted websites.  
**Functions:**
- Prevents users from visiting dangerous or non-compliant sites
- Can be implemented via firewalls, proxy servers, or dedicated appliances
- Helps enforce corporate policies and improve network security

## Trusted vs. Untrusted Zones
Networks are often segmented into zones based on trust levels.  
- **Trusted zone:** internal, secure network (LAN)
- **Untrusted zone:** external networks, like the Internet, considered risky  
**Purpose:** Limits exposure of sensitive resources by controlling access between zones

## Screened Subnet (DMZ)
A screened subnet, also called a Demilitarized Zone (DMZ), is a network segment that isolates public-facing services from the internal network.  
**Characteristics:**
- Hosts servers accessible from untrusted networks (e.g., web, email servers)
- Firewalls control traffic between the DMZ, internal network, and Internet
- Provides an additional security layer to protect internal resources
