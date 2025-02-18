# Cloud Computing Service Models

Cloud computing is based on different service models, which define how cloud services are delivered and consumed. These models can be broadly categorized into three main types:

## 1. Infrastructure-as-a-Service (IaaS)
IaaS provides fundamental computing resources such as servers, virtual machines, networking, and storage over the internet. Organizations can rent these resources on-demand instead of maintaining physical infrastructure.

### Key Features of IaaS:
- Provides virtualized computing resources over the cloud.
- Offers scalability and flexibility as businesses can scale resources up or down.
- Users have control over the operating system, applications, and storage.
- **Examples:** Amazon Web Services (AWS) EC2, Microsoft Azure Virtual Machines, Google Compute Engine (GCE).

---

## 2. Platform-as-a-Service (PaaS)
PaaS provides a development and deployment environment in the cloud, enabling developers to build, test, and deploy applications without worrying about the underlying infrastructure.

### Key Features of PaaS:
- Provides a runtime environment for applications.
- Includes development tools, databases, and middleware.
- Reduces complexity by managing the underlying hardware, operating system, and networking.
- Increases developer productivity by offering pre-built services and frameworks.
- **Examples:** Google App Engine, Microsoft Azure App Services, AWS Elastic Beanstalk.

---

## 3. Software-as-a-Service (SaaS)
SaaS delivers software applications over the internet on a subscription basis. Users can access these applications via a web browser without installing or maintaining them on their local devices.

### Key Features of SaaS:
- Applications are hosted and maintained by the service provider.
- Users can access the software through web browsers without installation.
- Offers automatic updates and maintenance.
- Reduces the need for in-house IT management.
- **Examples:** Google Workspace (Gmail, Docs, Drive), Microsoft 365, Salesforce, Dropbox.

---

# On-Premises (On-Prem) Infrastructure
If an organization hosts its entire infrastructure, platform, and software within its own data center, this setup is known as **On-Premises (On-Prem)** computing. Unlike cloud services, where resources are managed by third-party providers, On-Prem solutions require organizations to purchase, install, and maintain all the necessary hardware and software.

### Key Features of On-Prem:
- Full control over security and compliance.
- Requires significant capital investment in hardware and IT staff.
- No dependency on external cloud providers.
- Suitable for industries with strict regulatory requirements, such as healthcare and finance.

---

# Security in Cloud Computing

## **Network Security Groups (NSG)**
Network Security Groups (NSGs) control inbound and outbound traffic to and from network interfaces, subnets, and virtual machines (VMs). They act as virtual firewalls that define access control rules.

### Key Features of NSGs:
- Allow or deny network traffic based on rules.
- Help secure cloud environments by restricting access to critical resources.
- Can be applied at different levels (VM, subnet, or entire network).
- **Examples:** AWS Security Groups, Azure NSG, Google Cloud Firewall Rules.

---

## **Key Vault or Key Repository**
A **Key Vault** or **Key Repository** is a secure service that stores and manages cryptographic keys, secrets, and certificates used for encrypting data and securing applications.

### Key Features of Key Vault:
- Provides centralized management of encryption keys.
- Protects sensitive information like API keys, passwords, and connection strings.
- Supports access control and auditing for security compliance.
- **Examples:** AWS Key Management Service (KMS), Azure Key Vault, HashiCorp Vault.

---

## **Single Sign-On (SSO)**
Single Sign-On (SSO) is an authentication process that allows users to log in once and gain access to multiple applications without needing to re-enter credentials.

### Key Features of SSO:
- Reduces the need for multiple usernames and passwords.
- Enhances security by centralizing authentication.
- Simplifies user experience and access management.
- Often integrated with Identity and Access Management (IAM) solutions.
- **Examples:** Okta, Microsoft Azure AD, Google Identity Platform.

### **How SSO Works:**
1. The user logs in once using a primary authentication service (such as an Identity Provider - IdP).
2. The SSO system authenticates the user and provides a secure token.
3. The user can now access multiple connected applications without additional login prompts.

---

