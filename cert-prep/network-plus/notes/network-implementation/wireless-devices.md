# Wireless Devices

Wireless networking in Network+ focuses on how Wi-Fi operates, how it is secured, and how devices communicate through radio frequencies.

## 1. Frequency Options

Wi-Fi operates primarily on three frequency bands:

### 2.4 GHz
- Longer range
- Slower speeds
- More interference (crowded band: Bluetooth, microwaves, etc.)
- Only 3 non-overlapping channels (1, 6, 11)

### 5 GHz
- Shorter range
- Faster speeds
- Less interference
- More non-overlapping channels

### 6 GHz (Wi-Fi 6E)
- Very fast
- Very low congestion
- Shortest range
- Used for newer high-performance devices

Higher frequency = more speed, less range.  
Lower frequency = more range, less speed.

---

## 2. Channels

A channel is a specific frequency range within a band.

- 2.4 GHz has overlapping channels
- Best practice: use channels 1, 6, or 11 to avoid interference
- 5 GHz has many non-overlapping channels

Channel overlap causes interference and slow performance.

---

## 3. SSID (Service Set Identifier)

- The public name of a wireless network
- Example: "HomeWiFi" or "Office-Guest"
- Broadcast by the Access Point (AP)
- Can be hidden, but hiding does not improve real security

Multiple SSIDs can exist on one access point (e.g., internal + guest network).

---

## 4. Network Types

### Infrastructure Mode
- Most common
- Devices connect through an Access Point (AP)

### Ad Hoc Mode
- Devices connect directly to each other
- No access point required

### Mesh Network
- Multiple APs connected together
- Expands coverage
- Used in large homes or enterprises

---

## 5. Encryption (Protecting Data)

Encryption prevents unauthorized users from reading transmitted data.

### WEP
- Old and insecure
- Easily cracked
- Not recommended

### WPA
- Improved security over WEP
- Now outdated

### WPA2
- Strong encryption (AES)
- Widely used
- Secure if configured properly

### WPA3
- Strongest current standard
- Better protection against brute-force attacks

Best practice: Use WPA3 if available, otherwise WPA2 with AES.

---

## 6. Authentication (Controlling Access)

Authentication verifies identity before granting access.

### Pre-Shared Key (PSK)
- Common in home networks
- Everyone uses same password

### Enterprise Authentication (802.1X)
- Used in businesses
- Individual login credentials
- Uses RADIUS server
- More secure than PSK

---

## 7. Guest Networks

- Separate wireless network for visitors
- Isolated from internal LAN
- Prevents access to internal resources
- Often uses its own SSID

Improves security by segmenting traffic.

---

## 8. Access Points (AP)

An Access Point:
- Connects wireless devices to wired network
- Broadcasts SSID
- Manages authentication and encryption
- Controls channels and frequency bands

Enterprise environments may use:
- Multiple APs
- Centralized wireless controller
- Mesh configurations

---

## 9. Antennas

Antennas affect wireless signal coverage and direction.

### Omnidirectional Antenna
- Broadcasts signal in all directions
- Common in home routers

### Directional Antenna
- Focuses signal in one direction
- Used for long-distance connections

Higher gain antenna = longer range but narrower coverage area.

---

## Key Concepts Summary

- Frequency affects speed and range.
- Channels must be chosen carefully to reduce interference.
- SSID identifies the wireless network.
- WPA3 > WPA2 > WPA > WEP (security strength).
- Enterprise authentication (802.1X) is more secure than PSK.
- Guest networks isolate visitors.
- Access points connect wireless to wired networks.
- Antennas shape signal coverage.

Wireless networking is about balancing coverage, performance, and security.
