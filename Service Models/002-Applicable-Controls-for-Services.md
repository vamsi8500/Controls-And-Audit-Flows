# Cloud Service Models and Applicable Security Controls

Cloud computing service models require different security controls to ensure compliance, data protection, and operational efficiency. Below is a detailed breakdown of the applicable security controls for Software-as-a-Service (SaaS), Infrastructure-as-a-Service (IaaS), and Network Security Controls across different cloud environments.

## 1. Software-as-a-Service (SaaS)
### Definition:
SaaS provides users with software applications over the internet. The cloud provider manages all aspects of the software, including infrastructure, security, updates, and maintenance.

### Applicable Security Controls:
#### Application-Level Controls:
Application security is crucial for protecting user data, transactions, and software functionality from vulnerabilities and attacks.

**Secure Development Lifecycle (SDLC):**
- The security of an application starts from the design phase and continues through development, testing, deployment, and maintenance.
- Organizations must implement secure coding practices to prevent vulnerabilities such as SQL injection, cross-site scripting (XSS), and remote code execution (RCE).
- Security guidelines should align with frameworks like OWASP Top 10 and NIST Cybersecurity Framework.
- **Key Practices:**
  - Conducting threat modeling during software design.
  - Following secure coding guidelines for programming languages used.
  - Implementing automated security testing in CI/CD pipelines.

**Vulnerability Assessment and Penetration Testing (VAPT):**
- **Vulnerability assessment:** Automated scanning of applications to identify security weaknesses.
- **Penetration testing:** Ethical hacking techniques (black-box, white-box, grey-box testing) to simulate cyberattacks and find exploitable vulnerabilities.
- **Regular Testing Cycle:**
  - **Black Box Testing:** Simulates an external attack without insider knowledge.
  - **White Box Testing:** Tests with full knowledge of the system architecture and source code.
  - **Grey Box Testing:** Partial knowledge of the system with simulated internal access.
- Fixes must be implemented before application release to meet **Regulatory Assurance Framework (RAF).**

**Cryptography:**
- **Database Security (Data at Rest):**
  - Use AES-256 encryption to protect sensitive data stored in databases.
  - Enforce secure key management practices using cloud services like AWS KMS, Azure Key Vault, or HashiCorp Vault.
- **Application Security (Data in Transit):**
  - Enforce TLS 1.2 and above for encrypting data transmitted over networks.
  - Implement HTTPS and digital certificates to protect web communications.
  - Periodic SSL/TLS configuration reviews using SSL Labs to identify weak ciphers or misconfigurations.

**Change Management:**
- Any software updates, patches, or application modifications must follow a formal Change Management Process.
- Change logs should be documented, reviewed, and approved before deployment.

**Backup Management:**
- Ensure regular backups of SaaS applications and their configurations.
- Backups should be encrypted and stored in secure locations (on-prem/off-site cloud).
- Backup retention policies must comply with company and regulatory requirements.

**Access Management:**
- **Multi-Factor Authentication (MFA)** should be enabled for user authentication.
- **Single Sign-On (SSO)** integration with Identity and Access Management (IAM) solutions such as Okta, Azure AD, Google Identity Platform.

**Capacity Management:**
- Monitor and scale SaaS resources dynamically based on real-time demand.
- Key metrics include HTTP request rate, active users, and application server performance to prevent downtime or performance degradation.

---

## 2. Infrastructure-as-a-Service (IaaS)
### Definition:
IaaS provides virtualized computing resources (servers, networking, and storage) over the cloud. Organizations are responsible for managing applications, data, and security within their IaaS environment.

### Applicable Security Controls:
#### Infrastructure/Server/Endpoint Controls:

**Physical Security Controls:**
- Data center access should be restricted using **Two-Factor Authentication (2FA).**
- Implement biometric security and surveillance for physical security compliance (ISO 27001).

**Backup Management:**
- Automated snapshots and backups should be taken for IaaS virtual machines (VMs).
- Off-site storage of backups ensures **disaster recovery readiness.**

**Asset Management:**
- Maintain an inventory of cloud servers, storage devices, and networking hardware.
- Apply **disposal policies** when decommissioning old cloud resources.

**Logical Access Management:**
- Enforce **MFA for administrator and user logins** to virtual machines (VMs).
- Use **role-based access control (RBAC)** to limit unnecessary privileges.

**Removable Media Security:**
- Block unauthorized **USB drives, external hard disks, and removable media** using endpoint security tools such as **JAMF for Mac environments.**

**Antivirus and Endpoint Protection:**
- Deploy **antivirus solutions** on cloud instances to detect malware and unauthorized applications.
- Schedule periodic **security scans and patches** for IaaS servers.

---

## 3. Network Security Controls (Applicable to SaaS, PaaS, and IaaS environments)

Network security controls apply across cloud environments to prevent unauthorized access, data breaches, and cyber threats.

### Applicable Security Controls:

**Logical Access Controls:**
- Enforce **MFA for VPN and cloud-based access.**
- Integrate **Active Directory (AD) with cloud IAM** to manage authentication securely.

**Firewall Security:**
- Conduct **quarterly firewall rule reviews** to identify misconfigurations.
- Implement **cloud-based firewalls** (Azure Network Security Groups (NSG), AWS Security Groups).

**Network Segmentation:**
- **Separate production, testing, and development environments** to prevent lateral movement of attacks.
- Implement **zero-trust architecture** for least-privilege network access.

**Change Management:**
- Any **modifications to network architecture** should be **reviewed and approved.**
- **Network topology changes** should be documented and tested before deployment.

**Backup Management:**
- Ensure **network devices (firewalls, routers, switches) are backed up regularly.**
- Store network configuration backups securely.

**Asset Management:**
- Maintain **lifecycle policies** for networking equipment (e.g., firewalls, switches).
- Perform periodic audits to replace outdated network devices.

**Capacity Management:**
- Monitor **bandwidth usage, firewall performance, and network storage capacity.**
- **Autoscaling policies** should be defined to handle increased traffic demands.


---

# Case Study: Migration from Rackspace IaaS to Microsoft Azure (Europe Region)

## **Background:**
- Production environment for Europe was hosted in Rackspace IaaS.
- Migrated to Microsoft Azure in 2023.
- **TPS Team** managed **off-boarding from Rackspace** and **onboarding to Azure**.

## **Off-Boarding Rackspace (Decommissioning Activities):**
- **Asset Inventory and Disposal:**
  - Asset serial numbers, location tracking, disposal records.
  - Obtain **Certificate of Destruction (COD)** for audit evidence.
- **Secure Data Wiping & Migration:**
  - Data must be wiped before decommissioning.
  - Secure migration of workloads to Azure.

## **On-Boarding Microsoft Azure:**
- **Asset Inventory Update**
- **Security & Compliance Checks:** Azure NSGs, backup policies, AAD with MFA.
- **Capacity Planning & Performance Testing**

---

# **Audit & Assurance Process for Cloud Migration**

- **GIS Audit Management Team (TCS) and SGRC Audit Management Team** ensure security compliance.
- **Evidence Collection Challenges:** Escalation to **ISM/VRO (Weekly Calls)** and **Directors/SMEs/CISOs (Monthly Meetings)**.

# **Key Achievements (For Resume - Naukri Profile)**
- Led successful **On-Prem to Cloud transition** (Rackspace to Azure).
- Implemented **cloud security controls** across SaaS, PaaS, and IaaS.
- Managed **100% compliance** with cybersecurity frameworks.
- Developed **network segmentation strategies** for security enhancement.
