# ✅ Real-Time Use of Controls & How They Secure Data

## 🌐 1. SaaS (Software as a Service)

**Customer Responsibility:** User access, data input/output, basic configurations, audit reviews  
**Examples:** Salesforce, Google Workspace, Office 365

| Control                       | Real-Time Use Case                                            | How It Secures Data                                                   |
|------------------------------|----------------------------------------------------------------|------------------------------------------------------------------------|
| Multi-Factor Authentication (MFA) | You enable MFA on Office 365 accounts                         | Prevents unauthorized access to user accounts even if passwords are stolen |
| Role-Based Access Control (RBAC) | In Salesforce, only HR users can access employee data         | Limits exposure of sensitive data to only authorized roles            |
| Encryption at Rest and Transit   | Google Workspace encrypts docs stored in Drive (AES-256) and uses HTTPS for transit | Protects data from being read during transmission or storage compromise |
| Activity Logs / Audit Trails     | Admins review login anomalies on the SaaS admin console       | Detects account misuse, enables incident response                     |
| Vendor Certifications (SOC 2, ISO 27001) | You verify the provider complies with data security standards | Ensures they follow security best practices for storing your data     |

---

## 🧱 2. PaaS (Platform as a Service)

**Customer Responsibility:** Application code, configurations, API security, data handling  
**Examples:** AWS Elastic Beanstalk, Google App Engine, Azure App Service

| Control                       | Real-Time Use Case                                               | How It Secures Data                                                  |
|------------------------------|------------------------------------------------------------------|----------------------------------------------------------------------|
| Secure Coding Practices (SAST/DAST) | Use GitHub Actions to scan for SQL injection in app code       | Prevents injection attacks that can leak or modify sensitive DB data |
| API Gateway + WAF               | Deploy Azure API Management with WAF to protect public APIs     | Blocks malicious traffic (DDoS, XSS, SQLi), filters IPs              |
| Key Vaults for Secrets          | Use AWS Secrets Manager to store DB passwords                   | Prevents credential leakage in source code/config files              |
| Environment Isolation           | Deploy production and dev apps in separate App Engine projects | Reduces risk of dev/test bugs impacting real data                    |
| Application Logs + Monitoring   | Use Application Insights or Stackdriver to monitor app behavior | Detects misuse, failed logins, or data leaks in real-time            |

---

## 🏗️ 3. IaaS (Infrastructure as a Service)

**Customer Responsibility:** Everything except the physical infrastructure  
**Examples:** AWS EC2, Azure VMs, Google Compute Engine

| Control                       | Real-Time Use Case                                              | How It Secures Data                                                  |
|------------------------------|------------------------------------------------------------------|----------------------------------------------------------------------|
| Disk Encryption (EBS, Azure Disk) | Enable encryption for EC2 EBS volumes storing customer data   | Protects data if the disk or snapshot is copied or stolen           |
| VPC with Subnet Segmentation     | Place database server in private subnet; web server in public subnet | Prevents direct internet access to sensitive backend systems    |
| IAM with Least Privilege         | Developers only have read-only access to production S3 bucket | Limits accidental or malicious data deletion                        |
| Security Groups + NACLs          | Allow only port 443 from trusted IPs; deny all others         | Blocks unauthorized network traffic from reaching sensitive instances |
| SIEM & CloudTrail                | Log EC2 start/stop events, detect unauthorized instance creation | Helps detect and respond to insider threats or compromise         |
| Patch Management (Ansible, AWS SSM) | Automate weekly OS patching for EC2 using SSM               | Reduces risk from known software vulnerabilities                   |

---

## 🔐 How These Controls Protect Data End-to-End

| Data Lifecycle Phase | Relevant Controls                                 | Security Benefit                                       |
|----------------------|---------------------------------------------------|--------------------------------------------------------|
| Data in Transit      | TLS/SSL, API Gateways, VPN                        | Prevents data sniffing or MITM attacks                |
| Data at Rest         | Encryption, Backup, Disk Encryption, Key Management | Prevents data theft from storage compromise          |
| Data in Use          | Role-based access, App security, IAM policies     | Ensures only authorized processes/people access data  |
| Data Access/Logs     | Logging, Monitoring, Alerts                       | Detect and investigate suspicious access              |
| Data Recovery        | Automated Backups, Snapshots, DR                  | Ensures availability and restoration during incidents |

