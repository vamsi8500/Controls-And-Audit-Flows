## 🌥️ Why Cloud?

- **Scalability:** Cloud providers offer elastic resources that scale on demand.
- **Cost Efficiency:** Pay-as-you-go pricing avoids upfront infrastructure costs.
- **Agility:** Faster deployment and time-to-market for apps.
- **Resilience:** Built-in redundancy and disaster recovery options.
- **Global Reach:** Access from anywhere with multi-region support.

**Real-Time Example:** A startup hosts their app on AWS to avoid upfront hardware costs, scale globally, and focus on development.

---

## 🛡️ Shared Responsibility Model

| Layer                 | Cloud Provider Responsibility                | Customer Responsibility                           |
|----------------------|-----------------------------------------------|--------------------------------------------------|
| Physical Security    | Data center access, hardware                  | N/A                                              |
| Infrastructure       | Network, servers, storage                     | Configure securely                               |
| Virtualization Layer | Hypervisor, host OS                           | N/A                                              |
| OS & Applications    | -                                             | Patching, configuring, securing apps             |
| Data & Access        | -                                             | Access control, encryption, monitoring           |

**Example:** In AWS, AWS secures the physical data center, but you are responsible for securing EC2 instances and access to S3.

---

## ☁️ Cloud Deployment Models

1. **Public Cloud:** Shared infrastructure (e.g., AWS, Azure, GCP)
2. **Private Cloud:** Dedicated environment (e.g., VMware-based on-prem)
3. **Hybrid Cloud:** Mix of public + private (e.g., Azure Arc, AWS Outposts)
4. **Community Cloud:** Shared among organizations with similar needs (e.g., govt health depts)

---

## 📦 Cloud Service Models

| Model  | Provider Manages                   | Customer Manages                   | Example            |
|--------|------------------------------------|------------------------------------|--------------------|
| SaaS   | Everything (infra, apps, OS, etc.) | Data, user access, configs         | Google Workspace   |
| PaaS   | Infra + OS + runtime               | App code, data, access             | Azure App Service  |
| IaaS   | Infra (network, storage, VMs)      | OS, apps, data, access             | AWS EC2            |

---

## 🔐 General Cloud IT Security Controls

- **IAM:** Fine-grained access control
- **MFA:** Protects identity
- **Encryption (At rest & in transit):** Prevents unauthorized data access
- **Logging & Monitoring:** Detects threats
- **Security Groups/NACLs:** Controls network flow

---

## 🔧 Specific IT Controls for SaaS, PaaS, IaaS

_Refer to previous comprehensive table with real-time use cases._

---

## 🏢 IT Controls for On-Prem vs Cloud Hosting

| Area             | On-Prem                   | Cloud                                | Mitigation                      |
|------------------|----------------------------|---------------------------------------|----------------------------------|
| Access Control   | Local AD                   | IAM, MFA                              | Least privilege, periodic review |
| Network Security | Firewalls, VLAN            | Security Groups, VPC, NACL            | Segment networks, deny all by default |
| Asset Tracking   | Manual CMDB                | Cloud Config, tagging                 | Automate, enforce naming/tags    |
| Logging          | SIEM (Splunk)              | CloudTrail, CloudWatch                | Centralized logging               |
| Encryption       | Disk-based, DB native      | KMS, S3 Server-side, RDS encryption   | Enforce policies, audit keys     |

---

## 🏛️ Governance & Compliance During Migration

- **Change Control:** Git + CI/CD pipelines
- **Audit Logging:** CloudTrail, Azure Activity Logs
- **Identity Governance:** Temporary IAM roles
- **Tagging & Ownership:** Enforce using policies
- **Backup Governance:** Test backup/restore flows

---

## 🔐 IT Security Controls During Migration

**Pre-Migration:**
- Data classification (e.g., PHI, PII)
- Encrypt data before transfer
- Vulnerability scans (Nessus)

**During Migration:**
- Secure transfer (TLS, VPN)
- Least-privileged access
- Enable full activity logging

**Post-Migration:**
- Revalidate configurations
- Decommission on-prem assets
- Map cloud setup to ISO/SOC controls

---

## ⚠️ Third-Party Vendor Risks & Mitigations

| Risk                         | Example                                      | Mitigation                                    |
|------------------------------|----------------------------------------------|-----------------------------------------------|
| Lack of Transparency         | No SOC 2 report from cloud backup vendor     | Require certifications, due diligence         |
| Shared Responsibility Confusion | SaaS vendor unclear on data encryption role | Define SRM, RACI                              |
| Excessive Access             | Support team has admin access always         | Use break-glass access, monitor logs          |
| Insecure Transfers           | Vendor uses email or FTP                     | Require HTTPS/SFTP/VPN                        |
| No Exit Strategy             | No data return clause                        | Add SLA clauses for data access/ownership     |

---

## 🔥 Break Glass / Firecall Account

- **Use:** Emergency situations only
- **Controls:**
  - MFA
  - Store in secure vault (CyberArk)
  - Audit all access
  - Time-bound usage

