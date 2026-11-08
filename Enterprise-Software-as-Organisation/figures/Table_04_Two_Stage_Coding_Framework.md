# Table 4. Two-Stage Coding Framework

**Status:** Week 6 draft. Examples are pilot records about vendor reference representations, not organisational findings.

| Evidence ID | Source-close description | Stage 1 descriptive coding | Stage 2 theoretical interpretation | Rival and confidence |
|---|---|---|---|---|
| EV2608CH-0002 | Requisition initiation and conversion may be manual or automatic | ACTION, USER_ACTION, SYSTEM_ACTION, BUSINESS_OBJECT, CONFIGURATION | Alternative allocation of initiation and conversion work; sequential dependency; configurable discretion | May reflect product convenience rather than organisational design; moderate |
| EV2608CH-0006 | Purchase-order approval includes rework and an ad hoc approver option | WORKFLOW, APPROVAL, HANDOFF, CONFIGURATION, EXCEPTION | Represented approval gate and rework relation; candidate approval authority | Optional capability does not establish activated or real authority; moderate |
| EV2608CH-0008 | Sales order proceeds through delivery, picking, goods issue, and billing | ACTION, BUSINESS_OBJECT, OBJECT_STATE, HANDOFF, PROCESS_BOUNDARY | Represented sequential dependency across commercial, logistical, inventory, billing, and accounting work | High-level sequence may omit parallel and manual work; high |
| EV2608CH-0012 | Credit and approval rows include blocked review, withdrawal, rejection, and rework | DECISION, APPROVAL, CONTROL, EXCEPTION, WORKFLOW, OBJECT_STATE | Formal gate, exception signal, configurable authority and control candidate | Automated rules may resolve cases; real authority is unknown; moderate |
| EV2608CH-0018 | Journal-entry rows distinguish posting, verification, approval, rejection, editing, and reversal | ACTION, BUSINESS_OBJECT, OBJECT_STATE, APPROVAL, EXCEPTION | Differentiated initiation, review, correction, and reversal operations on one represented object | Rows may represent variants rather than one state system; moderate |
| EV2608CH-0020 | Reporting and validation rows include audit journal, balances, statements, and validation | INFORMATION, CONTROL, TRACE_RECORD, BUSINESS_OBJECT | Common accounting information may support review, validation, monitoring, and accountability | Availability does not establish use, intervention, or accountability forum; moderate |

## Reading rule

Stage 1 can be retained wherever the source explicitly supports it. Stage 2 is retained only when the relation satisfies the codebook test, carries a rival interpretation, and remains within the reference-architecture boundary.
