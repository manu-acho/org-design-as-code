# Coding Manual

## Purpose and unit

Code an evidence segment, not an entire document. Descriptive codes record what the artefact explicitly represents. Theoretical codes interpret relations. Emergent codes are quarantined until defined and reviewed. Co-coding is expected, but each code must answer a distinct question.

## Descriptive codebook

| Code | Definition and source basis | Include / exclude | SAP-context example / non-example / edge case | Level and relations |
|---|---|---|---|---|
| ROLE | Named actor category associated with responsibility, task, or permission | Include business role/template and explicit process actor; exclude a person's name or system component | Example: documented role performs a step. Non-example: app title. Edge: “processor” without a role—code ROLE with uncertainty | Micro; links ACTION, ACCESS, DECISION |
| ACTION | Organisationally meaningful operation on an object | Include create, review, approve, post; exclude descriptive state | Example: release a document. Non-example: “available”. Edge: automated derivation—also SYSTEM_ACTION | Micro |
| USER_ACTION | Action explicitly assigned to a human/business user | Include task or decision; exclude system execution | Example: user confirms receipt. Edge: user schedules automation | Micro; subtype ACTION |
| SYSTEM_ACTION | Automatic action attributed to system logic | Include determination, posting, notification; exclude unexplained passive wording | Example: system sets block. Edge: background job initiated by user | Micro; subtype ACTION |
| HANDOFF | Transfer of action obligation or process control between actors | Include routed task or actor change tied to an object; exclude mere visibility | Example: task sent to approver. Non-example: shared report | Micro/meso; suggests dependency, not its type automatically |
| INFORMATION | Represented data used or produced in work | Include field, document content, signal; exclude object mention without informational role | Example: approval status visible. Edge: material master—also MASTER_DATA | Micro |
| WORKFLOW | Defined orchestration with trigger, steps, actors, or outcomes | Include scenario and routed sequence; exclude informal list of steps | Example: condition starts approval. Non-example: static process taxonomy | Meso; relates RULE, HANDOFF |
| DECISION | Selection among alternatives with organisational consequence | Include approve/reject, choose source; exclude deterministic calculation | Edge: rule automatically decides—code DECISION only if documentation frames a decision outcome, plus SYSTEM_ACTION | Micro |
| APPROVAL | Authoritative acceptance/rejection enabling or preventing progression | Include explicit approval/release decision; exclude acknowledgement | Example: purchase document approval. Edge: automatic approval—record rule and absence of human authority | Micro; subtype DECISION/control |
| RULE | Explicit condition mapping inputs/states to required action or outcome | Include condition, decision table, derivation; exclude narrative recommendation | Example: start condition. Non-example: best-practice advice | Micro |
| THRESHOLD | Numeric/ordinal boundary changing routing, right, or outcome | Include amount/time/risk limit; exclude target with no consequence | Edge: reporting KPI threshold—code only if operative | Micro; subtype RULE |
| EXCEPTION | Explicit departure from expected path/state requiring alternate handling | Include error, mismatch, rejected state; exclude normal variant | Example: blocked invoice. Edge: optional path—code CONFIGURATION unless framed exceptional | Micro/meso |
| ESCALATION | Transfer or elevation caused by unresolved condition, risk, or time | Include deadline escalation or higher authority; exclude ordinary next approval | Edge: notification without authority transfer—also information signalling, not necessarily escalation | Micro |
| STRUCTURAL_UNIT | Formally modelled enterprise entity that scopes work/data | Include company code, plant, sales organisation; exclude role/team unless structural entity | Edge: profit centre—code if used as organisational scope, memo accounting interpretation | Macro/micro |
| CONTROL | Formal comparison, constraint, monitoring, or consequence | Include validation, block, reconciliation; exclude general visibility | Example: mismatch blocks progression. Non-example: list report alone | Micro/meso |
| STATUS | Named state with process, visibility, or action significance | Include lifecycle state; exclude cosmetic label | Edge: display-only status—describe but do not promote to primitive without consequence | Micro |
| ACCESS | Explicit permission or restriction over action/information | Include business catalogue/app/restriction relation; exclude role name alone | Example: company-code restriction. Edge: UI availability without data restriction | Micro/macro |
| MASTER_DATA | Persistent shared reference object reused by transactions | Include customer, supplier, material or organisational master when documented; exclude transaction document | Edge: configuration table—code CONFIGURATION | Macro/micro |
| CONFIGURATION | Supported choice that alters system/process behaviour | Include scope, parameter, workflow definition; exclude transactional choice | Example: business expert defines condition. Edge: extension versus setting—co-code only with distinct evidence | Macro/meso |
| ORGANISATIONAL_UNIT | Alias retained for requested scheme; use STRUCTURAL_UNIT as canonical | Same inclusion rules | Map legacy coding during import | — |

## Candidate primitive decision

Assign `SOFTWARE_PRIMITIVE` only if the construct is identifiable, reusable as a type, operative or constraining, and organisationally meaningful. Record primitive type, operation (`route/restrict/gate/signal/validate/aggregate/record/allocate`), target, scope, and relation. A Fiori app, module, screen colour, or broad “process” is not a primitive by default. Approval and workflow can be nested primitives; state the analytical granularity.

## Theoretical codebook

