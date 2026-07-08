# IAM User Access Troubleshooting and Lifecycle Support Lab | Microsoft Entra ID

## Overview

This project is a hands-on IAM support lab built in Microsoft Entra ID.

The lab simulates common IAM support and identity operations tickets, including MFA validation, new hire access, mover cleanup, leaver cleanup, and access validation.

I used fictional users, security groups, a simple access matrix, ticket documentation, and redacted screenshots to document how access issues can be reviewed, remediated, verified, and closed in a public-safe way.

## Scenario

Northstar Identity Lab is a fictional organization used for this portfolio project.

The lab includes five simulated IAM support tickets:

* MFA sign-in review
* New hire missing baseline access
* Mover access cleanup
* Leaver account cleanup
* Audit access validation

Each ticket follows a simple analyst workflow:

1. Review the ticket request
2. Identify the user and access issue
3. Compare current access against the access matrix
4. Decide whether access should be added, removed, disabled, or left unchanged
5. Complete the approved action in Microsoft Entra ID
6. Capture before and after evidence
7. Document findings, verification, and closure notes

## Lab status

Complete.

## What I built

* Fictional users for IAM support scenarios
* Security groups for baseline and department-based access
* Access matrix for expected group membership
* Ticket tracker for documenting ticket status and outcomes
* Conditional Access MFA pilot policy
* Redacted screenshot evidence for each ticket
* Ticket write-ups with findings, actions, verification, and closure notes

## Completed tickets

| Ticket                                                      | Scenario                         | User         | Outcome                                                  |
| ----------------------------------------------------------- | -------------------------------- | ------------ | -------------------------------------------------------- |
| [TKT-001](docs/tickets/TKT-001-mfa-sign-in-review.md)       | MFA sign-in review               | Maya Chen    | Validated successful MFA and Conditional Access behavior |
| [TKT-002](docs/tickets/TKT-002-new-hire-baseline-access.md) | New hire missing baseline access | Leo Grant    | Added missing baseline employee access                   |
| [TKT-003](docs/tickets/TKT-003-mover-access-cleanup.md)     | Mover access cleanup             | Nina Patel   | Added HR access and removed Finance access               |
| [TKT-004](docs/tickets/TKT-004-leaver-account-cleanup.md)   | Leaver account cleanup           | Owen Brooks  | Disabled account and removed active group access         |
| [TKT-005](docs/tickets/TKT-005-audit-access-validation.md)  | Audit access validation          | Sofia Rivera | Validated access with no remediation required            |

## Evidence collected

Each ticket includes redacted screenshots showing the relevant access review, action, or validation evidence.

| Ticket  | Screenshot folder                                                                     |
| ------- | ------------------------------------------------------------------------------------- |
| TKT-001 | [MFA sign-in review screenshots](screenshots/TKT-001-mfa-sign-in-review/)             |
| TKT-002 | [New hire baseline access screenshots](screenshots/TKT-002-new-hire-baseline-access/) |
| TKT-003 | [Mover access cleanup screenshots](screenshots/TKT-003-mover-access-cleanup/)         |
| TKT-004 | [Leaver account cleanup screenshots](screenshots/TKT-004-leaver-account-cleanup/)     |
| TKT-005 | [Audit access validation screenshots](screenshots/TKT-005-audit-access-validation/)   |

## Supporting files

| File                                            | Purpose                                                                   |
| ----------------------------------------------- | ------------------------------------------------------------------------- |
| [Access matrix](data/access-matrix.csv)         | Defines expected access by role                                           |
| [Ticket tracker](data/ticket-tracker.csv)       | Tracks ticket status, access decisions, actions, and verification results |
| [Lab setup](docs/lab-setup.md)                  | Documents fictional users, groups, memberships, and policy setup          |
| [Analyst workflow](docs/analyst-workflow.md)    | Documents the support workflow used across tickets                        |
| [Ticket template](templates/ticket-template.md) | Reusable format for documenting IAM support tickets                       |

## Tools used

* Microsoft Entra ID
* Security groups
* Conditional Access
* Sign-in logs
* Audit logs
* CSV files
* GitHub documentation

## Skills demonstrated

* IAM support ticket documentation
* User access review
* Joiner, mover, and leaver support
* Group membership review and cleanup
* Baseline access validation
* Least privilege review
* Conditional Access and MFA validation
* Audit log review
* Before and after evidence collection
* Public-safe technical documentation

## Public-safe documentation notes

This project uses fictional users, fictional group names, and a controlled lab tenant.

Screenshots were redacted before publishing. Sensitive details such as full UPNs, real domain details, object IDs, admin account information, request IDs, correlation IDs, and other tenant-specific identifiers were removed or blurred.

Fictional display names, group names, policy names, activity names, status fields, and access validation evidence were left visible so the work could be reviewed safely.

## What I learned

This lab helped me practice how IAM support work is documented from request review through closure.

The most useful part of the lab was connecting the technical action in Microsoft Entra ID to the analyst decision behind it. For each ticket, I had to confirm what access the user had, compare it to expected access, take the appropriate action, and verify the result with evidence.

This helped reinforce the importance of least privilege, accurate access documentation, and clear ticket closure notes.
