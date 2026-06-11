# TKT-001: MFA sign-in review

## Status

Closed

## Scenario

Maya Chen was included in the MFA pilot group for this lab. The purpose of this ticket was to review sign-in evidence and confirm whether the Conditional Access MFA policy applied as expected.

This was treated as a validation ticket. No failed sign-in was created or simulated.

## User

| Field           | Detail                   |
| --------------- | ------------------------ |
| Display name    | Maya Chen                |
| Fictional role  | Finance Analyst          |
| Group reviewed  | SG-LAB-MFA-Pilot         |
| Policy reviewed | CA-LAB-Require-MFA-Pilot |

## Ticket purpose

Validate MFA and Conditional Access behavior using Microsoft Entra ID sign-in evidence.

## Analyst findings

Reviewed Maya Chen’s group membership and confirmed the user was included in SG-LAB-MFA-Pilot.

Reviewed the Conditional Access policy CA-LAB-Require-MFA-Pilot and confirmed it was scoped to the MFA pilot group with a grant control requiring multifactor authentication.

Reviewed the Microsoft Entra sign-in logs after testing the user sign-in. The sign-in completed successfully and Conditional Access/MFA evidence was available in the sign-in details.

## Action taken

No access change was required.

Confirmed the user was in the correct MFA pilot group, reviewed the Conditional Access policy configuration, and validated the sign-in evidence in Microsoft Entra ID.

## Verification

Verified that the sign-in completed successfully.

Verified that CA-LAB-Require-MFA-Pilot applied successfully to the sign-in.

Verified that the authentication details showed the MFA requirement was satisfied.

## Closure notes

Closed as validated. MFA sign-in behavior matched the lab policy, and no remediation was needed.

## Screenshots

| Screenshot                                          | Description                                                                |
| --------------------------------------------------- | -------------------------------------------------------------------------- |
| `01-mfa-pilot-group-membership-redacted.png`        | Shows Maya Chen as a member of SG-LAB-MFA-Pilot                            |
| `02-conditional-access-policy-scope-redacted.png`   | Shows the Conditional Access policy scoped to SG-LAB-MFA-Pilot             |
| `03-conditional-access-grant-control-redacted.png`  | Shows the grant control requiring multifactor authentication               |
| `04-sign-in-log-overview-redacted.png`              | Shows the successful interactive sign-in event for Maya Chen               |
| `05-sign-in-detail-conditional-access-redacted.png` | Shows CA-LAB-Require-MFA-Pilot with a successful Conditional Access result |
| `06-authentication-details-redacted.png`            | Shows the MFA requirement was satisfied in authentication details          |

## Redaction notes

Sensitive tenant and user details were redacted, including full UPNs, real domain details, IP addresses, location details, device information, request IDs, correlation IDs, object IDs, and admin account information.

Fictional display names, group names, policy names, status fields, Conditional Access results, and MFA-related evidence were left visible for portfolio review.
