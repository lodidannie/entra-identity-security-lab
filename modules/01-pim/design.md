# PIM design and decisions

Status: configuration reported from live implementation; supporting technical validation artifacts pending. Source: implementer confirmations, October 12, 2026.

| Setting | Documented configuration | Reason and tradeoff |
| --- | --- | --- |
| Assignment | Permanently eligible | Supports ongoing responsibilities without standing active access through these eligible assignments; eligibility still requires recertification |
| Maximum activation | Eight hours | Supports a working day; longer privileged exposure than a shorter task window |
| Custom start time | Available as reported | Supports scheduled activity; exact scheduling behavior is not independently tested |
| Justification | Required | Records business purpose; does not itself verify that purpose |
| Eligibility expiration | None | Avoids recurring reassignment; obsolete eligibility can persist without review |
| Approval | Not required | Avoids business delays; removes a preactivation human checkpoint |
| Authentication | Conditional Access authentication context | Links activation to Conditional Access requirements |
| Linked policy label | LAB_Require_MFA_For_Admins | Sanitized substitute for the reported policy name |
| Policy state | On | Reported enforced policy state |
| Grant control | Require MFA | Microsoft Authenticator accepted; no specific authentication strength documented |

## Authentication boundary

MFA is not labeled phishing-resistant. Exact context name and identifier, assignments, exclusions, sign-in frequency, and allowed method policy are not supplied. A policy name and On state alone do not prove that its targeting covers the selected PIM authentication context. Capture sanitized evidence of the link and an activation evaluation before marking this independently validated.

## Validation to complete

- Show eligible assignment and absence of an active assignment for the tested privilege before activation.
- Show configured activation maximum, justification, approval, eligibility expiration and context selection.
- Verify the linked policy targets the context and intended identity and is On.
- Record activation, authentication evaluation, justification and effective privileged access.
- Record expiry or deactivation and test that privileged access is no longer effective, allowing for propagation and sessions.
- Check other direct and group-based access paths before claiming complete removal of standing privileges.

Results are pending. Screenshots, timestamps and logs should be sanitized before inclusion. Settings must be inspected separately for each relevant Entra role or PIM group member/owner policy.
