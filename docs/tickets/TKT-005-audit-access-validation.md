# TKT-005: Audit access validation

## Status

Closed

## Scenario

Sofia Rivera’s access was reviewed as part of an access validation request in the lab environment.

The purpose of this ticket was to confirm whether Sofia’s current group memberships matched the access matrix. No access issue was reported, and no access change was expected unless the review identified incorrect access.

## User

| Field           | Detail                                        |
| --------------- | --------------------------------------------- |
| Display name    | Sofia Rivera                                  |
| Fictional role  | HR Generalist                                 |
| Access reviewed | SG-LAB-Baseline-Employee and SG-LAB-HR-Access |
| Review type     | Access validation                             |

## Ticket purpose

Validate Sofia Rivera’s current access against the access matrix and confirm whether any remediation was required.

## Access matrix check

| Item                       | Result                   |
| -------------------------- | ------------------------ |
| Required baseline access   | SG-LAB-Baseline-Employee |
| Required department access | SG-LAB-HR-Access         |
| Access to remove           | None identified          |
| Change required            | No                       |

## Analyst findings

Reviewed Sofia Rivera’s group memberships in Microsoft Entra ID and compared them against the access matrix.

Sofia was assigned to SG-LAB-Baseline-Employee and SG-LAB-HR-Access, which matched the expected access for an HR user in this lab.

No unrelated access was identified during the review.

## Action taken

No access change was required.

No groups were added or removed.

## Verification

Verified that Sofia Rivera had the expected baseline and HR access.

Verified that no Finance, IT Support, Operations, or MFA pilot access was visible in the reviewed group membership evidence.

## Closure notes

Closed as validated. Sofia Rivera’s access matched the access matrix, and no remediation was needed.

## Screenshots

| Screenshot                               | Description                                                                                           |
| ---------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `01-user-membership-review-redacted.png` | Shows Sofia Rivera assigned to SG-LAB-Baseline-Employee and SG-LAB-HR-Access during access validation |

## Redaction notes

Sensitive tenant and user details were redacted, including full UPNs, real domain details, object IDs, admin account information, request IDs, correlation IDs, and other tenant-specific identifiers.

Fictional display names, group names, status fields, group membership evidence, and ticket closure information were left visible for portfolio review.
