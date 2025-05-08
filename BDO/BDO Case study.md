# Cybersecurity and Third-Party Risk Management (TPRM) Scenarios

## 1. Risk
**Definition**: A risk in cybersecurity is the potential for an adverse event resulting from the exploitation of a vulnerability by a threat actor, causing damage, disruption, or data loss.

> **Formula**: Risk = Threat × Vulnerability × Impact

**Scenario**:
A law firm allows remote access via outdated VPN software.
- A cybercriminal scans internet-facing systems and identifies the VPN version with known CVEs.
- The VPN lacks multi-factor authentication (MFA), making it easier to brute-force credentials.
- **Result**: The attacker gains access to sensitive client files, leading to a data breach.
- **Risk Mitigation**: VPN patched; MFA enforced; access logs monitored; internal security training conducted.

---

## 2. Risk, Threat, Vulnerability
**Definition**:
- **Threat**: Potential cause of an unwanted incident (e.g., hacker).
- **Vulnerability**: Weakness that can be exploited (e.g., weak passwords).
- **Risk**: Potential damage if a threat exploits a vulnerability.

**Scenario**:
An investment firm uses an outdated FTP server to share financial data.
- **Threat**: A malicious actor intercepting data during transfer.
- **Vulnerability**: FTP transmits data in plaintext, and the system is unpatched for a known exploit.
- **Risk**: Leakage of investor bank details, resulting in reputational damage, legal penalties, and client churn.
- **Controls Implemented**: Migrated to SFTP, enforced encryption, added file integrity checks, and trained staff on secure file handling.

---

## 3. New Onboarding Vendor
**Definition**: TPRM requires due diligence on vendors who handle sensitive data, including security assessments, contract clauses, and SLA reviews.

**Scenario**:
A digital lending platform wants to onboard a SaaS vendor to handle loan application processing.
- **Due Diligence**: Security questionnaire, SOC 2 Type II report, and privacy policy review.
- **Findings**: The vendor did not use encryption-at-rest and hosted data in a country with poor data protection laws.
- **Mitigation**: Requested data localization, contractual encryption, breach notification clauses, and periodic audits.
- **Outcome**: The vendor remediated issues; onboarding proceeded with monthly monitoring and quarterly risk assessments.

---

## 4. BCP, RTO, RPO
**Definition**:
- **BCP (Business Continuity Plan)**: Strategy to continue operations during disruptions.
- **RTO (Recovery Time Objective)**: Max acceptable time to restore service.
- **RPO (Recovery Point Objective)**: Max acceptable data loss in terms of time.

**Scenario**:
An eCommerce firm suffers a ransomware attack that encrypts its primary cloud storage during a holiday sale.
- **BCP Triggered**: Traffic rerouted to backup site using cloud failover.
- **RTO** was 1 hour; the platform was back online in 90 minutes.
- **RPO** was 15 minutes; 30 minutes of sales data were lost.
- **Improvements Made**: Real-time data replication, enhanced offsite backups, ransomware drills.

---

## 5. Types of Encryption
**Definition**:
- **Symmetric**: Same key for encryption/decryption (AES).
- **Asymmetric**: Public/private key pair (RSA).
- **Hashing**: One-way data fingerprinting (SHA-256).
- **Homomorphic**: Operate on encrypted data.
- **E2EE**: Encrypt at sender, decrypt at receiver (e.g., WhatsApp).

**Scenario**:
A payroll SaaS app uses AES-256 symmetric encryption for employee data but stores keys in a flat config file on the same server.
- **Risk**: If the server is compromised, both data and keys are stolen.
- **Fixes**: Moved keys to HSM, implemented envelope encryption, added asymmetric encryption for key exchange, used hashing for sensitive fields, and tokenization for bank account numbers.

---

## 6. User-Based Access Application
**Definition**: Access control should follow the principles of Least Privilege and Role-Based Access Control (RBAC).

**Scenario**:
A healthcare provider builds an internal portal for EHR management with role-based access for Admins, Doctors, Nurses, and Clerks.
- **Issue**: Misconfiguration grants a nurse admin-level access.
- **Impact**: Unintentional changes to medication records; medical liability risk.
- **Post-Incident Action**: Identity governance, access workflows, periodic access recertification, session recording, behavior monitoring for privileged users.

---

## 7. Principles of Information Security
**Definition**:
- **Confidentiality**: Prevent unauthorized access.
- **Integrity**: Protect data from unauthorized modification.
- **Availability**: Ensure systems/data are accessible.
- **Authentication**: Confirm identity.
- **Authorization**: Define access levels.
- **Non-repudiation**: Prevent denial of actions.
- **Accountability**: Enable auditability.

**Scenario**:
A bank deploys a mobile app update without rigorous QA.
- **Impact**: Customers unable to make transactions for 3 hours.
- **Issue**: Change control processes were bypassed.
- **Security Result**: Availability was compromised.
- **Actions Taken**: Secure SDLC enforcement, rollback plans, feature toggles, monitoring, CAB approvals introduced.

---

## 8. Domains of TPRM
**Definition**:
Refers to various functional areas covered in Third-Party Risk Management, including:
- Governance
- Contract Management
- Risk Assessment
- Security & Privacy Review
- Performance Monitoring
- Issue & Exception Management
- Termination Procedures

> Ensure each domain is covered during TPRM lifecycle phases and vendor interactions.
