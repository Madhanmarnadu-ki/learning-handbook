# Shared Responsibility Model -- Quick Notes

## 🔑 Concept

**Definition:** Responsibilities for security and management are split
between **cloud provider** and **consumer**.\
**Goal:** Ensure clear accountability for infrastructure, data, and
security in cloud computing.

------------------------------------------------------------------------

## 🏢 Traditional Datacenter (On-Premises)

-   Company is responsible for **everything**:
    -   Physical space, power, cooling, networking\
    -   Server maintenance/replacement\
    -   Patching & version upgrades\
    -   Security & access control

------------------------------------------------------------------------

## ☁️ Cloud -- Shared Responsibility

  -----------------------------------------------------------------------
  **Cloud Provider Always Handles**     **Consumer Always Handles**
  ------------------------------------- ---------------------------------
  Physical datacenter (security, power, Data & information stored in
  cooling)                              cloud

  Physical network & connectivity       Device security (phones, laptops,
                                        etc.)

  Physical hosts (hardware)             Accounts, identities, access
                                        management
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## ⚖️ Split Responsibilities -- Depends on Service Model

  -------------------------------------------------------------------------
  **Model**   **Who Handles More?** **Examples of Consumer Responsibility**
  ----------- --------------------- ---------------------------------------
  **IaaS**    **Consumer-heavy**    OS patches, network controls,
                                    applications, data

  **PaaS**    **Shared / Middle**   Data & access, some app configuration

  **SaaS**    **Provider-heavy**    Mainly user access & data usage
  -------------------------------------------------------------------------

------------------------------------------------------------------------

## 📌 Key Points

-   Even with cloud: **you always own your data & access security**.\
-   **Service model matters** -- more control = more responsibility.\
-   Cloud provider ensures physical availability & basic security so you
    focus on what you control.
