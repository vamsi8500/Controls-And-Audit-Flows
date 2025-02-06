# VAPT – Vulnerability Assessment and Penetration Testing Audit Flow

## STEP 1: Identify the Control Owner via Kickoff Meetings

### Kickoff Meeting Initiation
- **Schedule an initial kickoff meeting** with the key stakeholders.
- **Confirm the Control Owner (CO)** responsible for VAPT:
  - For **internal VAPT**, this is generally the SOC department (ethical hacker team).
  - For **external VAPT**, verify the external security firm that is listed in MeitY (Ministry of Electronics and Information Technology).

### Documentation
- **Record** the Control Owner’s **name, designation, and timestamp** of the meeting.
- **Clarify the scope** of VAPT:
  - Confirm that VAPT is conducted both **internally and externally**.
  - Verify the **type of testing** performed (Black Box, Grey Box, and White Box).
  - Ensure that the testing methodology is based on **OWASP guidelines** and covers the **Top 10 Application Security Risks**.

### VAPT Report Overview
- **Confirm** that each VAPT engagement results in a detailed post-assessment report, which includes:
  - A listing of all discovered vulnerabilities.
  - Risk ratings for each vulnerability.
  - Remediation recommendations.

---

## STEP 2: Inquiry – Process Related to Vulnerability Management Control

### Initial Inquiry with the Control Owner
- **Conduct interviews or send inquiries** to the identified CO to understand the governance and execution of the VAPT process.
- **Document details** including:
  - CO’s **Name, Designation**, and a **timestamp** for the inquiry.

### Inquiry Points

#### Internal and External VAPT Execution:
- **Who conducts the internal VAPT?** (Typically, the SOC ethical hacking team.)
- **Who is responsible for external VAPT?** (Verify that the external organization is listed in MeitY.)

#### Testing Methodology and Types:
- **Confirm the testing types** employed (Black Box, Grey Box, or White Box).
- **Verify** the use of established methodologies (e.g., OWASP Top 10).

#### Vulnerability Management Process:
- **Ask** how vulnerabilities are categorized and prioritized.
- **Check** if there is a process for retesting vulnerabilities once they are reported as “closed” to confirm remediation.
- **Inquire** about how SLAs are tracked and managed, and what the procedure is if an SLA is breached (e.g., issuance of a RAF ID and the corresponding RAF form).

---

## STEP 3: Walkthrough – Testing, Sampling, and Evidence Collection

### On-Site/Remote Walkthrough
- **Arrange a walkthrough session** with the CO (or designated team representative) and document the session (include **Name, Designation, and Timestamp**).
- **Observe the VAPT process in action** and request access to relevant documentation.

### Review of VAPT Reports
- **Collect both internal and external VAPT reports** for the audit period.
- **Verify** that each report includes:
  - The overall **methodology and type of testing** performed.
  - A **comprehensive list of identified vulnerabilities**.
  - A **prioritization scheme** for vulnerabilities (e.g., critical, high, medium, low).
  - **Defined SLAs** indicating the timeline for remediation.
  - **Status** of each vulnerability, including those marked as “closed.”

### Evidence of SLA Compliance
- **Check for documentation** that shows SLAs are met:
  - Identify any instances where SLAs were breached.
  - Confirm that when an SLA breach occurs, a **RAF ID is issued** and the corresponding **RAF form is obtained**.
- **Review screenshots or other forms of evidence** that demonstrate retesting was completed for vulnerabilities marked as “closed.”

### Sampling and Cross-Verification
- **Randomly sample** a selection of VAPT reports and associated evidence (e.g., retest screenshots, RAF forms).
- **Cross-verify** the evidence with the inquiry responses to ensure the vulnerability management process is robust and compliant with organizational standards.

---

## Final Audit Review & Reporting

### Compile Findings
- **Summarize the compliance status** of the VAPT process.
- **Document any gaps or non-compliance issues**, such as:
  - Incomplete reporting or retesting.
  - Missing documentation for SLA breaches or RAF forms.
  - Deviations from the established testing methodologies.

### Recommendations
- **Provide clear, actionable recommendations** for:
  - Improving the testing process.
  - Enhancing the vulnerability prioritization and retesting procedures.
  - Strengthening the evidence collection and tracking mechanisms.

### Audit Report Finalization
- **Prepare a final audit report** that includes:
  - An overview of the VAPT control domain.
  - Detailed findings, observations, and areas for improvement.
  - Recommendations and corrective actions.
- **Present the report** to key stakeholders and discuss next steps to ensure continuous improvement in the VAPT process.
