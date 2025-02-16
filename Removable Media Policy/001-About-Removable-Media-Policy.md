# Control Domain 11: Removable Media Policy

Removable media includes any portable storage device that can be easily attached to and detached from a system. These devices pose security risks due to their ability to store large amounts of data, making them susceptible to loss, theft, or malware infections.

## Examples of Removable Media
- **USB Flash Drives (Pendrives)**
- **External Hard Drives**
- **Solid State Drives (SSDs)**
- **Memory Cards (SD Cards, MicroSD, etc.)**
- **CDs/DVDs**
- **External Optical Drives**

## Security Risks of Removable Media
- **Data Loss or Theft** – Sensitive information can be easily lost or stolen.
- **Malware Infection** – USB devices can be used to spread malware.
- **Unauthorized Access** – Data leakage risk due to unregulated usage.

## Steps for Implementing Removable Media Policy

### 1. Identify and Restrict Usage
- Recognize all types of removable media used in the organization.
- Restrict or limit usage based on business needs.
- Only allow removable media for approved users with proper security controls.

### 2. Block External Removable Media
- Use endpoint management tools like **Jamf, Microsoft Intune, or Group Policies (GPO)** to disable unauthorized USB devices.
- Implement **Data Loss Prevention (DLP)** to prevent unauthorized file transfers.
- Apply **BitLocker encryption** for authorized USB usage.

### 3. Secure Endpoints and Servers
- Configure security settings to block unauthorized removable media.
- Use **Endpoint Detection and Response (EDR)** tools to monitor and control USB access.
- Ensure only **company-approved devices** are used for data transfer.

### 4. Implement Security Tools
- Deploy **automatic blocking mechanisms** for unauthorized removable media.
- Enforce **encryption and password protection** for authorized removable devices.
- Use **logging and monitoring tools** to track USB device activity.

## Conclusion
A **removable media policy** helps prevent **data breaches, malware infections, and unauthorized access** by restricting the use of external storage devices and enforcing security controls. Organizations should use **security tools, endpoint protection, and strict policies** to mitigate the risks associated with removable media.
