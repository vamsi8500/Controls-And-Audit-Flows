# Incident Management: A Clear Overview

Incident Management refers to handling any event that negatively impacts an organization concerning Confidentiality, Integrity, Availability, and Privacy (CIAP).

## 1. Understanding Incidents

### What is an Incident?
An incident is any event that negatively impacts an organization with respect to CIAP.

- **Confidentiality**: Unauthorized data access.
- **Integrity**: Unauthorized data modification.
- **Availability**: Service disruptions or outages.
- **Privacy**: Exposure of sensitive information.

### Event vs. Incident
- **Receiving a phishing email** = Security Event  
- **Clicking on a phishing link leading to a breach** = Security Incident

**Key Rule**: Every incident is an event, but not every event is an incident.

## 2. Handling an Incident

### Admin Access & Privileged Users
Users with admin privileges can read, write, and execute system files.  
Any misuse of admin access can lead to a security incident.

### Reporting Security Incidents
If a phishing email is received, it should be reported to the helpdesk (e.g., helpdesk@tes.com).  
Employee awareness about the distribution list for incident reporting is essential.

## 3. Incident Response Plan (CSIRP)

### What is CSIRP?
The Cybersecurity Incident Response Plan (CSIRP) defines how an organization responds to incidents. It is:
- ✅ Administered by GIS (Global Information Security Team).
- ✅ Handled by the Security Incident Manager (SIM).
- ✅ Executed by CSIRT (Cybersecurity Incident Response Team) & SOC (Security Operations Center).

### Roles in Incident Management

| Role | Responsibility |
| ---- | -------------- |
| Security Incident Manager (SIM) | Leads incident resolution and closure. |
| CSIRT | Investigates security incidents and takes necessary actions. |
| SOC Department | Monitors network, CCTV, and security logs for malicious activities. |

## 4. Common Security Incidents

| Type | Examples |
| ---- | ------- |
| Malware & Ransomware | Virus infections,

# Login Attack Scenario: Brute Force Attack

## Incident Overview:
A brute force attack targeted the company’s user login page, where the attacker attempted to guess the login credentials of multiple user accounts by trying many password combinations. The attack was detected when an abnormal number of login attempts were recorded from a single IP address.

## Steps Taken to Handle the Incident:

### 1. Incident Detection & Reporting:
- The IT security team noticed multiple failed login attempts originating from a single IP address within a short time frame.
- The monitoring system flagged these login attempts as suspicious and alerted the security team.
- The security team reported the incident to the Incident Response Team (IRT) for further investigation.

### 2. Incident Classification & Prioritization:
- This incident was classified as a **High-Priority (P2)** event because although the attacker hadn't gained access yet, there was a high likelihood of success given the volume of attempts.

### 3. Incident Containment:
- The IP address performing the brute force attack was immediately blacklisted and blocked from accessing the login page.
- The login page was temporarily disabled to prevent further attempts while the security team investigated.
- Multi-factor authentication (MFA) was enabled for all users to prevent unauthorized access in case passwords were compromised.

### 4. Incident Mitigation & Resolution:
- The attacker's IP address was traced, and further attempts from the same location were prevented by firewall rules.
- Security logs were analyzed to identify if any accounts had been compromised. No successful logins were detected, so no credentials were compromised.
- Password policies were reviewed, and stronger password requirements (e.g., minimum length, complexity, and expiration period) were implemented for all users.

### 5. Incident Closure & Preventive Measures:
- Affected users were informed about the attack, and they were required to reset their passwords as a precaution.
- Rate-limiting and CAPTCHA were introduced on the login page to prevent future brute force attempts.
- User awareness training was conducted on the importance of using strong, unique passwords and enabling MFA.

## Lessons Learned:
- **MFA is essential**: Even if passwords are compromised, MFA can stop attackers from gaining access.
- **Rate-limiting and CAPTCHA**: Implementing these mechanisms can significantly reduce the success of brute force attacks.
- **Stronger password policies**: Enforcing stronger password policies makes it harder for attackers to guess passwords.

- # Answer: How I Handled a Security Incident

## Type of Security Incident: Phishing Attack

I handled a security incident related to a phishing attack, where an employee unknowingly clicked on a malicious link in an email that appeared to be from the IT support team. The email requested the employee to reset their password, which led to the compromise of their login credentials.

## Steps Taken to Handle the Incident:

### Incident Detection & Reporting
- The employee realized the email was suspicious after entering their credentials and reported the incident to the helpdesk.
- The Security Operations Center (SOC) analyzed the logs and identified unauthorized login attempts originating from an unfamiliar IP address.

### Incident Classification & Prioritization
- Given that the employee's credentials were compromised, we classified the incident as a **High-Priority (P2)** event.
- If further signs of misuse were detected (such as unauthorized system access), the incident would have been escalated to **Critical (P1)**.

### Incident Containment
- The compromised account was immediately disabled to prevent further misuse of the stolen credentials.
- We also blocked the malicious domain across the network to stop additional attacks from the same source.
- The employee’s device was scanned for malware to ensure no other security threats existed.

### Incident Mitigation & Resolution
- The employee’s password was reset and **Multi-Factor Authentication (MFA)** was enforced to increase security.
- We analyzed security logs to confirm if the attacker accessed any sensitive data.
- If any further suspicious activity was found, a forensic investigation was initiated to trace the attacker's actions.

### Incident Closure & Preventive Measures
- After resolving the incident, we ensured that the affected employee, as well as other staff members, were trained on recognizing phishing emails.
- We updated email security filters to block similar phishing attempts in the future.
- Regular phishing simulation exercises were introduced to evaluate and improve employee awareness.
- The incident was documented for audit purposes, and we reviewed compliance with Service Level Agreements (SLAs).

## Lessons Learned:
- **Early Detection**: The prompt reporting of the incident helped prevent further damage.
- **MFA Enforcement**: The implementation of MFA helped ensure that the stolen credentials could not be misused.
- **Ongoing Awareness**: Continuous education on phishing and other cybersecurity threats is critical to reducing the risk of similar incidents in the future.


