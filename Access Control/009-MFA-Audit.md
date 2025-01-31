# Multi-Factor Authentication (MFA) – Audit Flow

## Objective
Enhance authentication security for all critical resources by enforcing MFA across users and systems.

---

## STEP 1: Identify the Control Owner (CO) via Kickoff Meetings
- Conduct a Kickoff Meeting to identify the Control Owner (CO) responsible for MFA implementation.
- Document CO’s Name, Designation, and Timestamp for accountability.

---

## STEP 2: Inquiry – MFA Implementation Process
Engage with the Control Owner to understand the MFA implementation process.

### Key Questions to Address:
1. **Access Procedure Document**
   - Does a documented MFA enforcement policy exist?
   - Are you using a tool to implement MFA?
     - Confirm the MFA tool (e.g., OKTA, Microsoft Authenticator, Duo Security).
2. **MFA Enforcement**
   - Are all employees enforced with MFA?
     - Ensure MFA is applied to all employees and privileged users.
     - Identify any exceptions and their approval process.

---

## STEP 3: Walkthrough – Audit, Testing & Evidence Collection
### Walkthrough Session with the Control Owner
- Record CO’s Name, Designation, and Timestamp.
- Validate MFA enforcement for the audit period (Feb 2022 – Feb 2023).

### Testing & Evidence Gathering
1. **OKTA (or other MFA tool) Configuration Review**
   - Check MFA enforcement settings in OKTA.
   - Verify MFA is applicable to all users and groups.
   - Identify any users or groups exempted from MFA and document.
2. **MFA Authentication Testing**
   - Ask users to log in and verify the MFA workflow:
     1. **First Factor**: Password (What you know).
     2. **Second Factor**: OTP via mobile/email (What you have).

3. **Sampling & Evidence Collection**
   - System reports showing MFA logs and enforcement.
   - User authentication logs verifying MFA usage.
   - Incident records (if any users bypassed MFA due to system issues).
   - Screenshots or audit logs of MFA configurations.
