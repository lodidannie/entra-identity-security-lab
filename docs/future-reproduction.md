# Future tenant reproduction guide

Status: planned and unexecuted. No personal test tenant exists for this case study.

1. Establish a separate test tenant. Confirm current licenses and permissions for each PIM and governance feature, and applicable guest billing prerequisites against Microsoft documentation.
2. Create a small subset of the fictional identities and groups. Preserve an appropriate emergency access path and document exclusions before enabling policies.
3. Choose the PIM surface: Entra directory role eligibility or PIM for Groups membership. Configure each relevant role or membership policy deliberately rather than assuming inheritance across surfaces.
4. Create an authentication context and a Conditional Access policy that targets it and the intended users. Validate targeting and exclusions before enabling enforcement; use the documented Require MFA control. Authenticator acceptance alone does not establish authentication strength.
5. Apply permanent eligibility, eight-hour activation maximum, mandatory justification and no approval to the chosen test scope. Inspect scheduling capabilities rather than assuming UI equivalence.
6. Execute P01-P04 from the validation plan and capture sanitized results.
7. Configure separate role, group and guest access review scenarios using current supported paths. Include eligible and active members where required. Apply quarterly recurrence, 14 days, auto-apply off and nonresponse No change.
8. Execute R01-R07 using reversible synthetic access. For guest inactivity, use genuine qualifying history or disclose a simulated outcome.
9. Remove test assignments, policies, groups and invited guests when finished. Confirm emergency access and intended privileges remain available.

This is a planning guide, not a tested deployment script or exact portal walkthrough. Scripts and Graph automation may be added only with documented permissions and actual execution results.
