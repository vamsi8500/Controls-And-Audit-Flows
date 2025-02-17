# Incident Management: A Detailed Overview

Incident management is a structured process that aims to reduce the impact of security incidents on an organization. It ensures that security threats are detected, assessed, mitigated, and prevented in a systematic manner.

## Understanding Incidents

### What is an Incident?
An incident is any event or series of activities that negatively impact an organization concerning:

- **Confidentiality** (Unauthorized access to data)
- **Integrity** (Unauthorized modification of data)
- **Availability** (Disruption in system operations)
- **Privacy** (Unauthorized exposure of sensitive information)

**Key Principle:** Every incident is an event, but not every event is an incident.

## Security Events vs. Security Incidents

| Aspect | Security Event | Security Incident |
|--------|---------------|------------------|
| **Definition** | Any observable occurrence that may impact an organization’s security posture. | A confirmed event that has compromised security (data breach, system failure, etc.). |
| **Example 1** | Receiving a phishing email. | Clicking on a phishing link, leading to malware infection. |
| **Example 2** | Provisioning admin access to a user. | The user misuses admin access and modifies critical settings. |
| **Example 3** | Laptop stolen. | Sensitive data from the stolen laptop is compromised. |

## Roles & Responsibilities in Incident Management

### Key Teams Involved

| Team | Responsibilities |
|------|----------------|
| **SOC (Security Operations Center)** | Reviews security events and escalates potential incidents. |
| **CSIRT (Cybersecurity Incident Response Team)** | Plans, enforces, documents, and remediates security incidents. |
| **EDR / SIEM Analysts** | Monitor and escalate potential threats detected by security tools. |
| **Security Incident Manager (SIM)** | Prioritizes incidents, ensures resolution, and aligns actions with CSIRP. |
| **Global Service Desk (GSD)** | Logs security incidents in the ticketing system. |

## Incident Response Plan (CSIRP)

The **Cybersecurity Incident Response Plan (CSIRP)** is a structured approach to responding to security incidents.

### Key Components of CSIRP

- **Incident Definition:** Criteria for identifying security events and incidents.
- **Incident Reporting & Handling:** Standard process for logging and escalating incidents.
- **Incident Prioritization:** Classification based on impact and severity.
- **Roles & Responsibilities:** Defined accountability matrix for handling incidents.
- **Documentation & Evidence Collection:** Proper logging of incident details.
- **Communication Protocols:** Internal and external reporting mechanisms.

### Types of Security Incidents

- Malware/Ransomware infections
- Network attacks (DDoS, brute force, MITM)
- Lost/Stolen IT assets (Laptops, storage devices)
- Credential theft
- Website defacement or service disruptions
- Data breaches & regulatory violations
- Third-party security incidents

## Incident Prioritization & Severity Levels

| Impact Level | Definition | Response Time |
|-------------|-----------|--------------|
| **Critical** | Severe impact on business operations (e.g., ransomware attack). | 30 minutes |
| **High** | Major impact on security but business continuity remains. | 4 hours |
| **Medium** | Moderate security impact, limited damage. | 24 hours |
| **Low** | Minor issue, minimal business impact. | 48 hours |

## Incident Response Workflow

### Step-by-Step Process

1. **Incident Detection & Reporting**
   - Global Service Desk (GSD) logs the incident.
   - Security teams review the incident.

2. **Incident Classification & Prioritization**
   - SIM assesses severity (Critical, High, Medium, Low).
   - Assigns appropriate SLA (Service Level Agreement).

3. **Incident Investigation & Containment**
   - CSIRT investigates and isolates the affected systems.
   - SIEM/EDR analysts gather logs for forensic analysis.

4. **Incident Resolution & Mitigation**
   - Deploy security patches, restore systems, revoke compromised access.

5. **Incident Closure & Documentation**
   - CAPA (Corrective and Preventive Actions) are implemented:
     - **Corrective Action:** Blocking attack vectors.
     - **Preventive Action:** Updating security policies.
   - Incident report is generated and stored for audits.

