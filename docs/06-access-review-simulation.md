# Access review simulation

## Goal

This section documents a simulated access review process in Microsoft Entra ID.

The goal was to show how group membership can be reviewed to determine whether users still have appropriate access based on role, department, and lifecycle status.

## Review scenario

This lab reviews access for role-based security groups created earlier in the project.

The access review simulation focuses on identifying whether users still require access and whether group membership aligns with their current role or lifecycle state.

## Groups reviewed

| Group | Review purpose |
|---|---|
| SG-All-Employees | Review baseline employee access |
| SG-HR-Analysts | Review HR role-specific access |
| SG-Finance-Analysts | Review Finance role-specific access |
| SG-IT-Support | Review IT support role-specific access |
| SG-CA-MFA-Pilot | Review pilot group membership for MFA Conditional Access testing |

## IAM concepts demonstrated

- Access review planning
- Group membership review
- Least-privilege validation
- Role-based access review
- Lifecycle-aware access decisions
- Access cleanup after mover and leaver events
- Audit-friendly access documentation

## Evidence

Screenshots for this section are stored in:

`screenshots/06-access-review-simulation/`
