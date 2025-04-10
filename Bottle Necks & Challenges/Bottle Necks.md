# Audit Challenges, Issues, and Resolutions

## Challenges Faced During the Audit

# Experience Handling Tough SPOCs and Identifying BCP Report Issues

## Dealing with SPOCs

The SPOCs I had to deal with were tough. It was very difficult to make them understand what the actual requirement was. They often refrained from listening to the requirements and unnecessarily escalated matters.

However, dealing with them helped shape me professionally. I've gained a better understanding of how to deal with crucial clients, manage expectations, and communicate effectively under pressure.





## Major Finding in BCP Reports

The BCP (Business Continuity Planning) reports furnished by the third party were found to be inaccurate:

- The **RTO (Recovery Time Objective)** and **RPO (Recovery Point Objective)** timings were misleading.
- There were discrepancies between the **server downtime and uptime timings** shown in screenshots and the ones documented in the BCP report.

This inconsistency was identified as a **major finding**, indicating a significant gap in the third party’s reporting accuracy and reliability.


### Gathering Evidence from the Auditee (Vendor)
- Vendors often delay providing necessary evidence, making the audit process time-consuming.

### Ensuring Understanding of Control Requirements
- Many vendors struggle to understand the actual control requirements, leading to irrelevant or incomplete evidence submissions.

### Incomplete Evidence Submission
- The evidence provided is often incomplete, inconsistent, or lacks completeness and accuracy (C&A).

### Multiple Follow-Ups for Each Control Domain
- Frequent follow-ups are required to obtain necessary documentation, causing inefficiencies in the audit process.

## Key Issues Identified During the Audit

### 1. Asset Disposal Policy Compliance
- **Issue:** Some servers exceeded their End of Life (EOL) but were still listed in the asset register.
- **Action Taken:** Requested evidence of decommissioning and Certificate of Disposal (COD).
- **Finding:** Assets were still active in the production environment despite claims of removal.

### 2. Removable Media Policy Non-Compliance
- **Issue:** USB ports were claimed to be blocked using JamF, but negative testing showed some devices were not configured.
- **Action Taken:** Requested evidence of JamF configuration settings.
- **Risk Treatment:** Implemented a market-wide tool for blocking USB access, fully configured JamF, and provided evidence.

### 3. Segregation of Duties (SOD) in Change Management
- **Issue:** The same person was approving changes and performing Post-Implementation Reviews (PIR), violating SOD principles.
- **Action Taken:** Implemented SOD controls ensuring different individuals handled:
  - Change Requests
  - Approvals
  - Post-Implementation Reviews

### 4. Backup Management Gaps
- **Issue:** No monitoring process was in place to track backup failures, leaving the backup team unaware of backup statuses.
- **Action Taken:** Implemented automated email notifications (SMTP: backup@tcs.com) to inform the backup team of failures.
- **Risk Treatment:** Created a Distribution List (DL) for weekly InfoSec Manager reviews.

### 5. Capacity Management SLA Violations
- **Issue:** P1 tickets were required to be resolved within 24 hours, but resolution times ranged from 3 to 12 days.
- **Action Taken:** Identified gaps in ticket resolution tracking and enforced stricter SLA monitoring.

### 6. Asset Management Non-Compliance
- **Issue:** The asset inventory lacked a dedicated field to track End of Lifecycle (EOL).
- **Action Taken:** Enforced a mandatory EOL field in the asset inventory system.

### 7. Access Revocation Delays
- **Issue:** Employee access (physical and logical) was not revoked within 24 hours after an employee’s exit, with delays ranging from 3 to 200 days.
- **Action Taken:** Strengthened offboarding with automated workflows for timely access revocation.

## Vendor Manipulation Case

### Scenario:
A vendor claimed their application complied with the latest encryption standards:
- **TLS 1.2 or above** for data in transit
- **RSA 2048-bit or higher** digital signature
- **No weak cipher suites**

### Issue:
- The provided screenshots were irrelevant and did not confirm compliance.

### Verification:
- Conducted an independent security analysis using **SSL Labs**, revealing:
  - System was running on **TLS 1.1** (not 1.2 or above).
  - Weak cipher suites were still enabled.

### Action Taken:
- Reported non-compliance to the **Vendor Risk Office (VRO)** for corrective actions.

## Bottlenecks in External and Internal Audits

### Challenges Faced During Internal Audits

#### Gathering Evidence from the Auditee
- The biggest challenge was obtaining complete and accurate evidence on time.
- Evidence provided was often unclear or lacked **completeness and accuracy (C&A).**

#### Delays in Evidence Collection and Escalation Process
- Process initiated via **Smartsheet** and tracked via **ITSM Tool**.
- **70% of escalations** were due to missing or delayed evidence.

### Escalation Levels for Missing Evidence

#### Level 3: Audit Contact
- If no evidence was provided, escalation was discussed in **weekly status calls**.

#### Level 2: ITSM / Vendor Risk Office (VRO)
- If the due date was approaching, escalation was discussed in **monthly calls**.

#### Level 1: Directors / SMEs / CISO
- If evidence was still missing, final escalation was made to top management.

### Audit Team Involvement
- The IT audit team participated in **weekly and monthly calls** to discuss audit progress.

## Case Study: Transition from On-Premise to Cloud

### Background
- The organization transitioned its **on-premise** infrastructure to the **cloud**, leading to decommissioning of facilities.
- Previously, all production environments were deployed in **CITRIX (IaaS)** servers, networks, OS, and applications.
- In **2023**, the company migrated to **Microsoft Azure Cloud** in the **Europe** region (**PaaS**).

### Risk and Compliance Team’s Responsibilities

#### Offboarding CITRIX and Onboarding Microsoft Azure Cloud
- Ensured a structured decommissioning of **CITRIX resources** before transitioning to **Azure**.

#### Decommissioning CITRIX Assets
- All **CITRIX assets** were identified, documented, and decommissioned.
- **Asset inventory** was updated to reflect decommissioned items.

#### Disposal and Compliance Requirements
- Ensured proper **disposal procedures**, including **Certificate of Disposal (COD) collection**.
- Verified compliance with **industry regulations**.

#### Updating Azure Inventory
- Ensured **Azure asset inventory** was up to date with the latest **server details**.
- Verified **configurations** to meet security and compliance standards.

## Key Takeaways from the Audit Process

1. **Evidence Collection:** A structured escalation matrix ensures timely evidence collection.
2. **Cloud Migration Compliance:** Ensured proper offboarding from **CITRIX** and onboarding to **Azure** with all compliance measures.
3. **Process Improvement:** Regular tracking through **weekly and monthly status calls** helped address delays in evidence collection.

---

## Full Forms of Abbreviations Used

### General IT and Audit Terms
- **C&A** - Completeness and Accuracy  
- **ITSM** - IT Service Management  
- **VRO** - Vendor Risk Office  
- **SME** - Subject Matter Expert  
- **CISO** - Chief Information Security Officer  
- **DL** - Distribution List  
- **SOD** - Segregation of Duties  

### Infrastructure and Cloud Computing
- **IaaS** - Infrastructure as a Service  
- **PaaS** - Platform as a Service  
- **CITRIX** - (Refers to **Citrix Systems**, a company providing virtualization solutions)  
- **EOL** - End of Life  

### Security and Compliance
- **PII** - Personally Identifiable Information  
- **SPII** - Sensitive Personally Identifiable Information  
- **PHI** - Protected Health Information  
- **BSI** - Business Sensitive Information  
- **COD** - Certificate of Disposal  

### Backup and Change Management
- **PIR** - Post-Implementation Review  
- **SMTP** - Simple Mail Transfer Protocol  
