
# 🌐 High Availability & Scalability – Quick Notes

## 🔑 Key Considerations in Cloud Apps
When designing or deploying cloud applications, two major goals are:  
1. **Uptime (Availability)** – Resources should be available when needed.  
2. **Scalability (Demand Handling)** – Ability to handle varying loads efficiently.

---

## 🟢 High Availability (HA)
- **Definition:** Ensures **maximum uptime** and continuous service delivery even during failures or disruptions.
- **How It’s Achieved:**
  - Redundancy (multiple instances in different zones/regions)
  - Fault tolerance (automatic failover mechanisms)
  - Monitoring & alerting for quick recovery
- **Azure SLAs (Service-Level Agreements):**
  - Azure guarantees uptime depending on the service (e.g., 99.9% or higher)
  - Important to design architecture to meet SLA requirements

---

## 📈 Scalability
- **Definition:** Ability to **adjust resources** to meet changing demand (scale up/down, scale in/out)
- **Benefits:**
  - Handle peak traffic smoothly
  - Avoid overpaying for unused capacity
  - Pay only for what you use (consumption-based model)

---

## 📊 Types of Scaling

| **Scaling Type**              | **Description**                                    | **Example**                                                   |
|-------------------------------|----------------------------------------------------|--------------------------------------------------------------|
| **Vertical Scaling (Up/Down)**| Increase/decrease the **power** of a single resource (CPU, RAM) | Add more CPU/RAM to an existing VM or reduce them if over-provisioned |
| **Horizontal Scaling (Out/In)**| Increase/decrease the **number** of resources       | Add more VMs/containers (scale out) or remove them when demand drops (scale in) |

