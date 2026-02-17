# Transceivers and Connectors

## 1. Transceivers

A **transceiver** (transmitter + receiver) is a device that both sends and receives signals over a network medium.

It converts:
- Electrical signals ↔ Light signals (fiber)
- Electrical signals ↔ Electrical signals (copper, different standards)

### Common Types

- **SFP (Small Form-factor Pluggable)**
  - Used in switches and routers
  - Supports fiber or copper
  - Hot-swappable

- **SFP+**
  - Similar to SFP but supports higher speeds (10 Gbps)

- **QSFP**
  - Used for high-speed connections (40 Gbps and above)

Transceivers allow flexibility — you can change the type of connection without replacing the whole device.

---

## 2. Fiber Connectors

Used with fiber-optic cables (light signals instead of electricity).

### SC (Subscriber Connector)
- Square shape
- Push-pull design
- Common in data centers
- Often used for single-mode fiber

### LC (Lucent Connector)
- Smaller than SC
- Very common in modern networks
- Used in high-density fiber environments
- Often paired with SFP modules

### ST (Straight Tip)
- Round connector
- Twist-lock (bayonet style)
- Older design
- More common in legacy networks

### MPO (Multi-fiber Push On)
- Supports multiple fiber strands in one connector
- Used for high-speed connections (40G, 100G)
- Common in data centers

---

## 3. Copper Connectors

Used with copper cables (electrical signals).

### RJ11
- Smaller connector
- Used for telephone lines
- Typically 2–4 wires

### RJ45
- Standard Ethernet connector
- Used with Cat5e, Cat6, Cat6a cables
- 8 pins (8P8C)
- Used for LAN connections

RJ45 is the most common network connector in offices and homes.

---

## 4. Coaxial Connectors

Used for coaxial cables (older networking and cable internet).

### F-type
- Used for cable TV and cable modems
- Screw-on design

### BNC (Bayonet Neill-Concelman)
- Twist-lock design
- Used in older Ethernet (10BASE2)
- Also used in CCTV systems

---

## Quick Comparison Table

| Connector | Cable Type | Common Use |
|------------|------------|------------|
| SC | Fiber | Data centers |
| LC | Fiber | Modern fiber networking |
| ST | Fiber | Legacy fiber networks |
| MPO | Fiber | High-speed data centers |
| RJ11 | Copper | Telephone lines |
| RJ45 | Copper | Ethernet LAN |
| F-type | Coax | Cable TV / Modems |
| BNC | Coax | Legacy Ethernet / CCTV |

---

## Tip

- Know which connectors are **fiber vs copper vs coax**.
- Know that RJ45 = Ethernet.
- Know that SC/LC/ST/MPO = fiber.
- Know that BNC and F-type = coaxial.
- Understand that transceivers convert signals between formats.
