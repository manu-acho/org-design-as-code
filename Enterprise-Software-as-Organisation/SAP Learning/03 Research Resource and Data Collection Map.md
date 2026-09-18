# Research Resource and Data Collection Map

## Purpose

The study notes reveal several useful discovery routes for the research programme. They also create a risk: learning notes can easily be mistaken for empirical evidence. This map establishes what may guide learning, what may enter the corpus, and how to start data collection without collapsing encoded architecture into implementation practice.

## 1 Source classes

| Source class | Use for study | Use as Paper 1 evidence |
|---|---|---|
| Current official SAP reference-process content | Primary learning source | Yes, when release, region, product, process ID, URL, and retrieval date are registered |
| Official SAP Help documentation | Primary verification source | Yes, for explicitly documented functionality and constraints |
| Official SAP Learning content | Certification authority and conceptual orientation | Contextual evidence only; use product/reference artefacts for detailed architectural claims where possible |
| Official test scripts, setup guides, task tutorials, role/app references | Detailed process learning | Yes; especially valuable for steps, roles, prerequisites, exceptions, and configuration |
| Official SAP Activate Roadmap content | Method and implementation learning | Yes for encoded implementation method and decision structures, not for customer behaviour |
| Supplied Word notes | Revision and discovery | No, unless a claim is traced to the underlying official artefact |
| HackMD notes | Supplementary revision and link discovery | No; researcher-created notes are not independent evidence |
| SAP Community posts | Troubleshooting and discovery | Normally secondary; verify against SAP Help or reference content |
| Partner or consultancy pages | Interpretation and discovery | Secondary only; do not use to establish SAP reference architecture when official evidence exists |

## 2 Highest-value official sources identified

### SAP Signavio Process Navigator

This should be the centre of the first corpus. SAP’s official documentation confirms that solution-process pages can expose diagrams, solution activities, applications and application roles, descriptions, key steps, accelerators, integration information, regional variants, licensing indicators, and activation information.

For each selected process, capture:

1. solution scenario name and version;
2. solution-process name and official ID;
3. product/edition and country/region;
4. description and key-process steps;
5. process-flow diagram as PDF or SVG where permitted;
6. activity-to-application and application-role details;
7. test script and available task tutorials;
8. setup or configuration instructions;
9. integration and solution-component details;
10. licensing and “excluded from default activation” indicators;
11. retrieval date and stable locator;
12. comparison with the previous version if the selected content changed.

### SAP Help Portal

Use SAP Help to validate what a construct does and which conditions apply. Relevant categories include:

- enterprise structure and organisational assignments;
- Business Partner and master-data views;
- flexible workflow and approval conditions;
- business roles, catalogues, restrictions, and IAM;
- configuration activities and implementation guidance;
- document flow, statuses, blocks, and exception handling;
- account determination and integration postings;
- released APIs and extensibility;
- country/region-specific functions.

### Fiori Apps Reference Library or current app-reference surfaces

Use the current official application-reference source to identify app purpose, business roles/catalogues, implementation information, dependencies, and availability. Record the product version and do not infer data access solely from app assignment.

### SAP Activate Roadmap Viewer

Roadmap Viewer is useful for analysing the encoded implementation method: phases, deliverables, tasks, accelerators, roles, quality gates, and Fit-to-Standard guidance. It supports RQ5 but cannot establish what occurs in a real workshop.

### SAP Cloud ALM documentation

Official documentation is useful for the formal relations among process scope, requirements, tasks, user stories, testing, teams, and implementation status. It can show how the project architecture represents governance and traceability. Access to a live customer tenant would be a different data source and would require explicit ethical and access decisions.

## 3 Recommended pilot scope

The existing protocol proposes P2P, O2C, and R2R. The study notes now provide enough understanding to start with a small, auditable pilot while deeper process learning continues.

### Cross-cutting structural mini-corpus

Collect official artefacts for:

- company code and relevant enterprise-structure assignments;
- business roles, application roles, and access restrictions;
- Business Partner and one shared master-data object;
- workflow/approval configuration;
- one example of released extensibility or configuration governance.

### Two complementary artefacts per process

For one selected solution process in each domain, collect at minimum:

- the official solution-process page and process-flow diagram; and
- its official test script or procedural accelerator.

Add role/app and configuration artefacts where available. Two artefacts are a pilot minimum, not a complete corpus.

### Candidate process-selection logic

