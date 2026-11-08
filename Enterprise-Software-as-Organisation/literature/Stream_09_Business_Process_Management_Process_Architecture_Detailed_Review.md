# Stream Nine: Business-Process Management and Process Architecture

## Scope and evidence boundary

This review supplies the representational vocabulary needed to analyse end-to-end process artefacts. It distinguishes process from process model, case from event, role from actor, business object from document view, prescribed path from observed trace, and process architecture from one isolated flow.

The evidence base combines verified books, publisher records, complete open articles, and author or institutional manuscripts. Claims based only on abstracts are limited accordingly. The review does not treat business-process management as proof that modelled processes are enacted as designed. A process model is a selective representation produced for a purpose. An event log is also selective because it contains only recorded events at a chosen granularity. Neither is the organisation itself.

## Part I: Learning guide

### 1. The practical problem

SAP reference content often appears process-like: a diagram contains activities and gateways; a test script lists steps, roles, and applications; a document passes through statuses; an event starts or completes a task. These representations are indispensable, but they answer different questions.

A reference process shows an offered arrangement. A configured workflow specifies selected executable logic. A test script gives a normative procedure for demonstrating a scenario. A transaction log records selected system events. A performed business process includes human interpretation, unrecorded communication, waiting, repair, and work outside the system.

Stream Nine provides a disciplined way to move among these artefacts without collapsing them.

### 2. Concepts to master

#### Business process

A business process is an organised collection of activities and events through which an outcome is produced for a customer or organisational purpose. BPM combines management and information-technology perspectives on operational processes (van der Aalst, 2013; Dumas et al., 2018).

The definition should not be reduced to a diagram. A process includes temporal, informational, organisational, and object relations, some of which may not appear in one model.

#### Process model

A process model is a purposeful representation of selected aspects of a process. Curtis, Kellner, and Over (1992) show that process models can serve description, prescription, explanation, communication, and improvement. Van der Aalst (2013) distinguishes uses including analysis, enactment, monitoring, and redesign.

Every model omits detail. Its adequacy depends on its purpose, notation, scope, audience, and level of abstraction.

#### Event and activity

An event records or represents something that happens, such as receipt of an order or posting of goods issue. An activity represents work performed over some interval. An event may trigger an activity, mark its completion, or describe a change of state.

The distinction matters because a recorded event is not the full activity. “Invoice posted” does not reveal all checking, discussion, waiting, correction, or judgement that preceded the posting.

#### Case or process instance

A case is one instance of a process, such as one purchase order or one sales order. Process models usually describe possible behaviour across many cases; event logs record traces for particular cases.

Case identification is analytical work. One end-to-end outcome can span several technical document identifiers, while one document can participate in several processes.

#### Actor, role, and organisational unit

An actor is a person, group, system, or other participant performing or supporting an activity. A role is a defined capacity or responsibility that may be occupied by different actors. An organisational unit locates work within a structural boundary.

A swimlane labelled “Purchaser” represents a role category. It does not establish which person acted, what authority that person held, or whether work was delegated or shared.

#### Business object and state

A business object is an entity about which the process records and changes information, such as a purchase requisition, purchase order, material document, journal entry, or invoice. State represents the object's condition at a particular point.

Object-state transitions provide a useful bridge between process and enterprise-software architecture. They reveal what changes, which action or event changes it, and which later actions become possible.

#### Gateway, variation, and exception

A gateway or decision point represents alternative routing, synchronisation, or branching logic. Variation is an admitted alternative within the process family. An exception is a case that departs from the expected path or requires special handling.

Not every gateway is a human decision. It may evaluate a rule automatically. Not every exception is an error. Some exceptions are designed alternatives, while others arise from mismatch, failure, or unforeseen conditions.

#### Process architecture

Dijkman, Vanderfeesten, and Reijers (2016) describe business-process architecture as a way to organise consistent, integrated collections of process models. Architecture addresses relationships among processes, decomposition, scope, and the organisation of the process landscape.

This matters because P2P, O2C, and R2R are not independent sequences. They share master data, organisational structures, records, controls, and accounting consequences. Process architecture makes these relations visible.

### 3. Reading route

1. Read Curtis, Kellner, and Over (1992) for process-model purposes and perspectives.
2. Read van der Aalst (2013) for the BPM field, process-aware information systems, lifecycle activities, flexibility, and process mining.
3. Read Dumas et al. (2018) for a systematic treatment of identification, discovery, analysis, redesign, automation, monitoring, and BPM capability.
4. Read Mendling, Reijers, and van der Aalst (2010) for model-quality and understandability guidelines.
5. Read Dijkman, Vanderfeesten, and Reijers (2016) for process architecture.
6. Read vom Brocke et al. (2014) for BPM as a contextual, holistic, continuous organisational capability rather than a modelling exercise.
7. Read Fahland and van der Aalst (2015) for the gap between a model and recorded behaviour.

### Study pause: identify the artefact before interpreting it

