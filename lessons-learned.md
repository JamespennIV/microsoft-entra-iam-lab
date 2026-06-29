# **Lessons Learned**

## Overview

This document summarizes the main lessons learned while building the Microsoft Entra ID IAM lab using an Azure for Students tenant.

---

## 1. Tenant Creation May Be Restricted

The original plan was to create a new dedicated Microsoft Entra workforce tenant. However, tenant creation was denied because the Azure for Students account did not have a paid subscription.

This required redesigning the lab to use the existing tenant.

### Lesson

IAM labs should be flexible. A separate tenant is ideal, but an existing student tenant can still support useful hands-on practice if the configuration is documented clearly and sensitive information is protected.

---

## 2. A Simulated Organization Can Still Demonstrate Real IAM Skills

Even without a separate tenant, it was possible to build a realistic simulated company structure using:

* Fake users
* Department groups
* Admin accounts
* Help desk accounts
* Contractor accounts
* Terminated-user scenarios

### Lesson

Portfolio labs do not need to be production environments. They need to show clear technical reasoning, realistic design, and security awareness.

---

## 3. Group-Based Access Is Central to IAM

Instead of thinking about access one user at a time, this lab used department-based security groups such as:

* SG-HR-Employees
* SG-Finance-Employees
* SG-Sales-Employees
* SG-IT-Helpdesk
* SG-IAM-Admins
* SG-Contractors

### Lesson

In real IAM environments, access is often managed through groups, roles, and policies rather than individual manual assignments.

---

## 4. Least Privilege Matters

Administrative roles were separated by function:

* Global Administrator for the main lab owner
* User Administrator for identity lifecycle tasks
* Groups Administrator for group management
* Helpdesk Administrator for help desk support tasks

### Lesson

Administrative access should be assigned based on job responsibility, not convenience. This reduces risk and supports least privilege.

---

## 5. Documentation Is Part of the Skill

The lab was designed not only to practice configuration, but also to create portfolio evidence.

Good IAM documentation should explain:

* What was configured
* Why it was configured
* What security principle it demonstrates
* What evidence proves it was completed
* What sensitive information was removed before publishing

### Lesson

Being able to document security work clearly is a major professional skill, especially in IAM, compliance, audit, and security operations.

---

## 6. Screenshots Must Be Sanitized

Screenshots can expose sensitive information if uploaded carelessly.

Information that should be removed or blurred includes:

* Tenant IDs
* Subscription IDs
* Personal email addresses
* Phone numbers
* MFA methods
* Temporary passwords
* Billing information
* Recovery methods
* Secrets or tokens

### Lesson

A security portfolio should demonstrate good security judgment. Evidence is useful, but sensitive data must be protected.

---

## 7. This Lab Creates a Foundation for Advanced IAM

This first lab created the foundation for future labs involving:

* User onboarding
* User offboarding
* MFA
* Conditional Access
* Privileged Identity Management
* Access reviews
* Suspicious sign-in investigation
* Identity governance

### Lesson

IAM skills build progressively. Users, groups, roles, and documentation come first. Advanced controls become easier to understand once the identity foundation exists.
