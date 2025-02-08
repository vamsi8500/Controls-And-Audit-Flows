# Backup Management – Control Domain

Backup management ensures data protection and recovery in case of system failures or disasters. This process involves identifying responsible personnel, verifying backup procedures, and conducting regular audits.

## Step 1: Identify the Control Owner
- Conduct **Kickoff Meetings** to identify the **Control Owner (CO)** responsible for managing backups.
- **Key factors to consider for data backup:**
  - **Backup Frequency & Type**: How often backups are taken (Daily, Weekly, Monthly).
  - **Backup Location**: Ensure backups are stored in different seismic zones for safety.
  - **Backup Security**: Use encryption and access controls to protect data.

### Types of Backup
There are three main types of backups:
1. **Full Backup**: A complete copy of all data.
2. **Differential Backup**: Copies only files changed since the last full backup.
3. **Incremental Backup**: Copies only files changed since the last backup (Full or Incremental).

## Step 2: Inquiry – Understanding the Backup Process
This step involves gathering details from the Control Owner through interviews and reviewing backup procedures.

### Inquiry Checklist
#### Identify the Control Owner
- **Name**
- **Designation**
- **Timestamp of Inquiry**

#### Review Backup Procedures
- Examine the **Backup Procedure Document** to ensure a well-defined strategy.
- Verify if any **automated backup tools** are used (e.g., Veeam, Azure Backup).
- Confirm **backup frequency, location, and type**.

#### Backup Configuration Details
- Scheduled **backup time** and **retention period**.
- **Distribution List (DL)** for backup notifications.
- **Backup success/failure logs**.
- **Email notifications** for failed backups.

#### Handling Backup Failures
- What actions are taken if a **backup fails**?
- **Re-run process** to restart the backup.

#### Backup Restoration Testing
- Backups must be **tested quarterly (Q1, Q2, Q3, Q4)** to ensure data can be restored successfully.

## Step 3: Walkthrough – Auditing the Backup Process
This step involves **testing, evidence collection, and verification** of backup procedures.

### Walkthrough Checklist
#### Identify the Control Owner
- **Name**
- **Designation**
- **Timestamp of Audit**

#### Review Backup Records for the Audit Period
- **Audit period**: February 2022 – February 2023.
- Examine **backup configurations and system dashboards**.
- Verify **scheduled backup jobs and automation**.

#### Check Backup Notifications & Monitoring
- Confirm if **email notifications** are configured for successful and failed backups.
- Ensure **backup monitoring** is actively performed.

#### Validate Data Restoration Process
- Verify **restoration logs** to ensure backups can be recovered.
- **Preserve evidence** of successful restorations as part of the audit.

## Summary
- Identify and verify the **Control Owner** responsible for backups.
- Review **backup frequency, security, and automated tools** used.
- Check for **proper notifications, monitoring, and failure handling**.
- Conduct **quarterly restoration testing** to confirm data recovery reliability.
- Gather **audit evidence** to ensure compliance with backup policies.
