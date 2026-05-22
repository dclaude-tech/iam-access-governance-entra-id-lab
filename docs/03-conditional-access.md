# Conditional Access

## Goal

This section documents a Microsoft Entra Conditional Access policy used to require multifactor authentication for a controlled pilot group of lab users.

The policy was created in report-only mode first to safely validate the configuration before enforcement.

## Policy created

| Setting | Value |
|---|---|
| Policy name | CA001-Require-MFA-Pilot-Users |
| Policy type | Conditional Access |
| Target users/groups | SG-CA-MFA-Pilot |
| Target resources | All resources |
| Grant control | Require multifactor authentication |
| Initial policy state | Report-only |

## Pilot group

The policy was scoped to the following pilot group:

| Group | Purpose |
|---|---|
| SG-CA-MFA-Pilot | Test group used to validate MFA Conditional Access behavior before broader enforcement |

The pilot group included the following lab users:

| User | Role |
|---|---|
| Ava Patel | HR Analyst |
| Marcus Chen | Finance Analyst |
| Jordan Lee | IT Support Specialist |

## Safety controls

The policy was configured using a controlled pilot group instead of applying directly to all users.

An emergency access account was also created before enforcement testing so the tenant would have a fallback administrator account if a Conditional Access policy caused sign-in issues.

## IAM concepts demonstrated

- Conditional Access policy creation
- MFA requirement configuration
- Pilot group scoping
- Report-only testing
- Emergency access planning
- Safer rollout approach for access policies
- Least-privilege access control design

## Evidence

Screenshots for this section are stored in:

`screenshots/03-conditional-access/`

Included evidence:

- Conditional Access policy scoped to the MFA pilot group
- MFA grant control configured in report-only mode
