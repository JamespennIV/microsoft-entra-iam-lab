# RBAC Role Assignment Summary

## Purpose

This document summarizes the administrative role assignments used in the Microsoft Entra ID IAM lab.

The purpose of these assignments is to demonstrate least privilege, administrative separation, and realistic IAM delegation.

---

## Role Assignment Table

| Account | Assigned Role | Purpose |
|---|---|---|
| james.admin | Global Administrator | Main lab owner account |
| iam.admin | User Administrator | Manage user lifecycle tasks |
| iam.admin | Groups Administrator | Manage group membership and group-based access |
| helpdesk.tech | Helpdesk Administrator | Simulate help desk identity support tasks |

---

## Security Rationale

### james.admin — Global Administrator

The `james.admin` account is used as the main lab owner. This account has broad permissions and should be protected carefully.

In a real environment, Global Administrator access should be highly restricted, monitored, and preferably managed through just-in-time privileged access.

---

### iam.admin — User Administrator

The `iam.admin` account was assigned the User Administrator role to simulate IAM administration tasks such as:

- Creating users
- Updating user profiles
- Managing user lifecycle tasks
- Supporting onboarding and offboarding scenarios

This role is more limited than Global Administrator and better aligns with least privilege.

---

### iam.admin — Groups Administrator

The `iam.admin` account was also assigned the Groups Administrator role to support group-based access control.

This allows the IAM admin to manage:

- Security groups
- Group memberships
- Department-based access
- Access assignment workflows

---

### helpdesk.tech — Helpdesk Administrator

The `helpdesk.tech` account was assigned the Helpdesk Administrator role to simulate real help desk support tasks.

This role supports lower-risk identity support responsibilities while avoiding unnecessary broad administrative access.

---

## Security Concepts Demonstrated

- Role-Based Access Control
- Least privilege
- Administrative separation
- Delegated administration
- Identity lifecycle management
- Help desk support boundaries

---

## Future Improvements

Future labs may include:

- Privileged Identity Management
- Eligible role assignment
- Just-in-time admin access
- Role activation approval
- Admin access reviews
- Audit log review for privileged actions