**Example:** AWS account with CloudTrail logs, MFA, no access keys by default

---

## 🌐 Public vs Private Subnets

| Subnet Type | Description                                     | Security Practice                   |
|-------------|--------------------------------------------------|-------------------------------------|
| Public      | Has Internet Gateway route                      | Use SGs/NACLs, limit inbound IPs     |
| Private     | No direct internet access                        | Use NAT Gateway for egress          |

**Example:** 3-tier app with web in public, DB in private subnet.

---

## 📡 API Integrations in Cloud & Security Controls

| Control               | Purpose                      | Tool/Example                     |
|------------------------|-------------------------------|----------------------------------|
| AuthN/AuthZ            | Verify access                 | OAuth, API keys, JWT             |
| Rate Limiting          | Prevent DoS abuse             | API Gateway throttle settings    |
| Input Validation       | Prevent injection             | OWASP best practices             |
| WAF                    | Block malicious traffic       | AWS WAF, Azure Front Door        |
| Logging & Monitoring   | Track misuse                  | CloudWatch, API Gateway logs     |
| TLS Everywhere         | Secure in transit             | HTTPS enforced                   |

---

## 🗂️ How to Secure Logs from Modification/Deletion

| Control                        | Method/Tool                            | Benefit                            |
|-------------------------------|----------------------------------------|-------------------------------------|
| WORM Storage                  | S3 Object Lock (Compliance Mode)       | Prevents tampering                  |
| Centralized Logging           | SIEM, CloudWatch, ELK Stack            | Better analysis & visibility        |
| IAM Restrictions              | Block delete on logs                   | Prevents accidental/mod access      |
| Cryptographic Hashing         | SHA256, Tripwire                       | Detects unauthorized changes        |
| Audit Log Access              | CloudTrail                             | Tracks log viewing/modification     |
| Retention Policies            | S3 lifecycle, SIEM archive             | Prevents premature deletion         |

---

## ✅ TPRM: Third-Party Risk Management

### General TPRM Process:
- Vendor onboarding request
- Risk-based tiering (low, med, high)
- Security questionnaire
- Review certifications (SOC 2, ISO 27001)
- Contractual controls
- Periodic reassessments

### TPRM Cycle:
1. **Identify** vendors
2. **Assess** risks
3. **Mitigate** with controls
4. **Monitor** ongoing security posture

---

## 🏛️ ISO 27001 Clauses (Relevant Ones)

- A.6: Organization of information security  
- A.9: Access control  
- A.12: Operations security (logging, malware protection)  
- A.15: Supplier relationships  
- A.16: Incident management  

---

## 🔁 SDLC in Secure Cloud Context

| Phase         | Security Activity                      |
|---------------|------------------------------------------|
| Requirements  | Define compliance needs (HIPAA, GDPR)   |
| Design        | Threat modeling                         |
| Develop       | SAST/DAST scans, secrets scanning       |
| Test          | Security testing, fuzzing               |
| Deploy        | CI/CD with security gates               |
| Maintain      | Patch management, logging, alerting     |

---

## ✅ SOC 2 Type 2 (Trust Service Criteria)

- Security  
- Availability  
- Processing Integrity  
- Confidentiality  
- Privacy  

**Real-Time:** Review CSP’s SOC 2 report for controls over change mgmt, access, etc.

---

## 🏥 HIPAA Compliance (Healthcare)

- **Safeguards:** Physical, technical, administrative  
- **Key Needs:** Access control, encryption, audit trails  
- **Example:** AWS supports HIPAA-eligible services; use BAA, encrypt PHI  

---

## 🔐 Cryptography

| Type        | Description                     | Use Case                            |
|-------------|----------------------------------|--------------------------------------|
| Symmetric   | Same key for encryption/decrypt | S3 Server-Side Encryption            |
| Asymmetric  | Public/private key pair         | TLS, email encryption, SSH access    |

---

## ⚖️ Regulations vs Standards

| Regulations         | Standards             |
|----------------------|------------------------|
| Legally enforced     | Voluntary/adopted best practices |
| HIPAA, GDPR          | ISO 27001, NIST       |

---

## 📘 AWS Logs: Types

- **CloudTrail:** API activity  
- **CloudWatch:** App & infra logs  
- **VPC Flow Logs:** Network traffic  
- **S3 Access Logs:** Bucket access  
- **ELB Logs:** Load balancer requests  

---

## 🌐 NAT Gateway vs Internet Gateway

| Feature           | NAT Gateway                    | Internet Gateway               |
|-------------------|----------------------------------|--------------------------------|
| Internet Access   | Outbound only (private subnet) | Bi-directional (public subnet) |
| Use Case          | DBs, app servers                | Web servers, public APIs       |
| Direction Control | Egress only                     | Egress + Ingress               |

**Example:** Private subnet uses NAT Gateway to reach patch repos. Public subnet connects via IGW for internet-facing APIs.
