# Research Protocol

## Epistemological position and design

The study adopts a critical-realist-compatible interpretive stance: reference artefacts are treated as materially consequential representations of intended capabilities, not transparent descriptions of organisational reality. Documentary and architectural analysis reconstructs encoded mechanisms through abductive movement between SAP evidence and organisation theory. The single instrumental case is SAP S/4HANA Cloud Public Edition, with embedded P2P, O2C, and R2R process domains selected for theoretical variation.

The core unit is an **encoded organisational arrangement**: a bounded relation among differentiated actor/activity/object, dependency, and software mechanism. Micro units are primitive-in-relation observations; meso units are solution processes; macro inference compares processes plus enterprise-structure and cross-cutting governance artefacts.

## Evidence hierarchy

| Grade | Source | Permissible use |
|---|---|---|
| A | Release-specific official process flow, product help, configuration documentation, Fiori reference, setup/test script | Architectural description within stated release |
| B | Current official SAP method, learning, or conceptual documentation without precise release | Conceptual interpretation; corroboration, not fine-grained behaviour alone |
| C | Official SAP Community contribution or recorded demonstration | Discovery and contextual corroboration; label authorship/status |
| D | Scholarly/credible secondary analysis of SAP | Positioning or rival interpretation |
| E | Consultancy/blog/undated derivative material | Discovery only; exclude from claim support unless uniquely necessary and explicitly qualified |

No single process diagram should support a governance claim when product or authorisation documentation is available. Screenshots preserve visual evidence but must be accompanied by title, URL, retrieval date, release, and a text summary.

## Inclusion and exclusion

Include artefacts explicitly applicable to SAP S/4HANA Cloud Public Edition and the recorded release; artefacts that define enterprise structure, scoped processes, roles, rights, workflows, master data, configuration, or extensions; and method documents necessary to interpret Fit-to-Standard. Include cross-cutting artefacts when they directly affect a scoped process.

Exclude private-edition/on-premise evidence unless used as a labelled contrast; obsolete or release-ambiguous material when a release-specific source exists; marketing claims without architectural detail; partner customisations; customer practices; and process domains outside scope. Do not silently transfer functionality across editions or releases.

## Corpus construction and version control

Freeze a study release before full collection: `[TARGET SAP RELEASE]`. Record source release independently because some cross-cutting pages use rolling documentation. Store stable PDFs or screenshots where licence and access permit; otherwise store a locator, access metadata, and a content hash or detailed source-location description. Name files `ARTIFACTID_short-title_release_YYYY-MM-DD.ext`. Never overwrite a changed source: create a new corpus record and link it with `supersedes_artifact_id`.

Every item enters the corpus register before coding. A weekly change log records additions, exclusions, duplicate resolution, broken links, and release drift. Raw evidence remains immutable; extracts and analytic notes are separate.

## Coding procedure

1. Segment evidence at the smallest passage or diagram element that supports a coherent observation; retain enough context to prevent meaning loss.
2. Apply descriptive codes without theoretical labels. Record actor, action, object, condition, sequence, state, source modality, and uncertainty.
3. Propose a software primitive only after the construct meets the codebook criteria.
4. Apply theoretical codes to relations, not keywords. A dependency requires two differentiated activities and a relation; governance requires an actor–right–object–scope relation.
5. Write an inference statement: `Because [documented operation], the architecture may instantiate [mechanism] for [dependency], within [scope].`
6. Record at least one plausible alternative interpretation for theoretically consequential observations.
7. Promote patterns only through within-process replication or a justified critical instance; promote macro patterns only after cross-process comparison.

Pilot coding uses a deliberately varied sample of at least two artefacts per process plus one structural, one authorisation, and one workflow source. Revise code definitions before freezing codebook version 1.0. If multiple coders are available, independently code a shared purposive subset, discuss disagreements by rule, and report agreement as a diagnostic rather than a substitute for interpretive resolution.

## Memoing, negative cases, and rivals

Observation and interpretation occupy separate memo sections. Negative-case searches are designed before findings: look for ungated handoffs, optional rather than mandatory workflow, rights without explicit decisions, exceptions that leave the system, local-information requirements not represented, and mechanisms contradicting the dominant process pattern. Rival interpretations include technical necessity, accounting/legal compliance, interface convenience, and documentation convention. These do not automatically defeat an organisational interpretation; the analysis must show why the organisational mechanism adds explanatory value.

## Quality and validity

Construct validity comes from explicit definitions and triangulation across artefact classes. Interpretive validity comes from inference chains, rival explanations, peer challenge, and negative cases. Reliability is pursued through a frozen manual, corpus identifiers, coding decision logs, and versioned matrices - not through a claim of theory-free replication. Triangulation compares process, product, role/authorisation, and configuration representations. Divergence is data and receives a discrepancy memo.

The audit trail comprises corpus register, immutable captures or locators, evidence log, coding matrix, codebook version, memo links, analytic displays, claim–evidence table, and manuscript commit history. A reader should be able to move from a manuscript claim back to evidence and forward from each evidence segment to its interpretations.

## Ethics and limitations

Public documentary analysis normally involves no human participants, but licence terms, access controls, copyright, and institutional requirements must be checked. Do not reproduce restricted SAP content beyond permitted quotation or screenshot use. If workshops or interviews are added, obtain ethics approval before collection.

The study analyses intended/reference architecture. It cannot establish adoption, compliance, behaviour, outcomes, or superiority. Vendor documents are selective and normative; release change threatens stability; SAP limits generalisability; and theoretical coding is interpretive. These are design boundaries managed through qualification, not inconveniences to be written away.

