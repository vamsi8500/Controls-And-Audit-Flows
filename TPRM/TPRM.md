# Third-Party Risk Management (TPRM) Overview

## 1. What is Third-Party Risk Management (TPRM)?
Third-Party Risk Management (TPRM) is the process of assessing and managing risks associated with external vendors, suppliers, or service providers that have a contractual or business relationship with an organization. These third parties may handle sensitive data such as Personally Identifiable Information (PII), Sensitive Personal Information (SPII), Protected Health Information (PHI), or Business Sensitive Information (BSI).

## 2. Importance of Third-Party Risk Management
Since businesses rely on multiple vendors for various services (e.g., cloud providers, HR management systems, IT infrastructure, etc.), it is crucial to evaluate and monitor these vendors to ensure they meet security, compliance, and operational standards. Failure to manage vendor risks can lead to security breaches, operational disruptions, and reputational damage.

### Examples of Third-Party Vendors and Services:
- **IT Services:** AWS for cloud hosting
- **HR Management:** Workday for payroll processing
- **Network Services:** Cisco for network infrastructure

## 3. Components of Third-Party Risk Management
The entire third-party risk management process is divided into two key components:

### A. Third-Party Due Diligence (TPDD)
- This process is performed before onboarding a new vendor.
- It involves a thorough review of the vendor’s security, financial health, reputation, and compliance with legal and regulatory standards.

### B. Third-Party Security Review (TPSR)
- This is an ongoing review process conducted periodically (e.g., annually).
- It ensures that vendors maintain security and compliance standards throughout the contract duration.

#### Example:
If Amazon wants to onboard a new vendor for payroll processing, the **TPDD process** will be performed before establishing contact with the vendor. Once onboarded, the vendor will undergo a **TPS Review (TPSR)** periodically.

## 4. Third-Party Risk Management Life Cycle (TPRM Life Cycle)
The TPRM process follows a structured life cycle with six key steps:

### Step 1: Screening & Vendor Selection
- The business identifies potential vendors.
- Top management evaluates and selects the vendor based on business needs and compliance requirements.

### Step 2: Risk Assessment
- A deep-dive assessment of the vendor is conducted.
- The evaluation includes security controls, data protection policies, and compliance with industry regulations.

### Step 3: Risk Mitigation
- Any risks identified during the assessment must be mitigated.
- Findings and remediation plans are documented and tracked.

### Step 4: Onboarding
- Once risks are addressed, the vendor is formally onboarded.
- Contractual agreements and security policies are established.

### Step 5: Continuous Monitoring
- The organization performs periodic security reviews (TPS Review).
- This includes evaluating changes in vendor operations, compliance status, and emerging risks.

### Step 6: Offboarding & Decommissioning
- When a vendor relationship ends, proper offboarding steps must be followed.
- Ensure secure data deletion, contract closure, and system decommissioning.

#### Example of Business Continuity Risk:
- **Indigo Airlines** relies on **Microsoft Cloud Services** for its operations.
- If Microsoft’s servers go down, Indigo’s business operations will be impacted.
- This highlights the need for **business continuity planning** with third-party vendors.

## 5. Data Flow & Data Classification in TPRM

### A. Understanding Vendor Data Flow
Before engaging a vendor, it is crucial to analyze how data flows between the organization and the vendor.

#### Example of Data Flow:
- Amazon uses **Workday** for payroll processing.
- A **Vendor Relationship Officer (VRO)** will define the data flow between Amazon and Workday.

### B. Data Transfer Mechanisms
Data is typically shared with vendors through:
- **Secure File Transfer Protocol (SFTP)**
- **Web Services / APIs**

### C. Data Classification Levels
Data shared with vendors is classified into different levels based on sensitivity:

| Classification | Data Type | Examples |
|---------------|------------|------------|
| **Public** | No sensitive data | Company website data, general reports |
| **Confidential** | Business-sensitive information | Employee names, internal business reports |
| **Restricted** | Any two or more sensitive data types | Employee salaries, internal strategy |
| **Highly Confidential** | Any single sensitive data type | Payment info, PHI, SPII, BSI |
| **Critical** | Extremely sensitive information | Full customer databases, financial records |

## 6. Vendor Tiering in Third-Party Risk Management
Vendors are categorized into different tiers based on the type of data they handle and their risk level.

| Tier | Description | Assessment Frequency |
|------|------------|----------------------|
| **Tier 1** | Handles payment-related information | Annual deep-dive review |
| **Tier 2** | Handles restricted information | Every 3 years |
| **Tier 3** | Handles confidential data | Light assessment |
| **Tier 4** | Handles non-sensitive public data | Minimal review |

### Vendor Risk Assessment Questionnaire
- Tier 1 and Tier 2 vendors undergo a **detailed questionnaire (200+ questions)** based on security frameworks such as **NIST 800-53 and CIS Top 14 Controls**.
- Tier 3 and Tier 4 vendors undergo a **lighter questionnaire (30 questions)**.

## 7. Audit & Compliance in TPRM

### A. Audit Process
1. **Kickoff Meeting:** TPRM team and Vendor Relationship Officer (VRO) initiate the audit.
2. **Evidence Gathering:** Vendor submits required documents.
3. **Assessment Review:** TPRM team verifies compliance with security policies.
4. **Findings Management:** If risks are identified, corrective actions are taken.

### B. Common Audit Issues
- Security controls not in place
- Vendor delays in providing evidence
- Compliance violations (e.g., data privacy breaches)

## 8. Finding Management in TPRM

### A. Common Risk Findings

| Risk Type | Example | Resolution |
|-----------|------------|------------|
| **Security Gap** | Multi-Factor Authentication (MFA) missing | Implement MFA within 6 months |
| **Policy Violation** | Vendor not following change management | Implement corrective actions |
| **Operational Risk** | Vendor does not meet service uptime SLAs | Improve infrastructure reliability |

### B. Exception Handling for Risk Mitigation
- **Option 1: Immediate Fix** (e.g., patch security vulnerability within 2 weeks)
- **Option 2: Risk Acceptance** (if mitigation takes longer, a temporary solution is agreed upon)

## 9. Tools Used for TPRM
Organizations use different tools to manage TPRM processes:

- **Manual:** Excel sheets
- **Automated Platforms:**
  - **OneTrust**
  - **VISAER**
  - **NIST 800-53 Framework**
  - **CIS Critical Security Controls**

## 10. Roles & Responsibilities in TPRM

| Role | Responsibility |
|------|--------------|
| **Vendor Relationship Officer (VRO)** | Acts as the main contact for vendor management |
| **Third-Party Security Team (TPS Team)** | Conducts risk assessments and security reviews |
| **Audit Team** | Performs audits, gathers evidence, and enforces compliance |
| **Finding Management Team** | Tracks risk findings and ensures mitigation |

## Conclusion
Effective **Third-Party Risk Management (TPRM)** ensures that vendors comply with security, privacy, and regulatory requirements. By implementing a structured TPRM life cycle, classifying vendor risks, and conducting regular audits, organizations can mitigate potential threats and ensure smooth business operations.
