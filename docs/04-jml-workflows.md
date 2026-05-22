# Joiner, mover, and leaver workflows

## Goal

This section documents simulated identity lifecycle workflows in Microsoft Entra ID.

The goal is to show how user access can be created, changed, and removed based on a user's employment or role status.

## Workflow scenarios

| Scenario | Description |
|---|---|
| Joiner | A new user is created and assigned baseline and role-specific group access |
| Mover | An existing user changes roles or departments and receives updated group access |
| Leaver | A user account is disabled and access is removed when the user leaves the organization |

## Joiner workflow

Ava Patel was used as the joiner example for this lab.

The joiner workflow simulated a new HR employee being created in Microsoft Entra ID and assigned access based on role and department.

| Attribute | Value |
|---|---|
| User | Ava Patel |
| User principal name | ava.patel@NorthstarIdentityLab.onmicrosoft.com |
| Job title | HR Analyst |
| Department | Human Resources |
| Account status | Enabled |

## Joiner access assignment

Ava was assigned baseline employee access and HR-specific access through Microsoft Entra security groups.

| Group | Purpose |
|---|---|
| SG-All-Employees | Baseline access for standard employee users |
| SG-HR-Analysts | Role-specific access for HR analyst users |
| SG-CA-MFA-Pilot | Pilot group used for Conditional Access MFA testing |

This demonstrates a group-based joiner process where access is assigned through security groups instead of direct, one-off user permissions.

## IAM concepts demonstrated

- Identity lifecycle management
- Joiner, mover, and leaver process design
- User provisioning
- Group-based access assignment
- Least-privilege access changes
- Access removal and account disablement
- Audit-friendly documentation

## Evidence

Screenshots for this section are stored in:

`screenshots/04-jml-workflows/`

Included evidence:

- Joiner user profile created with HR job and department attributes
- Joiner group access assigned through baseline and role-specific security groups
