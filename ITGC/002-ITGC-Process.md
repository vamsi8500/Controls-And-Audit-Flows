# IT General Controls (ITGC) Audit Documentation

## 1. Access Management Controls

### 1.1 Periodic Access Review
**Evidence to Gather:**
- System-generated access review logs for general and privileged users.
- Evidence of validation for completeness and accuracy of the user access listing.
- Review sign-off from authorized personnel.
- Documentation of remediation actions taken for identified issues.

**Process to Gather Evidence:**
1. Retrieve the most recent system-generated user access listing.
2. Verify the listing includes all active and inactive users.
3. Check if an independent review was conducted by the appropriate owner.
4. Ensure sign-off documentation exists for the review process.
5. Capture evidence that any discrepancies found were addressed and remediated.

### 1.2 User Access Creation & Modification
**Evidence to Gather:**
- System-generated report for all user creation and modification activities.
- Authorization matrix detailing approval levels.
- Formal approval documentation (email approvals, ticketing system logs).
- System access request forms for new users.

**Process to Gather Evidence:**
1. Extract the user access creation/modification logs from the system.
2. Cross-check against approval documentation in the ticketing system.
3. Ensure access modifications align with the authorization matrix.
4. Verify if access was granted as per request and within the defined SLA.
5. Document any deviations and evidence of corrective actions.

### 1.3 User Access Revocation
**Evidence to Gather:**
- System-generated report of deleted/disabled users, including timestamps.
- List of terminated/transferred employees.
- Logs showing user access was revoked on time.
- Periodic audit reports of inactive accounts.

**Process to Gather Evidence:**
1. Retrieve the employee termination/transfers list from HR.
2. Extract system logs for user deactivation, ensuring matching timestamps.
3. Confirm that access was revoked in a timely manner after termination.
4. Validate if periodic audits of inactive accounts are performed.
5. Collect documentation showing any follow-ups on late revocations.

### 1.4 Privileged Access Review
**Evidence to Gather:**
- System-generated list of privileged users and their access rights.
- Evidence of periodic review of privileged access.
- Documentation of review approvals and actions taken on findings.
- Logs of privileged access usage.

**Process to Gather Evidence:**
1. Obtain the latest system-generated privileged user list.
2. Validate that the list is complete and accurate.
3. Check if privileged access logs are reviewed periodically.
4. Verify if any unauthorized privileges were detected and corrected.
5. Collect approval documentation from security or risk teams.

### 1.5 Password Configuration
**Evidence to Gather:**
- Documented password policy.
- System-generated password configuration report.
- Results of negative testing (e.g., attempts to set weak passwords).
- Logs of password policy violations and corrective actions.

**Process to Gather Evidence:**
1. Retrieve the password policy document.
2. Generate a system report showing password configuration settings.
3. Perform a negative test to ensure weak passwords are rejected.
4. Validate that password settings align with policy requirements.
5. Capture evidence of exceptions and actions taken.

## 2. Change Management Controls

### 2.1 Access to Production Migration
**Evidence to Gather:**
- System-generated list of developers and migrators with access to production.
- Evidence of access modifications with authorization details.
- Logs of production deployments with approvals.

**Process to Gather Evidence:**
1. Generate a list of users with access to production systems.
2. Verify access approvals against the authorization matrix.
3. Ensure access is restricted only to authorized personnel.
4. Validate if production migration approvals are documented.
5. Document any unauthorized access findings and remediation steps.

### 2.2 Change Management
**Evidence to Gather:**
- System-generated report of changes, including timestamps.
- Authorization matrix and approval documentation.
- UAT sign-off evidence before production deployment.
- Change rollback plan documentation.

**Process to Gather Evidence:**
1. Extract a report of changes made to production systems.
2. Verify approvals exist for all changes per the authorization matrix.
3. Ensure UAT testing evidence and approvals are available.
4. Check if rollback plans exist for major changes.
5. Capture any unapproved changes and corrective actions taken.

## 3. Incident Management Controls

### 3.1 Incident Management
**Evidence to Gather:**
- Incident management policy.
- List of incident tickets, including severity levels.
- Root Cause Analysis (RCA) reports for major incidents.
- Logs of incident resolution and corrective measures.

**Process to Gather Evidence:**
1. Obtain the latest incident management policy document.
2. Extract a list of incidents reported within the audit period.
3. Verify if incidents were resolved within SLA timelines.
4. Ensure RCA reports exist for critical incidents.
5. Document any unresolved incidents and follow-up actions.

## 4. Backup & Recovery Controls

### 4.1 Backup and Recovery
**Evidence to Gather:**
- Backup and restoration policy.
- System logs showing backup jobs and failures.
- Evidence of successful restoration for selected backup requests.
- Backup failure resolution logs.

**Process to Gather Evidence:**
1. Obtain the organization's backup policy.
2. Retrieve logs of scheduled backup jobs.
3. Verify if failed backups were identified and resolved.
4. Perform a test restoration to confirm backup integrity.
5. Capture documentation of restoration results.

## 5. Job Scheduling Controls

### 5.1 Batch Job Management
**Evidence to Gather:**
- System-generated list of scheduled jobs.
- List of authorized personnel who can modify job schedules.
- Logs of failed batch jobs and evidence of resolution.
- Documentation of job execution failures and corrective actions.

**Process to Gather Evidence:**
1. Extract a system report listing all scheduled jobs.
2. Validate if jobs align with operational requirements.
3. Verify logs for failed jobs and evidence of troubleshooting.
4. Ensure only authorized personnel can modify jobs.
5. Document any unauthorized changes or failures and corrective actions.
