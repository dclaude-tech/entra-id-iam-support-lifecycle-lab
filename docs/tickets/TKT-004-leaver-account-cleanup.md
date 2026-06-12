# TKT-004: Leaver account cleanup

## Status

Closed

## Scenario

Owen Brooks is a leaver in the lab environment.

The purpose of this ticket was to disable the user account and remove active group access as part of a leaver cleanup process.

## User

| Field                   | Detail                                                |
| ----------------------- | ----------------------------------------------------- |
| Display name            | Owen Brooks                                           |
| Fictional role          | IT Support Specialist                                 |
| Account action reviewed | Disable account                                       |
| Access reviewed         | SG-LAB-Baseline-Employee and SG-LAB-IT-Support-Access |

## Ticket purpose

Review a leaver access issue, disable the user account, remove active group access, and verify that cleanup actions were completed.

## Access matrix check

| Item                          | Result                                             |
| ----------------------------- | -------------------------------------------------- |
| Account status before cleanup | Enabled                                            |
| Groups before cleanup         | SG-LAB-Baseline-Employee, SG-LAB-IT-Support-Access |
| Required action               | Disable account and remove active group access     |
| Change required               | Yes                                                |

## Analyst findings

Reviewed Owen Brooks’ account and group memberships in Microsoft Entra ID.

The account was enabled before cleanup. Owen was also assigned to SG-LAB-Baseline-Employee and SG-LAB-IT-Support-Access, which represented active access that should not remain for a leaver.

## Action taken

Disabled the Owen Brooks user account.

Removed Owen Brooks from the following groups:

| Group removed            | Reason                                            |
| ------------------------ | ------------------------------------------------- |
| SG-LAB-Baseline-Employee | Baseline access no longer required for a leaver   |
| SG-LAB-IT-Support-Access | IT support access no longer required for a leaver |

## Verification

Verified that the Owen Brooks account status changed from enabled to disabled.

Verified that Owen Brooks was no longer a member of any groups after cleanup.

Reviewed audit log evidence showing successful leaver cleanup actions, including account disablement and group membership removal.

## Closure notes

Closed as resolved. Owen Brooks’ account was disabled and active group access was removed as part of the leaver cleanup process.

## Screenshots

| Screenshot                                 | Description                                                                                |
| ------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `01-user-account-before-redacted.png`      | Shows Owen Brooks’ account was enabled before cleanup                                      |
| `02-user-membership-before-redacted.png`   | Shows Owen Brooks had SG-LAB-Baseline-Employee and SG-LAB-IT-Support-Access before cleanup |
| `03-user-account-disabled-redacted.png`    | Shows Owen Brooks’ account status changed to disabled                                      |
| `04-user-membership-after-redacted.png`    | Shows Owen Brooks is not a member of any groups after cleanup                              |
| `05-audit-log-leaver-actions-redacted.png` | Shows audit log evidence for successful account disablement and group membership removal   |

## Redaction notes

Sensitive tenant and user details were redacted, including full UPNs, real domain details, object IDs, admin account information, request IDs, correlation IDs, and other tenant-specific identifiers.

Fictional display names, group names, activity names, status fields, group membership evidence, account status, and ticket closure information were left visible for portfolio review.
