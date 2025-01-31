# Access Control Audit

## Access Control Audit: JML Process (Provisioning, De-provisioning, Re-certification)

### Control Domain: Logical Access

### Step 1: Identify the Control Owner (CO) via Kickoff Meetings

#### JML Process:
- **Joining** – Granting access to new employees.
- **Leaving** – Removing access when employees leave.
- **Moving** – Modifying access when employees switch roles/projects.

**Action:** Identify the Control Owner (CO) and document their **Name, Designation, and Timestamp** of the meeting.

---

### Step 2: Inquiry – Process Related to Disposal Control

#### Key Questions to Ask the Control Owner (CO):

**Access Procedure Documentation**
- Is there a documented process for provisioning, de-provisioning, and modifying access?

**Tool Usage**
- Is an automated tool used for access management? (e.g., CyberArk)

#### Process Flow
- **Joining:** HR Email → Respective Department → Access Provisioning
- **Leaving:** HR Email → Respective Department → De-provisioning within **48 hours**
- **Moving:**  
  - **Project A to Project B** → Revoke access for Project A (within **24 hours**)
  - Grant access for Project B

---

### Step 3: Walkthrough – Testing, Sampling, and Gathering Evidence

- Conduct **walkthroughs with CO** and record the **Name, Designation, and Timestamp**.
- **Audit Period:** **Feb 2022 – Feb 2023**
   Access shoud be granted only after approval Date
   here access requestor and approver should be different as part of (seggrigation of duties)
#### Evidence Collection & Validation
- Gather supporting evidence through:
  - Review of **Master List** for new joiners.
  - **Active Directory (AD) Active User Listings** verification.
  - Screenshots of **queries and access logs**.
  - Email correspondence from HR to the Network team.
  - Cross-checking exit lists with AD records to ensure **de-provisioning** is completed timely.

---
