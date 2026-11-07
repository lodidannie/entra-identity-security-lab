# Validation plan

All technical execution results below are pending. Criteria describe future evidence collection, not tests already passed.

| ID | Test | Expected observation |
| --- | --- | --- |
| P01 | Inspect eligible and active assignments | Tested privilege is eligible and inactive before activation |
| P02 | Activate with justification | Justification recorded; activation no longer than eight hours |
| P03 | Evaluate authentication context | Correct enforced policy evaluated and MFA requirement satisfied |
| P04 | Allow activation to expire | Privilege no longer effective after propagation and session checks |
| R01 | Inspect running reviews | Quarterly schedule and 14-day duration visible |
| R02 | Inspect group subjects | Both eligible and active members covered |
| R03 | Inspect guest scope | Guest-only scope and 90-day threshold shown; precise resources identified |
| R04 | Approve continued access | Decision recorded; access remains after validation |
| R05 | Deny unnecessary access | Decision recorded; operator manually removes target access and verifies result |
| R06 | Leave an item unanswered | No automatic access change; item escalated |
| R07 | Apply review results manually | Only validated decisions applied with before/after record |

Record date, evidence ID, expected result, actual result, status and limitation for each test. A successful portal configuration alone is not end-to-end validation. For a future tenant, use fictional test identities and reversible access before testing removals. A newly invited guest cannot supply historical 90-day inactivity immediately; wait for real qualifying history or label that scenario simulated.
