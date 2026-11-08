# Pilot Coding Decision Log

**Pilot:** SAP S/4HANA Cloud Public Edition 2608, Switzerland

**Processes:** J45, BD9, J58

**Date:** 8 November 2026

**Codebook:** Version 1.0

## Decision 1: preserve two-stage coding

**Problem.** Initial evidence summaries already contained interpretive wording.

**Decision.** The pilot matrix uses `raw_description` for a source-close representation and places organisational meaning only in `interpretation`. Existing evidence-log claims are not copied automatically into theoretical fields.

**Consequence.** Full coding must return to the cited page or diagram location whenever the evidence summary combines observation and inference.

## Decision 2: narrow the unit of coding

**Problem.** Several evidence records summarise an overview table or interactive diagram containing several mechanisms.

**Decision.** Bundle-level records may test the codebook but cannot support a high-confidence mechanism claim unless the relation is explicit. Before Weeks 7 and 8, high-value rows must be segmented by individual page, step, branch, or object-state transition.

**Consequence.** Pilot interpretations based on overview bundles are marked moderate or low and carry a collect-more instruction.

## Decision 3: add process-representation codes

**Problem.** The original descriptive codebook could identify actions and statuses but could not reconstruct process architecture reliably.

**Decision.** Add EVENT, BUSINESS_OBJECT, OBJECT_STATE, and PROCESS_BOUNDARY.

**Consequence.** Full coding can now distinguish occurrence, work, entity, state, and scope.

## Decision 4: distinguish classification from generic information

**Problem.** Organisational assignments, account structures, document types, and status categories can determine downstream action. INFORMATION alone hides that operation.

**Decision.** Add CLASSIFICATION when a category or code has an identified or explicitly investigable consequence.

**Consequence.** A category with no demonstrated consequence remains descriptive and receives no infrastructure or governance inference.

## Decision 5: separate traceability from accountability

**Problem.** Change histories and workflow records could be over-coded as accountability.

**Decision.** Add TRACE_RECORD descriptively and GOV_ACCOUNTABILITY_SUPPORT theoretically. Reserve GOV_ACCOUNTABILITY for evidence of an actor-forum relationship with explanation, judgement, and possible consequence.

**Consequence.** No pilot segment establishes full accountability.

## Decision 6: separate configuration from extension

**Problem.** Selectable options and released mechanisms for adding fields or logic represent different forms of discretion.

**Decision.** CONFIGURATION records selection among predefined options. EXTENSION records use or availability of a released adaptation mechanism.

**Consequence.** Neither code establishes that a customer selected or used the mechanism.

## Decision 7: treat role templates as offered actor categories

**Problem.** Test-script roles may appear to allocate jobs or authority.

**Decision.** Code ROLE only. Add governance or segregation codes only when a separate source establishes the relevant right, restriction, incompatibility, or consequence.

**Consequence.** Different role names do not establish segregation of duties.

## Decision 8: do not force one dependency type

**Problem.** Exception and reconciliation bundles may combine sequential and reciprocal relations.

**Decision.** Use the least inferential supported code. Record a reciprocal candidate only when two activities materially adjust one another. Otherwise retain sequential dependency and state the possible feedback interpretation as a rival.

## Decision 9: record the single-coder limitation

**Problem.** No second coder participated in the Week 6 pilot.

**Decision.** Do not report inter-coder reliability. Use evidence-to-code fit, explicit exclusion tests, rival interpretations, and a second-pass consistency review by the same researcher.

**Consequence.** A later peer debrief or independent recoding remains desirable before submission but is not represented as completed.

## Decision 10: freeze version 1.0 provisionally

**Problem.** Weeks 7 and 8 require a stable codebook, but narrower evidence may reveal further edge cases.

**Decision.** Freeze version 1.0 for within-process coding. Any new code requires the emergent-code promotion rule and a version increment.

**Consequence.** Clarifications that do not change inclusion rules may be logged without increment; substantive additions or redefinitions require version 1.1 or 2.0 depending on compatibility.
