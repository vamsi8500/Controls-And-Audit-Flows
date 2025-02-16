# Removable Media Policy – Control Domain: Detailed Audit Flow

## Objective:
To ensure that removable media usage is restricted within the organization, reducing the risk of data loss, malware infections, and unauthorized data transfers.

## STEP 1: Identify the Control Owner via Kickoff Meetings

### Purpose:
- Identify the control owner responsible for enforcing and monitoring removable media policies.
- Establish accountability for policy enforcement and compliance.

### Activities:
#### Schedule a Kickoff Meeting
- Involve key stakeholders such as:
  - IT Security Team
  - Compliance Team
  - System Administrators
  - Control Owner (CO)
- Define roles and responsibilities for each team member.

#### Define Control Ownership
- Identify the Control Owner (CO) who will be responsible for enforcing and maintaining the removable media policy.
- Document their name, designation, and timestamp of assignment.

#### Discuss Removable Media Risks
- Highlight security risks such as data loss, theft, and malware infections.
- Explain the necessity of restricting removable media within the organization.

## STEP 2: Inquiry – Process Related to Disposal and Control

### Objective:
- Understand the existing removable media disposal and control process.
- Verify if removable media usage is already restricted.

### Activities:
#### Conduct Inquiry with Control Owner
- Document the CO’s name, designation, and timestamp of inquiry.
- Discuss current processes for removable media control and disposal.
- Identify any gaps in security controls related to removable media.

#### Check Blockage of Removable Media Usage
- Confirm if removable media is blocked across all endpoints (laptops, desktops, servers).
- Verify whether the blocking mechanism is enforced at the system level.
- Assess whether users have workarounds or exceptions to bypass the policy.

#### Validate the Tools Used for Blocking Removable Media
- Confirm the usage of Jamf or similar tools for removable media restriction.
- Check if policy enforcement settings are correctly applied to all devices.
- Ensure that the security team is monitoring and logging removable media access attempts.

## STEP 3: Walkthrough – Testing, Sampling, and Evidence Collection

### Objective:
- Conduct a walkthrough of security controls to verify the effectiveness of the removable media policy.
- Perform audit testing, sampling, and evidence collection.

### Activities:
#### 1. Review Jamf Configuration
- Verify the Jamf security configuration for removable media restriction.
- Ensure that the policy applies to all users in the organization.
- Check if Jamf logs block events and unauthorized USB usage attempts.

#### 2. Validate the User List and Asset Register
- Cross-check if all employees’ systems are listed in the Jamf configuration.
- Review the Asset Register to ensure that all endpoints (laptops, servers) have the required security configurations.

#### 3. Audit Period and Sampling Criteria
- Define the audit period from **Feb 2022 to Feb 2023**.
- Include **3045 laptops and servers** in the audit.
- Select **25 laptops** as a sample group for detailed verification.
- Capture **screen prints of Jamf tool settings** for evidence.

#### 4. Conduct Negative Testing
- Insert a USB stick into one of the laptops.
- Verify that the system detects but blocks access to the USB device.
- Check that an alert is generated in Jamf logs for unauthorized media access.

#### 5. Gather and Review Evidence
- Collect **screenshots of Jamf configurations and security logs**.
- Document evidence for **Compliance & Assurance (C&A) review**.
- Ensure that findings align with **organizational security policies**.

## Conclusion:
The **removable media audit flow** ensures that **security policies are enforced** and **removable storage devices are effectively blocked**. By following the structured steps of **identifying control owners, conducting inquiries, performing walkthroughs, and validating compliance evidence**, organizations can **mitigate the risks associated with removable media usage**.
