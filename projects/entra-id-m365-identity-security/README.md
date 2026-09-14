# 04 — Entra ID & Microsoft 365 Identity Security

## Overview
A practical identity-security case study covering authentication hardening, Conditional Access, MFA, identity-risk monitoring, compromised-account response, privileged access and hybrid identity operations.

## Objective
Strengthen identity security across a Microsoft 365 environment by improving authentication controls, monitoring identity risks, protecting privileged access, and establishing a structured response process for suspicious and compromised accounts.

## Scope
- Microsoft Entra ID
- Conditional Access
- MFA
- Identity Protection
- Privileged Identity Management (PIM)
- Microsoft Entra Connect
- Active Directory
- Immutable ID
- Hard Match / Soft Match
- Password Hash Synchronization
- B2B / Guest access
- Risky sign-in monitoring
- Compromised-account investigation and remediation

## Identity Security Model
```text
Cloud / AD identities
        |
        v
Microsoft Entra Connect
  Hard Match / Soft Match
  Immutable ID / PHS
        |
        v
Microsoft Entra ID
  Identity Protection
  Authentication
  PIM
  B2B / Guests
        |
        v
Conditional Access + MFA
        |
        v
Microsoft 365 workloads
```

## Risk Investigation Workflow
```text
Risk detected
     |
     v
Review sign-in details
     |
     v
Validate activity
     |
     v
Contain / remediate
     |
     v
Validate recovery
```

## Operational Activities
### Authentication & Access
- Reviewed authentication requirements.
- Implemented and enforced MFA controls.
- Managed Conditional Access policy scope and exclusions.
- Supported controlled rollout and validation.
- Troubleshot authentication and policy issues.

### Identity Risk
- Monitored risky sign-ins.
- Investigated suspicious authentication activity.
- Validated whether activity was legitimate or suspicious.
- Performed appropriate containment and remediation.
- Validated subsequent account activity.

### Compromised Accounts
Used a repeatable Identify → Investigate → Contain → Remediate → Validate workflow for suspected account compromise.

### Privileged Access
Used Microsoft Entra PIM to support privileged-access management, review privileged assignments and reduce unnecessary standing administrative exposure.

### Hybrid Identity
Worked with Active Directory and Microsoft Entra Connect for synchronization and identity-matching scenarios, including Immutable ID, Hard Match, Soft Match and Password Hash Synchronization.

### External Access
Reviewed B2B / guest identities and unnecessary access to support controlled external collaboration.

## Outcome
- Stronger authentication controls
- Better visibility into risky authentication activity
- Structured compromised-account investigation and remediation
- Better control over privileged access
- More consistent hybrid identity troubleshooting
- Reduced unnecessary access exposure
- Repeatable identity-security monitoring and response

## Architecture
See [`identity-security-architecture.svg`](./identity-security-architecture.svg).

> Sanitized for portfolio use. No customer names, tenant identifiers, domains, IP addresses or confidential information are included.
