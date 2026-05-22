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
| Final policy state | On |

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

The policy was first configured in report-only mode to validate the setup before enforcement.

The policy was scoped to a controlled pilot group instead of being applied directly to all users. This reduced the risk of accidentally affecting administrator access or locking out the tenant.

An emergency access account was created before enforcement testing so the tenant would have a fallback administrator account if a Conditional Access policy caused sign-in issues.

After validating the pilot group scope and MFA grant control, security defaults were disabled and the policy was moved from report-only mode to On.

## Testing

After the policy was enabled, Ava Patel was used as a pilot user to test the MFA sign-in experience.

Ava was a member of the SG-CA-MFA-Pilot group, which placed her in scope for the Conditional Access policy. After completing the MFA setup and sign-in process, the Microsoft Entra sign-in logs showed successful sign-in activity for the pilot user.

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
- MFA Conditional Access policy enabled for pilot users
- Successful pilot user sign-in activity after MFA testing
