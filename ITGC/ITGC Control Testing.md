# ITGC Control Testing – Access Provisioning, Management, and De-Provisioning

### 🎯 Objective:
Ensure proper control over access provisioning, management, and de-provisioning, guaranteeing that only authorized users can access relevant systems and data.

### ✅ Key Controls in ITGC Access Management

| Control | Type | Description |
|---------|------|-------------|
| User Access Request Process | Preventive | New users must submit a formal request (e.g., ticket, form). |
| Managerial Approval | Preventive | Access is granted only after supervisor/manager approval. |
| Role-Based Access Control (RBAC) | Preventive | Users are assigned roles with predefined permissions. |
| Segregation of Duties (SoD) | Preventive | Users should not have conflicting roles (e.g., request + approve). |
| Documentation of Access Requests | Detective | Maintain records of who requested, approved, and provisioned access. |
| Regular Access Reviews | Detective | Periodic reviews of user access against current job responsibilities. |
| De-Provisioning of Access | Corrective | Access must be removed timely when users no longer need it (e.g., employee leave). |

### 🔍 Control Testing Steps

#### 1. User Access Request Process

| Test Step | Purpose |
|-----------|---------|
| Review a sample of access requests | Confirm that access was formally requested |
| Ensure request submission channels are official | Validate tickets/forms are used and tracked |
| Confirm appropriate roles are requested | Ensure users request correct access level |

#### 2. Managerial Approval

| Test Step | Purpose |
|-----------|---------|
| Review access request logs for managerial approval | Ensure approval is obtained before provisioning |
| Verify approval documentation | Confirm manager has signed off on the access |
| Validate approval timelines | Ensure approval occurred within reasonable time frame |

#### 3. Role-Based Access Control (RBAC)

| Test Step | Purpose |
|-----------|---------|
| Review role definitions | Ensure each role has appropriate permissions |
| Validate role assignment against job descriptions | Confirm users are given access based on roles |
| Test for least privilege | Ensure users only have necessary permissions |

#### 4. Segregation of Duties (SoD)

| Test Step | Purpose |
|-----------|---------|
| Review roles for conflicting duties | Ensure no one role allows conflicting functions (e.g., request + approve access) |
| Identify users with conflicting roles | Spot users with access that violates SoD policy |
| Verify corrective actions are taken | Ensure conflicts are resolved promptly |

#### 5. Documentation of Access Requests

| Test Step | Purpose |
|-----------|---------|
| Verify documentation of requests | Ensure a complete audit trail exists for all requests |
| Ensure requests are stored for audit purposes | Validate compliance with retention policies |
| Check if all required approvals are documented | Ensure all necessary approvals are recorded |

#### 6. Regular Access Reviews

| Test Step | Purpose |
|-----------|---------|
| Review the frequency of access reviews | Ensure periodic reviews are happening as per policy (e.g., quarterly, annually) |
| Sample reviewed access records | Confirm access reviews were completed for a sample of users |
| Validate findings from reviews | Ensure corrections or removals are done when necessary |

#### 7. De-Provisioning of Access

| Test Step | Purpose |
|-----------|---------|
| Sample de-provisioning records | Check if access is removed when users leave, transfer, or change roles |
| Ensure access is revoked immediately upon termination | Confirm that access is revoked as soon as a user is no longer authorized |
| Verify proper documentation for de-provisioning | Ensure records are kept for future audit and compliance |

### 📝 Evidence Collected:
- Access request forms or tickets
- Email/ticket confirming managerial approval
- Access role matrix or RBAC documentation
- SoD analysis or conflict resolution reports
- Regular access review logs
- De-provisioning logs or access termination reports

### ⚠️ Common Findings:
- Access granted without formal request or approval
- Roles not aligned with job responsibilities (excessive permissions)
- Conflicts in duties (e.g., user can both approve and execute transactions)
- Lack of access reviews or outdated access reviews
- Delayed or incomplete de-provisioning (e.g., accounts not disabled after employee termination)

---

# ITGC Control Testing – Change Management & Incident Management

### 🎯 Objective:
Ensure that changes to systems and applications are properly controlled and documented, and that incidents are efficiently managed to minimize risk and restore normal operations.

### ✅ Key Controls in ITGC Change Management

| Control | Type | Description |
|---------|------|-------------|
| Change Request Process | Preventive | All changes must be formally requested and logged in a change management system. |
| Change Approval | Preventive | Changes must be approved by the designated change authority before implementation. |
| Testing & Validation | Preventive | Changes must be thoroughly tested in a controlled environment before being deployed. |
| Change Implementation & Documentation | Preventive | All changes must be implemented as per the approved plan and properly documented. |
| Post-Change Review | Detective | A post-change review must be conducted to ensure the change was successful and does not negatively affect other systems. |
| Segregation of Duties (SoD) | Preventive | Separate roles should be assigned for requesting, approving, and implementing changes. |

### 🔍 Control Testing Steps for Change Management

#### 1. Change Request Process

| Test Step | Purpose |
|-----------|---------|
| Review change request logs | Confirm that all changes are logged in the change management system |
| Verify proper documentation for each change | Ensure request details (purpose, scope, and impact) are recorded |
| Check for completeness of requests | Ensure that all necessary information (e.g., impact, testing plan) is provided |

