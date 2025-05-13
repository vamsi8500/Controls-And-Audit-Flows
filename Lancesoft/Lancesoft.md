# ✅ 1. Interested Parties

Interested parties (also called stakeholders) are individuals or groups who have a stake in the organization's information security or its outcomes. Identifying interested parties is a core requirement in ISO 27001:2022 Clause 4.2 and helps define expectations and compliance obligations.

| Type               | Example                                      |
|--------------------|----------------------------------------------|
| Internal Parties   | Employees, management, board                 |
| External Customers | Clients using the product/service            |
| Regulators         | Data protection authorities, FDA             |
| Vendors/Third Parties | Cloud providers, data processors         |
| Auditors/Assessors | ISO auditors, SOC 2 assessors                |

### Why Important?

- Helps align the ISMS or SOC 2 controls with legal, regulatory, and contractual obligations.
- Determines the scope and risk appetite for the security program.

---

# ✅ 2. Term Disclosure

**Term disclosure** refers to the communication of terms and conditions related to privacy, data usage, and service levels between a service provider and its users or clients.

### Common Areas of Disclosure:

- Privacy Policies
- Data Processing Agreements
- Security Terms (e.g., encryption standards, retention policies)
- Subprocessor lists

### Purpose:

- Ensures transparency, a key principle in SOC 2 Privacy and ISO 27001.
- Protects the organization from legal disputes.
- Builds trust with clients and regulators.

---

# ✅ 3. Term Exceptions

**Term exceptions** refer to deviations or exclusions from standard terms or security policies due to business needs or limitations.

### Example:

A customer requests access logs retention for 180 days instead of the standard 90 days. You grant this with proper approval and documentation.

### Key Practices:

- Formal exception approval process
- Risk assessment before granting the exception
- Compensating controls to mitigate associated risk
- Documented and time-bound exception tracking

---

# ✅ 4. What is "Process Integrity" in SOC 2?

**Process Integrity** is a principle under the SOC 2 Trust Services Criteria, primarily aligned with **Processing Integrity (PI).**

### Definition:

Ensures that system processing is complete, valid, accurate, timely, and authorized.

### 🔍 Key Areas under Processing Integrity:

| Control Area        | Description                                         |
|---------------------|-----------------------------------------------------|
| Input validation    | Ensures only correct and authorized data is processed |
| Error detection     | Detects and corrects errors during data processing  |
| Job scheduling      | Ensures jobs run in the correct sequence, on time   |
| Reconciliation      | Verifies that outputs match expected results        |
| Logging and monitoring | Tracks and reviews processing activities       |
| Authorization workflows | Only authorized personnel/processes can modify data |

### 📌 Example:

A financial SaaS provider processes monthly payrolls. The system must:

- Process employee hours correctly (valid & accurate)
- Run payrolls on time (timely)
- Prevent unauthorized changes to salary fields (authorized)

Any failure in this process affects **Processing Integrity**.

---

# ✅ 5. Major Changes in ISO 27001:2022 Revision

### 🆚 Key Changes from ISO 27001:2013 to ISO 27001:2022:

| Area              | ISO 27001:2013                  | ISO 27001:2022 (New)                          |
|-------------------|----------------------------------|------------------------------------------------|
| Control Set       | 114 controls in 14 domains      | 93 controls in 4 themes                        |
| Structure         | Annex A - Linear List           | Annex A - Thematic: Organizational, People, Physical, Technological |
| New Controls      | None                            | 11 new controls                                |
| Control Merging   | Many duplicate/overlapping      | Merged & simplified controls                   |
| Control Attributes| Not defined                     | Optional: For tagging controls (e.g., governance, cloud) |
| Emphasis          | Process control + documentation | Greater emphasis on risk-based, tech-driven controls |

### 📌 Notable New Controls:

- Threat Intelligence
- Data Masking
- Data Leakage Prevention
- Cloud Services Use
- ICT Readiness for Business Continuity