---

## ✅ 1. IT Controls to Test – On-Prem vs Cloud Hosting

| Area              | On-Prem Control                  | Cloud Control                         | Risk                              | Mitigation                                   |
|------------------|----------------------------------|----------------------------------------|-----------------------------------|----------------------------------------------|
| Access Management| Local AD, physical access control| IAM (AWS IAM, Azure RBAC), MFA         | Unauthorized access               | Apply least privilege, enforce MFA           |
| Network Security | Firewalls, VLANs                 | Security Groups, NACLs, VPC/Subnets    | Exposure of services to public    | Use private subnets, restrict IP ranges      |
| Asset Inventory  | Manual CMDB updates              | Auto-discovery via Cloud Config, AWS Config | Asset mismanagement              | Automate inventory updates, tag resources    |
| Logging          | Local SIEM (Splunk)              | CloudTrail, CloudWatch, Azure Monitor  | Missed logs or log tampering      | Centralize logs, enable immutability         |
| Encryption       | Disk-level (BitLocker), DB encryption | KMS-based Encryption (EBS, S3, RDS) | Data leak or theft                | Enforce encryption at rest and transit using KMS |

---

## 🔄 2. Governance and Compliance During Migration

### ⚙️ Real-Time Governance Controls

| Governance Area        | Control                                | Real-Time Example                             | Risk if Missing               | Mitigation                                   |
|------------------------|----------------------------------------|------------------------------------------------|-------------------------------|----------------------------------------------|
| Change Management      | Approval workflow                      | Use Jira + GitOps for infra changes            | Unauthorized deployments      | Use CI/CD with manual approvals              |
| Audit & Compliance     | Audit trails, change logs              | Enable CloudTrail, Config Rules, Azure Policy  | Lack of traceability          | Review logs weekly, implement alerts         |
| Resource Tagging       | Tag resources                          | E.g., Environment=Prod, Owner=IT               | Cost overrun                  | Enforce via service control policies         |
| Identity Governance    | IAM reviews, temporary access          | Review AWS IAM access quarterly                | Over-permissioned users       | Use IAM Access Analyzer, revoke unused roles |
| Backup & Recovery      | DR planning, BCP testing               | Schedule AWS Backup, test recovery quarterly   | Data loss or downtime         | Regular restore testing & automation         |

---

## 🔐 3. IT Security Controls During Migration

### 🚀 Pre-Migration Security Activities

| Activity                  | Control                        | Example                            |
|---------------------------|--------------------------------|------------------------------------|
| Data Classification       | Tag sensitive data             | Classify PHI, PII, financial records |
| Data Encryption           | AES-256 encryption             | Use pre-signed encrypted S3 URLs  |
| Baseline Assessment       | Vulnerability scans, risk rating| Use Nessus, Qualys on on-prem assets|

### 🏃 During Migration

| Activity           | Control              | Example                                          |
|--------------------|----------------------|--------------------------------------------------|
| Secure Transmission| TLS, IPsec VPN       | Encrypt via AWS Direct Connect or VPN            |
| IAM Segregation    | Role-based permissions| Migration team gets limited-time access only     |
| Activity Logging   | CloudTrail, VPC Logs | Capture infra & data changes during migration    |

### 🔁 Post-Migration

| Control                 | Real-Time Use                  | How It Helps                                  |
|-------------------------|-------------------------------|-----------------------------------------------|
| Decommission On-Prem    | Wipe and retire old servers   | Prevent dual write paths or outdated access   |
| Revalidate Security     | Re-run vulnerability scans    | Catch config drift or cloud weaknesses        |
| Compliance Mapping      | Check setup vs ISO/SOC controls | Meet regulatory & audit needs                 |

---

## 🤝 4. Challenges with Third-Party Vendors During Cloud Migration

