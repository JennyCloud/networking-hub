# Network Device Life-Cycle Management

Life-cycle management refers to how network hardware and software are handled from deployment to retirement.  
Good life-cycle management reduces downtime, security risks, and unexpected costs.

## 1. EOL (End of Life)

**Definition:**  
End of Life (EOL) is the point when a vendor stops selling a product.

**Key Points:**
- The device is no longer manufactured or sold.
- It may still receive limited support for a period of time.
- Replacement planning should begin.

**Why It Matters:**
- No new hardware units available.
- Risk of outdated technology.
- Planning for upgrades becomes critical.

---

## 2. EOS (End of Support)

**Definition:**  
End of Support (EOS) is when the vendor stops providing technical support, patches, and updates.

**Key Points:**
- No security updates.
- No bug fixes.
- No technical assistance from the vendor.

**Risk:**
Devices at EOS become security liabilities.  
Unpatched vulnerabilities can be exploited.

---

## 3. Software Management

Software management ensures devices run stable and secure operating systems and firmware.

### Includes:

- **Firmware updates**
- **Operating system patches**
- **Configuration backups**
- **Version control and documentation**
- **Testing updates before deployment**

**Best Practices:**
- Schedule updates during maintenance windows.
- Test updates in a lab environment first.
- Always back up configurations before upgrading.
- Keep documentation of version changes.

---

## 4. Decommissioning

**Definition:**  
The safe and secure removal of a device from the network.

### Steps:

1. Back up configurations (if needed).
2. Remove the device from monitoring systems.
3. Wipe sensitive data (secure erase).
4. Remove from asset inventory.
5. Dispose or recycle according to policy.

**Security Consideration:**
Improper decommissioning can cause data leaks.

---

# Summary

| Term | Meaning | Risk if Ignored |
|------|----------|----------------|
| EOL | Product no longer sold | Hard to replace |
| EOS | No more vendor support | Security vulnerabilities |
| Software Management | Maintain updates & patches | Instability & security gaps |
| Decommissioning | Safe device removal | Data exposure |
