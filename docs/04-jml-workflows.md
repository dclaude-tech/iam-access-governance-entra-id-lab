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

## Mover workflow

Ava Patel was also used as the mover example for this lab.

The mover workflow simulated Ava moving from Human Resources to Finance. Her user profile attributes were updated first, then her group access was changed to match her new role.

| Attribute | Before | After |
|---|---|---|
| User | Ava Patel | Ava Patel |
| Job title | HR Analyst | Finance Analyst |
| Department | Human Resources | Finance |
| Account status | Enabled | Enabled |

## Mover access update

Ava’s access was updated to remove HR-specific access and add Finance-specific access.

| Access change | Group |
|---|---|
| Retained baseline access | SG-All-Employees |
| Removed prior role access | SG-HR-Analysts |
| Added new role access | SG-Finance-Analysts |
| Retained MFA pilot access | SG-CA-MFA-Pilot |

This demonstrates a least-privilege mover process where access is updated when a user changes departments. The user keeps baseline access, loses access that no longer matches the role, and receives access required for the new role.

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
