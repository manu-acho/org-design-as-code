# Enterprise Software as Codified Organisation Design

This repository is the research environment for a programme examining enterprise software as a form of codified organisation design. Rather than beginning with what happens after a system is implemented, the project asks what model of organisation is already represented in an enterprise-software reference architecture: how work is divided, dependencies are coordinated, decisions are allocated, information is made visible, and behaviour is constrained or enabled.

SAP S/4HANA Cloud Public Edition is the instrumental case. The initial empirical study focuses on Procure-to-Pay (P2P), Order-to-Cash (O2C), and Record-to-Report (R2R), using release-controlled official reference artefacts.

## Research objective

The primary research question is:

> **How are organisational coordination and governance mechanisms encoded within enterprise software reference architectures?**

The project has five objectives:

1. Reconstruct the forms of interdependence and coordination encoded in enterprise processes.
2. Identify how roles, decision rights, information access, and control are distributed through the architecture.
3. Examine how standardisation, discretion, exception handling, and escalation are represented.
4. Assess where encoded arrangements correspond to, combine, or depart from classical organisation theory.
5. Develop a rigorous foundation for later research on Fit-to-Standard, implementation choices, cross-platform variation, and AI agents as organisational actors.

Thompson's theory of interdependence, Galbraith's information-processing view, and Mintzberg's coordination mechanisms provide the main theoretical lenses. A candidate contribution is the concept of the **software organisational primitive**: a recurring construct - such as a role, workflow, status, rule, approval, block, access right, master-data object, or system event - that performs an identifiable organisational operation.

## Scope and analytical boundary

The first study analyses **encoded organisational logic**: the possibilities, constraints, relations, and assumptions represented in vendor reference artefacts. It deliberately distinguishes this from:

- **Implemented organisational configuration:** what a particular organisation selects, configures, extends, and integrates.
- **Enacted organisational practice:** how people actually perform, interpret, adapt, or work around those arrangements.

Documentary evidence can establish what the reference architecture represents or permits. It cannot establish customer behaviour, implementation outcomes, performance effects, or how work is enacted. The project therefore does not assume that software determines organisation.

## Intended deliverables

### Paper 1: Software as Codified Organisation Design

The immediate deliverable is a journal-ready study comprising:

- a release-controlled corpus of official SAP reference artefacts;
- an auditable evidence register and coded evidence set;
- a validated two-stage coding framework linking software constructs to organisational mechanisms;
- within-process dependency and mechanism maps for P2P, O2C, and R2R;
- a cross-process comparison of coordination, governance, information-processing, and control arrangements;
- an evaluated set of software organisational primitives, including counter-evidence and boundary conditions;
- a claim–evidence–rival interpretation table with confidence judgements;
- analytical figures, tables, research memos, and a complete manuscript.

### Longer-term research programme

The first study provides the conceptual and methodological foundation for subsequent work on:

1. Fit-to-Standard as organisational design negotiation.
2. Cloud ERP configuration as bounded organisational discretion.
3. Comparative organisational logics across enterprise-software platforms.
4. AI agents as coordination, delegation, and governance actors.

See [12_Paper_Pipeline.md](12_Paper_Pipeline.md) for the provisional sequence, data requirements, and contribution of each paper.

### Research monograph

The programme now includes a provisional research monograph, **Enterprise Software as Organisation Design: Coordination, Processes and Transformation in SAP S/4HANA**. The book will integrate the theoretical framework, documentary method, end-to-end process analyses, comparative findings, and transformation implications for a broader academic and reflective-practitioner audience. It will share the verified literature and empirical evidence base but will not reproduce the dissertation or article manuscripts.

The proposal is gated by empirical progress: it should not be submitted until the SAP scope is frozen, the pilot and codebook are accepted, at least one process analysis is complete, and the comparative promise is evidence-supported. See the [book workspace](book/README.md) and [book status](book/BOOK_STATUS.md).

### Postgraduate course and derived pathways

The programme now includes a postgraduate master course, **Enterprise Software as Organisation Design: Processes, Coordination and Digital Transformation**. The course converts verified theory, process learning, documentary method, and eventual empirical cases into a twelve-week curriculum with aligned learning outcomes, activities, and assessments.

The postgraduate design is the source curriculum. Advanced undergraduate and executive pathways may be derived from it through controlled adaptations in depth, pacing, readings, activities, and assessment. Course content shares the project's literature, bibliography, SAP corpus, and evidence controls. No module or case may be designated teaching-ready until it passes the course's source, provenance, instructional-alignment, and inferential checks. See the [course workspace](course/README.md) and [course status](course/COURSE_STATUS.md).

## Research workflow

1. Freeze the target SAP release and exact solution-process scope.
2. Register and preserve each source using the corpus protocol.
3. Segment artefacts into traceable evidence records.
4. Code descriptive software constructs before applying theoretical interpretations.
5. Build within-process maps and cross-process analytical displays.
6. Test candidate claims against rival explanations and negative cases.
7. Draft findings only from evidenced analytical memos.

Start with [06_Research_Protocol.md](06_Research_Protocol.md), use [07_Data_Collection_Protocol.md](07_Data_Collection_Protocol.md) for corpus construction, apply [08_Coding_Manual.md](08_Coding_Manual.md), and produce comparisons using [09_Analytical_Framework.md](09_Analytical_Framework.md).

## Repository structure

| Location | Purpose |
|---|---|
| `00_Research_Vision.md`–`05_SAP_Knowledge_Map.md` | Research framing, questions, theory, literature, and case knowledge |
| `06_Research_Protocol.md`–`10_Research_Memos.md` | Collection, coding, analysis, and inferential discipline |
| `11_Figure_and_Table_Plan.md`–`15_Execution_Plan.md` | Outputs, paper programme, translation, risks, and delivery plan |
| `data/` | Corpus, evidence-log, and coding-matrix templates |
| `literature/` | Reading list, source audits, detailed reviews, and note templates |
| `memos/` | Analytical, theoretical, and methodological memo templates |
| `paper/` | Working manuscript blueprint and section drafts |
| `book/` | Research-monograph concept, Springer proposal, market analysis, chapter architecture, and reuse controls |
| `course/` | Postgraduate master curriculum, derived pathways, module scaffolds, cases, assessments, and teaching standards |
| `references/` | Working bibliography and verification notes |
| `figures/` | Guidance and eventual analytical figure outputs |
| `SAP Learning/` | Cumulative E2E and SAP Activate lessons, source register, and research data-collection bridge |
| `PROJECT_STATUS.md` | Authoritative record of completed and outstanding work |

## Current status

The project is at **research-design and corpus-readiness**. The conceptual framework, research and collection protocols, coding manual, analytical framework, manuscript architecture, templates, and execution plan are in place.

No SAP corpus has yet been collected or coded, and no empirical findings are claimed. The next milestone is to freeze the target SAP release and process IDs, verify the core bibliography, and build the pilot corpus. For the current completion boundary and next actions, see [PROJECT_STATUS.md](PROJECT_STATUS.md).

## Research quality principles

- Do not use em dashes in project prose. Use commas, colons, parentheses, or sentence breaks instead.
- Keep observation, interpretation, and theoretical inference separate.
- Preserve source version, provenance, and exact evidence location.
- Distinguish template roles and capabilities from configured or exercised authority.
- Require traceable evidence, a rival interpretation, and a stated scope for every retained claim.
- Search for exceptions and negative cases rather than analysing only normative process flows.
- Never convert a vendor representation into a claim about organisational outcomes without appropriate implementation or field evidence.