| Vendor Challenge              | Real-Time Example                          | Risk                        | Mitigation Strategy                                   |
|------------------------------|--------------------------------------------|-----------------------------|-------------------------------------------------------|
| Lack of visibility           | Backup vendor won’t share SOC 2 reports    | Non-compliance, data leak   | Request TPRM, require ISO/SOC reports                 |
| Shared responsibility confusion| Vendor says encryption is your job       | Security gaps               | Use SRM diagrams, define RACI                         |
| Access Over-provisioning     | Vendor has permanent admin rights          | Insider threats             | Use break-glass accounts, log access, JIT            |
| Unsecured data transfers     | Vendor uses unsecured FTP                  | Data interception           | Enforce HTTPS, SFTP, VPN                              |
| No exit strategy/SLA         | No guarantee of data access post-contract  | Lock-in or data loss        | Include SLAs for data ownership/export                |

---

## 🔓 Break-Glass (Firecall) Account

| Control              | Description                             | How It Helps                                 |
|----------------------|-----------------------------------------|----------------------------------------------|
| MFA                  | Mandatory                               | Prevents misuse even if creds are leaked     |
| Vaulted Storage      | Secure vault (CyberArk, Vault)          | Prevents unauthorized access                 |
| Time-bound Access    | Limited-time access                     | Reduces misuse                               |
| Audit Logging        | Logs all usage                          | Ensures accountability                       |
| No Daily Use         | Reserved only for emergencies           | Avoids privilege abuse                       |

---

## 🌐 Public vs Private Subnets on Cloud

| Type           | Use Cases             | Security Control                          |
|----------------|-----------------------|--------------------------------------------|
| Public Subnet  | Web server, bastion   | Use Security Groups, NACLs                 |
| Private Subnet | DB, app backend       | No Internet Gateway, use NAT               |

**Real-Time Use Case:**  
In AWS 3-tier architecture:
- Web in public
- App and DB in private
- DB subnet has no internet access

---

## 🔗 API Integrations & Security Controls

| Control                 | Purpose                          | Tool/Example                    |
|-------------------------|----------------------------------|----------------------------------|
| Auth & Authorization    | Validate identity                | OAuth 2.0, JWT, API keys         |
| Rate Limiting           | Prevent DoS/Abuse                | AWS API Gateway throttling       |
| Input Validation        | Block injections                 | OWASP API Sec #8                 |
| Logging & Monitoring    | Track & alert                    | CloudWatch, API Gateway Logs     |
| TLS Encryption          | Secure transit                   | HTTPS                            |
| Schema Validation       | Enforce proper requests          | Swagger, OpenAPI                 |
| WAF + Gateway           | Filter bad traffic               | AWS WAF, Azure Front Door        |

---

## 📂 How to Secure Logs from Modification/Deletion

| Control                  | How It Works                            | Example/Tool                       |
|--------------------------|------------------------------------------|------------------------------------|
| Write Once, Read Many    | Prevent delete/edit                      | S3 Object Lock                     |
| Centralized Logging      | Access control, alerting                 | ELK, CloudWatch                    |
| IAM Restrictions         | Limit delete/view                        | No delete in prod roles            |
| Log Hashing              | Integrity check                          | SHA256, Tripwire                   |
| Audit Logging            | Log who accessed what                    | CloudTrail                         |
| Retention Policies       | Auto-archive, prevent deletion           | S3 Lifecycle                       |
| Separation of Duties     | Admin ≠ Log auditor                      | Dedicated monitoring roles         |

**Real-Time:**  
- Logs in S3 with Object Lock  
- Read-only to audit team  
- CloudTrail + Splunk alerts for tampering  

---

## ✅ Summary Table

| Topic              | Key Takeaway                                                  |
|--------------------|----------------------------------------------------------------|
| Break Glass Account| Emergency-use only, highly controlled & audited                |
| Subnet Strategy    | Public for internet-facing; private for internal use           |
| API Security       | Use OAuth, WAF, rate limits, logging, validation               |
| Log Protection     | WORM storage, restrict IAM, hash logs, centralize, monitor     |
