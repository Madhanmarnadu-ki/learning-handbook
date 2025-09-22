
# ⚙️ Platform as a Service (PaaS) – Quick Notes

## 📌 Definition
- **Middle ground** between IaaS (infrastructure) and SaaS (fully managed solution).
- **Cloud provider manages:**
  - Physical infrastructure, physical security, network connectivity
  - Operating systems, middleware, databases
  - Development tools & business intelligence services
- **You focus on:**
  - Building and deploying applications
  - Managing your data and users

No need to worry about **licensing, patching, or maintaining OS/databases** — provider takes care of it.

---

## ⚖️ Shared Responsibility in PaaS

| **Responsibility**                  | **Cloud Provider** | **Consumer** |
|------------------------------------|-------------------|-------------|
| Physical datacenter, network, security | ✅                | ❌          |
| OS, middleware, development tools  | ✅                | ❌          |
| Application code & data            | ❌                | ✅          |
| User access & identity             | ❌                | ✅          |
| Networking & app security          | ⚠️ (Shared)      | ⚠️ (Shared) |

---

## 📚 Common Scenarios for PaaS
- **Development Framework:** Quickly build, test, and deploy applications with built-in scalability, HA, and multi-tenant capability.
- **Analytics & Business Intelligence:** Use PaaS tools to analyze data, find patterns, and predict outcomes to improve decisions.
- **API Development:** Host APIs easily with integrated security and monitoring.
