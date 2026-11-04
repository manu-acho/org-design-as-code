# Enterprise Software as Codified Organisation Design

## Programme overview

Enterprise software represents more than transactions and data. Through roles, workflows, business objects, rules, permissions, approvals, controls, and exceptions, it also represents assumptions about how organisational work should be arranged.

This research programme examines enterprise-software reference architecture as a form of codified organisation design. Its central concern is the organisational logic visible before attention turns to a particular customer implementation: how work is divided, dependencies are coordinated, decisions are structured, information is distributed, and behaviour is enabled or constrained.

SAP S/4HANA Cloud Public Edition provides the instrumental case for the first empirical study. Procure-to-Pay, Order-to-Cash, and Record-to-Report provide the initial basis for comparison across end-to-end enterprise processes.

## Central research question

> **How are organisational coordination and governance mechanisms encoded within enterprise-software reference architectures?**

Five supporting objectives guide the programme:

1. Reconstruct the forms of interdependence and coordination represented in enterprise processes.
2. Identify how roles, information access, decision opportunities, and control are distributed through the architecture.
3. Examine how standardisation, discretion, exception handling, and escalation are represented.
4. Compare encoded arrangements with established organisation theory.
5. Build a foundation for later research on implementation, Fit-to-Standard, configuration, platform variation, and AI agents.

## Intellectual position

The programme begins from a simple proposition: enterprise software can carry organisational design without fully determining organisation.

Reference architecture can represent how activities should connect, which roles may act, what information must be available, when approval is required, and how exceptions should proceed. Those representations are organisationally consequential, but they are not equivalent to a customer's configured system or to work as performed in practice.

The analysis therefore distinguishes:

- **encoded organisational logic**, represented in vendor reference architecture;
- **implemented organisational configuration**, selected and adapted in a particular organisation;
- **enacted organisational practice**, performed and interpreted in everyday work.

This distinction makes it possible to study software architecture seriously without assuming technological determinism.

## Theoretical architecture

Thompson's account of interdependence, Galbraith's information-processing view, and Mintzberg's coordination mechanisms provide the initial organisation-design foundation. The programme then connects these foundations with decision theory, enterprise-systems research, organisational routines, technology and materiality, digital infrastructure, governance, and business-process management.

The shared literature programme contains nine streams:

| No. | Literature stream | Principal contribution |
|---:|---|---|
| 1 | Organisation design | Division of work, integration, information processing, configuration, and fit |
| 2 | Coordination theory | Dependencies, mechanisms, accountability, predictability, and common understanding |
| 3 | Decision theory | Bounded rationality, premises, programmes, authority, and discretion |
| 4 | Enterprise systems, implementation, and transformation | Integration, standardisation, lifecycle, misfit, adaptation, and implementation choice |
| 5 | Organisational routines | Artefacts, ostensive understandings, recurrent performance, stability, and change |
| 6 | Technology, materiality, and organisation | Practice, affordance, constraint, actualisation, and sociomateriality |
| 7 | Digital infrastructure, standards, and classification | Installed bases, shared classifications, generativity, and path dependence |
| 8 | Governance, control, accountability, and decision rights | Monitoring, intervention, answerability, legitimacy, and consequences |
| 9 | Business-process management and process architecture | Process representation, events, actors, objects, variation, and orchestration |

Detailed reviews for Streams 1 to 6 are complete. Streams 7 to 9 will complete the theoretical foundation before the consolidated review is written. See the [literature map](03_Literature_Map.md) and [reading route](literature/Reading_List.md).

## Candidate conceptual contribution

The programme develops the candidate concept of the **software organisational primitive**: a recurring software construct that performs an identifiable organisational operation.

Possible primitives include:

- roles and access rights that allocate possible action;
- workflows and statuses that structure progression;
- rules, thresholds, and approvals that programme or constrain decisions;
- master-data objects and shared records that organise information;
- blocks, alerts, and exception routes that govern deviation;
- system events that connect activities across processes.

