# Coding Manual

**Version:** 1.0

**Frozen:** 8 November 2026 after the 2608 Swiss pilot

**Pilot boundary:** J45 Procurement of Direct Materials, BD9 Sell from Stock, and J58 Accounting and Financial Close

## Purpose and unit

Code an evidence segment, not an entire document. Descriptive codes record what the artefact explicitly represents. Theoretical codes interpret relations. Emergent codes are quarantined until defined and reviewed. Co-coding is expected, but each code must answer a distinct question.

## Descriptive codebook

| Code | Definition and source basis | Include / exclude | SAP-context example / non-example / edge case | Level and relations |
|---|---|---|---|---|
| ROLE | Named actor category associated with responsibility, task, or permission | Include business role/template and explicit process actor; exclude a person's name or system component | Example: documented role performs a step. Non-example: app title. Edge: “processor” without a role - code ROLE with uncertainty | Micro; links ACTION, ACCESS, DECISION |
| ACTION | Organisationally meaningful operation on an object | Include create, review, approve, post; exclude descriptive state | Example: release a document. Non-example: “available”. Edge: automated derivation - also SYSTEM_ACTION | Micro |
| EVENT | Represented occurrence that starts, ends, interrupts, or records a process-relevant change | Include receipt, posting, expiry, release, or scheduled trigger; exclude an activity performed over an interval | Example: goods receipt posted. Edge: a source may use an activity label for a completion event, so preserve its wording | Micro; links ACTION, STATUS, BUSINESS_OBJECT |
| BUSINESS_OBJECT | Persistent or transactional entity on which process-relevant operations are performed | Include requisition, order, delivery, invoice, journal entry, or material document; exclude a screen or app | Example: purchase order. Edge: one end-to-end case may contain several linked objects | Micro/meso; links ACTION, OBJECT_STATE |
| OBJECT_STATE | Process-relevant condition of a business object that enables, blocks, or records progression | Include approved, blocked, posted, cleared, or reversed where the state has consequence; exclude a cosmetic label | Example: blocked sales order. Edge: use STATUS as the source-close code and OBJECT_STATE when the status is tied to an identified object | Micro; subtype relation between STATUS and BUSINESS_OBJECT |
| PROCESS_BOUNDARY | Explicit start, end, scope, or inclusion relation for a represented process | Include trigger, terminal outcome, included subprocess, release, region, and official process ID; exclude an informal umbrella label | Example: J45 in release 2608 for CH. Edge: a reference boundary is not a customer boundary | Meso/macro |
| USER_ACTION | Action explicitly assigned to a human/business user | Include task or decision; exclude system execution | Example: user confirms receipt. Edge: user schedules automation | Micro; subtype ACTION |
| SYSTEM_ACTION | Automatic action attributed to system logic | Include determination, posting, notification; exclude unexplained passive wording | Example: system sets block. Edge: background job initiated by user | Micro; subtype ACTION |
| HANDOFF | Transfer of action obligation or process control between actors | Include routed task or actor change tied to an object; exclude mere visibility | Example: task sent to approver. Non-example: shared report | Micro/meso; suggests dependency, not its type automatically |
| INFORMATION | Represented data used or produced in work | Include field, document content, signal; exclude object mention without informational role | Example: approval status visible. Edge: material master - also MASTER_DATA | Micro |
| CLASSIFICATION | Category or code that assigns an object, event, actor, or transaction to a consequential class | Include document type, account class, organisational assignment, or status category when downstream action depends on it; exclude descriptive labels with no identified consequence | Example: category selects a processing path. Edge: consequence may require a separate source, so retain descriptive confidence | Micro/macro; links RULE, MASTER_DATA, STRUCTURAL_UNIT |
| TRACE_RECORD | Durable record that attributes or reconstructs an action, state transition, or change | Include change history, workflow log, posting record, or audit-relevant trace; exclude general visibility without durable attribution | Example: journal-entry change history. Edge: traceability supports but does not establish accountability | Micro; links INFO_VISIBILITY and ACCOUNTABILITY_SUPPORT |
| WORKFLOW | Defined orchestration with trigger, steps, actors, or outcomes | Include scenario and routed sequence; exclude informal list of steps | Example: condition starts approval. Non-example: static process taxonomy | Meso; relates RULE, HANDOFF |
| DECISION | Selection among alternatives with organisational consequence | Include approve/reject, choose source; exclude deterministic calculation | Edge: rule automatically decides - code DECISION only if documentation frames a decision outcome, plus SYSTEM_ACTION | Micro |
| APPROVAL | Authoritative acceptance/rejection enabling or preventing progression | Include explicit approval/release decision; exclude acknowledgement | Example: purchase document approval. Edge: automatic approval - record rule and absence of human authority | Micro; subtype DECISION/control |
| RULE | Explicit condition mapping inputs/states to required action or outcome | Include condition, decision table, derivation; exclude narrative recommendation | Example: start condition. Non-example: best-practice advice | Micro |
| THRESHOLD | Numeric/ordinal boundary changing routing, right, or outcome | Include amount/time/risk limit; exclude target with no consequence | Edge: reporting KPI threshold - code only if operative | Micro; subtype RULE |
| EXCEPTION | Explicit departure from expected path/state requiring alternate handling | Include error, mismatch, rejected state; exclude normal variant | Example: blocked invoice. Edge: optional path - code CONFIGURATION unless framed exceptional | Micro/meso |
| ESCALATION | Transfer or elevation caused by unresolved condition, risk, or time | Include deadline escalation or higher authority; exclude ordinary next approval | Edge: notification without authority transfer - also information signalling, not necessarily escalation | Micro |
| STRUCTURAL_UNIT | Formally modelled enterprise entity that scopes work/data | Include company code, plant, sales organisation; exclude role/team unless structural entity | Edge: profit centre - code if used as organisational scope, memo accounting interpretation | Macro/micro |
| CONTROL | Formal comparison, constraint, monitoring, or consequence | Include validation, block, reconciliation; exclude general visibility | Example: mismatch blocks progression. Non-example: list report alone | Micro/meso |
| STATUS | Named state with process, visibility, or action significance | Include lifecycle state; exclude cosmetic label | Edge: display-only status - describe but do not promote to primitive without consequence | Micro |
| ACCESS | Explicit permission or restriction over action/information | Include business catalogue/app/restriction relation; exclude role name alone | Example: company-code restriction. Edge: UI availability without data restriction | Micro/macro |
| MASTER_DATA | Persistent shared reference object reused by transactions | Include customer, supplier, material or organisational master when documented; exclude transaction document | Edge: configuration table - code CONFIGURATION | Macro/micro |
| CONFIGURATION | Supported choice that alters system/process behaviour | Include scope, parameter, workflow definition; exclude transactional choice | Example: business expert defines condition. Edge: extension versus setting - co-code only with distinct evidence | Macro/meso |
| EXTENSION | Released mechanism for adding or adapting fields, logic, interfaces, or user experience outside ordinary transaction processing | Include documented key-user, developer, or side-by-side extension points; exclude a selectable standard configuration option | Example: released custom field. Edge: available extension capability is not evidence of its use | Macro/meso |
| ORGANISATIONAL_UNIT | Alias retained for requested scheme; use STRUCTURAL_UNIT as canonical | Same inclusion rules | Map legacy coding during import |  -  |

