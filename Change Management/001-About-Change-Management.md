# Understanding Change Management in Detail

## 1. What is Change Management?
Change Management (CM) is a preventive control designed to ensure that any modifications to IT systems, applications, and services are controlled, approved, and managed properly. The goal is to minimize risks while maintaining the confidentiality, integrity, and availability of the IT environment.

## 2. Key Components of Change Management
- **Change Management Policy:** The overall guiding principles that dictate how changes should be handled.
- **Change Management Procedure:** The step-by-step process to be followed when making changes.

## 3. Types of Changes in Change Management
Changes in IT environments are classified into three main types:

### A. Standard Change
- These are pre-approved by the **Change Approval Board (CAB)** and occur frequently.
- They are considered **low-risk** and follow a well-documented process.
- Must still be **logged, reviewed, and scheduled** properly.

**Examples:**
- Recurring batch job updates.
- Antivirus updates.

### B. Normal Change
- These changes must follow the complete **Change Management Process** before being implemented.
- They require **logging, review, assessment, scheduling, and approval by CAB** before execution.

**Examples:**
- Cloud configurations.
- Windows security patch update on production servers.

### C. Emergency Change
- These changes are **critical and cannot wait** for the normal release cycle.
- They are necessary when an **unexpected error or security threat** needs immediate attention.

**Examples:**
- Fixing an **SMB port vulnerability (port 445)** after a ransomware attack.
- Addressing a critical flaw in the IT infrastructure.

## 4. Change Management Process Steps

### Step 1: Request for Change (RFC) Submission
- The request can come from various sources:
  - Customers, Auditors, Internal Teams, Security Teams, Management, etc.
- The **requester** (who is requesting the change) creates a **Change Ticket** in tools like **JIRA, ServiceNow, etc.**
- The ticket includes:
  - **Employee details** (who is requesting).
  - **What the change is about** and **why it is needed**.
  - **Request for Change (RFC) Form**, which contains:
    - Application details.
    - Server IPs.
    - Customer name.
    - Implementation date.
- **For production environments, the RFC form is mandatory.**

### Step 2: Change Ticket Assignment
- The **Change Management Team** reviews the request and assigns it to an appropriate resource.

### Step 3: Approval Process (Approval Matrix)
- The following approvals are required before implementation:
  - **Customer Approval**
  - **Manager Approval**
  - **Information Security (GRC) Team Approval**
  - **CAB (Change Advisory Board) Approval**

### Step 4: Change Implementation
- Once approved, the **Change Management Team** starts the implementation.
- The change is **first tested in a lower environment** (development/test/staging) before deployment.

### Step 5: Testing and Validation
- After implementation in the **test environment**, the results are documented.
- The **testing/validation team** conducts a **User Acceptance Test (UAT)** to ensure the change works as expected.

### Step 6: Customer Approval for Production Deployment
- If UAT is **successful**, the **customer’s final approval** is obtained before deploying in production.

### Step 7: Change Deployment in Production
- The change is implemented in **the production environment**, and results are documented.
- A **Production Implementation Report** is prepared.

### Step 8: Post-Implementation Review (PIR)
- A **PIR (Post Implementation Review)** is conducted to verify if the change was successfully implemented.
- If the PIR is successful, the change is considered completed.
- If the PIR **fails**, a **Rollback Plan (RBP)** is initiated to restore the system to its previous state.

## 5. Auditing the Change Management Process

**Audit Period:** January 1st – December 31st.

**Total Change Tickets Processed:** 380.

**Audit Sample:** 25 randomly selected change tickets.

### Audit Checklist - Evidence Collection

✅ Request from **the requester** (Emails, ITSM Ticket, Audit Findings)

✅ **Change Ticket** with all necessary details

✅ **Request for Change (RFC) Form** (mandatory for production)

✅ **Approval Records** (Customer, Manager, GRC, CAB, etc.)

✅ **UAT Reports** (Testing in Lower Environment)

✅ **Validation Reports** (Successful or Failed UAT)

✅ **Production Change Implementation Reports**

✅ **Customer Approval for Production Deployment**

✅ **PIR Documentation** (Who performed it? Findings?)

✅ **Rollback Plan Execution (if applicable)**

✅ **Change Ticket Closure Confirmation**

## 6. Key Control Considerations

- **Integrity Control:** Ensures that all changes are properly recorded, preventing unauthorized modifications.
- **Approval Requirements:** Every change must be approved before being implemented.
- **Proper Documentation:** Every step should be documented, including testing results and post-implementation reviews.
- **Auditable Process:** Change management must be aligned with **ISO standards** and organizational policies.
- **Risk Management:** Emergency changes must be **assessed quickly** but **should still follow documentation and approval processes**.

## 7. Important Considerations for Compliance and Governance

- **Separation of Duties (SoD):**
  - The **Requester, Approver, and PIR Reviewer** should be **different people**.
  - No **self-approval** of changes.
- **Sampling for Audits:**
  - All change requests should be **properly documented and approved**.
  - If approvals or closures are missing, **management must provide justifications**.
- **All Change Tickets Should Have:**
  - Approved status.
  - Proper closure status.
  - Necessary **approvals, implementation logs, and test reports**.

## Conclusion
Change Management is **a crucial process in IT governance** that ensures changes to systems, applications, and services are **controlled, approved, tested, and reviewed** to minimize risks.

By following a structured **change classification, approval workflow, testing, and auditing process**, organizations can ensure that IT changes do not **disrupt business operations or compromise security.**


# Change Implementation Flowchart

```plaintext
Start
  │
  ▼
Request for Change (RFC) Submission
  │
  ▼
Change Ticket Creation (JIRA, ServiceNow, etc.)
  │
  ▼
Change Ticket Assigned to Change Management Team
  │
  ▼
Approval Process (Customer, Manager, InfoSec, CAB)
  │
  ▼
Approved? ────► No ────► Reject/Revise Change
  │
  ▼
Yes
  │
  ▼
Implement Change in Test Environment (Lower Env)
  │
  ▼
Document Results & Conduct Initial Testing
  │
  ▼
User Acceptance Testing (UAT) by Validation Team
  │
  ▼
UAT Successful? ────► No ────► Rollback Plan & Fix Issues
  │
  ▼
Yes
  │
  ▼
Customer Approval for Production Deployment
  │
  ▼
Implement Change in Production Environment
  │
  ▼
Document Production Results
  │
  ▼
Post-Implementation Review (PIR)
  │
  ▼
PIR Successful? ────► No ────► Rollback & Re-evaluate
  │
  ▼
Yes
  │
  ▼
Close Change Ticket
  │
  ▼
End
```
