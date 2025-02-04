# Encryption (Cryptography) – Control Domain Audit Flow

This audit ensures encryption controls are effectively implemented to protect data-at-rest and data-in-transit. It follows a structured approach involving control owner identification, governance inquiry, walkthrough testing, and evidence gathering.

## Step 1: Identify the Control Owner via Kickoff Meetings
### Objective: Determine the responsible person (Control Owner) for encryption-related controls.

- Conduct kickoff meetings with key stakeholders.
- Identify the Control Owner (CO) responsible for encryption governance.
- Document the **Name, Designation, and Timestamp** of the meeting.

## Step 2: Inquiry – Process Related to Governance Control
### Objective: Understand encryption governance procedures, tools, and compliance requirements.

### Inquiry with the Control Owner (CO)
- **CO Name, Designation, and Timestamp** recorded.
- Discuss encryption-related **procedures, policies, and approvals** for tools in use.

### Governance & Approved Procedures
- Identify encryption policies: **Approved for Use** vs. **Not Approved for Use**.
- Verify **Key Management System (KMS) Procedures**:
  - **Encryption tools**: Azure Key Vault, AWS KMS.
  - **Key inventory management**, key rotation frequency, and access control.

## Step 3: Walkthrough – Testing, Sampling, and Evidence Gathering
### Objective: Perform an in-depth evaluation of encryption controls through testing and evidence collection.

### A. Data-at-Rest Encryption Audit
#### Scope: Secure storage of data on endpoints, backups, and cloud environments.

#### Endpoints & Backup Security
- Verify **disk-level encryption** on endpoints (laptops, servers).
- Confirm usage of **BitLocker (Windows) for disk encryption**.

#### Cloud Encryption
- Check encryption standards in cloud storage (AWS, Azure).
- Verify **Amazon EBS encryption** is enabled for AWS storage.

#### Encryption Algorithm Compliance
- Confirm the use of **AES-256 or higher** for encryption.

### B. Data-in-Transit Encryption Audit
#### Scope: Secure data transmission across applications, networks, and communication channels.

#### Security Protocols Verification
- Validate encryption protocols used in applications and networks:
  - **HTTPS** (for secure web traffic).
  - **SMTPS** (for encrypted email communication).
  - **SSH** (for secure remote access).

#### Certificate Compliance
- Verify **TLS Certificates** are in place.
- Ensure **TLS v1.2 or above** is enforced.

#### Digital Signature & Encryption Strength
- Validate the use of **RSASSA-PSS** digital signature algorithm.
- Ensure **RSA 2048-bit keys or larger** are used.
- Conduct **SSL Labs testing** to confirm security configurations.

### C. Key Management System (KMS) & Access Control Audit
#### Scope: Evaluate key security, access management, and logging mechanisms.

#### Key Inventory & Rotation Compliance
- Verify that **key registers** are maintained.
- Check **key rotation frequency** and policy compliance.

#### Access Management Review
- Assess **KMS procedures** for managing encryption keys (Azure Key Vault, AWS KMS).
- Ensure key access is restricted using **VPN access** and role-based access control (RBAC).

#### Logging & Monitoring
- Check if encryption key activities are **logged**.
- Validate **audit logs** to ensure accountability.
- Perform **Over-the-Shoulder Testing** to verify monitoring practices.

## Step 4: Evidence Collection & Compliance Assessment (C&A)
### Objective: Gather and validate evidence to confirm encryption control effectiveness.

### Collect Encryption Logs & Reports
- Endpoint encryption logs (BitLocker, AWS EBS).
- TLS/SSL certificate reports.
- KMS access logs.

### Sampling & Testing
- Randomly test encryption implementation on different systems.
- Conduct **evidence-based verification** for compliance.

### Compliance Reporting
- Document findings, risks, and gaps in encryption control.
- Recommend **corrective actions** if non-compliance is found.
