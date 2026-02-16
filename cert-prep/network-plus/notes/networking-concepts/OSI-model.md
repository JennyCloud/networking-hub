# OSI Model

The **OSI (Open Systems Interconnection) Model** is a conceptual framework used to understand and standardize how different networking protocols interact in a network. It divides network communication into **7 layers**, from physical transmission to application-level interactions.

---

## 7 Layers of the OSI Model

| Layer | Name                  | Function / Key Points |
|-------|----------------------|---------------------|
| 7     | Application          | Interfaces with software applications; provides network services to end-users. Examples: HTTP, FTP, SMTP. |
| 6     | Presentation         | Translates data between network and application formats; handles encryption, compression. Examples: SSL/TLS, JPEG, ASCII. |
| 5     | Session              | Manages sessions and connections between applications. Examples: RPC, NetBIOS sessions. |
| 4     | Transport            | Ensures reliable data transfer; handles segmentation, flow control, and error recovery. Protocols: TCP (reliable), UDP (unreliable). |
| 3     | Network              | Determines best path for data delivery (routing); handles logical addressing. Examples: IP, ICMP. |
| 2     | Data Link            | Handles physical addressing (MAC), error detection/correction, and frame delivery within a LAN. Examples: Ethernet, PPP, Switches. |
| 1     | Physical             | Transmits raw bits over physical medium; defines cabling, voltages, connectors. Examples: Ethernet cables, hubs, repeaters. |

---

## Key Points

- **Layer 1–3**: Mostly concerned with moving data (physical devices, switches, routers)  
- **Layer 4–7**: Mostly concerned with data handling, reliability, and user-facing applications  
- Each layer communicates with the layers directly above and below it.  
- Helps troubleshoot network problems:  
  - Physical layer issues → check cables, hardware  
  - Data Link → check MAC addresses, switches  
  - Network → check IP addressing, routing  
  - Transport → check TCP/UDP connections, port availability  
  - Upper layers → check applications, protocols, encryption  

---

## Quick Example

Sending an HTTP request from a browser:

1. **Application Layer (7):** Browser generates HTTP request  
2. **Presentation Layer (6):** Data formatted (e.g., HTML encoded)  
3. **Session Layer (5):** Session established with web server  
4. **Transport Layer (4):** TCP segments data and manages delivery  
5. **Network Layer (3):** IP address assigned; packet routed  
6. **Data Link Layer (2):** Encapsulated into frames with MAC addresses  
7. **Physical Layer (1):** Bits transmitted over cable or Wi-Fi
