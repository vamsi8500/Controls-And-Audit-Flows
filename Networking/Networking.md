# Network Security Overview

## 1. IP and Ports
- Every IP address has **65,535 ports** available for communication.
- Ports allow different services (**HTTP, FTP, SSH, etc.**) to function on the same machine.
- **Port Number Ranges:**
  - **Well-known ports (0-1023):** Common services like HTTP (80), HTTPS (443), SSH (22).
  - **Registered ports (1024-49151):** Used by software applications.
  - **Dynamic/private ports (49152-65535):** Used for temporary connections.

## 2. Firewall (First Layer of Defense)
A **firewall** acts as a security barrier between networks. It inspects and filters incoming and outgoing traffic based on predefined security rules.

### Types of Firewalls
- **Network Firewalls** – Filters traffic at the network level.
- **Application Firewalls** – Filters specific application traffic (e.g., a web application firewall).
- **Stateful Inspection Firewalls** – Tracks the state of active connections and decides which packets to allow.

### Firewall Rule Set
- Defines which **ports, IPs, and services** are **allowed** or **blocked**.
- Needs to be **reviewed regularly** by management.
- **Least privilege principle:** Only allow necessary access.

### Example Ruleset
| Protocol | Port | Action | Reason |
|----------|------|--------|--------|
| HTTP     | 80   | Allow  | Public website access |
| SSH      | 22   | Deny   | Prevent unauthorized remote access |
| SMTP     | 25   | Allow  | Email service |

## 3. Demilitarized Zone (DMZ)
A **DMZ** is a **buffer zone** between the **internet and an organization's internal network**. It hosts public-facing services (**e.g., websites, email servers**) while preventing direct access to the internal network.

### DMZ Components
- **Internet-facing servers** (e.g., web servers, mail servers).
- **Firewalls** separate the DMZ from both the internet and internal networks.
- **Purpose:** If an attacker compromises a DMZ system, they don’t get direct access to internal networks.

## 4. Intranet vs. Internet
- **Internet:** Public network, accessible to anyone.
- **Intranet:** Private network, restricted to an organization.
- **Extranet:** A controlled network allowing external partners/vendors access.

## 5. Network Isolation and Security
- **Micro-segmentation:** Divides the network into isolated sections to limit breaches.
- **Air-gapped systems:** Physically separated from other networks for high security.
- **Zero Trust Model:** No device is automatically trusted; access is given based on verification.

## 6. Vulnerability Assessment and Penetration Testing (VAPT)
- **Vulnerability Assessment (VA):** Identifies security weaknesses.
- **Penetration Testing (PT):** Simulates cyberattacks to find vulnerabilities.

### Types of VAPT
- **Application-Level VAPT** – Tests for web application flaws (e.g., SQL Injection, XSS).
- **Network-Level VAPT** – Identifies weak network configurations.

**Reports from VAPT must be reviewed periodically.**

## 7. VPN (Virtual Private Network)
A **VPN** securely connects users to a network over the internet.

### Types of VPNs
#### **SSL VPN (Secure Socket Layer VPN)**
- Used for remote access.
- Clients use a web browser to connect.

#### **IPsec VPN (Internet Protocol Security VPN)**
- Used for **site-to-site** connections.
- Encrypts data between two locations (e.g., office branches).

#### **Site-to-Site VPN**
- Connects entire networks securely (**e.g., headquarters to a backup site**).
- **Example:** Azure Key Vault uses VPN for secure access.

## 8. Security Monitoring and Auditing
- **Firewall logs should be monitored daily.**
- **Vulnerability scanning should be performed regularly.**
- **Audits ensure that security policies are followed.**

### Example
- **If port 8000 is open, there should be a business justification.**

## Key Takeaways
- **Firewalls** control network traffic.
- **DMZ** isolates public servers from internal networks.
- **VPNs** ensure secure remote access.
- **VAPT** identifies security gaps.
- **Security monitoring and audits** are necessary for compliance.
- 

# IPS and IPD in Networking

## IPS (Intrusion Prevention System)
A security system that monitors network traffic for malicious activities and takes actions (like blocking or alerting) to prevent attacks.

- Works in real-time to stop threats before they impact the network.
- Can be host-based (**HIPS**) or network-based (**NIPS**).

## IPD (Intrusion Prevention and Detection)
A broader term that includes both **Intrusion Detection Systems (IDS)** and **Intrusion Prevention Systems (IPS)**.

- **IDS** detects and alerts about malicious activity, while **IPS** actively blocks threats.
- Some systems combine both functions, providing a comprehensive security solution.

## Real-Time Example of IPS (Intrusion Prevention System)
Imagine you're working in a company's IT security team. One day, an attacker tries to exploit a vulnerability in your organization's web server by sending malicious SQL injection requests.

1. Your **IPS**, which is actively monitoring network traffic, detects the unusual pattern of incoming requests.
2. It immediately blocks the attack before it reaches the server, preventing data breaches.
3. At the same time, it sends an alert to the security team for further investigation.

## Real-Time Example of IPD (Intrusion Prevention and Detection)
Now, consider a scenario where an employee unknowingly downloads a malware-infected file from an email.

1. The **Intrusion Detection System (IDS)** detects unusual behavior, such as unexpected outbound traffic to an unknown server, and raises an alert.
2. If an **IPS** is also in place, it not only detects the threat but also blocks the malicious connection, stopping the malware from communicating with the hacker.

This combination of **IDS + IPS (IPD)** ensures both detection and prevention of cyber threats in real-time.

