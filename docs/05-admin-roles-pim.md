# Admin roles and Privileged Identity Management

## Goal

This section documents privileged access management in Microsoft Entra ID using Privileged Identity Management.

The goal was to assign privileged access using an eligible role assignment instead of giving a user permanent active administrator access.

## Role assignment created

| Setting | Value |
|---|---|
| User | Jordan Lee |
| Role | Privileged Role Administrator |
| Scope | Directory |
| Assignment type | Eligible |
| Membership | Direct |
| Assignment duration | Time-bound |

## Why this matters

Privileged roles should be managed carefully because they can grant access to sensitive administrative actions.

Instead of assigning Jordan Lee permanent active access, this lab used an eligible PIM assignment. This supports a just-in-time access model where privileged access is available when needed but not continuously active by default.

## IAM concepts demonstrated

- Privileged Identity Management
- Eligible role assignment
- Just-in-time privileged access
- Least-privilege administration
- Time-bound privileged access
- Reduction of standing admin privileges
- Privileged access governance

## Evidence

Screenshots for this section are stored in:

`screenshots/05-admin-roles-pim/`

Included evidence:

- PIM eligible role assignment configured
- PIM eligible role assignment created for Jordan Lee
