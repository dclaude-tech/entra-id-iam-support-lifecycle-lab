# Lab setup

This lab uses fictional users, security groups, and simulated IAM support tickets in Microsoft Entra ID.

The purpose of this setup is to create realistic joiner, mover, leaver, MFA validation, and access validation scenarios for an entry-level IAM Analyst portfolio lab.

## Fictional organization

Organization name: Northstar Identity Lab

This is not a real organization. It is a fictional lab environment created for portfolio learning.

## Fictional users

| Display name | Fictional role        | Lab purpose                      |
| ------------ | --------------------- | -------------------------------- |
| Maya Chen    | Finance Analyst       | MFA sign-in review               |
| Leo Grant    | Operations Specialist | New hire missing baseline access |
| Nina Patel   | HR Coordinator        | Mover access cleanup             |
| Owen Brooks  | IT Support Specialist | Leaver account cleanup           |
| Sofia Rivera | HR Generalist         | Audit access validation          |

## Security groups

| Group name               | Purpose                                               |
| ------------------------ | ----------------------------------------------------- |
| SG-LAB-Baseline-Employee | Standard baseline access for active employees         |
| SG-LAB-Finance-Access    | Finance department access                             |
| SG-LAB-HR-Access         | HR department access                                  |
| SG-LAB-IT-Support-Access | IT support access                                     |
| SG-LAB-Operations-Access | Operations department access                          |
| SG-LAB-MFA-Pilot         | Pilot group for MFA and Conditional Access validation |

## Starting group memberships

| User         | Starting groups                                                   | Intended issue                                       |
| ------------ | ----------------------------------------------------------------- | ---------------------------------------------------- |
| Maya Chen    | SG-LAB-Baseline-Employee, SG-LAB-Finance-Access, SG-LAB-MFA-Pilot | Used to validate MFA and Conditional Access behavior |
| Leo Grant    | SG-LAB-Operations-Access                                          | Missing baseline employee access                     |
| Nina Patel   | SG-LAB-Baseline-Employee, SG-LAB-Finance-Access                   | Needs Finance access removed and HR access added     |
| Owen Brooks  | SG-LAB-Baseline-Employee, SG-LAB-IT-Support-Access                | Needs account disabled and access removed            |
| Sofia Rivera | SG-LAB-Baseline-Employee, SG-LAB-HR-Access                        | Access should be validated with no change required   |

## Conditional Access policy

| Policy name              | Purpose                                   | Status  |
| ------------------------ | ----------------------------------------- | ------- |
| CA-LAB-Require-MFA-Pilot | Require MFA for users in SG-LAB-MFA-Pilot | Planned |

## Setup status

| Setup item | Status |
|---|---|
| Fictional users | Created |
| Security groups | Created |
| Starting group memberships | Created |
| Conditional Access MFA pilot policy | Planned |
| Ticket evidence screenshots | Not started |

## Notes

This lab uses fictional users and simulated tickets, but the evidence will be captured from Microsoft Entra ID.

Sensitive tenant details will be redacted from screenshots before publishing, including full UPNs, tenant identifiers, object IDs, admin account names, IP addresses, location details, request IDs, and correlation IDs.