For each SAP source, ask:

1. Is it a reference model, configured model, test procedure, application page, business-object definition, event trace, or report?
2. Is it descriptive, normative, executable, analytical, or instructional?
3. What is the process boundary and level of abstraction?
4. Which actors, objects, states, events, and exceptions are represented?
5. Which relations are omitted?
6. What evidence would be needed to connect it with actual performance?

## Part II: Readable scholarly synthesis

### 4. BPM joins management and information technology

Van der Aalst (2013) defines BPM as a discipline joining knowledge from management sciences and information technology around operational business processes. This dual character is important. BPM is not only workflow automation, and it is not only managerial process improvement.

His survey organises BPM around modelling, enactment, analysis, and management. Process models can configure systems, support understanding, enable simulation, guide execution, and provide a basis for monitoring. Process-aware information systems include workflow and BPM systems as well as ERP, CRM, case handling, rule systems, and other applications that support processes without relying on one generic workflow engine.

This account fits the SAP corpus. Process behaviour can be distributed across applications, business objects, workflow definitions, scheduled jobs, authorisations, validations, and accounting logic. A visible diagram is therefore an entry point rather than a complete specification.

### 5. A process model is purposeful and selective

Curtis, Kellner, and Over (1992) review process modelling through several purposes and perspectives. Models may support communication, analysis, planning, improvement, training, or enactment. Different purposes require different elements and levels of precision.

The implication is methodological. A model should not be criticised merely because it omits something that its purpose did not require. Equally, it should not be used to support claims outside that purpose. A high-level reference diagram may be appropriate for orientation but inadequate for analysing exception logic or authority.

The SAP study therefore triangulates artefacts. Process Navigator establishes a reference boundary and broad sequence. Test scripts add steps, roles, applications, data, and variations. Product documentation adds configuration, workflow, object, and authorisation detail. No one artefact stands for the whole architecture.

### 6. Process modelling quality concerns comprehension as well as correctness

Mendling, Reijers, and van der Aalst (2010) develop seven process-modelling guidelines from empirical work on structural properties, error probability, and understanding. Their intervention responds to the practical problem that process models are often created by occasional modellers and can become unnecessarily complex or error prone.

Model quality has several dimensions. Syntactic correctness asks whether a model follows the notation. Semantic quality asks whether it adequately represents the intended domain. Pragmatic quality concerns whether relevant readers can understand it. A formally valid model may still obscure roles, exceptions, or dependencies.

For documentary analysis, visual complexity should not be mistaken for organisational complexity. Conversely, a simple diagram may conceal extensive configuration and exception handling. The analysis should reconstruct relations across sources rather than count diagram elements alone.

### 7. Process architecture connects models into a landscape

Dijkman, Vanderfeesten, and Reijers (2016) respond to the proliferation of process models in organisations. Process architecture provides principles for organising consistent and integrated collections, including decomposition and relationship among processes.

This changes the unit of analysis. An end-to-end process has upstream prerequisites, downstream consequences, shared services, management processes, and master-data dependencies. Goods receipt belongs to procurement and inventory management while creating information relevant to invoice verification and accounting. Billing belongs to sales while creating a receivable and financial posting.

The organisation-design question therefore concerns both the internal coherence of each process and the coherence of relations across the process architecture.

### 8. BPM is a continuous organisational capability

Vom Brocke et al. (2014) propose ten principles of good BPM, including context awareness, continuity, enablement, holism, institutionalisation, involvement, joint understanding, purpose, simplicity, and technology appropriation. The framework rejects a one-off modelling project as an adequate account of BPM.

This is an important boundary for reference-content research. SAP architecture can reveal a process design and sanctioned variation mechanisms. It cannot establish whether an organisation has the capabilities to govern, monitor, improve, and sustain the process over time.

### 9. Executable models and actual work remain distinct

An executable workflow can constrain which system transitions occur and in what order. It may therefore be more consequential than a descriptive diagram. Yet execution still does not capture the complete process. Human preparation, interpretation, waiting, communication, and work outside the system may remain invisible.

Van der Aalst (2013) distinguishes modelling, enactment, logging, monitoring, analysis, and adaptation. This helps place enterprise artefacts at the right level. A reference model is not an executable model. An executable model is not a trace. A trace is not a complete performance.

### 10. Event logs provide evidence, not transparent reality

Process mining connects models with recorded events. Discovery creates models from logs; conformance checking compares models and logs; enhancement adds information or improves a model using recorded behaviour.

Fahland and van der Aalst (2015) address model repair by aligning a process model with an event log. Their work demonstrates that observed and modelled behaviour can diverge and that the model can be adjusted to replay recorded traces while remaining close to its original structure.

The analytical warning is equally important. Event logs record what the information system has been designed to record. They can omit manual work, conversation, interpretation, failed attempts, and activity in other systems. Even conformance analysis compares two representations: a model and a log. Later research should therefore combine event evidence with interviews, observation, configuration records, and organisational context.

