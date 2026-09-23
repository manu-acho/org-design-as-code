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

The programme is designed to produce a connected portfolio of scholarly, educational, and practitioner outputs from one verified literature and evidence base. These deliverables have different readiness gates and must not be treated as if they were all complete.

| Deliverable family | Principal output | Current maturity |
|---|---|---|
| Scholarly foundation | Nine detailed literature streams, source assessments, shared bibliography, and consolidated review | Streams 1 to 4 complete; Streams 5 to 9 planned |
| Empirical infrastructure | Release-controlled SAP corpus, evidence register, coding framework, analytical displays, and research memos | Designed but not yet populated |
| Research papers | Paper 1 and a longer-term article programme | Paper 1 architecture drafted; empirical findings not yet available |
| Research monograph | Springer-oriented research book integrating theory, method, process analysis, and transformation | Concept and proposal architecture established |
| Academic course | Postgraduate master course with undergraduate and executive pathways | Curriculum architecture established; modules not yet teaching-ready |
| SAP learning assets | Cumulative End-to-End Processes and SAP Activate lessons, sources, and research bridge | Active and progressively updated |
| Serious game | Course-companion enterprise-design simulation | Concept memo only; intentionally deferred |

### 1. Scholarly foundation

The immediate theoretical programme is to complete nine non-duplicative literature streams:

1. organisation design;
2. coordination theory;
3. decision theory;
4. enterprise systems, implementation, and transformation;
5. organisational routines;
6. technology, materiality, and organisation;
7. digital infrastructure, standards, and classification;
8. governance, control, accountability, and decision rights;
9. business-process management and process architecture.

Each stream should produce a detailed review and source assessment. The streams will then support a consolidated literature review, theory-led book chapters, and theory-led course modules without duplicating literature work. See the [literature map](03_Literature_Map.md), [reading route](literature/Reading_List.md), and [writing standard](literature/WRITING_STANDARD.md).

### 2. Empirical research infrastructure

The empirical programme will produce:

- a release-controlled corpus of official SAP reference artefacts;
- an auditable evidence register and coded evidence set;
- a validated two-stage coding framework linking software constructs with organisational mechanisms;
- within-process maps for P2P, O2C, and R2R;
- cross-process comparisons of coordination, governance, information, decision, and control arrangements;
- negative-case and rival-interpretation records;
- claim-evidence-rival tables with confidence judgements;
- analytical figures, tables, and research memos.

These outputs remain gated by the SAP release freeze, exact process scope, corpus registration, and codebook pilot.

### 3. Research papers

The immediate paper is **Software as Codified Organisation Design**. It will develop and evaluate a documentary method for reconstructing the organisational logic represented in enterprise-software reference architecture. It will also assess the candidate concept of the software organisational primitive.

The longer-term paper programme addresses:

1. Fit-to-Standard as organisational design negotiation;
2. cloud ERP configuration as bounded organisational discretion;
3. comparative organisational logics across enterprise-software platforms;
4. AI agents as coordination, delegation, and governance actors.

See the [paper pipeline](12_Paper_Pipeline.md) and [paper blueprint](paper/00_Paper_Blueprint.md).

### 4. Research monograph

The provisional monograph is **Enterprise Software as Organisation Design: Coordination, Processes and Transformation in SAP S/4HANA**. It will integrate the theoretical framework, documentary method, end-to-end process analyses, comparative findings, and transformation implications for academic and reflective-practitioner audiences.

The book will share the verified literature and evidence base without reproducing the paper manuscripts. Theory-led chapters may be developed after the nine streams are complete. Empirical chapters remain conditional on the corpus and analysis. A proposal should not be submitted until the empirical gate recorded in the book workspace is satisfied. See the [book workspace](book/README.md) and [book status](book/BOOK_STATUS.md).

### 5. Academic course and pathways

The postgraduate master course is **Enterprise Software as Organisation Design: Processes, Coordination and Digital Transformation**. It converts verified theory, process knowledge, documentary method, and eventual empirical cases into a twelve-week curriculum with aligned outcomes, activities, and assessments.

The postgraduate design is the source curriculum. Advanced undergraduate and executive pathways will be derived through controlled changes in depth, pacing, readings, activities, and assessment. Theory-led modules can be developed from completed literature streams. SAP teaching cases remain gated by controlled empirical evidence. See the [course workspace](course/README.md), [literature crosswalk](course/06_Literature_Crosswalk.md), and [course status](course/COURSE_STATUS.md).

### 6. SAP learning and professional knowledge assets

The SAP Learning workspace will continue to consolidate End-to-End Business Processes and SAP Activate study material. Its outputs include cumulative lessons, a source register, a research-resource map, and a bridge from certification learning to controlled data collection. Certification notes support learning and source discovery but do not replace verified scholarly or empirical evidence. See [SAP Learning](SAP%20Learning/README.md).

### 7. Serious game companion

The deferred **Enterprise Design Lab: The Organisation Behind the System** concept may eventually accompany the course. The proposed tabletop simulation would allow participants to experience trade-offs among standardisation, coordination, authority, discretion, control, exception handling, and resilience.

Active development will begin only after the nine literature streams and initial theory-led modules are complete. SAP-specific scenarios will require controlled corpus evidence and permissions review. See the [serious game concept memo](course/07_Serious_Game_Concept_Memo.md).

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
