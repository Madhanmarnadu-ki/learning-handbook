# ☁️ Cloud Models -- Quick Notes

## 📌 Definition

Cloud models define **how cloud resources are deployed**.\
Main models: **Private**, **Public**, **Hybrid**\
Also relevant: **Multi-Cloud** & tools like **Azure Arc**.

------------------------------------------------------------------------

## 🏢 Private Cloud

-   **Definition:** Cloud infrastructure used by a **single
    organization**.
-   **Hosting:** On-premises or dedicated offsite datacenter.
-   **Pros:**
    -   Full control over resources, security, compliance
    -   Data not shared with other orgs
-   **Cons:**
    -   High capital expenditure (CapEx) for hardware
    -   Responsible for maintenance, patching

------------------------------------------------------------------------

## 🌍 Public Cloud

-   **Definition:** Cloud services offered to **anyone** over the
    internet by a 3rd-party provider (e.g., Azure, AWS, GCP).
-   **Pros:**
    -   No CapEx --- pay-as-you-go (OpEx)
    -   Quick provisioning & scalability
-   **Cons:**
    -   Less control over resources & security

------------------------------------------------------------------------

## 🔀 Hybrid Cloud

-   **Definition:** Combines **private + public cloud** in a connected
    environment.
-   **Benefits:**
    -   Flexibility --- choose where to run apps
    -   Burst workloads to public cloud for demand spikes
    -   Stronger security / compliance options

------------------------------------------------------------------------

## 🔄 Multi-Cloud

-   **Definition:** Use of **multiple public cloud providers**.
-   **Reasons:**
    -   Leverage unique features from different providers
    -   Migration in progress
-   **Challenges:**
    -   Must manage resources & security across clouds

------------------------------------------------------------------------

## 🛠 Key Azure Technologies

-   **Azure Arc:**\
    Manage resources across Azure, on-prem, hybrid, and multi-cloud.
-   **Azure VMware Solution:**\
    Run VMware workloads natively on Azure with seamless migration &
    scalability.

------------------------------------------------------------------------

# Cloud Models — Comparison Table 

| Aspect       | Public Cloud                                     | Private Cloud                                   | Hybrid Cloud                                               |
|--------------|---------------------------------------------------|-------------------------------------------------|------------------------------------------------------------|
| Cost         | No CapEx; pay‑as‑you‑go                           | High CapEx; purchase & maintain hardware        | Mix of OpEx & CapEx                                       |
| Control      | Limited; provider controls infra                  | Full control by organization                    | Organization chooses per workload                          |
| Scalability  | Very fast, elastic                                | Limited by owned hardware                       | Burst to public cloud for peaks                            |
| Security     | Provider handles physical; logical is shared      | Fully controlled by organization                | Keep sensitive on private; run other parts on public cloud |
| Typical Use  | Startups, variable demand, quick experiments      | Regulated workloads, strict data residency      | Enterprises balancing compliance with agility              |

---


