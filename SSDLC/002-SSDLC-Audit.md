# SSDLC Audit Flow

The audit of Separation of Development, Test, and Production Environments ensures that organizations follow best practices to maintain the confidentiality, integrity, and availability of information assets. This control helps in preventing unauthorized access, accidental modifications, and security risks due to environment mixing.

The audit process follows a structured approach with three key steps:

## Step 1: Identifying the Control Owner via Kickoff Meetings

The first step in the audit process is to identify the control owner (CO), who is responsible for ensuring the separation of environments. This is done through kickoff meetings, where auditors and relevant stakeholders discuss:

- The scope of the audit.
- The responsible personnel for implementing and maintaining the separation of environments.
- The current security policies and procedures in place.

### Outcome:
Identify the Control Owner (CO) with their Name, Designation, and Timestamp for documentation.

## Step 2: Inquiry – Process Related to Disposal Control

In this step, auditors conduct an inquiry with the Control Owner (CO) to understand how the organization ensures separation between Development, Test, and Production environments. The goal is to verify whether assets and environments are properly segregated.

### Key Questions to Ask During Inquiry:

#### Separation of Environments:
- How do you ensure that Development, Test, and Production environments remain separate?
- What policies or guidelines are in place for environment segregation?

#### Separation of Assets:
- Are the assets (servers, databases, storage, etc.) also separated for each environment?
- How are access permissions and roles managed across environments?

### Evidence Collected:
Document the responses from CO along with their Name, Designation, and Timestamp to ensure accountability.

## Step 3: Walkthrough – Testing, Sampling, and Gathering Evidence

The walkthrough phase involves validating the separation controls through testing, sampling, and evidence collection. The auditor reviews the actual implementation of the separation policy by inspecting system configurations, access controls, and network setups.

### Key Areas to Examine:

#### Application-Level Separation
- Review how applications are deployed in different environments.
- Validate application links and ensure they correspond to the correct environment:
  - Development Environment → [https://developer.salesforce.com/](https://developer.salesforce.com/)
  - Testing Environment → [https://test.salesforce.com/](https://test.salesforce.com/)
  - Production Environment → [https://login.salesforce.com/?locale=uk](https://login.salesforce.com/?locale=uk)
- Collect screen prints of the environments to verify segregation.

#### Asset-Level Separation
- Verify if assets are documented in an Asset Register and categorized by environment.
- Check how the organization manages asset location and segregation at different levels:
  - Asset Register → Review logs of assets assigned to Dev, Test, and Prod.
  - Asset Location → Validate asset tagging and deployment locations.
  - Server Separation → Ensure production databases are not accessible from non-production environments.
  - Network Devices → Confirm that firewalls, VLANs, and access controls restrict movement between environments.

### Evidence Collection:
- Screenshots of environment segregation from system settings.
- Asset register extracts to validate asset categorization.
- Change management logs showing restricted movement of data/code across environments.
- Access control logs confirming users are assigned only to their relevant environments.

## Final Audit Assessment: Evidence Collection & Compliance Analysis (C&A)

After the walkthrough and evidence collection, auditors analyze the data to check compliance with the organization's information security policies and regulatory requirements (e.g., ISO 27001: A.14.2.2 – System Change Control Procedures).

### Audit Compliance Decision:
- **Compliant** → If evidence confirms proper separation and security controls are in place.
- **Partially Compliant** → If some separation exists, but there are gaps (e.g., shared databases between environments).
- **Non-Compliant** → If no clear separation exists, leading to security risks.
