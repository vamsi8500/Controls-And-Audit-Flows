# Secure Software Development Life Cycle (SSDLC)

The Secure Software Development Life Cycle (SSDLC) aligns with ISO 27001 and ISO 27002 controls, ensuring that security is integrated at every phase of software development. The primary ISO control that applies here is:

## ISO 27001: A.14 – System Acquisition, Development, and Maintenance

This control ensures that organizations build secure systems by implementing security practices at every stage of the software development life cycle.

## 1. Requirement Gathering & Analysis

### ISO 27001 Control: A.14.1.1 – Secure Development Policy
- Define security requirements for the application.
- Identify potential risks and compliance needs.
- Decide whether to develop in-house or acquire a third-party solution.
- If using third-party software, include security requirements in the SLA (Service Level Agreement).

## 2. Design (Secure Coding Checklist)

### ISO 27001 Control: A.14.2.5 – Secure System Engineering Principles
- Define secure design principles and architecture.
- Ensure secure coding guidelines are followed.
- Identify potential threats and mitigation strategies.

## 3. Coding/Development

### ISO 27001 Control: A.14.2.1 – Secure Development Environment
- Developers should follow secure coding practices (e.g., OWASP Top 10).
- Ensure access control and code reviews are in place.

## 4. Testing & Validation (Quality Assurance)

### ISO 27001 Control: A.14.2.8 – Testing of Security Functionality
- Conduct security testing, including:
  - Vulnerability Assessment (VA) – Identifying security weaknesses.
  - Penetration Testing (PT) – Simulating real-world attacks.
- Validate false positives and true positives in test results.

## 5. Deployment

### ISO 27001 Control: A.14.2.9 – System Acceptance Testing
- Ensure User Acceptance Testing (UAT) is performed before deployment.
- Implement security controls in the production environment.

## 6. Maintenance & Monitoring

### ISO 27001 Control: A.14.2.7 – Outsourced Development & ISCM
- Continuously monitor security using ISCM (Information Security Continuous Monitoring).
- Follow change management processes to handle security patches.

## 7. Disposal (End-of-Life Management)

### ISO 27001 Control: A.11.2.7 – Secure Disposal or Reuse of Equipment
- Follow data retention policies for secure deletion.
- Use data sanitization techniques like overwriting or destroying sensitive information.

# Auditing SDLC (Software Development Life Cycle)

Auditing the Software Development Life Cycle (SDLC) ensures that security controls are in place to protect applications from threats. The key security requirements focus on:

- Separation of environments (Development, Testing, and Production).
- Vulnerability Assessment & Penetration Testing (VAPT).
- Following OWASP Top 10 security guidelines.
- Implementing security controls during design, development, and deployment.

## 1. Separation of Development, Test, and Production Environments

### Why is it important?
- Keeping these environments separate prevents accidental data leaks, unauthorized changes, and security breaches.

### What happens if they are not separated?
- A developer might accidentally push untested code to production, causing application failures.
- Test data may include real customer information, leading to data leaks.

### Control Measure
- Maintain strict access controls between these environments to avoid cross-contamination.

## 2. Vulnerability Assessment & Penetration Testing (VAPT)

- VAPT is a security testing process that finds and fixes application vulnerabilities before hackers exploit them.
- Vulnerability Assessment (VA) → Identifies security weaknesses using automated tools.
- Penetration Testing (PT) → Ethical hacking to exploit vulnerabilities and test real-world security risks.

### Requirement
- Perform VAPT before deployment and fix critical issues before go-live.

## 3. OWASP Top 10 Security Risks

The OWASP Top 10 is a list of the most critical security threats for web applications. Some common threats include:

- SQL Injection → Hackers can manipulate database queries.
- Broken Authentication → Weak login systems allow attackers to bypass authentication.
- Cross-Site Scripting (XSS) → Injecting malicious scripts into web pages.
- Cross-Site Request Forgery (CSRF) → Forcing users to perform unwanted actions.
- Using Components with Known Vulnerabilities → Outdated third-party software can introduce risks.

### Requirement
- Follow secure coding practices to prevent these attacks.

## 4. Security Requirements During Development

Security must be included from the start of development. Some key controls include:

- Secure Authentication → Unique UserID, strong passwords, MFA, and SSO.
- Password Management → Enforce complexity, expiration, and reuse policies.
- Encryption → Use TLS 1.2 or above for data transmission.
- Session Management → Implement session expiration and idle timeouts.
- Logging → Maintain audit trails for security monitoring.
- Vulnerability Management → Fix security issues within SLA.
- Secure Disposal → Follow data retention policies to remove sensitive data securely.

### Requirement
- These security guidelines must be shared with the development team during coding.

## 5. Software Composition Analysis (SCA)

### What is SCA?
- SCA analyzes the open-source components used in software to check for:
  - Security vulnerabilities in third-party libraries.
  - License compliance (ensuring legal use of open-source code).

### Why is it important?
- Over 80% of modern applications use open-source software.
- If a vulnerable component is used, hackers can exploit it.
- Ensures compliance with software licenses to avoid legal issues.

### Control Measure
- Use SCA tools to scan open-source dependencies and fix vulnerabilities.

## 6. Penetration Testing (Pentesting) Approaches

- Penetration testing simulates cyberattacks to find weaknesses in applications.
- White Box Testing → The tester has full knowledge of the system (network maps, credentials).
- Black Box Testing → The tester has no prior information and mimics a real-world attacker.
- Grey Box Testing → The tester has partial knowledge of the system.

### Control Measure
- Use the appropriate pentesting method based on security needs.

## 7. Change Management & Outsourced Development

- Any changes in the application should go through a proper approval process.
- If development is outsourced, ensure the vendor follows security best practices and has secure coding policies.

### Requirement
- Maintain a change management process and perform regular security audits for outsourced software.

## 8. Security Testing & Approval

Before releasing software, it must pass three levels of approval:

- Functionality Testing → Ensures features work as expected.
- Validation Testing → Confirms the application meets business requirements.
- Security Testing (VAPT) → Finds and fixes vulnerabilities before deployment.

### Requirement
- No software should go live without passing all three approvals.

## 9. Reports & Compliance

- VAPT Report → Documents security testing results and fixes.
- SCA Report → Lists vulnerabilities in open-source components and recommended actions.

### Requirement
- Security reports must be reviewed, and vulnerabilities must be fixed before release.

## Key Takeaways

- Keep Development, Test, and Production environments separate to prevent security risks.
- Perform VAPT before deployment and fix critical security issues.
- Follow OWASP Top 10 guidelines to prevent common application attacks.
- Use SCA tools to check for vulnerabilities in open-source components.
- Implement authentication, encryption, logging, and secure coding practices.
- Follow a change management process and review security reports before going live.
