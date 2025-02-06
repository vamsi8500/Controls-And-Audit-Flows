# Data Center Audit Flow

## **STEP 1: Identify the Control Owner via Kickoff Meetings**
- Conduct initial meetings with key stakeholders to understand the ownership and implementation of security controls.
- Identify the **Control Owner (CO)** responsible for the security domain.
- Document the **Control Owner's name, designation, and timestamp** of the meeting for audit tracking.

---

## **STEP 2: Inquiry – Process Related to Governance Control**
In this step, the audit team conducts inquiries with the **Control Owner** to assess governance and compliance.

### **Inquiry Points:**

### **Two-Factor Authentication (2FA) in Data Center:**
- Verify **how 2FA is implemented** for physical access.
- Identify the authentication methods:
  - **Punch Card** – "Something you have"
  - **Retina Scan** – "Something you are"
- Ensure both methods are **working together** to prevent unauthorized access.

### **Visitor & Asset Security Policy (BYOD Policy):**
- **No external devices** should be allowed inside the data center.
- **Mobile Phones:**
  - Must be **sealed**, especially the **camera and ports**.
- **Laptops:**
  - The **camera and ports must be sealed** before entry.
- **Undertaking Forms:**
  - Employees must **sign an undertaking** agreeing that if a **seal is broken, a physical reset** must be performed before re-entering the facility.

---

## **STEP 3: Walkthrough – Testing, Sampling, and Evidence Collection**
The audit team conducts a **walkthrough** to test compliance and collect necessary evidence.

### **Testing Approach:**

#### **Verification of 2FA Implementation:**
- Check the **physical security checkpoints** where punch card and retina scan are used.
- Confirm that **access is granted only** when both authentication factors are satisfied.
- Perform **Negative Testing:**
  - Try using **only a punch card** without retina scan.
  - Ask another person (who is unauthorized) to attempt access with an allowed user’s punch card.
  - **Expected Outcome:** System should **deny access** due to biometric mismatch.

#### **Visitor & Asset Security Compliance:**
- Verify **physical security measures** for visitor devices.
- Ensure BYOD (Bring Your Own Device) policies are followed:
  - Check if **mobile phones and laptops are sealed**.
  - **Randomly sample** undertaking forms signed by employees.
  - If any seal is **broken**, check if a **physical reset was performed** before granting further access.

---

## **STEP 4: Evidence Collection & Compliance Assessment (C&A)**
- **Gather audit evidence** such as:
  - **Access logs** from security systems.
  - **Undertaking forms** for BYOD policy compliance.
  - **CCTV footage** verifying security procedures.
- **Cross-check evidence** against security policies to ensure compliance.
- Identify any **gaps or non-compliance issues** and document findings.

---

## **Final Audit Review & Reporting**
- Prepare an **audit report** summarizing:
  - **Compliance status** of 2FA implementation and physical security.
  - **Any security violations** or non-compliance findings.
  - **Recommendations** for improving security controls.
- Discuss findings with **stakeholders** and ensure corrective actions are implemented.

---
