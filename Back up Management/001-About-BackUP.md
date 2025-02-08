# Backup Management – Detailed Explanation

## What is a Backup?
A backup is a copy of critical data that is stored separately to protect against data loss. If the original data is lost due to system failure, accidental deletion, cyber-attacks, or natural disasters, the backup can be used to restore the data.

## Key Factors to Consider for Data Backup
When planning a backup strategy, the following factors must be considered:

### Backup Frequency & Type
- Determine how often backups should be taken (daily, weekly, monthly).
- Choose the right backup type (full, differential, or incremental).

### Backup Location
- Store backups in multiple locations to prevent data loss due to local disasters.
- Example: Backups stored in different seismic zones to reduce risk.

### Backup Security
- Ensure data is encrypted to protect against unauthorized access.
- Use strict access control for backup storage.

## Types of Backup
Backups are classified into three main types:

### Full Backup
- A complete backup of all selected files and databases.
- Provides the highest level of protection but requires more storage and time.
- **Example**: A full backup of a company's ERP system taken weekly.

### Differential Backup
- Backs up only the files that have changed since the last full backup.
- Requires less space and time than a full backup.
- **Example**: If a full backup was taken on Monday, a differential backup on Wednesday would back up only the changes made on Tuesday and Wednesday.

### Incremental Backup
- Backs up only the files that have changed since the last backup (full or incremental).
- Requires less storage but takes longer to restore data.
- **Example**: If a full backup was taken on Monday, an incremental backup on Wednesday would back up only the changes since the Tuesday backup.

## Backup Schedule & Data Protection
A well-defined backup schedule ensures that critical data is always protected.

### Backup Strategy
- **Full Snapshot Backup**: Taken daily for all cloud-based resources (Databases, Applications, OS, and Configuration settings).
- **Backup Retention**: Backups are kept for 7 days before being overwritten.
- **Backup Timing**: Scheduled to run automatically at 12 AM every day.
- **Backup Monitoring**: The Information Security team monitors backup status (Successful / Failed).
- **Failure Alerts**: If a backup fails, an automated email is sent to the Backup Team (backup@tcs.com).
- **Daily Status Recording**:
  - Backup status is recorded in the Backup Status Register.
  - One Information Security personnel logs the status, and another approves it.

## Backup Schedule Details
| Region / Place | Environment | Type | Data/Resource | Frequency |
|--------------|-------------|------|--------------|----------|
| Ohio | Production | Full Backup (Snapshot) | Database, OS, Application Stack | Daily |
| N. Virginia | Production | Full Backup (Snapshot) | Database, OS, Application Stack | Daily |
| N. California | Production | Full Backup (Snapshot) | Database, OS, Application Stack | Daily |
| Ohio | Development | Full Backup (Snapshot) | Database, OS, Application Stack | Daily |
| Coimbatore | Office Location | Incremental | CCTV Footage | Daily |
| Coimbatore | Office Location | Incremental | Biometric System Data | Daily |
| Cloud-NC | Office Location | Incremental | SharePoint / OneDrive | Daily |
| Cloud-NC | Production | Full Backup (Snapshot) | Firewalls / Switches / Routers | Monthly |

## Backup Failure Handling & Re-run Procedures
If a backup job fails, the System Administrator follows these steps to fix the issue:

| Error Type | Cause | Solution / Re-run Procedure |
|-----------|------|---------------------------|
| Policy Issue | Backup storage is full | 1. Manually cancel the backup job. 2. Increase storage space. 3. Modify backup destination if needed. 4. Restart the backup process. |
| Server Restart | Server restarted accidentally during backup | 1. Wait for the server to restart. 2. Modify the backup job in the backup server. 3. Re-run the backup. |
| Server Crash | Backup server crashed | 1. Reinstall backup software. 2. Reconfigure backup schedule. 3. Restore data from the last successful backup. 4. Restart backup. |

## Backup Review & Storage Management
### Quarterly Backup Review
- The Information Security Manager reviews backup processes every three months.
- Meeting Minutes of Meeting (MOMs) serve as evidence of compliance.

### On-Site Backup Storage
- Backups are stored securely with restricted access.
- Fireproof cabinets are used for external hard drive storage.
- **Cabinet Key Access**: Only Admin Manager and Cyber Security Head have access.

| Environment | Instance Location | Backup Storage Location |
|------------|-----------------|------------------------|
| Production | Noida | Hyderabad |
| Production | N. Virginia | N. California |
| Production | N. California | Ohio |
| Development | Ohio | N. Virginia |

## Why is Restoration Testing Important?
- Ensures that backup data is **readable and functional**.
- Helps detect **backup system issues** before a real data loss occurs.
- Confirms that **data can be restored quickly** when needed.
- Provides **evidence of compliance** for security and audit requirements.

## Backup Control & Compliance Testing
### Control 1: Automated Backup System
- The backup system is configured to run **daily backups automatically**.
- Evidence includes backup **configuration details, schedules, and backup success/failure logs**.

### Control 2: Backup Notification System
- Backup jobs send **email notifications** to the operations team after completion.
- IT Team must **provide past 30 days of backup notifications** as proof.

### Control 3: Data Restoration Testing
- IT personnel must perform **backup restoration testing every quarter**.
- Evidence of tests from **Q1 and Q3 2021** must be provided.
- Must include data specific to **Oracle HFM, Oracle ERP, and other critical systems**.