## Candidate primitive decision

Assign `SOFTWARE_PRIMITIVE` only if the construct is identifiable, reusable as a type, operative or constraining, and organisationally meaningful. Record primitive type, operation (`create/route/restrict/gate/signal/validate/aggregate/record/allocate/transfer/integrate/schedule/reverse`), target, scope, and relation. A Fiori app, module, screen colour, or broad “process” is not a primitive by default. Approval and workflow can be nested primitives; state the analytical granularity.

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
| COORD_DIRECT_SUPERVISION | An actor is given authority to direct, accept, or reject another's work | Require authority relation; any approval is not automatically hierarchical supervision | Approver may be governance without line supervision - memo ambiguity |
| COORD_MUTUAL_ADJUSTMENT | Actors coordinate through direct iterative communication/adaptation | Require channel and reciprocal adjustment; workflow loop alone excluded | Often underrepresented in reference documents |
| INFO_CREATE/TRANSFER/AGGREGATE/INTEGRATE/VISIBILITY | Respectively produces, moves, summarises, combines, or exposes information | Code the operation and actor/object; do not infer comprehension | Shared view may combine visibility and integration |
| INFO_EXCEPTION_SIGNAL | Brings deviation to an actor/system's attention | Require deviation plus signal/recipient | Alert or inbox task; a block without notification is CONTROL |
| INFO_UNCERTAINTY_REDUCTION | Supplies information plausibly addressing a stated task uncertainty | Require explicit inference memo; never code solely because data exists | Higher-inference code, reviewed during pattern analysis |
| GOV_DECISION_RIGHT | Legitimate authority to choose among alternatives for an object/scope | Require actor, decision, object, scope | Approval authority; access alone excluded |
| GOV_ACCESS_RIGHT | Permission to act on or view data | Require explicit permission/restriction | Role catalogue plus organisational restriction |
| GOV_APPROVAL_AUTHORITY | Authority to accept/reject and change progression | Require consequence | Subtype decision right; automatic release is not human authority |
| GOV_ACCOUNTABILITY | Identifiable answerability or attributable responsibility | Require assignment plus trace/obligation; logging alone may be traceability | Edge must be memoed |
| GOV_ACCOUNTABILITY_SUPPORT | Represented trace, attribution, forum, or review capability that supplies one component of an accountability relation | Use when the full actor-forum-explanation-judgement-consequence relation is not established; exclude generic data availability | Workflow history may support later review without proving answerability |
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

Enter proposed codes in a code-development log with definition, three supporting segments, two exclusion contrasts, relation to existing codes, and theoretical value. Candidate examples - not active codes - include `ALGORITHMIC_DELEGATION`, `TEMPORAL_CLOSURE`, and `CROSS_PROCESS_OBJECT`. Promote only after review; recode the corpus consistently and increment the manual version.

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

## Pilot decisions incorporated into version 1.0

1. Evidence records that combine several process steps remain eligible for pilot coding but receive no high-confidence mechanism code unless the relation is explicit. Full coding requires narrower page-level segmentation.
2. `BUSINESS_OBJECT`, `OBJECT_STATE`, `EVENT`, and `PROCESS_BOUNDARY` were added because process architecture cannot be reconstructed reliably from action and status codes alone.
3. `CLASSIFICATION` was added because organisational units, document types, account structures, and status categories may organise downstream action without being reducible to information visibility.
4. `TRACE_RECORD` and `GOV_ACCOUNTABILITY_SUPPORT` were added to prevent logs and histories from being over-coded as accountability.
5. `EXTENSION` was separated from `CONFIGURATION`. Configuration selects within predefined options; extension uses a released mechanism to add or adapt behaviour or representation.
6. A process label, role template, app identifier, or overview row never establishes actual authority, enacted work, effective control, or organisational outcome.
7. The pilot was single-coded. Codebook stability was assessed through evidence-to-code fit, rival interpretation, and re-coding consistency, not through inter-coder agreement.

