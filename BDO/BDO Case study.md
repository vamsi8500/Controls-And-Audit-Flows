# Third-Party Risk Management (TPRM) Overview

TPRM refers to identifying, assessing, monitoring, and mitigating the risks associated with third-party vendors, suppliers, or partners that have access to your organization's systems, data, or operations.

## Key Phases in TPRM:
- Vendor Onboarding & Due Diligence
- Risk Assessment (Inherent & Residual Risk)
- Contractual & Legal Risk Mitigation
- Ongoing Monitoring
- Offboarding & Data Disposal

---

## ✅ 1. What is a Risk?

**Definition:**  
A risk is the potential for an unwanted outcome resulting from an event or action. In cybersecurity and compliance, risk typically arises from threats exploiting vulnerabilities, leading to consequences like data breaches, downtime, or regulatory fines.

**Risk Equation:**  
`Risk = Threat × Vulnerability × Impact`

**Example:**  
- **Threat:** Phishing email  
- **Vulnerability:** Employees not trained in spotting phishing  
- **Impact:** Credential theft, unauthorized access

---

## ✅ 2. Case Study: Risk, Vulnerability, and Threat

### 🏥 Scenario:
A healthcare provider uses an outdated EHR system accessible through a public-facing web portal. A hacker attempts to exploit the outdated authentication module.

- **Threat:** Unauthorized hacker attempting access  
- **Vulnerability:** Outdated login module lacking 2FA  
- **Risk:** Data breach of patient records → HIPAA violation

### 🛡️ Mitigation:
- Upgrade the authentication module  
- Enforce Multi-Factor Authentication (MFA)  
- Conduct regular vulnerability assessments

---

## ✅ 3. Case Study: New Onboarding Vendor

### 🏢 Scenario:
A bank wants to onboard a third-party document digitization vendor that will process KYC documents.

### 🔍 Key Observations:
- Vendor is a startup without prior experience handling financial data  
- No recent penetration test results or ISO 27001 certification  
- Cloud servers hosted on shared infrastructure

### 🛡️ TPRM Actions:
- Conduct security questionnaire and risk rating (high inherent risk)  
- Request and review:  
  - SOC 2 Type II or ISO 27001 report  
  - Data encryption standards  
  - Employee background checks  
- Include the following in the contract:  
  - Right to audit clause  
  - Data handling SLAs  
  - Breach notification timelines (e.g., within 24 hours)

### ✅ Outcome:
Vendor implemented required controls, including role-based access and encryption. Onboarding approved with monthly risk reviews.

---

## ✅ 4. Case Study: BCP, RTO, and RPO

### 🌪️ Scenario:
A fintech company’s data center in Chennai was flooded, resulting in critical service outages, including loan processing systems.

### 📘 Definitions:
- **BCP (Business Continuity Plan):** Ensures operations continue during/after disruption  
- **RTO (Recovery Time Objective):** Maximum tolerable downtime (e.g., 4 hours)  
- **RPO (Recovery Point Objective):** Maximum data loss allowed (e.g., 15 minutes)

### 🛡️ Actions Taken:
- Activate BCP and switch to DR site in Mumbai  
- Data replicated every 10 minutes → met RPO  
- Systems back online in 3.5 hours → met RTO

### ✅ Outcome:
Minimal business disruption, compliant with regulatory expectations. Post-event review enhanced infrastructure redundancy.

---

## ✅ 5. Types of Encryption

### 🔐 Encryption Types:

|