6. **Post-Incident Review & Lessons Learned**
   - Conduct awareness training for employees.
   - Review CSIRP for improvements.

## Flowchart: Incident Response Plan

```plaintext
                           [ Security Event Detected ]
                                      |
                                      V
                     [ Service Desk Logs the Incident ]
                                      |
                                      V
          [ Security Team Reviews & Classifies Incident ]
                     |                    |
                     |                    |
               (Not an Incident)       (Confirmed Incident)
                     |                    |
                     |                    V
             [ Logged for Record ]   [ Prioritize Incident ]
                                           |
                                           V
                    [ Investigate & Contain the Threat ]
                                           |
                                           V
            [ Resolve & Implement Corrective Actions ]
                                           |
                                           V
             [ Conduct Post-Incident Review & Update CSIRP ]
```

## Incident Reporting & Documentation

An incident report must contain:

- **Incident Assessment** (Critical, Significant, Minor).
- **Information Sharing** (Affected network, users, etc.).
- **Technical Details** (Malware, attack type).
- **Number of Affected Hosts** (1-100, 100-1000).
- **Attacker’s IP Address** (e.g., 192.168.144.1 - 192.168.144.254).
- **Damage Assessment** (Data loss, system compromise).
- **Incident Log** (Timeline of actions taken).
- **Additional Information** (Lessons learned, audit findings).

## RACI (RASCI) Matrix for Incident Management

| Activity | Responsible (R) | Accountable (A) | Support (S) | Consulted (C) | Informed (I) |
|----------|---------------|---------------|-----------|-----------|-----------|
| **Incident Logging** | Service Desk | SIM | IT Team | SOC | Management |
| **Incident Classification** | SOC | SIM | IT Team | CSIRT | Management |
| **Incident Investigation** | CSIRT | SIM | IT Security | Legal | Management |
| **Incident Containment** | CSIRT | SIM | IT Security | Legal | Management |
| **Incident Resolution** | IT Security | SIM | CSIRT | Legal | Management |
| **Post-Incident Review** | SIM | SOC | IT Security | Legal | Management |

## Incident Closure: CAPA Implementation

At the end of each incident, **Corrective and Preventive Actions (CAPA)** are taken:

- **Corrective Actions (Fixing the immediate issue)**
  - Example: Blocking a malicious IP address.
- **Preventive Actions (Reducing future risk)**
  - Example: Updating firewall rules to filter out phishing emails.

## Employee Awareness & Communication

### Training & Induction Sessions
- Employees should be trained to identify and report phishing emails.

### Incident Reporting Mechanisms
- **Internal:** incident@abc.com (Employee reports).
- **External:** thirdpartyincident@abc.com (Vendor reports).

### Audit & Assurance
- Ensure CSIRP compliance and verify SLA adherence.


# INCIDENT REPORT

## 1. Incident Assessment:
- **Severity Level:** ____________________
- **Options:** Critical | Significant | Minor | Negligible

## 2. Information Sharing:
- **Issue:** Developer LAN network is not updated with antivirus

## 3. Technical Details (If applicable):
- **Issue Type:** Malware affected

## 4. Number of Hosts Affected:
- [ ] 1 to 100
- [ ] 100 to 1000
- [ ] More than 1000

## 5. IP Address of Apparent or Suspect Source:
- **Source IP Address Range:** 192.168.144.1 - 192.168.144.254
- **Other Information:**
  - **IP Address:** 192.168.144.1 - 192.168.144.254
  - **Computer/Host Name:** Manohar
  - **Operating System:** Linux
  - **Other Applications:** Not specified

## 6. Damage Observations Resulting from Incident:
- Malware-affected systems can be compromised via the network.

## 7. Incident Log:
- _______________________________________________________

## 8. Additional Information:
- 150 machines are affected with malware.

**Reviewed By:** ____________________  
**Approval Sign-Off:** ____________________  
**Date:** ____________________

- # Incident Mitigation and Resolution

