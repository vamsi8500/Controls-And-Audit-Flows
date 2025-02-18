# Vendor Onboarding and Offboarding Process in Third-Party Risk Management (TPRM)

Managing third-party vendors effectively is crucial for organizations, as improper onboarding and offboarding can lead to data privacy risks, compliance violations, and operational inefficiencies. This document outlines a structured approach to onboarding and offboarding vendors, including key steps, stakeholders, and best practices.

## Vendor Onboarding Process

### Scenario: Amazon Onboarding a Payroll Vendor
Amazon wants to onboard a new payroll vendor that will be integrated into their Workday payroll system. This involves multiple steps, including vetting, risk assessments, data flow design, and compliance checks.

### Key Steps in Vendor Onboarding

#### Vendor Request and Pre-Screening
- Business heads request a new vendor.
- The Third-Party Due Diligence (TPDD) Team conducts initial screening to check if the vendor meets organizational standards.
- Business justification is reviewed to ensure the vendor is necessary.

#### Third-Party Due Diligence (TPDD)
- Before reaching out to the vendor, the TPDD team performs due diligence.
- Ensures the vendor meets regulatory and compliance requirements.
- TPDD works with respective departments to confirm vendor requirements.

#### Registration and Use Case Documentation
- The vendor registers within the organization’s procurement system.
- The Vendor Relationship Officer (VRO) registers the vendor's use case.
- Business teams (e.g., HR, Payroll) document their requirements.

#### Data Flow Design and Security Assessment
- The Vendor Risk Officer (VRO) and Third-Party Security (TPS) Team design a data flow diagram.
- Ensures secure data exchange between Amazon and the vendor.
- Identifies data classification (e.g., PII, SPI, PHI, BSI).
- Determines data-sharing mechanisms:
  - Secure File Transfer Protocol (SFTP)
  - Web Services / APIs

#### Data Classification and Compliance Checks
- Determines data sensitivity:
  - **Public Data** – No classification needed.
  - **Non-Public Data** – Requires classification per Data Classification Policy.
- **Data Elements Checked:**
  - **PII (Personally Identifiable Information)** – Name, address, SSN.
  - **SPI (Sensitive Personal Information)** – Payroll details, banking info.
  - **PHI (Protected Health Information)** – Healthcare data.
  - **Confidential Data** – Internal company documents.

#### Vendor Tiering and Risk Assessment
- Vendors are categorized into risk tiers based on data sensitivity and security risk:
  - **Tier 1 (Critical Vendors)** – Handle sensitive payment data.
  - **Tier 2 (Restricted Vendors)** – Handle financial data but lower risk.
  - **Tier 3 (Limited Vendors)** – Handle low-risk confidential data.
  - **Tier 4 (Public Vendors)** – Minimal risk, publicly available data.

#### Contracting and Compliance Approval
- Contracts are reviewed by legal and compliance teams.
- Security assessments performed using:
  - **NIST 800-53**
  - **CIS Critical Security Controls**
  - **OneTrust / VISER**
- Final Approval by Vendor Relationship Officer (VRO).

#### Vendor System Integration and Testing
- Secure data access is granted.
- Vendor systems are integrated with Workday payroll.
- End-to-end testing ensures smooth functionality.

#### Ongoing Monitoring and Risk Management
- Continuous monitoring of vendor activities.
- Annual security audits for Tier 1 & 2 vendors.
- Findings Management Process ensures risk mitigation.

## Vendor Offboarding Process
When a vendor is no longer required, proper offboarding is necessary to avoid data security risks.

### Key Steps in Vendor Offboarding

#### Vendor Decommissioning Request
- Business team submits a request to offboard the vendor.
- VRO and TPS team review the request.

#### Contract Review and Termination
- Legal team reviews contract obligations.
- Ensure exit clauses are followed.
- Vendor is notified about contract termination.

#### System Access Deactivation
- Vendor access to organizational systems is revoked.
- API keys, SFTP credentials, and user accounts are disabled.

#### Data Retention and Deletion
- Data retention policies are followed.
- Sensitive data shared with the vendor is retrieved or securely deleted.

#### Security Audit and Compliance Check
- A final security audit ensures all vendor-related data has been removed.
- The VRO certifies that offboarding is complete.

#### Final Documentation and Closure
- All offboarding steps are documented.
- Vendor is removed from active vendor lists.

### Example: Payroll Vendor Offboarding Scenario
1. Amazon decides to stop using Vendor X for payroll.
2. HR submits an offboarding request to the VRO.
3. VRO and legal team review contract termination requirements.
4. Access to Workday and other systems is revoked.
5. **Data cleanup process begins:**
   - Sensitive payroll data is securely deleted.
   - All shared files are removed from Amazon servers.
6. Final security audit is conducted.
7. Vendor is officially decommissioned from the system.

## Key Takeaways
- Onboarding and offboarding vendors require strict controls to mitigate risks.
- Vendor risk tiering helps prioritize security efforts.
- Proper data classification ensures compliance with regulations.
- Findings management tracks security issues and ensures timely resolution.
- Regular audits and monitoring keep vendor risks under control.

# Vendor Onboarding and Offboarding Flow

## Vendor Onboarding Flow

Start  
↓  
Amazon Business Team requests a new vendor  
↓  
Vendor Relationship Officer (VRO) reviews the request  
↓  
Third-Party Security (TPS) Team conducts risk assessment  
↓  
**Decision: Vendor approved?**  
→ **No:** Reject vendor & notify business team → End  
→ **Yes:** Proceed to next step  
↓  
Vendor registered in system & integrated with Workday Payroll  
↓  
**Data Classification Check**  
↓  
**Decision: What type of data is shared with the vendor?**  
→ **Public:** No special restrictions → Proceed  
→ **Confidential:** Data protection policies apply → Proceed  
→ **Critical (PII, PHI, SPI, BSI):** Additional security & compliance checks  
↓  
**Decision: Secure Data Sharing Mechanism?**  
→ **SFTP:** Secure File Transfer Protocol  
→ **API:** Web Services  
→ **Other:** Secure Transfer Methods  
↓  
Vendor is active and processing payroll transactions  
↓  
Ongoing monitoring & security audits  
↓  
End  

## Vendor Offboarding Flow

Start  
↓  
Amazon Business Team requests vendor removal  
↓  
VRO reviews & approves deactivation  
↓  
Vendor access to Workday Payroll is revoked  
↓  
**Data Classification Check**  
↓  
**Decision: What type of data was shared?**  
→ **Public:** No special actions needed → Proceed  
→ **Confidential:** Ensure proper deletion or retention  
→ **Critical (PII, PHI, SPI, BSI):** Special deletion process & compliance audit  
↓  
**Decision: Secure Data Removal?**  
→ **Encrypt & Archive:** If needed for compliance  
→ **Complete Deletion:** If required by policy  
↓  
Final security audit & compliance check  
↓  
Vendor completely decommissioned  
↓  
End  

## Key Data Classifications Used in the Flowchart
- **Public Data:** Available to everyone, no restrictions.  
- **Confidential Data:** Requires controlled access, e.g., internal company documents.  
- **Critical Data (PII, PHI, SPI, BSI):** Highly sensitive, subject to strict security measures.  

