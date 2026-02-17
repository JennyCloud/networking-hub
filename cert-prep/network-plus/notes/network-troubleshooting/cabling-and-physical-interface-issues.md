# Cabling and Physical Interface Issues

## 1. Cable Issues
Cable problems are common sources of network connectivity problems. Key issues include:

- **Incorrect Cable Type**  
  - Using the wrong type of cable for a connection (e.g., straight-through vs crossover, Cat5e vs Cat6 for higher speeds).  
  - Can result in no connectivity or degraded performance.

- **Signal Degradation**  
  - Occurs over long cable runs or due to poor-quality cables.  
  - Symptoms: intermittent connectivity, slow speeds, high error rates.

- **Improper Termination**  
  - Badly crimped RJ-45 connectors or damaged cables.  
  - Causes open circuits or cross-talk between pairs.

- **TX/RX Transposed**  
  - Transmit and receive wires are reversed.  
  - Devices may fail to communicate unless auto-MDIX is supported.

---

## 2. Interface Issues
Problems with the physical network interface on devices can manifest as:

- **Increasing Error Counters**  
  - CRC errors, collisions, or late collisions indicate cabling or interface problems.  
  - Monitoring counters helps identify recurring issues.

- **Port Status Indicators**  
  - Link lights (LEDs) show connectivity.  
  - Down or amber lights can indicate faulty cables, mismatched speeds, or disabled ports.

---

## 3. Hardware Issues
Hardware components can also impact network performance:

- **PoE (Power over Ethernet) Problems**  
  - Devices may not power on if the switch cannot supply sufficient PoE.  
  - Check PoE budget and device requirements.

- **Transceiver Mismatch**  
  - Fiber SFPs or copper modules must match the network standard (speed, duplex, fiber type).  
  - Mismatch can prevent the link from establishing.

- **Signal Strength / Quality**  
  - Weak or noisy signals can affect fiber and wireless links.  
  - Use appropriate testing tools to measure signal loss or attenuation.
