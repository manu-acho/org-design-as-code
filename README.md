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

The project will produce a connected portfolio from one verified literature and evidence base:

1. **Scholarly foundation:** nine detailed literature streams, source assessments, a shared bibliography, and a consolidated review.
2. **Empirical infrastructure:** a release-controlled SAP corpus, evidence register, coding framework, analytical displays, and research memos.
3. **Research papers:** Paper 1 on software as codified organisation design, followed by studies of Fit-to-Standard, configuration, platform comparison, and AI agents.
4. **Research monograph:** **Enterprise Software as Organisation Design: Coordination, Processes and Transformation in SAP S/4HANA**.
5. **Academic course:** a postgraduate master course with controlled undergraduate and executive pathways.
6. **SAP learning assets:** cumulative End-to-End Processes and SAP Activate lessons, sources, and a research data-collection bridge.
7. **Serious game companion:** the deferred **Enterprise Design Lab** tabletop simulation concept.

The deliverables have different readiness gates. Theory-led outputs depend on the nine literature streams. Empirical papers, book chapters, and teaching cases depend on a frozen SAP scope, registered corpus, and validated coding. The serious game remains deferred until the literature and initial course modules are complete.

See the detailed [project README](Enterprise-Software-as-Organisation/README.md), [project status](Enterprise-Software-as-Organisation/PROJECT_STATUS.md), [book workspace](Enterprise-Software-as-Organisation/book/README.md), and [course workspace](Enterprise-Software-as-Organisation/course/README.md).

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
| `book/` | Research-monograph concept and proposal architecture |
| `course/` | Postgraduate curriculum, pathway designs, modules, cases, exercises, and assessments |
| `references/` | Working bibliography and verification notes |
| `figures/` | Guidance and eventual analytical figure outputs |
| `PROJECT_STATUS.md` | Authoritative record of completed and outstanding work |

## Current status

The project is at **research-design and corpus-readiness**. The conceptual framework, research and collection protocols, coding manual, analytical framework, manuscript architecture, templates, and execution plan are in place.

No SAP corpus has yet been collected or coded, and no empirical findings are claimed. The next milestone is to freeze the target SAP release and process IDs, verify the core bibliography, and build the pilot corpus. For the current completion boundary and next actions, see [PROJECT_STATUS.md](PROJECT_STATUS.md).

## Research quality principles

- Keep observation, interpretation, and theoretical inference separate.
- Do not use em dashes in project prose.
- Write for scholarly precision and teaching clarity: introduce the problem, define the concept, explain how authors connect, show its research use, and state its boundary.
- Preserve substantive detail during readability revisions; relocate complexity when necessary, but do not silently delete it.
- Preserve source version, provenance, and exact evidence location.
- Distinguish template roles and capabilities from configured or exercised authority.
- Require traceable evidence, a rival interpretation, and a stated scope for every retained claim.
- Search for exceptions and negative cases rather than analysing only normative process flows.
- Never convert a vendor representation into a claim about organisational outcomes without appropriate implementation or field evidence.

See the [Scholarly Writing and Teaching Standard](literature/WRITING_STANDARD.md) for the project-wide approach to reviews, the consolidated literature review, and the book.