Select processes that make the mechanism of interest visible and have strong official documentation. Do not freeze IDs from course shorthand. Search Process Navigator in the selected S/4HANA Cloud Public Edition scenario and record the exact current IDs.

- **P2P:** a procurement process with requisition/order, receipt, supplier invoice, and approval or exception evidence.
- **O2C:** a sales process with order, fulfilment, billing, receivable, and a control such as credit, availability, or block handling.
- **R2R:** a process such as Accounts Payable or Accounting and Financial Close with explicit postings, roles, dependencies, and regional/accounting variants.

Official SAP documentation currently uses examples such as Accounts Payable `(J60)` and Accounting and Financial Close `(J58)`, but those examples must not be adopted automatically. Confirm their availability, scenario, region, and version when scope is frozen.

## 4 How to access and capture the data

### Process Navigator procedure

1. Open SAP Signavio Process Navigator.
2. Select the solution scenario for the exact product edition.
3. record the version and country/region before searching.
4. Filter by line of business or search for the process.
5. Open the solution process and record its official ID.
6. Inspect every available tab rather than relying on the diagram alone.
7. Download permitted diagrams and accelerators.
8. Save a stable capture or, where licensing prevents local preservation, record an exact locator and detailed source location.
9. Calculate or record a content hash for files retained locally.
10. Add the artefact immediately to `data/Corpus_Register_Template.csv` or a working copy derived from it.
11. Never overwrite a changed source; create a successor record linked through `supersedes_artifact_id`.

### What may require user access

- Process Navigator content or downloads that require an SAP Universal ID or entitlement.
- SAP for Me Roadmap Viewer content behind authentication.
- SAP Learning content tied to a Learning Hub subscription.
- SAP Cloud ALM live project or tenant data.
- HackMD notes that are not published for anonymous viewing.

If an official artefact is visible only in an authenticated browser session, you can open and sign in to that service, then provide the live page for assisted inspection. Do not share credentials. Any customer or project data must be assessed separately for confidentiality and research ethics.

## 5 Evidence extraction questions

For every evidence segment, ask:

1. What exactly does the artefact state or depict?
2. Which actor, organisational unit, object, or activity is involved?
3. What prerequisite, sequence, state transition, rule, or information relation is explicit?
4. Is the construct mandatory, configurable, extensible, exceptional, or merely available?
5. Which role can act, decide, configure, approve, or view, and within what scope?
6. What consequence follows if a condition is met or not met?
7. Is this normal-path documentation, an exception, or an integration boundary?
8. Does another official artefact corroborate or qualify it?
9. What is the narrowest defensible organisational interpretation?
10. What technical or alternative interpretation must be retained?

## 6 Connection to the research questions

| Research question | Evidence to prioritise |
|---|---|
| RQ1 Interdependence and coordination | process sequence, prerequisites, document flow, shared objects, handoffs, loops, exceptions |
| RQ2 Roles, rights, visibility, control | application roles, catalogues, restrictions, approvals, blocks, monitoring, audit-relevant statuses |
| RQ3 Standardisation and discretion | required fields, configuration activities, workflow conditions, extension points, exclusions from default activation |
| RQ4 Relation to theory | recurring supported mechanism patterns plus counter-examples across processes |
| RQ5 Fit-to-Standard | Activate tasks, workshop guidance, requirement categories, backlog relations, standard/deviation governance |

## 7 What can start now

Data collection can begin before the full literature review is complete, provided the release and scope are frozen first. Literature and empirical work should inform one another through memos without allowing new theoretical ideas to overwrite descriptive coding.

The first executable research package should contain:

1. a scope memo naming release, scenario, region, and three process IDs;
2. a populated corpus register for the structural mini-corpus and six process artefacts;
3. an evidence log with descriptive observations only;
4. a pilot coding matrix using the current codebook;
5. a method memo recording access limitations and ambiguities;
6. a theory memo recording candidate, rival, and rejected interpretations;
7. a completeness assessment before expanding the corpus.

## 8 Current access limitation

The Word files contain numerous HackMD links. Subsequent testing on 15 September 2026 established that the published finance and Recruit-to-Retire notes are readable, and their relevant content has been incorporated into the learning guide. Three directly tested links returned 403 Forbidden and were not used: `HJlJgdwEfe`, `ryenJuvVGg`, and `HJaRnrd8Ml`. Untested HackMD links remain discovery items rather than verified sources. In all cases, official SAP material remains the authority for certification and admissible product claims.
