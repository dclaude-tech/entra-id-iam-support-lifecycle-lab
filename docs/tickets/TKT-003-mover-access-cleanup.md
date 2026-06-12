# TKT-003: Mover access cleanup

## Status

Closed

## Scenario

Nina Patel moved from Finance to HR in the lab environment.

The access matrix shows that an HR user should have baseline employee access and HR access. Nina still had Finance access and was missing HR access.

## User

| Field                    | Detail                   |
| ------------------------ | ------------------------ |
| Display name             | Nina Patel               |
| Fictional role           | HR Coordinator           |
| Previous access reviewed | SG-LAB-Finance-Access    |
| Required access reviewed | SG-LAB-HR-Access         |
| Baseline group reviewed  | SG-LAB-Baseline-Employee |

## Ticket purpose

Review a mover access issue and update group memberships so the user’s access matches the access matrix.

## Access matrix check

| Item                       | Result                   |
| -------------------------- | ------------------------ |
| Required baseline access   | SG-LAB-Baseline-Employee |
| Required department access | SG-LAB-HR-Access         |
| Access to remove           | SG-LAB-Finance-Access    |
| Change required            | Yes                      |

## Analyst findings

Reviewed Nina Patel’s group memberships and compared them against the access matrix.

Nina had SG-LAB-Baseline-Employee, which was correct. However, she still had SG-LAB-Finance-Access from her previous role and did not have SG-LAB-HR-Access for her new HR role.

## Action taken

Added Nina Patel to SG-LAB-HR-Access.

Removed Nina Patel from SG-LAB-Finance-Access.

No change was made to SG-LAB-Baseline-Employee because baseline access was still required.

## Verification

Verified that Nina Patel is now a member of the correct groups:

| Group                    | Verification result |
| ------------------------ | ------------------- |
| SG-LAB-Baseline-Employee | Present             |
| SG-LAB-HR-Access         | Present             |
| SG-LAB-Finance-Access    | Removed             |

Reviewed audit log evidence showing that HR access was added successfully and Finance access was removed successfully.

## Closure notes

Closed as resolved. Nina Patel’s access was updated to match the access matrix for an HR Coordinator. Previous Finance access was removed as part of mover cleanup.

## Screenshots

| Screenshot                                    | Description                                                                            |
| --------------------------------------------- | -------------------------------------------------------------------------------------- |
| `01-user-membership-before-redacted.png`      | Shows Nina Patel had SG-LAB-Baseline-Employee and SG-LAB-Finance-Access before cleanup |
| `02-hr-group-add-member-redacted.png`         | Shows audit log evidence for adding Nina Patel to SG-LAB-HR-Access                     |
| `03-finance-group-remove-member-redacted.png` | Shows audit log evidence for removing Nina Patel from SG-LAB-Finance-Access            |
| `04-user-membership-after-redacted.png`       | Shows Nina Patel with SG-LAB-Baseline-Employee and SG-LAB-HR-Access after cleanup      |

## Redaction notes

Sensitive tenant and user details were redacted, including full UPNs, real domain details, object IDs, admin account information, request IDs, correlation IDs, and other tenant-specific identifiers.

Fictional display names, group names, activity names, status fields, group membership evidence, and ticket closure information were left visible for portfolio review.
