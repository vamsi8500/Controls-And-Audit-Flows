# Cloud Service Models and Applicable Controls

## **1. Software-as-a-Service (SaaS)**

### **Applicable Security Controls:**
#### **Application Level Controls:**
- **Secure Development Lifecycle (SDLC)**
- **Vulnerability Assessment and Penetration Testing (VAPT)**
- **Cryptography:**
  - **Database Security (Data at Rest):** AES-256 encryption.
  - **Application Security (Data in Transit):** TLS 1.2 and above.
- **Change Management**
- **Backup Management**
- **Access Management:** MFA and SSO.
- **Capacity Management:** Monitoring HTTP requests, active users, application servers.

---

## **2. Infrastructure-as-a-Service (IaaS)**

### **Applicable Security Controls:**
#### **Infrastructure/Server/Endpoint Controls:**
- **Physical Security Controls:** 2FA for data center access.
- **Backup Management:** Off-site backups.
- **Asset Management:** Inventory tracking and disposal policies.
- **Logical Access Management:** MFA enforcement.
- **Removable Media Security:** USB and external hard drive blocking (JAMF, etc.).
- **Antivirus and Endpoint Protection:** Regular updates and scans.

---

## **3. Network Security Controls** (Applicable to SaaS, PaaS, and IaaS environments)

- **Logical Access Controls:** MFA and VPN enforcement.
- **Firewall Security:** Quarterly firewall rule reviews.
- **Network Segmentation:** Security enforcement and isolation.
- **Change Management:** Approval process for network modifications.
- **Backup Management:** Regular updates of networking device backups.
- **Asset Management:** Network hardware lifecycle policies.
- **Capacity Management:** Monitoring bandwidth, storage, firewalls.

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
