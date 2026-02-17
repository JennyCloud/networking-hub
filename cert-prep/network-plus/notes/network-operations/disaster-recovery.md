# Disaster Recovery Concepts

Disaster recovery ensures that IT services can continue or be restored quickly after an unexpected disruption. Key concepts include recovery objectives, system reliability metrics, site strategies, and testing.

---

## 1. Recovery Objectives

### **RPO (Recovery Point Objective)**
- Defines the **maximum tolerable data loss** measured in time.
- Example: An RPO of 4 hours means backups must be at least every 4 hours to prevent data loss beyond that point.

### **RTO (Recovery Time Objective)**
- Defines the **maximum acceptable downtime** after a disruption.
- Example: An RTO of 2 hours means the system must be restored and operational within 2 hours of an outage.

---

## 2. System Reliability Metrics

### **MTTR (Mean Time To Recovery / Repair)**
- Average time to **restore a failed system**.
- Focuses on the repair process and efficiency of response.

### **MTBF (Mean Time Between Failures)**
- Average time a system operates **without failure**.
- Used to assess reliability and predict maintenance needs.

---

## 3. Disaster Recovery Site Types

### **Cold Site**
- **No active systems**, only space and basic infrastructure.
- Requires longer setup and data restoration.
- Cost: Low

### **Warm Site**
- Partially equipped with servers and network; data may be periodically updated.
- Recovery is faster than a cold site but slower than a hot site.
- Cost: Medium

### **Hot Site**
- Fully operational and synchronized with primary systems.
- Minimal downtime in case of failure.
- Cost: High

---

## 4. Active vs Passive Systems

### **Active-Active**
- Two or more systems **running simultaneously**, sharing the load.
- Provides high availability and load balancing.

### **Active-Passive**
- Primary system is active; secondary system is **standby**.
- Secondary system activates only when primary fails.

---

## 5. Disaster Recovery Testing

- **Purpose:** Validate the effectiveness of recovery plans.
- **Types of tests:**
  - **Simulation** – Test procedures without impacting live systems.
  - **Parallel** – Run backup systems alongside production to verify readiness.
  - **Full Interruption** – Actual switchover to backup systems.
- **Frequency:** Regularly scheduled based on RTO/RPO requirements.

---

**Summary Table**

| Term | Definition | Example |
|------|-----------|---------|
| RPO | Max data loss tolerance | 4 hours of data |
| RTO | Max downtime tolerance | 2 hours to restore |
| MTTR | Avg repair time | 30 min to fix a server |
| MTBF | Avg time between failures | 180 days of uptime |
| Cold Site | Empty backup facility | Needs full setup |
| Warm Site | Partially ready site | Data updated daily |
| Hot Site | Fully ready site | Near-instant recovery |
| Active-Active | Both systems running | Load-balanced web servers |
| Active-Passive | Backup system standby | Secondary DB server |

