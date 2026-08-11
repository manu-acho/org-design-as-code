# Data Collection Protocol

## Collection sequence

Freeze `[TARGET SAP RELEASE]` and define included solution-process IDs. For each process, collect in this order: overview/process flow; test or procedural script; roles; app references; configuration; workflow/control documentation; master-data and organisational-structure dependencies; exceptions; extensibility. This sequence begins with process context but prevents the process diagram from becoming the sole representation.

Search official sources in priority order: SAP Signavio Process Navigator, SAP Help Portal, SAP Fiori Apps Reference Library, SAP Best Practices content, SAP Learning, then clearly labelled official SAP Community material. Log unsuccessful searches where absence informs a negative case.

## Corpus identifiers

Format: `DOMAIN-CLASS-NNN[-Vn]`.

- Domain: `P2P`, `O2C`, `R2R`, `STR` (enterprise structure), `XPR` (cross-process), `MTH` (method).
- Class: `PROC`, `ROLE`, `GOV`, `INFO`, `CTRL`, `CONF`, `EXT`, `MDAT`, `APP`, `METH`.
- NNN: zero-padded sequence assigned once.
- `Vn`: optional captured-version suffix; prior record is retained.

Examples such as `P2P-PROC-001`, `O2C-GOV-001`, `R2R-INFO-001`, and `STR-ORG-001` are identifiers only, not evidence that such records exist. (`ORG` may be used as a class alias for legacy consistency but `STR` domain plus `CONF`/`INFO` is preferred.) Evidence segments append `-E001`; coding observations receive independent `C-000001` IDs.

## Required capture record

Each corpus item must contain: artefact ID; process domain and official solution-process ID; artefact class; exact title; SAP product/edition; release/version; source URL; retrieval date and timezone; publisher/source status; document status; relevant organisational unit, business role, process step, object, and configuration object; source location; faithful evidence summary; short excerpt where permitted; screenshot or archive reference; analytical note separated from description; inclusion decision and rationale; supersession relation; and researcher initials.

## Capture rules

Record “not stated” rather than infer release. Preserve terminology exactly in the descriptive field and normalise only in separate analytic columns. For diagrams, identify node/edge/lane and transcribe labels. For videos or interactive content, record timestamp or stable element identifier plus screenshot where permitted. Excerpts must be short and necessary; the evidence summary is the main working representation.

One corpus item can yield many evidence segments. Do not create duplicate source records for cross-process relevance. Link the same artefact to multiple process codes in the coding matrix. If a page changes, capture it as a new version and write a release-drift memo.

## Completeness check per process

A process is collection-ready for analysis only when it has: an official boundary and identifier; process sequence; actor/role representation; primary business objects; organisational-unit relations; at least one control/exception search; configuration and extension search; source-release metadata; and a logged search for disconfirming or optional paths. Missing evidence is marked, not backfilled from another edition.

## Corpus-register schema

The operational CSV adds fields beyond the minimum: `artifact_id, process_domain, official_process_id, artifact_type, artifact_title, sap_product, sap_edition, sap_release, source_url, retrieval_date, publisher, source_grade, organisational_unit, business_role, process_step, business_object, configuration_object, source_location, archive_reference, document_status, inclusion_status, inclusion_rationale, supersedes_artifact_id, researcher, notes`. See `data/Corpus_Register_Template.csv`.

