# Theory-to-Evidence Operationalisation Matrix

**Status:** Week 6 pilot instrument

**Date:** 8 November 2026

**Codebook:** Version 1.0

## Purpose

This matrix connects the nine literature streams with observable SAP reference evidence without collapsing observation into theory. It is an analytical bridge, not a claim that every theoretical construct is visible in vendor documentation.

The sequence for every retained interpretation is:

1. source-close observation;
2. descriptive code;
3. organisational relation or primitive operation;
4. theoretical interpretation;
5. rival interpretation;
6. confidence and scope decision.

## Stream-level operationalisation

| Stream | Question explained | Observable reference evidence | Primary descriptive codes | Permitted inference | Required rival or boundary | Prohibited inference |
|---|---|---|---|---|---|---|
| 1. Organisation design | How is differentiated work divided and integrated? | Roles, activities, structural units, shared objects, workflow boundaries, information relations | ROLE, ACTION, HANDOFF, STRUCTURAL_UNIT, BUSINESS_OBJECT, INFORMATION | The reference architecture represents a division and integration of work within a stated boundary | Technical decomposition, documentation convenience, or product modularity may explain the representation | The adopting organisation has the represented structure or achieves fit |
| 2. Coordination theory | Which dependency is represented, and which mechanism addresses it? | Prerequisite states, shared resources, routed work, feedback, scheduling, common records | ACTION, HANDOFF, WORKFLOW, BUSINESS_OBJECT, OBJECT_STATE, MASTER_DATA | A specified mechanism is represented as addressing an identified pooled, sequential, or reciprocal dependency | Temporal order alone may not be dependency; a shared platform alone may not be pooled interdependence | Coordination is successful or organisational performance improves |
| 3. Decision theory | How are premises, alternatives, attention, and programmes distributed? | Rules, thresholds, defaults, approval alternatives, exception categories, automated determinations | DECISION, RULE, THRESHOLD, APPROVAL, CLASSIFICATION, SYSTEM_ACTION | The architecture supplies or constrains decision premises and programmes | Deterministic logic, transaction consistency, or a technical status change may explain the artefact | A user exercised judgement, accepted authority, or made a high-quality decision |
| 4. Enterprise systems, implementation, and transformation | What is encoded, what can be configured, and what remains implementation work? | Reference scope, configuration options, extension points, project and transport documentation | PROCESS_BOUNDARY, CONFIGURATION, EXTENSION, ROLE, STRUCTURAL_UNIT | The product offers a bounded architecture and sanctioned variation mechanisms | Customer configuration, implementation choice, and adaptation are not observed in reference content | Reference architecture equals implementation fit or transformation outcome |
| 5. Organisational routines | How do artefacts relate to recurrent patterns of action? | Test scripts, procedures, workflows, statuses, exception and rework paths | WORKFLOW, ACTION, STATUS, OBJECT_STATE, EXCEPTION, TRACE_RECORD | An artefact may prescribe, cue, record, or constrain aspects of a possible routine | A test script may be instructional; a workflow may be optional; a trace may omit unrecorded work | The reference process is an ostensive routine or evidence of recurrent performance |
| 6. Technology, materiality, and organisation | What material arrangements create candidate possibilities or constraints? | Required fields, permissions, routing logic, automation, shared records, interfaces | ACCESS, RULE, WORKFLOW, SYSTEM_ACTION, INFORMATION, EXTENSION | A represented arrangement supports a conditional candidate-affordance or constraint statement | Perception, goal, capability, and actualisation remain unknown | Feature availability establishes use, affordance actualisation, practice, or outcome |
| 7. Digital infrastructure, standards, and classification | How do standards, categories, installed-base relations, and control points connect distributed work? | Master data, organisational codes, classifications, interfaces, releases, extension and change rules | MASTER_DATA, CLASSIFICATION, STRUCTURAL_UNIT, PROCESS_BOUNDARY, EXTENSION | The reference architecture contains candidate infrastructural components and cross-process dependencies | A bounded product may remain one application; embeddedness and maintenance work require field evidence | A large or global ERP product is infrastructure-in-use by definition |
| 8. Governance, control, accountability, and decision rights | Who may act, decide, monitor, intervene, override, and demand an account? | Authorisations, restrictions, approvals, blocks, validations, monitoring, escalation, traces | ACCESS, APPROVAL, CONTROL, ESCALATION, TRACE_RECORD, RULE | Formal rights, standards, observation, intervention, and accountability support are represented within a stated scope | Formal and real authority may diverge; traceability may lack a forum, judgement, or consequence | Permission is legitimate authority; traceability is accountability; control presence proves effectiveness |
| 9. BPM and process architecture | What does the process representation include, exclude, connect, and vary? | Events, activities, actors, objects, states, gateways, variants, exceptions, process relationships | EVENT, ACTION, ROLE, BUSINESS_OBJECT, OBJECT_STATE, PROCESS_BOUNDARY, EXCEPTION | A release-controlled reference-process architecture can be reconstructed by triangulating artefacts | Models and logs are selective representations with different purposes and granularity | A diagram, test script, executable model, or event log is the complete performed process |

## Relation-level tests

| Candidate relation | Minimum evidence | Confidence blocker |
|---|---|---|
| Sequential interdependence | Named output or state of activity A required by activity B | Mere ordering in an overview list |
| Pooled interdependence | Differentiated activities demonstrably rely on one governed resource, category, or output | Shared product or database without reliance evidence |
| Reciprocal interdependence | Two activities or actors revise or condition each other's substantive inputs | One-way rejection or return without mutual adjustment |
| Decision right | Actor or role, alternatives, object, scope, and organisational consequence | App access or role label alone |
| Formal control | Standard or expected state, observation or comparison, and intervention or consequence | Report, rule, or block in isolation |
| Accountability | Actor, domain, forum, obligation to explain, questioning, judgement, and possible consequence | Attribution, logging, responsibility label, or approval alone |
| Candidate affordance | Actor class, technical arrangement, possible action, goal, and conditions stated conditionally | Feature name without actor, action, or conditions |
| Infrastructural relation | Cross-setting dependency, standard or classification, installed-base relation, and evidence of embeddedness | Product scale or availability alone |

## Pilot use

The matrix governs the 15-segment pilot. It does not require every stream to appear in every segment. Codes are applied only where the evidence satisfies the minimum test. An empty theoretical field is preferable to a plausible but unsupported interpretation.
