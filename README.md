# IAM Access Governance Lab | Microsoft Entra ID with Okta and SailPoint Concept Mapping

## Overview

This project is a hands-on IAM access governance lab built in Microsoft Entra ID. It demonstrates identity lifecycle management, role-based access control, MFA enforcement, Conditional Access, least-privilege administration, Privileged Identity Management, access review concepts, and joiner/mover/leaver workflows.

Okta and SailPoint are included only as conceptual comparisons. This project does not configure live integrations with Okta or SailPoint.

## Project status

Core lab complete.

This lab includes Microsoft Entra tenant setup, test users, role-based security groups, MFA and Conditional Access, joiner/mover/leaver workflows, Privileged Identity Management, and access review simulation.

A future phase may add Microsoft Entra ID Governance features such as access packages, Lifecycle Workflows, automated access requests, approvals, and advanced access reviews.

## Lab environment

The lab was built in a Microsoft Entra ID tenant named **Northstar Identity Lab**.

The environment uses fictional users, departments, and security groups to model common IAM scenarios across HR, Finance, IT, Conditional Access, privileged access, and access review workflows.

## Skills demonstrated

- Microsoft Entra ID tenant setup
- User provisioning
- Security group creation
- Role-based access control
- Least-privilege access assignment
- MFA and Conditional Access policy configuration
- Conditional Access report-only testing and enforcement
- Joiner, mover, and leaver workflow simulation
- Privileged Identity Management eligible role assignment
- Access review simulation
- IAM documentation and evidence collection

## Project sections

| Section | Description |
|---|---|
| Lab overview | Defines the project scope, lab environment, and IAM goals |
| Users and groups | Documents test users, security groups, and RBAC assignments |
| Conditional Access | Shows MFA policy creation, pilot group scoping, report-only testing, and enforcement |
| JML workflows | Simulates joiner, mover, and leaver lifecycle workflows |
| Admin roles and PIM | Demonstrates eligible privileged role assignment using PIM |
| Access review simulation | Reviews group membership and validates access cleanup after lifecycle changes |

## Repository structure

```text
docs/
screenshots/
artifacts/
README.md
```

## Documentation

- [Lab overview](docs/01-lab-overview.md)
- [Users and groups](docs/02-users-and-groups.md)
- [Conditional Access](docs/03-conditional-access.md)
- [Joiner, mover, and leaver workflows](docs/04-jml-workflows.md)
- [Admin roles and PIM](docs/05-admin-roles-pim.md)
- [Access review simulation](docs/06-access-review-simulation.md)

## Evidence

Screenshots are organized by lab section in the `screenshots/` folder.

Evidence includes:

- Microsoft 365 and Entra tenant setup
- Role-based security groups
- Test users and group memberships
- Conditional Access MFA policy configuration
- MFA policy enforcement and sign-in testing
- Joiner, mover, and leaver workflow changes
- PIM eligible role assignment
- Access review simulation results

## Important note

This lab is built hands-on in Microsoft Entra ID only. Okta and SailPoint are discussed only for conceptual IAM mapping and are not integrated into the lab environment.
