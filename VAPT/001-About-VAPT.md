# Vulnerability Assessment and Penetration Testing (VAPT)

## 1. What is VAPT?
VAPT stands for **Vulnerability Assessment and Penetration Testing**. It is a **security testing process** used to find and fix vulnerabilities in **computer systems, networks, and applications**.

VAPT is conducted by **ethical hackers** from the **Security Operations Center (SOC) department** or **external security firms**. After the assessment, a **detailed report** is generated, listing security weaknesses and recommended fixes.

---

## 2. How is VAPT Performed?
VAPT can be done in **two ways** based on the scope and organization’s needs:

### A. Internal VAPT
- Performed **within the organization** by the **SOC team (ethical hackers)**.
- Focuses on **internal systems, databases, and network security**.
- Helps detect threats that may arise **from within the company**, such as **insider attacks**.

### B. External VAPT
- Conducted by **external cybersecurity firms** registered under **MeitY (Ministry of Electronics and Information Technology, India)**.
- Focuses on **external-facing systems**, such as **websites, APIs, cloud services, and external networks**.
- Helps identify security loopholes that an **outside attacker** could exploit.

---

## 3. Types of Penetration Testing
VAPT includes different types of **penetration testing** based on what needs to be tested:

### A. Network & Infrastructure Testing
- Evaluates security in **routers, firewalls, servers, databases, and networks**.

### B. Web Application Testing
- Tests **web applications** like **banking apps, CRM software, and e-commerce platforms** for vulnerabilities like **SQL injection, Cross-Site Scripting (XSS), and authentication bypass**.

### C. Wireless Network Testing
- Ensures **Wi-Fi networks** are secure from unauthorized access or attacks.

### D. Mobile Application Testing
- Focuses on **iOS and Android applications**, testing for **security flaws, weak encryption, and unauthorized data access**.

---

## 4. VAPT Testing Approaches
VAPT is performed using **three main approaches**, depending on the level of access provided to the testers:

### A. Black Box Testing
- **No prior knowledge** of the system is given to the tester.
- Only **basic details like URL or IP address** are provided.
- Simulates a **real-world hacker attack** from an outsider’s perspective.

### B. White Box Testing
- Testers have **full access** to the system, including **source code, credentials, and documentation**.
- Helps in **thorough security analysis** and **code review**.

### C. Grey Box Testing
- The tester has **partial knowledge** about the system, such as **some access credentials**.
- Ensures that users have the **correct access permissions** and can’t perform unauthorized actions.

---

## 5. VAPT Testing Methodology
Penetration testers follow a structured **methodology** to identify vulnerabilities. The most common framework used is **OWASP Top 10**, which focuses on the most critical web application security risks.

### A. Scoping
- Define **which systems, networks, and applications** will be tested.
- Understand **security goals** and **regulatory compliance requirements**.

### B. Reconnaissance (Information Gathering)
- Collect details about the target system using **manual and automated tools**.
- Map out **potential attack surfaces**.

### C. Vulnerability Assessment
- Identify **security weaknesses** using tools like **Nmap, Burp Suite, Nessus, Metasploit**.
- Analyze **configuration flaws, outdated software, weak passwords, etc.**

### D. Exploitation (Penetration Testing)
- Attempt to **exploit vulnerabilities** to understand their impact.
- Simulate **real-world attacks** to test system security.

### E. Reporting & Documentation
- Create a **detailed report** listing all vulnerabilities found, along with their **risk levels and remediation steps**.

### F. Retesting & Validation
- Once fixes are applied, **retest the system** to confirm that all vulnerabilities are resolved.

---

## 6. Security Aspects to Review in Web Applications
During a VAPT audit, security teams check for common vulnerabilities, including:

- **DDoS (Distributed Denial of Service) Attacks** – Ensuring the system can withstand large traffic spikes.
- **SQL Injection** – Preventing attackers from manipulating databases using malicious SQL queries.
- **Authentication & Password Security** – Ensuring strong password policies and multi-factor authentication.
- **Whitelisting & Blacklisting Checks** – Verifying that users can only upload **authorized** documents.
- **Vulnerability Fixes & SLA Compliance** – Ensuring that all identified issues are fixed within the **Service Level Agreement (SLA) timeframe**.

---

## 7. SLA Breach & RAF ID Tracking
- **SLA Breach**: If a vulnerability is not fixed within the **agreed timeframe**, it is considered an SLA breach.
- **RAF ID (Risk Acceptance Form ID)**: If a vulnerability **cannot be fixed**, it must be **documented, reviewed, and risk-accepted** by the management.

---

## Conclusion
VAPT is a **critical cybersecurity process** that helps businesses identify and fix security vulnerabilities before they can be exploited. Regular security testing ensures that **systems remain safe, compliant, and resilient** against cyber threats.

---