---

# ✅ 6. How Many Samples Are Tested in SOC 2 Type 1 vs Type 2?

| Type     | Description           | Sample Testing Scope                             |
|----------|-----------------------|--------------------------------------------------|
| Type 1   | Point-in-time audit   | No sample testing over time; just verifies control design |
| Type 2   | Over a period (3–12 mo)| Sample testing is required for operating effectiveness |

### 🔍 SOC 2 Type 2 Sample Size Guidelines:

Depends on control frequency:

- Daily → 25–30 samples
- Weekly → 8–12 samples
- Monthly → 3–6 samples
- Quarterly → 1–2 samples

The AICPA expects **evidence sufficient to support assurance** over the audit period.

---

# ✅ Summary Table

| Topic                      | Summary                                                      |
|---------------------------|--------------------------------------------------------------|
| Interested Parties         | Stakeholders affected by ISMS/SOC 2 (e.g., clients, regulators) |
| Term Disclosure            | Communicating service/data/security terms clearly            |
| Term Exceptions            | Documented deviations from standard security terms           |
| Process Integrity (SOC 2)  | Ensures accurate, timely, valid, and authorized system processing |
| ISO 27001:2022 Changes     | 93 controls, 4 themes, new controls like threat intelligence  |
| SOC 2 Type 1/2 Sampling    | Type 1 = design only; Type 2 = sample testing by frequency    |

---

# ✅ How the Control Design is Verified (in SOC 2 Type 1 and Type 2)

Verifying the design of a control means assessing whether the control is properly designed to meet its objective—i.e., if implemented, would it be capable of preventing or detecting a risk related to the applicable Trust Services Criteria (TSCs)?

---

### 🔍 Control Design Verification – SOC 2 Type 1

In a SOC 2 Type 1 audit, the design effectiveness of controls is evaluated at a specific point in time. The auditor checks whether the controls:

- Exist (i.e., are formally documented and in place)
- Are appropriate to mitigate the identified risks
- Align with the Trust Services Criteria (e.g., Security, Availability, Processing Integrity)
- Include clear responsibilities and defined procedures

---

### 🔎 Methods to Verify Control Design:

| Method                  | Purpose                               | Example                                       |
|-------------------------|---------------------------------------|-----------------------------------------------|
| Policy & Procedure Review | Check if documented processes exist | Review access control policy                  |
| Interviewing Personnel  | Understand control intent             | Ask IT Admin how new users are onboarded     |
| Walkthroughs            | Trace a hypothetical scenario         | Simulate onboarding a new employee            |
| System Config Review    | Examine security settings             | Check IAM/firewall configurations             |
| Control Mapping         | Match control to risk/TSC             | Map control to CC6.1 (access control)         |

---

### 📌 What the Auditor Asks:

- Does the control address the specific risk?
- Is the control sufficient to prevent/detect a failure?
- Is it repeatable and not ad-hoc?
- Is the control owned and maintained?

---

### ✅ Example: Verifying Control Design

| Control                             | Design Verification Steps                                               |
|-------------------------------------|-------------------------------------------------------------------------|
| Only authorized users have access   | - Review access policy <br> - Check user provisioning process <br> - Review IAM settings |
| Data is encrypted in transit & rest | - Review encryption policy <br> - Check TLS/storage configs             |
| Backups performed daily             | - Review backup policy <br> - Interview DevOps <br> - Check tool logs   |

---

### 🧠 In SOC 2 Type 2:

- Design is verified first
- Then **operating effectiveness** of the design is tested over time using samples

---

### ✅ Summary

| Aspect              | Type 1                       | Type 2                              |
|---------------------|------------------------------|--------------------------------------|
| Design Verification | Reviewed at a single point   | Reviewed + tested for consistent execution |
| Focus               | Appropriateness and existence| Ongoing effectiveness + evidence     |