The unit of explanation is not the isolated primitive but the configuration. Organisational design becomes visible in the relations among tasks, actors, information, decision rights, controls, and coordination mechanisms.

## Empirical strategy

The first study uses controlled documentary analysis of official SAP reference artefacts. Descriptive coding identifies what the architecture represents before theoretical coding interprets the organisational operation.

The comparison of Procure-to-Pay, Order-to-Cash, and Record-to-Report will examine:

- forms of interdependence;
- coordination and information mechanisms;
- role and responsibility allocation;
- decision premises and approval structures;
- control, visibility, and traceability;
- variation, exception handling, and escalation;
- relations among activities, objects, roles, and events.

The method preserves the boundary between architectural evidence and claims about implementation or practice. Later empirical studies can extend the analysis to configured systems, Fit-to-Standard activity, and enacted organisational work.

## Research programme and outputs

### Scholarly research

The immediate paper, **Software as Codified Organisation Design**, develops and evaluates the documentary method and the candidate concept of the software organisational primitive. The wider paper programme addresses Fit-to-Standard, cloud ERP configuration, cross-platform comparison, and AI agents as coordination and governance actors.

See the [paper pipeline](12_Paper_Pipeline.md) and [paper blueprint](paper/00_Paper_Blueprint.md).

### Research monograph

The proposed monograph, **Enterprise Software as Organisation Design: Coordination, Processes and Transformation in SAP S/4HANA**, brings together the theoretical framework, documentary method, process analyses, comparative findings, and implications for digital transformation.

See the [book overview](book/README.md).

### Academic course

The postgraduate course, **Enterprise Software as Organisation Design: Processes, Coordination and Digital Transformation**, translates the research into a twelve-week curriculum. Advanced undergraduate and executive pathways extend the same intellectual foundation at different levels of depth and application.

See the [course overview](course/README.md).

### Applied research

The theoretical framework can support separately designed studies of inter-organisational systems, supply networks, platform governance, and digitally mediated coordination. These applications remain analytically distinct from the SAP case while drawing on the shared literature and method.

See the [research workstreams](workstreams/README.md).

### Enterprise-design simulation

The proposed **Enterprise Design Lab: The Organisation Behind the System** is a future course companion. It is intended to make trade-offs among standardisation, coordination, discretion, authority, control, exception handling, and resilience visible through simulation.

## Explore the repository

| Research area | Public material |
|---|---|
| Vision and questions | [Research vision](00_Research_Vision.md) and [research questions](01_Research_Questions.md) |
| Conceptual framework | [Conceptual framework](02_Conceptual_Framework.md) |
| Literature | [Literature map](03_Literature_Map.md), [reading list](literature/Reading_List.md), and [detailed reviews](literature/) |
| SAP case orientation | [SAP knowledge map](05_SAP_Knowledge_Map.md) |
| Research method | [Research protocol](06_Research_Protocol.md), [data-collection protocol](07_Data_Collection_Protocol.md), and [coding manual](08_Coding_Manual.md) |
| Analysis | [Analytical framework](09_Analytical_Framework.md) and [figure and table plan](11_Figure_and_Table_Plan.md) |
| Papers | [Paper pipeline](12_Paper_Pipeline.md) and [paper workspace](paper/) |
| Book | [Research monograph](book/README.md) |
| Course | [Postgraduate course](course/README.md) |
| Applied studies | [Research workstreams](workstreams/README.md) |
| Progress | [Public project status](PUBLIC_PROJECT_STATUS.md) |

## Current stage

The programme has completed its initial research architecture and six of the nine literature streams. The conceptual framework, documentary method, coding structure, and comparative design are established.

The next stage completes the remaining literature streams and begins controlled collection and pilot analysis of official SAP reference artefacts. Findings about customer configurations, organisational practice, and performance will require later implementation and field evidence.
