# Microsoft Entra ID IAM Lab

## Project Overview

This project documents a hands-on Microsoft Entra ID Identity and Access Management lab built inside an Azure for Students tenant. The lab simulates a small organization called **Penn Identity Labs** and demonstrates practical IAM concepts including user lifecycle management, security groups, group-based access control, administrative role assignment, RBAC, least privilege, and IAM documentation.

The original plan was to create a dedicated Microsoft Entra workforce tenant. However, tenant creation was denied because the Azure for Students account did not have a paid subscription. To continue the lab safely and avoid unnecessary cost, the project was redesigned to use the existing Azure for Students tenant as the identity environment.

---

## Business Scenario

**Penn Identity Labs** is a simulated organization with users across IT, IAM Administration, Help Desk, HR, Finance, Sales, Contractors, and Terminated Users.

The organization needs a basic Microsoft Entra ID identity structure to support:

* User provisioning
* User deprovisioning
* Department-based access
* Help desk delegation
* IAM administration
* Least-privilege role assignment
* Future Conditional Access and privileged access workflows

---

## Lab Objectives

* Use an existing Azure for Students tenant as a Microsoft Entra ID lab environment
* Create a realistic simulated organization structure
* Create fake users for admin, help desk, HR, Finance, Sales, contractor, and terminated-user scenarios
* Create security groups for department-based access control
* Assign users to groups based on business role
* Assign administrative roles using least privilege
* Document the configuration with sanitized screenshots
* Build a portfolio-ready IAM case study

---

## Tools Used

* Microsoft Azure
* Microsoft Entra ID
* Azure for Students
* Entra Admin Center
* GitHub
* Markdown documentation

---

## Skills Demonstrated

* Identity lifecycle management
* User provisioning
* Group-based access control
* Role-Based Access Control
* Least privilege
* Administrative separation
* Help desk delegation
* IAM documentation
* Security portfolio development

---

## Lab Architecture

```text
Azure for Students Tenant
│
└── Penn Identity Labs — Simulated Organization
    │
    ├── Admin Accounts
    │   ├── james.admin
    │   ├── iam.admin
    │   └── helpdesk.tech
    │
    ├── Department Users
    │   ├── hr.user1
    │   ├── finance.user1
    │   └── sales.user1
    │
    ├── Special User Types
    │   ├── contractor.user
    │   └── terminated.user
    │
    └── Security Groups
        ├── SG-HR-Employees
        ├── SG-Finance-Employees
        ├── SG-Sales-Employees
        ├── SG-IT-Helpdesk
        ├── SG-IAM-Admins
        ├── SG-Contractors
        └── SG-Terminated-Users
```

---

## Lab Status

* [x] Existing Azure for Students tenant confirmed
* [x] Lab users created
* [x] Security groups created
* [x] Users assigned to groups
* [x] Basic admin roles assigned
* [ ] Screenshots sanitized and uploaded
* [ ] Lab documentation finalized
* [ ] Future labs added

---

## Completed Labs

| Lab | Description | Status |
|---|---|---|
| [Lab 01](labs/01-existing-tenant-setup.md) | Existing Tenant IAM Environment Setup | Complete |
| Lab 02 | User Onboarding and Offboarding | Planned |
| Lab 03 | RBAC and Admin Role Delegation | Planned |
| Lab 04 | MFA and Conditional Access | Planned |
| Lab 05 | Privileged Identity Management | Planned |
| Lab 06 | Access Reviews | Planned |
| Lab 07 | Suspicious Sign-In Review | Planned |

---

## Security Note

All screenshots used in this repository are sanitized before upload. Sensitive information such as tenant IDs, subscription IDs, personal email addresses, temporary passwords, MFA methods, billing details, and authentication secrets are removed or blurred.

---

## Key Takeaway

This project demonstrates that even without a paid Azure subscription or dedicated tenant, an existing Azure for Students tenant can be used to build a practical Microsoft Entra ID IAM lab. The value of the project comes from realistic identity design, security reasoning, documentation quality, and the ability to explain IAM decisions clearly.
