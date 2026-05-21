# Users and groups

## Goal

This section documents the starter identity and access structure for the Northstar Identity Lab in Microsoft Entra ID.

The goal was to create realistic test users, organize access by job role, and assign users to security groups based on least-privilege access needs.

## Test users created

| User | Job role | Department |
|---|---|---|
| Ava Patel | HR Analyst | Human Resources |
| Marcus Chen | Finance Analyst | Finance |
| Jordan Lee | IT Support Specialist | Information Technology |

## Security groups created

| Group | Purpose |
|---|---|
| SG-All-Employees | Baseline access group for standard employee users |
| SG-HR-Analysts | Department-specific access group for HR analyst users |
| SG-Finance-Analysts | Department-specific access group for Finance analyst users |
| SG-IT-Support | Department-specific access group for IT support users |

## Group assignment model

| User | Assigned groups |
|---|---|
| Ava Patel | SG-All-Employees, SG-HR-Analysts |
| Marcus Chen | SG-All-Employees, SG-Finance-Analysts |
| Jordan Lee | SG-All-Employees, SG-IT-Support |

## IAM concepts demonstrated

- User provisioning
- Security group creation
- Role-based access control
- Least-privilege access assignment
- Department-based access modeling
- Baseline access versus role-specific access
- Foundation for joiner, mover, and leaver workflows

## Evidence

Screenshots for this section are stored in:

`screenshots/02-users-and-groups/`

Included evidence:

- Role-based security groups created
- Test users created
- Baseline group membership assigned
- HR user group membership assigned
