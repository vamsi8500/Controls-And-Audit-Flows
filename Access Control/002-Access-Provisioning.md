## Access Provisioning Principles

Access is granted based on three key principles:

### Role-Based Access Control (RBAC)
- Access is assigned based on job roles.
- **Example:** A manager receives manager-level access.
- like manager have access to development environment and test environment

### Business Justification
- Access is provided based on business needs.
- **Example:** A client requests IP whitelisting, which requires approval before implementation.
- need to mention the purpose for why u want to provision access for that person
- need to raise a request for access-> manager Approve-> complete the task

### Least Privilege
- Users receive only the minimum access required to complete their tasks.
- **Example:** A manager requesting to review database logs gets read-only access.

## Types of Permissions

1. **Read (R)**
   - Allows viewing files but not modifying them.
   - **Example:** A security analyst reviews log files but cannot delete them.

2. **Write (W)**
   - Allows modifying and saving changes.
   - **Example:** A developer writes and updates code in the repository.

3. **Execute (X)**
   - Allows executing files, renaming, and saving changes.
   - **Example:** A system administrator runs shell scripts to restart servers.
