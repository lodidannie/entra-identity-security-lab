# Identity governance access review configuration

Status at handover on October 12, 2026: all three controls reported actively running. Completion, applied decisions and remediation outcomes are not yet evidenced.

| Setting | Privileged roles | PIM group memberships | Inactive guest access |
| --- | --- | --- | --- |
| Scope | All active and eligible assignments in 14 roles | Eligible and active members of six groups | Guest users only; precise resource scope not supplied |
| Inactivity filter | Not specified | Off | On, 90 days |
| Duration | 14 days | 14 days | 14 days |
| Recurrence | Quarterly | Quarterly | Quarterly |
| Reviewers | Alex Morgan and Jordan Ellis | Alex Morgan and Jordan Ellis | Alex Morgan and Jordan Ellis |
| Handover notifications | Alex Morgan and Jordan Ellis | Alex Morgan and Jordan Ellis | Alex Morgan and Jordan Ellis |
| Auto-apply | Disabled initially | Disabled initially | Disabled initially |
| Nonresponse | No change | No change | No change |
| Stages | Not supplied | Single-stage unless a second layer is required; actual stage count needs verification | Not supplied |
| Emails and reminders | Not supplied | Not supplied | Enabled |

Names and group labels are fictional substitutions. Source: supplied implementation report, with subsequent implementer confirmations resolving status, eligible membership, guest threshold and handover notification recipients.

## Privileged roles in documented scope

Global Administrator; Privileged Role Administrator; Privileged Authentication Administrator; User Administrator; Authentication Administrator; Application Administrator; Cloud Application Administrator; Security Administrator; Password Administrator; Security Operator; SharePoint Administrator; Exchange Administrator; Intune Administrator; Teams Administrator.

These are standard product role names, not employee data. Membership in a privileged group and assignment to a directory role are distinct review targets; neither review should be presented as automatically replacing the other.

## Fictional group scope

LAB_Cloud_Admin; LAB_CyberSecAnalyst; LAB_ServiceDeskAdmin; LAB_EndpointEngineer; LAB_CollaborationAdmin; LAB_GlobalReader.

## Rationale

Quarterly recurrence balances regular recertification with workload. Fourteen days provides a response window. Both eligible and active members are included because eligibility preserves potential privileged access. Initial manual application enables validation of decisions before removals. Nonresponse retains access and therefore requires explicit escalation rather than being treated as approval.

## Guest scope limitation

This records an inactive guest access review. It does not establish a tenant-wide guest inventory, guest account deletion, or that every guest is included. Exact groups, applications or other reviewed resources and guest licensing/billing configuration require separate evidence. Removing resource access and deleting a guest identity are different actions.

## Completion workflow

Reviewers decide whether continued access is justified. The designated operator validates decisions, applies approved changes, verifies effective access and records exceptions. No such completion is claimed here. Proposed owner assignments appear in the handover runbook and require confirmation.
