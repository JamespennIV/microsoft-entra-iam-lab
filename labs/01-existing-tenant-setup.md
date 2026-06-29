# Lab 01: Existing Tenant IAM Environment Setup

## Objective

Use an existing Azure for Students tenant to create a simulated Microsoft Entra ID IAM environment for portfolio-based identity and access management practice.

---

## Scenario

The original plan was to create a dedicated Microsoft Entra workforce tenant for **Penn Identity Labs**. Tenant creation was denied because the Azure for Students account did not have a paid subscription.

To continue the lab safely and avoid unnecessary cost, the existing Azure for Students tenant was used as the identity environment. A simulated company structure was then created inside the tenant using fake users, security groups, and administrative role assignments.

---

## Environment

| Component         | Description                                           |
| ----------------- | ----------------------------------------------------- |
| Cloud Platform    | Microsoft Azure                                       |
| Identity Platform | Microsoft Entra ID                                    |
| Subscription Type | Azure for Students                                    |
| Lab Organization  | Penn Identity Labs                                    |
| Lab Type          | Simulated IAM environment                             |
| Primary Focus     | IAM foundation, user lifecycle, RBAC, least privilege |

---

## Steps Performed

1. Signed in to the Microsoft Entra admin center.
2. Confirmed access to the existing Azure for Students tenant.
3. Created fake lab users for admin, help desk, HR, Finance, Sales, contractor, and terminated-user scenarios.
4. Created department-based security groups.
5. Added users to their appropriate groups.
6. Assigned basic administrative roles using least privilege.
7. Captured screenshots for portfolio documentation.

---

## Users Created

| User Principal Name | Display Name     | Purpose                                    |
| ------------------- | ---------------- | ------------------------------------------ |
| james.admin         | James Admin      | Main lab owner / administrator             |
| iam.admin           | IAM Admin        | Identity administration practice account   |
| helpdesk.tech       | Helpdesk Tech    | Help desk role practice account            |
| hr.user1            | HR User One      | HR department test user                    |
| finance.user1       | Finance User One | Finance department test user               |
| sales.user1         | Sales User One   | Sales department test user                 |
| contractor.user     | Contractor User  | Contractor access test account             |
| terminated.user     | Terminated User  | Offboarding and disabled-account test user |

---

## Security Groups Created

| Group Name           | Purpose                                       |
| -------------------- | --------------------------------------------- |
| SG-HR-Employees      | Group for HR department users                 |
| SG-Finance-Employees | Group for Finance department users            |
| SG-Sales-Employees   | Group for Sales department users              |
| SG-IT-Helpdesk       | Group for help desk personnel                 |
| SG-IAM-Admins        | Group for IAM administrators                  |
| SG-Contractors       | Group for contractor accounts                 |
| SG-Terminated-Users  | Group for terminated or disabled user testing |

---

## Group Memberships

| Group                | Members         |
| -------------------- | --------------- |
| SG-HR-Employees      | hr.user1        |
| SG-Finance-Employees | finance.user1   |
| SG-Sales-Employees   | sales.user1     |
| SG-IT-Helpdesk       | helpdesk.tech   |
| SG-IAM-Admins        | iam.admin       |
| SG-Contractors       | contractor.user |
| SG-Terminated-Users  | terminated.user |

---

## Administrative Role Assignments

| Account       | Role                   | Reason                                          |
| ------------- | ---------------------- | ----------------------------------------------- |
| james.admin   | Global Administrator   | Main lab owner account                          |
| iam.admin     | User Administrator     | Practice identity lifecycle administration      |
| iam.admin     | Groups Administrator   | Practice group management and access assignment |
| helpdesk.tech | Helpdesk Administrator | Practice help desk identity support tasks       |

---

## Security Concepts Practiced

* Tenant usage and identity environment planning
* User provisioning
* Security group creation
* Group-based access control
* Role-Based Access Control
* Least privilege
* Administrative separation
* Help desk delegation
* IAM documentation

---

## Evidence

Screenshots for this lab are stored in:

```text
/screenshots/lab-01-tenant-users-groups/
```
| Screenshot                                                                                                                     | Description                              |
| ------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------- |
| [01-tenant-overview.png](../screenshots/lab-01-tenant-users-groups/01-tenant-overview.png)                                     | Existing Microsoft Entra tenant overview |
| [02-lab-users-created.png](../screenshots/lab-01-tenant-users-groups/02-lab-users-created.png)                                 | Lab users created in Microsoft Entra ID  |
| [03-sample-user-profile.png](../screenshots/lab-01-tenant-users-groups/03-sample-user-profile.png)                             | Example user profile                     |
| [04-security-groups-created.png](../screenshots/lab-01-tenant-users-groups/04-security-groups-created.png)                     | Security groups created                  |
| [05-hr-employee-group-membership.png](../screenshots/lab-01-tenant-users-groups/05-hr-employee-group-membership.png)                   | HR group membership                 |
| [06-iam-admins-group-membership.png](../screenshots/lab-01-tenant-users-groups/06-iam-admins-group-membership.png)             | IAM admins group membership              |
| [07-roles-and-administrators.png](../screenshots/lab-01-tenant-users-groups/07-roles-and-administrators.png)                   | Roles and administrators page            |
| [08-global-administrator-assignment.png](../screenshots/lab-01-tenant-users-groups/08-global-administrator-assignment.png)         | Global Administrator role assignment       |
| [09-user-administrator-assignment.png](../screenshots/lab-01-tenant-users-groups/09-user-administrator-assignment.png)     | User Administrator role assignment     |
| [10-groups-administrator-assignment.png](../screenshots/lab-01-tenant-users-groups/10-groups-administrator-assignment.png) | Groups Administrator role assignment   |
| [11-helpdesk-administrator-assignment.png](../screenshots/lab-01-tenant-users-groups/11-helpdesk-administrator-assignment.png) | Helpdesk Administrator role assignment   |
| [12-final-lab01-environment-state.png](../screenshots/lab-01-tenant-users-groups/12-final-lab01-environment-state.png)         | Final completed Lab 01 environment state |


---

## Outcome

A simulated Microsoft Entra ID IAM environment was successfully created inside an existing Azure for Students tenant. The lab is ready for future IAM exercises, including onboarding, offboarding, Conditional Access, Privileged Identity Management, access reviews, and privileged access workflows.

---

## Lessons Learned

A dedicated Microsoft Entra tenant is useful but not always required for entry-level IAM practice. When tenant creation is restricted, an existing Azure for Students tenant can still be used to simulate an identity environment and practice core IAM concepts.

The most important portfolio value comes from:

* Clear documentation
* Realistic scenarios
* Sanitized evidence
* Least-privilege reasoning
* Ability to explain the security purpose behind each configuration
