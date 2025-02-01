# Control Functions Based on Their Role

## Preventive Controls:
- **Function:** Prevent an incident from occurring.
- **Examples:**
  - Antivirus installation before exposure to threats.
  - User authentication to restrict unauthorized access.

## Detective Controls:
- **Function:** Identify and alert on incidents as they occur.
- **Examples:**
  - Anti-malware software that alerts administrators upon detecting a virus.
  - Ransomware response plans that trigger notifications.

## Corrective Controls:
- **Function:** Limit damage and restore systems after an incident.
- **Examples:**
  - System reset or reimaging after a virus attack (even if it causes data loss).
  - Cybersecurity insurance and revised incident response plans.

## Compensating Controls:
- **Function:** Alternative controls that provide the necessary protection when primary controls are insufficient.
- **Note:** Discussed in greater detail in contexts such as encryption and additional layers of security.

## Deterrent Controls:
- **Function:** Discourage potential attackers or improper behavior.
- **Examples:**
  - Warning signs.
  - Login banners.
  - Auditing measures.
  - Posters or digital signage (e.g., “No Password Sharing” notices).

---

# Controls in the Context of CIA

## Confidentiality Controls:
- **Examples:**
  - Password management.
  - Cryptography (encryption) to protect sensitive data.
  - Communication security measures.

## Integrity Controls:
- **Examples:**
  - Change management.
  - Capacity management.
  - Media handling and asset classification.
  - Inventory control (e.g., tracking backups, management systems).

## Availability Controls:
- **Examples:**
  - Access controls.
  - Authentication measures.
  - Business continuity measures such as backup management, disaster recovery planning, and asset management.

---

# Sampling in Audits: A Comprehensive Breakdown

## I. Introduction to Sampling in Audits
In security and compliance audits, it is often impractical to examine 100% of the available evidence due to time and resource constraints. Instead, auditors use sampling techniques to select a representative portion of the population to draw valid conclusions.

### A. Types of Audits and Sampling Necessity

#### Internal Security Audit
- **Duration:** 3 to 4 days
- **Conducted by:** Internal audit team
- **Objective:** Assess internal compliance with security policies and controls

#### External Security Audit
- **Duration:** Maximum of 3 days
- **Conducted by:** External auditors (e.g., certification bodies)
- **Objective:** Ensure regulatory and standard compliance (e.g., ISO 27001, SOC 2, HIPAA)

### B. Why is Sampling Necessary?
- Auditing every record is unrealistic due to limited time and budget.
- Sampling allows auditors to check a portion of the records while still making accurate assessments.
- Helps achieve audit objectives efficiently by focusing on high-risk areas or randomly selected samples.

---

## II. Types of Sampling Methods
Auditors use two broad types of sampling techniques:

### A. Statistical Sampling
- Uses mathematical and statistical methods to ensure that the selected sample represents the entire population.
- Allows results from the sample to be extrapolated to the whole population with a defined confidence level.
- **Common Statistical Sampling Methods:**
  - Random Sampling – Every item has an equal chance of being selected.
  - Systematic Sampling – Items are selected at fixed intervals (e.g., every 10th record).

### B. Non-Statistical Sampling
- Does not use mathematical models; instead, the selection is based on auditor judgment or convenience.
- Results cannot be extrapolated to the entire population, as the sample may not be truly representative.
- **Common Non-Statistical Sampling Methods:**
  - Haphazard Sampling – Samples are picked arbitrarily, without a defined structure.
  - Judgmental Sampling – The auditor selects items based on their experience and risk assessment.
- **Why do auditors prefer Non-Statistical Sampling?**
  - It is simpler and faster, especially when dealing with smaller populations.
  - Allows flexibility in choosing records that may be high-risk.

---

## III. Common Sampling Methodologies

### 1. Simple Random Generator Sampling (Statistical Sampling)
- Each sample is assigned a serial number.
- A random selection tool (e.g., Excel, online randomizer) is used to pick samples.
- **Example:** If there are **1,000 samples**, the tool randomly picks **25 records** from the total dataset.

### 2. Systematic Sampling (Statistical Sampling)
- Used when a fixed interval-based selection is preferred.
- **Formula:**
  - Interval = Total Population / Sample Size
- **Example:** If there are **1,000 records** and we need **25 samples**, we divide:
  - 1000 ÷ 25 = 40
  - This means selecting every **40th** record (40, 80, 120, etc.).

### 3. Haphazard Sampling (Non-Statistical Sampling)
- The auditor selects samples without assigning numbers or using formulas.
- No structured approach—items are selected from the dataset randomly.
- **Example:** An auditor might casually pick **25 records** from a file of **1,000** without any predefined logic.

### 4. Block Sampling (Non-Statistical Sampling)
- Instead of selecting **random** samples, auditors select a **continuous block** of the most recent records.
- **Example:** If there are **1,000 records**, an auditor may take the **latest 25** (e.g., records **976 to 1,000**).
- Used in scenarios where recent data is **more relevant** for audit purposes.

---

## IV. Determining Sample Size

### A. Key Rules for Sample Size Determination
- **If population size is less than 50 → No sampling is required.**
- **If population size is greater than 50 → Perform sampling using:**
  - **10% of the total population** OR
  - **25 records (whichever is smaller)**

### B. Steps to Determine Sample Size and Methodology
1. **Identify total population data (N):**
   - Count the number of total available records.
2. **Apply sampling formula:**
   - Use **10% of the population or 25 records, whichever is smaller**.
3. **Choose a sampling method:**
   - **Simple Random Sampling** (Random selection using a tool)
   - **Systematic Sampling** (Every nth record)
   - **Haphazard Sampling** (Arbitrary selection by auditor)
   - **Block Sampling** (Most recent records)
4. **Evaluate the sample results:**
   - If all samples **pass the audit criteria**, the control is deemed effective.
   - If any sample **fails**, a **finding or non-conformity** is raised.

---

## V. Case Study: Background Verification (BGV) Audit

### **Scenario:**
- HR department needs to verify **Background Verification (BGV)** reports for new employees.
- **Total new employees during the audit period:** **950**
- **Objective:** Ensure BGV compliance without reviewing all **950 reports**.

### **Audit Approach Using Sampling:**
- **Sample Size:** **10% of 950** = **95** OR **fixed 25 sample rule** → **Select the lower value → 25 samples**

---

## VI. Conclusion
- Proper sample selection ensures a balanced and efficient audit while maintaining compliance and security assurance.