| Family/code | Definition | Inclusion and exclusion test | Example, edge, relation |
|---|---|---|---|
| INTERDEPENDENCE_POOLED | Differentiated activities contribute to a whole or rely on a common resource without direct ordered exchange | Identify activities and common resource/output; do not infer from shared platform alone | Shared governed master object may qualify if activities depend on it |
| INTERDEPENDENCE_SEQUENTIAL | Output/state of A is prerequisite or input to B | Require directional dependency; temporal order alone is insufficient | Posted receipt enables matching; branching may contain several sequences |
| INTERDEPENDENCE_RECIPROCAL | Outputs/actions of A and B mutually condition one another through iteration | Require bidirectional substantive adjustment; rework to same actor is insufficient | Exception resolution across roles may qualify if both revise inputs |
| COORD_STANDARD_WORK | Procedures/actions are specified | Require prescribed method, not merely outcome | Workflow steps plus validation; distinguish technical execution detail |
| COORD_STANDARD_OUTPUT | Required result, state, or measure is specified while means retain variation | Require output criterion | Required balanced state; a mandatory step is work standardisation instead |
| COORD_STANDARD_SKILLS | Coordination relies on certified/standard expertise | Require explicit skill/qualification evidence; role label alone excluded | Likely sparse in architecture; absence is reportable |
| COORD_PLANNING | Schedules, plans, prerequisites, or resource allocations coordinate future activity | Require ex ante relation | Planned period close; status gating may instead be sequence control |
| COORD_DIRECT_SUPERVISION | An actor is given authority to direct, accept, or reject another's work | Require authority relation; any approval is not automatically hierarchical supervision | Approver may be governance without line supervision—memo ambiguity |
| COORD_MUTUAL_ADJUSTMENT | Actors coordinate through direct iterative communication/adaptation | Require channel and reciprocal adjustment; workflow loop alone excluded | Often underrepresented in reference documents |
| INFO_CREATE/TRANSFER/AGGREGATE/INTEGRATE/VISIBILITY | Respectively produces, moves, summarises, combines, or exposes information | Code the operation and actor/object; do not infer comprehension | Shared view may combine visibility and integration |
| INFO_EXCEPTION_SIGNAL | Brings deviation to an actor/system's attention | Require deviation plus signal/recipient | Alert or inbox task; a block without notification is CONTROL |
| INFO_UNCERTAINTY_REDUCTION | Supplies information plausibly addressing a stated task uncertainty | Require explicit inference memo; never code solely because data exists | Higher-inference code, reviewed during pattern analysis |
| GOV_DECISION_RIGHT | Legitimate authority to choose among alternatives for an object/scope | Require actor, decision, object, scope | Approval authority; access alone excluded |
| GOV_ACCESS_RIGHT | Permission to act on or view data | Require explicit permission/restriction | Role catalogue plus organisational restriction |
| GOV_APPROVAL_AUTHORITY | Authority to accept/reject and change progression | Require consequence | Subtype decision right; automatic release is not human authority |
| GOV_ACCOUNTABILITY | Identifiable answerability or attributable responsibility | Require assignment plus trace/obligation; logging alone may be traceability | Edge must be memoed |
| GOV_SEPARATION_DUTIES | Incompatible tasks/rights are allocated separately | Require explicit separation or conflict rule; different role names insufficient | SoD documentation |
| GOV_ESCALATION | Authority/attention is elevated under defined condition | Require condition and changed recipient/level | Deadline routing |
| GOV_MONITORING | State/conduct is made inspectable for oversight | Require observer and object where possible | Monitoring app; visibility without oversight is INFO_VISIBILITY |
| GOV_FORMAL_CONTROL | Rule/standard, comparison, and consequence constrain action/output | Seek all three elements; partial controls remain descriptive | Validation rejects entry |
| DISC_MANDATORY | Architecture provides no sanctioned alternative in stated scope | Require explicit requirement | Required relation/field; absence of alternatives is weak evidence |
| DISC_CONFIGURABLE | Authorised setting among predefined options | Record config actor, lifecycle, options | Workflow conditions |
| DISC_EXTENSIBLE | Released mechanism permits added field/logic/integration | Record boundary and upgrade constraints | Key-user extension |
| DISC_EXCEPTIONAL | Discretion becomes available only under exception path | Require exception trigger and authorised response | Manual resolution task |
| DISC_OVERRIDABLE | Rule/outcome can be intentionally superseded by authorised actor | Use only with explicit override and trace/consequence evidence | Do not equate reject or reconfigure with override |

## Emergent codes

Enter proposed codes in a code-development log with definition, three supporting segments, two exclusion contrasts, relation to existing codes, and theoretical value. Candidate examples—not active codes—include `ALGORITHMIC_DELEGATION`, `TEMPORAL_CLOSURE`, and `CROSS_PROCESS_OBJECT`. Promote only after review; recode the corpus consistently and increment the manual version.

## Decision rules

1. Explicit description precedes theory. Never code theoretical significance from a feature name alone.
2. Code relations: every interdependence has at least two activities; every right has actor, action/object, and scope; every control identifies standard and consequence where present.
3. Distinguish absent evidence from evidence of absence. Negative findings require a documented purposive search.
4. Prefer the least inferential code. Mark inference confidence `high`, `moderate`, or `low` and explain low-confidence retention.
5. Do not force exclusivity. Record co-occurring mechanisms, then use memos to distinguish complementary and rival explanations.
6. Edition and release mismatches block coding into the main corpus.
7. A template is coded as offered logic, never as implemented allocation.
8. “Can” indicates capability; “must” indicates constraint; preserve modal language.
9. Separate observation, interpretation, and theoretical inference in every consequential record.
10. Resolve disagreement by revising definitions or documenting an irreducible interpretive choice, not by silent majority.

