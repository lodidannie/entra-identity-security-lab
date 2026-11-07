# Microsoft Entra Identity Security Case Study

A sanitized implementation case study covering just-in-time privileged access and recurring identity governance reviews. Two connected modules document configuration, design rationale, operational ownership, and validation criteria.

## Evidence and scope

The underlying work was performed in a live Microsoft Entra environment. Northstar Services, all employee names, group names, and sample identities in this repository are fictional substitutes. They do not describe a separate deployed tenant. Configuration and implementation status are transcribed from a supplied implementation report and the implementer's confirmations on October 12, 2026. No production screenshots, logs, tenant identifiers, raw exports, or original employer documents are included.

This is a documented production case study, not an independently reproduced test lab. Configuration confirmation is distinct from technical validation evidence. No screenshots or execution results have been fabricated.

## Modules

| Module | Documented behavior | Status at handover |
| --- | --- | --- |
| [PIM and just-in-time access](modules/01-pim/design.md) | Permanent eligibility, activation up to eight hours, justification, no approval, authentication context with enforced MFA | Implementation reported; independent activation and expiration evidence pending |
| [Identity governance access reviews](modules/02-access-reviews/configuration.md) | Privileged roles, eligible and active group members, inactive guest access | All three controls reported actively running; completion and remediation evidence pending |

## Read the project

1. [Architecture and scope](docs/architecture.md)
2. [Fictional organization and identities](docs/fictional-scenario.md)
3. Module designs linked above
4. [Evidence register](evidence/evidence-register.csv) and [sanitized configuration record](evidence/sanitized-configuration-record.md)
5. [Validation plan](docs/validation-plan.md)
6. [Handover runbook](docs/handover-runbook.md)
7. [Lessons and tradeoffs](docs/lessons-learned.md)

## Outcomes and limits

The documented design provides time-limited elevation through permanent eligibility and establishes recurring certification of privileged and guest access. Reviews being active does not establish that reviewers completed decisions or that access was removed. MFA is documented; phishing-resistant authentication is not claimed. No measured risk reduction, complete elimination of standing access, or executed automation is claimed.

## Future lab extension

A future personal tenant can reproduce the designs with synthetic identities. Licensing, permissions, guest billing, and current portal behavior must be checked before deployment. [Future reproduction guide](docs/future-reproduction.md) is unexecuted. This package contains no tenant-changing code.

## References

Official product references are in [references](docs/references.md). Publication review instructions are in [sanitization](docs/sanitization.md).