### 11. Variation and exception are central, not peripheral

Happy-path diagrams are attractive because they provide a clear sequence. Organisational work becomes most revealing where the path branches, fails, reverses, or requires judgement. Credit blocks, approval rework, goods-receipt reversal, invoice reduction, journal rejection, clearing reset, and period restrictions reveal control, authority, information, and coordination relations that a normal path can hide.

A rigorous process review should therefore sample at least five kinds of segment: normal progression, approval or authority, exception or reversal, information or monitoring, and configuration or extensibility. The current SAP collection protocol adopts this variety requirement.

## Part III: Complete technical expansion

### 12. Artefact taxonomy

| Artefact | Primary contribution | Main limitation |
|---|---|---|
| Reference process | Offered scope, broad sequence, roles and variants | Not customer configuration or performance |
| Test script | Normative steps, data, roles, applications and expected results | Demonstration procedure, not routine work |
| Configured workflow | Selected executable routing and conditions | Does not show all surrounding work or actual use |
| Business-object documentation | States, fields, relations and operations | May not show process purpose or organisational meaning |
| Authorisation documentation | Formal access structure and restrictions | Does not show accepted or real authority |
| Event log | Recorded events, order, timing and actor or object identifiers where captured | Selective technical trace, not full practice |
| Process model discovered from logs | Pattern fitted to recorded traces | Depends on log quality, case construction and algorithm |
| Interview or observation | Meaning, judgement, workarounds and situated practice | Requires triangulation for recurrence and system state |

### 13. Minimum process-segment record

Each coded segment should state:

1. process and release boundary;
2. source artefact and exact location;
3. event or trigger;
4. activity or operation;
5. actor or role;
6. business object and state transition;
7. organisational unit or restriction;
8. predecessor and successor dependency;
9. rule, gateway, threshold, or condition;
10. information produced, consumed, or made visible;
11. normal, optional, exception, reversal, monitoring, or configuration status; and
12. inference limit.

### 14. Process boundary questions

An end-to-end label should never substitute for a boundary decision. Record:

- starting event and terminating outcome;
- customer or organisational purpose;
- included and excluded subprocesses;
- prerequisite and successor processes;
- cross-process objects and postings;
- country, release, and edition;
- normal and exceptional completion states; and
- whether the process is reference, configured, executed, or observed.

### 15. Cross-stream boundaries

**Organisation design:** BPM identifies activities, roles, objects, and handoffs. Organisation design explains how these form a wider division and integration of work.

**Coordination:** A sequence displays dependencies. Coordination theory explains the mechanism used to manage them.

**Decision theory:** Gateways and rules can represent decision premises, but they do not show the complete judgement process.

**Enterprise systems:** BPM shows how application capabilities enter process arrangements. Implementation research explains selection, configuration, adaptation, and transformation.

**Routines:** A process model is an artefact related to a routine, not the routine's complete ostensive or performative aspect.

**Materiality:** Executable logic can participate materially in work, but actualisation and consequence require practice evidence.

**Infrastructure:** Processes depend on standards, classifications, master data, and interfaces that can extend beyond the diagram.

**Governance:** Approval and monitoring steps expose candidate governance relations, but legitimacy and accountability require additional evidence.

### 16. Prohibited inferences

- A process diagram is not the process itself.
- A reference process is not a customer implementation.
- A test script is not evidence of routine performance.
- A swimlane label is not proof of actual role occupancy or authority.
- A gateway is not necessarily a human decision.
- An event is not the complete activity that produced it.
- A status change is not the complete organisational judgement.
- A log is not transparent reality.
- A discovered model is not a complete process.
- A happy path is not the full organisational architecture.
- Conformance to a model is not automatically effective or legitimate performance.
- Deviation is not automatically error, resistance, or failure.

### 17. Strongest defensible contribution

Stream Nine makes the SAP empirical corpus analysable at the right level. It provides a vocabulary for identifying events, activities, roles, objects, states, boundaries, handoffs, variants, exceptions, and process relationships. It also prevents those representations from being mistaken for implemented or performed work.

The documentary study can reconstruct a release-controlled reference-process architecture by triangulating diagrams, test scripts, roles, applications, object documentation, workflow, authorisation, configuration, and exception sources. Claims about actual process frequency, conformance, judgement, workaround, effectiveness, or outcome must wait for implementation and enactment evidence.

## Part IV: Audit conclusion

The verified literature supports six conclusions.

1. BPM combines managerial and technical perspectives and is broader than workflow automation.
2. Process models are purposeful, selective representations whose adequacy depends on use.
3. Process architecture connects individual models into an integrated landscape.
4. Executable models, event logs, and performed work are distinct empirical objects.
5. Variation, exception, reversal, and repair are essential to organisational analysis.
6. SAP reference artefacts can support a rigorous reconstruction of encoded process architecture, but not claims about actual performance without additional evidence.
