# TKT-002: New hire missing baseline access

## Status

Closed

## Scenario

Leo Grant is a new Operations user in the lab environment. The access matrix shows that all active employees should have baseline employee access.

Leo already had Operations access, but he was missing the baseline employee group.

## User

| Field                      | Detail                   |
| -------------------------- | ------------------------ |
| Display name               | Leo Grant                |
| Fictional role             | Operations Specialist    |
| Department access reviewed | SG-LAB-Operations-Access |
| Baseline group reviewed    | SG-LAB-Baseline-Employee |

## Ticket purpose

Review a new hire access issue and add missing baseline employee access based on the access matrix.

## Access matrix check

| Item                       | Result                   |
| -------------------------- | ------------------------ |
| Required baseline access   | SG-LAB-Baseline-Employee |
| Required department access | SG-LAB-Operations-Access |
| Access to remove           | None                     |
| Change required            | Yes                      |

## Analyst findings

Reviewed Leo Grant’s group memberships and compared them against the access matrix.

Leo was already assigned to SG-LAB-Operations-Access, which matched his Operations role. However, Leo was not assigned to SG-LAB-Baseline-Employee, which is required for all active employees in this lab.

## Action taken

Added Leo Grant to SG-LAB-Baseline-Employee.

No other access was added or removed.

## Verification

Verified that Leo Grant is now a member of both required groups:

| Required group           | Verification result |
| ------------------------ | ------------------- |
| SG-LAB-Baseline-Employee | Present             |
| SG-LAB-Operations-Access | Present             |

Reviewed audit log evidence showing that the group membership update completed successfully.

## Closure notes

Closed as resolved. Missing baseline employee access was added, and Leo Grant’s group membership now matches the access matrix for an Operations Specialist.

## Screenshots

| Screenshot                                  | Description                                                                                              |
| ------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `01-user-membership-before-redacted.png`    | Shows Leo Grant had SG-LAB-Operations-Access before remediation but was missing SG-LAB-Baseline-Employee |
| `02-baseline-group-add-member-redacted.png` | Shows Leo Grant as a member of SG-LAB-Baseline-Employee after being added                                |
| `03-user-membership-after-redacted.png`     | Shows Leo Grant with both SG-LAB-Baseline-Employee and SG-LAB-Operations-Access after remediation        |
| `04-audit-log-add-member-redacted.png`      | Shows audit log evidence for the successful group membership update                                      |

## Redaction notes

Sensitive tenant and user details were redacted, including full UPNs, real domain details, object IDs, admin account information, request IDs, correlation IDs, and other tenant-specific identifiers.

Fictional display names, group names, activity names, status fields, group membership evidence, and ticket closure information were left visible for portfolio review.
