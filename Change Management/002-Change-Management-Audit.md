# Change Management Audit Process – Detailed Flow

## Objective:
The Change Management audit aims to verify whether all changes to IT systems, applications, and services are controlled, approved, and managed as per the organization’s Change Management Policy. The audit will check compliance with governance controls, approval workflows, testing procedures, and documentation.

## Audit Process Steps

### Step 1: Identify the Control Owner via Kickoff Meetings
- Conduct kickoff meetings to identify the **Control Owner (CO)** responsible for Change Management.
- Verify that **Change Management (CM)** ensures all changes are **controlled, approved, and managed** as per policy.
- Confirm **change classification**:
  - **Standard Change** → Pre-approved by **CAB Team**.
  - **Normal Change** → Follows **full Change Management Process**.
  - **Emergency Change** → Applied immediately (e.g., cyberattacks), approvals obtained post-implementation.

### Step 2: Inquiry – Process Verification & Governance Controls
- Gather the **Change Management Procedure** and confirm compliance.
- Verify the **Change Management Tool**:
  - ITSM (e.g., **ServiceNow, JIRA**) is used for **logging, approving, and reviewing changes**.
- Check the **Change Approval Matrix**:
  - Approvals from **CAB Team, Customer, and Manager**.
- Check for **Post Implementation Review (PIR)**:
  - Who conducts the PIR?
  - How is it documented?
- **Testing Requirements:**
  - Ensure that **UAT Testing** is conducted in a **lower environment** before moving to production.

### Step 3: Walkthrough – Audit, Sampling, & Evidence Collection
1. **Conduct a Walkthrough with the Control Owner (CO):**
   - Document **Name, Designation, and Timestamp** of the meeting.
   - Request access to the **ITSM Dashboard** to list changes from **Feb 2022 – Feb 2023**.
   - Total Changes Logged: **254 Change Tickets** during the audit period.

2. **Verify Closure & Approval Status:**
   - Before sampling, check if **all 254 tickets are closed and approved**.

3. **Perform Sampling:**
   - **Select 25 sample change tickets** for detailed review.
   - For each sampled change, verify:
     - **Request for Change (RFC) Details:**
       - Who requested the change?
       - What was the change?
       - Why was it required?
     - **Approval Process:**
       - Were approvals obtained from **CAB, Customer, and Manager**?
       - Check if approvals are documented.
     - **Separation of Duties (SoD) Compliance:**
       - Ensure different personnel handled:
         - Request submission
         - CAB approval
         - PIR execution
     - **Testing (UAT) and Validation:**
       - Was the change **implemented in a test environment first**?
       - Was **UAT successful or failed**?
     - **Customer Approvals:**
       - Verify customer sign-off before production deployment.
     - **Production Implementation & Documentation:**
       - Confirm that the change was implemented in the production environment.
       - Check production deployment logs.
     - **Post Implementation Review (PIR):**
       - Was the PIR conducted and documented?
     - **Rollback Plan (RBP) Compliance:**
       - If the change failed, was a rollback plan executed properly?

## Audit Flow Diagram

```plaintext
Start Audit  
  │  
  ▼  
Identify Control Owner & Conduct Kickoff Meeting  
  │  
  ▼  
Gather Change Management Procedure & Tool Details  
  │  
  ▼  
Verify Change Classification & Approval Matrix  
  │  
  ▼  
Walkthrough with CO & Review ITSM Dashboard  
  │  
  ▼  
Check Closure & Approval Status of 254 Tickets  
  │  
  ▼  
Select 25 Sample Tickets for Detailed Audit  
  │  
  ▼  
For Each Sampled Ticket:  
  - Verify RFC, Approvals, SoD Compliance  
  - Validate UAT, Testing, and Customer Sign-off  
  - Confirm Production Implementation & Documentation  
  - Check PIR Execution & Rollback Plan (if applicable)  
  │  
  ▼  
Audit Findings & Compliance Report  
  │  
  ▼  
End Audit  
```

## Audit Checklist – Evidence Collection
During the audit, the following evidence should be collected to verify compliance with the Change Management process:

### 1. Request and Approval Evidence
✅ Request from **the requester** (Emails, ITSM Ticket, Audit Findings)  
✅ **Change Ticket** with details (Logged in ITSM)  
✅ **Request for Change (RFC) Form** (Mandatory for production changes)  
✅ **Approval Records** (Customer, Manager, CAB, GRC Team)  

### 2. Implementation and Testing Evidence
✅ **UAT Reports** (Testing in Lower Environment)  
✅ **Validation Reports** (Successful or Failed UAT)  
✅ **Production Change Implementation Reports**  

### 3. Post-Implementation and Compliance Evidence
✅ **Customer Approval for Production Deployment**  
✅ **PIR Documentation** (Who performed it? Findings?)  
✅ **Rollback Plan Execution (if applicable)**  
✅ **Change Ticket Closure Confirmation**  

## Audit Conclusion
At the end of the audit, the findings will determine:

- **Compliance Level:** Whether the Change Management process follows governance policies.
- **Gaps & Risks:** If there are any missing approvals, incomplete UAT, or skipped PIR reviews.
- **Actionable Recommendations:** Steps to improve compliance and process adherence.

By following this structured **audit approach**, organizations ensure that **IT changes are properly managed**, minimizing **risks, downtime, and security threats** while maintaining **process integrity**. 🚀