#### 2. Change Approval

| Test Step | Purpose |
|-----------|---------|
| Verify approval by authorized personnel | Ensure changes are approved by the appropriate authority (e.g., change manager) |
| Check approval timelines | Confirm that approvals occur within the required timeframe |
| Review approval documentation | Ensure approvals are properly documented for auditing purposes |

#### 3. Testing & Validation

| Test Step | Purpose |
|-----------|---------|
| Review testing and validation procedures | Ensure that changes are tested in a non-production environment |
| Check test results | Verify that changes pass necessary tests before implementation |
| Validate change impact analysis | Confirm that any impact on existing systems or operations is evaluated |

#### 4. Change Implementation & Documentation

| Test Step | Purpose |
|-----------|---------|
| Verify implementation against change request | Ensure changes are implemented according to the approved plan |
| Check for proper documentation | Confirm that all changes are fully documented (e.g., time, person responsible, affected systems) |
| Ensure rollback procedures are in place | Confirm that the implementation plan includes rollback steps if issues arise |

#### 5. Post-Change Review

| Test Step | Purpose |
|-----------|---------|
| Verify completion of post-change reviews | Ensure that reviews are conducted after each change to assess success and any unintended effects |
| Confirm corrective actions from post-change review | Ensure corrective actions are taken if problems are identified |

#### 6. Segregation of Duties (SoD)

| Test Step | Purpose |
|-----------|---------|
| Ensure segregation of roles in the change process | Validate that different individuals are involved in requesting, approving, and implementing changes |
| Review SoD conflicts | Check that no one individual is responsible for all three roles (requesting, approving, implementing) |

### ✅ Key Controls in ITGC Incident Management

| Control | Type | Description |
|---------|------|-------------|
| Incident Response Plan | Preventive | A formal incident response plan must be in place to address potential security or operational incidents. |
| Incident Reporting Process | Preventive | Employees must report incidents promptly and through a predefined process (e.g., helpdesk, ticketing system). |
| Incident Categorization & Prioritization | Preventive | Incidents must be categorized and prioritized based on severity and impact. |
| Incident Investigation & Resolution | Detective | Investigations must be conducted to understand the cause and implement resolutions. |
| Incident Documentation | Detective | All incidents must be thoroughly documented, including steps taken and resolution. |
| Post-Incident Review | Detective | A post-incident review must be conducted to identify lessons learned and improve future responses. |

### 🔍 Control Testing Steps for Incident Management

#### 1. Incident Response Plan

| Test Step | Purpose |
|-----------|---------|
| Review incident response plan | Ensure the plan covers all potential incident scenarios |
| Test plan effectiveness | Verify that the plan has been tested through simulations or real incidents |
| Check for updates | Confirm that the plan is updated regularly to reflect new threats or changes in infrastructure |

#### 2. Incident Reporting Process

| Test Step | Purpose |
|-----------|---------|
| Verify reporting channels | Ensure incidents can be reported through multiple channels (e.g., email, ticketing system) |
| Check for timely incident reports | Confirm that incidents are reported promptly after identification |
| Review incident log entries | Ensure all incidents are logged with sufficient details |

#### 3. Incident Categorization & Prioritization

| Test Step | Purpose |
|-----------|---------|
| Review incident categorization process | Ensure incidents are categorized based on their impact and urgency |
| Check prioritization alignment with severity | Confirm that higher-priority incidents are addressed more quickly |
| Verify consistency across incidents | Ensure incidents are categorized and prioritized consistently |

#### 4. Incident Investigation & Resolution

| Test Step | Purpose |
|-----------|---------|
| Ensure investigations are thorough | Verify that the root cause is identified for each incident |
| Review resolution timelines | Confirm that incidents are resolved within the defined service level agreements (SLAs) |
| Check for corrective actions | Ensure that the proper actions are taken to prevent recurrence of similar incidents |

#### 5. Incident Documentation

| Test Step | Purpose |
|-----------|---------|
| Ensure complete incident records | Verify that all relevant details are recorded (e.g., time, actions taken, results) |
| Check for post-resolution follow-up documentation | Ensure that any follow-up actions are documented and tracked |

#### 6. Post-Incident Review

| Test Step | Purpose |
|-----------|---------|
| Verify post-incident reviews are conducted | Confirm that reviews take place after major incidents to assess the response |
| Ensure lessons learned are documented | Check that findings from the review are documented and shared for future improvements |
| Verify corrective actions are implemented | Ensure that any improvements from the review are put into practice to prevent recurrence |

### 📝 Evidence Collected:
- Change request logs, approvals, and documentation
- Incident response plans and test results
- Incident logs, reports, and categorization
- Documentation of incident investigations and resolutions
- Post-incident reviews and follow-up actions

### ⚠️ Common Findings:
- Lack of approval or incomplete change requests
- Inadequate testing or validation before change deployment
- Missing documentation or incomplete post-change reviews
- Delayed incident reporting or categorization errors
- Inconsistent incident investigations or follow-up actions

---

### Summary:
ITGC Change Management ensures that all changes are documented, approved, and tested to minimize operational risks, while Incident Management helps organizations swiftly detect, respond to, and learn from incidents to prevent future occurrences.
