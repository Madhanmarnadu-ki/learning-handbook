
# 🖥 Infrastructure as a Service (IaaS) – Quick Notes

## 📌 Definition
- Most **flexible** cloud service model.
- **Cloud provider manages:**
  - Physical infrastructure (servers, storage, networking)
  - Network connectivity
  - Physical security
- **Consumer manages:**
  - OS installation/configuration
  - Network configuration
  - Database/storage setup
  - Patching, updates, and security

Essentially, you’re **renting hardware** in a cloud datacenter — what you do with it is up to you.

---

## ⚖️ Shared Responsibility in IaaS

| **Responsibility**            | **Cloud Provider** | **Consumer** |
|-------------------------------|-------------------|-------------|
| Physical datacenter & security| ✅                | ❌          |
| Network connectivity (internet)| ✅               | ❌          |
| Operating system & middleware | ❌                | ✅          |
| Application installation/config| ❌               | ✅          |
| Data, access, and security    | ❌                | ✅          |

---

## 📚 Common Scenarios for IaaS
- **Lift-and-Shift Migration:** Move existing on-prem workloads to IaaS with minimal changes.
- **Testing & Development:** Rapidly spin up/down dev/test environments with full control over configuration.
- **Custom Solutions:** When you need flexibility to choose OS, runtime, network configuration, and have specific compliance/security requirements.
