# Types of Network Attacks

---

## 1. Denial of Service (DoS) & Distributed Denial of Service (DDoS)

### DoS
A **Denial of Service (DoS)** attack attempts to overwhelm a system (server, router, website) so legitimate users cannot access it.

- Single attacking source
- Overloads bandwidth, CPU, or memory
- Example: Sending massive amounts of SYN requests (SYN flood)

### DDoS
A **Distributed Denial of Service (DDoS)** attack uses multiple compromised systems (botnet) to attack a single target.

- Multiple attacking devices
- Much harder to block
- Often uses infected IoT devices

**Goal:** Make services unavailable.

---

## 2. VLAN Hopping

VLAN hopping is an attack that allows a malicious device to send traffic into a VLAN it should not have access to.

### Methods:
- Switch spoofing (pretending to be a trunk port)
- Double tagging (adding two VLAN tags to bypass segmentation)

**Goal:** Break VLAN isolation.

**Prevention:**  
- Disable unused ports  
- Set ports to access mode  
- Disable auto trunking  

---

## 3. MAC Flooding

MAC flooding occurs when an attacker overwhelms a switch with fake MAC addresses.

- Switch MAC table becomes full
- Switch behaves like a hub
- Traffic is broadcast to all ports

**Goal:** Capture network traffic (sniffing).

**Prevention:**  
- Enable port security  
- Limit MAC addresses per port  

---

## 4. ARP Poisoning / ARP Spoofing

ARP (Address Resolution Protocol) maps IP addresses to MAC addresses.

In ARP poisoning:
- Attacker sends fake ARP messages
- Associates attacker’s MAC address with victim’s IP
- Traffic gets redirected to attacker

**Result:** Man-in-the-middle (on-path) attack.

**Prevention:**  
- Dynamic ARP inspection (DAI)  
- Static ARP entries  
- Encrypted protocols (HTTPS, SSH)

---

## 5. DNS Poisoning / DNS Spoofing

DNS translates domain names to IP addresses.

In DNS poisoning:
- Attacker inserts false DNS records
- Users are redirected to malicious websites

Example:
User types `bank.com` → attacker redirects to fake bank site.

**Goal:** Credential theft or malware distribution.

**Prevention:**  
- DNSSEC  
- Secure DNS servers  
- Monitoring DNS changes  

---

## 6. Rogue Devices / Rogue Services

### Rogue Device
Unauthorized hardware connected to a network.
Example:
- Unauthorized wireless access point
- Employee plugging in personal router

### Rogue Service
Unauthorized software service running on network.
Example:
- Fake DHCP server
- Fake DNS server

**Risk:** Traffic interception, credential theft.

**Prevention:**  
- Network access control (NAC)  
- Port security  
- Regular network scans  

---

## 7. Evil Twin

An evil twin is a fake Wi-Fi access point that mimics a legitimate one.

Example:
- Real network: CoffeeShopWiFi
- Fake network: CoffeeShopWiFi_Free

Users connect unknowingly.
Attacker captures credentials and traffic.

**Prevention:**  
- Use VPN  
- Avoid auto-connect  
- Verify certificates  

---

## 8. On-Path Attack (Man-in-the-Middle)

An on-path attack occurs when an attacker secretly intercepts and possibly alters communication between two parties.

Common methods:
- ARP poisoning
- Rogue Wi-Fi
- Session hijacking

**Goal:** Eavesdrop or modify data.

**Prevention:**  
- Encryption (TLS/HTTPS)  
- VPN  
- Strong authentication  

---

## 9. Social Engineering Attacks

Social engineering manipulates people instead of systems.

### Phishing
Fraudulent emails or messages trick users into revealing credentials.

- Spear phishing (targeted)
- Whaling (executives)
- Smishing (SMS)
- Vishing (voice)

### Dumpster Diving
Searching trash for sensitive information.

### Shoulder Surfing
Watching someone enter passwords or PINs.

### Tailgating
Following an authorized person into a restricted area without authentication.

**Prevention:**  
- Security awareness training  
- Multi-factor authentication (MFA)  
- Clean desk policy  
- Physical security controls  

---

# Tip

- DoS/DDoS = availability attack  
- VLAN hopping = segmentation bypass  
- MAC flooding = switch table overload  
- ARP poisoning = Layer 2 redirection  
- DNS poisoning = name resolution manipulation  
- Evil twin = fake Wi-Fi AP  
- On-path = traffic interception  
- Social engineering = human manipulation  

Understand what layer is being attacked:
- Layer 2 → ARP, MAC flooding, VLAN hopping  
- Layer 3/4 → DoS  
- Application layer → DNS poisoning, phishing  