## 1. Incident Mitigation Using ASIRP (Automated Security Incident Response Plan)

### What is ASIRP?
ASIRP (Automated Security Incident Response Plan) is used to:

- Automatically mitigate risks using predefined security rules.
- Trigger containment actions (e.g., block IPs, disable compromised accounts).
- Alert relevant teams for manual intervention if necessary.

### Mitigation Actions Taken Based on Severity

| **Incident Type** | **Mitigation Actions (ASIRP)** |
|------------------|--------------------------------|
| **Phishing Attack** | Quarantine email, block sender domain, scan endpoint. |
| **Malware Infection** | Isolate infected system, deploy antivirus scans. |
| **Data Breach** | Lock affected accounts, reset passwords, notify compliance team. |
| **DDoS Attack** | Activate Web Application Firewall (WAF), block malicious traffic. |

---

## 2. SLA (Service Level Agreement) Definition

### What is SLA in Incident Management?
SLA defines the **maximum response and resolution time** for each incident based on its priority.

| **SLA Metrics** | **Definition** |
|---------------|--------------|
| **Time to Detect (TTD)** | How long it takes to identify an incident. |
| **Time to Respond (TTR)** | How long it takes to take action after detection. |
| **Time to Mitigate (TTM)** | How long it takes to contain the impact. |
| **Time to Resolve (TTRV)** | How long it takes to fully restore normal operations. |

### SLA Example: **Critical Incident (Data Breach)**

- **Time to Detect:** 10 minutes  
- **Time to Respond:** 30 minutes  
- **Time to Contain:** 2 hours  
- **Time to Resolve:** 24 hours  

The **Security Incident Manager (SIM)** ensures that **SLA compliance** is maintained, and if delays occur, **escalations are made**.

---

## 3. Incident Resolution & Closure

### Steps to Close an Incident

1️⃣ **Incident is logged and categorized.**  
2️⃣ **Investigation & root cause analysis are performed.**  
3️⃣ **Containment and mitigation actions are taken.**  
4️⃣ **Incident is resolved within SLA.**  
5️⃣ **CAPA (Corrective & Preventive Actions) are implemented.**  
6️⃣ **Final Incident Report is documented.**  
7️⃣ **Lessons learned are shared with teams.**  

### Final Incident Report Components

✅ **Incident ID & Type** (e.g., Malware Infection).  
✅ **Affected Systems & Users** (e.g., 150 endpoints).  
✅ **Root Cause** (e.g., Phishing email with malicious link).  
✅ **Actions Taken** (e.g., Isolated systems, blocked domain).  
✅ **Resolution & Prevention Steps** (e.g., MFA enabled, email filters updated).  
✅ **Incident Closure Approval** (by Security Head).  

---

## 4. Post-Incident Review & Preventive Measures

### What Happens After Incident Closure?

- **Security policies are updated** based on the findings.
- **Employee awareness training** is conducted (e.g., how to detect phishing emails).
- **Security tools are fine-tuned** (e.g., update SIEM rules, improve detection logic).
- **Incident trends are analyzed** to predict and prevent future threats.

---

## 5. Incident Response Flowchart

```plaintext
            [ Incident Reported ]
                    |
                    V
       [ Incident Logged in ITSM System ]
                    |
                    V
      [ Incident Classification & Prioritization ]
            |           |          |
        Low Risk    Medium Risk   High Risk
            |           |          |
       [ Monitor ]    [ Contain ] [ Immediate Action ]
                                    |
                                    V
                  [ Investigation & Forensic Analysis ]
                                    |
                                    V
             [ Eradication & Risk Mitigation Actions ]
                                    |
                                    V
                 [ SLA Compliance & Incident Closure ]
                                    |
                                    V
                  [ CAPA & Post-Incident Review ]
## Key Takeaways

- Every incident must be handled systematically following CSIRP.
- Roles & responsibilities should be well-defined.
- Incident response should be prioritized based on severity.
- Proper documentation & reporting are crucial for compliance & improvement.
- Continuous training and awareness help reduce future incidents.
