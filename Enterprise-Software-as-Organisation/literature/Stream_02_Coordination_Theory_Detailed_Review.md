# Stream Two: Coordination Theory, Detailed Literature Review

## How to use this review

This review has three layers. The **learning guide** introduces the problem and vocabulary. The **readable scholarly synthesis** develops the argument while explaining how the authors connect. The **complete technical expansion** preserves the full source-rich analysis, qualifications, propositions, and coding implications.

The stream asks one practical question:

> When work is interdependent, what must be coordinated, how is that coordination attempted, and what conditions make it possible?

Enterprise software matters because it can represent dependencies and proposed ways of managing them. It cannot, by its presence alone, prove that people coordinate successfully.

## Learning guide

### 1. Begin with the dependency

Coordination theory starts neither with teamwork nor with software features. It starts with a dependency. One activity may require the output of another, several activities may compete for the same resource, or different actors may need to use compatible representations of the same object.

Malone and Crowston define coordination as managing dependencies among activities. This gives the analysis a disciplined sequence:

1. Identify the activities and actors.
2. Identify the dependency connecting them.
3. Identify the mechanism proposed to manage it.
4. Ask what human, informational, and relational conditions that mechanism requires.
5. Separate the designed arrangement from what happens in practice.

### 2. Common dependency types

| Dependency | Plain-language meaning | Possible encoded response |
|---|---|---|
| Flow | One activity needs an output from another | Sequence, status, hand-off, notification |
| Shared resource | Activities need the same scarce resource | Allocation rule, schedule, queue, priority |
| Fit | Separate contributions must be mutually compatible | Common model, validation, reconciliation |
| Task assignment | Work must reach an appropriate actor | Role, responsibility, routing rule |
| Producer-consumer | A producer must supply what a consumer needs | Specification, acceptance criterion, feedback |

The table is a starting vocabulary, not a claim that every dependency is fully visible in documentation.

### 3. A mechanism is not an outcome

A workflow, meeting, shared record, plan, rule, or role is a coordination mechanism. Accountability, predictability, and common understanding are coordination conditions that such mechanisms may help produce. Successful performance is an outcome. These categories should not be collapsed.

For example, a shared record may make an order visible. Visibility may support accountability and predictability. Yet actors may interpret the record differently, distrust it, lack permission to correct it, or coordinate through an unofficial channel. The artefact exists, but its practical effect remains an empirical question.

### 4. Shared data are not automatically shared meaning

Carlile shows that knowledge boundaries differ in difficulty. At a simple boundary, information can be transferred. At a more difficult boundary, groups may use different meanings and must translate. At a pragmatic boundary, interests conflict and existing knowledge may need to be transformed.

This distinction is especially important for enterprise software. A common object or field can standardise representation, but semantic agreement cannot be inferred from technical integration. Cross-functional coordination may require explanation, negotiation, and change to the representation itself.

### 5. Coordination also depends on relationships and expertise

Gittell demonstrates that coordination may depend on shared goals, shared knowledge, mutual respect, and timely problem-solving communication. Faraj and Sproull show that knowing where expertise resides is insufficient unless expertise can be brought into the work. Faraj and Xiao add that fast-moving, safety-critical work requires protocols alongside situated expertise and adjustment.

The lesson is not that formal mechanisms are unimportant. It is that their effectiveness may depend on conditions that architecture cannot guarantee.

### 6. Coordination is continually accomplished

Practice research shows that coordination is not installed once and then completed. People repair breakdowns, align interpretations, renegotiate responsibilities, and adapt routines. Plans, schedules, boundary objects, and digital records participate in this work, but people still have to use and sometimes modify them.

This gives the project a careful formulation: enterprise software is a **codified coordination proposal**. It represents how dependencies are expected to be managed. Evidence of enacted coordination requires observation, interviews, logs, or comparable implementation evidence.

### 7. A practical reading route

When reading a process diagram, configuration guide, role definition, or system description, ask:

1. What activities are connected?
2. What passes between them: material, information, authority, money, or expertise?
3. What kind of dependency is present?
4. What mechanism is encoded?
5. What should become accountable, predictable, or mutually understood?
6. What assumptions are made about interpretation, trust, expertise, and willingness to cooperate?
7. What evidence would be needed to show that the arrangement works in practice?

### 8. Claim labels used throughout the project

- **Established claim:** Supported directly by identified scholarship.
- **Project interpretation:** A reasoned application of theory to the research problem.
- **Illustrative example:** Helps explain a concept but is not an empirical finding.
- **Proposition:** A claim to examine through data.
- **Evidence boundary:** States what available material cannot establish.
- **Verification required:** A citation, edition, or access issue still needs resolution.

## Readable scholarly synthesis

### 1. Coordination theory changes what we look for

Coordination is often described loosely as collaboration. Malone and Crowston provide a sharper starting point: coordination is the management of dependencies among activities. The practical benefit is that analysis can move from a vague question, such as whether a system improves collaboration, to a traceable one: what dependency is present, and what arrangement is intended to manage it?

Crowston develops this approach by treating coordination processes as bundles of mechanisms that can sometimes be compared across settings. For this project, that makes software artefacts analytically useful. Sequences, assignments, shared objects, queues, validation rules, and exception paths can be read as candidate mechanisms. The word candidate is essential because documentation presents a design, not proof of its use or success.

**Section takeaway:** Start with the dependency, then interpret the feature.

### 2. Different dependencies require different responses

Thompson distinguishes pooled, sequential, and reciprocal interdependence. Malone and Crowston offer a complementary mechanism-oriented vocabulary that includes flows, shared resources, fit, task assignment, and producer-consumer relations. Together, these ideas prevent an overly simple reading of integration.

A sequential dependency may be managed through a hand-off and status control. A shared-resource dependency may require allocation and priority rules. A reciprocal dependency may require repeated adjustment and richer communication. A fit dependency may require common standards plus reconciliation. No single mechanism is universally appropriate.

**Illustrative example:** A required goods receipt before invoice verification can be read as an encoded sequence. An invoice block and resolution route can be read as an exception mechanism. Neither feature proves that users experience the process as coordinated.

**Section takeaway:** Coordination design should be matched to the dependency it addresses.

### 3. Mechanisms work through coordination conditions

Okhuysen and Bechky connect a diverse literature by distinguishing mechanisms from three integrating conditions: accountability, predictability, and common understanding. Roles and responsibilities may support accountability. Plans, schedules, and routines may support predictability. Shared representations and interaction may support common understanding.

This distinction improves the coding framework. A document may show that a role receives a task, but analysis should ask what condition the assignment is intended to create. It may clarify responsibility, make progress visible, or establish who must respond to an exception. It may fail if responsibilities are disputed or the assigned actor lacks the necessary information or authority.

**Section takeaway:** Code both the device and the condition it is meant to support.

### 4. Representation helps, but meaning may still diverge

Carlile explains why common information is sometimes insufficient. At syntactic boundaries, actors mainly need a common format. At semantic boundaries, they need translation because terms and objects carry different meanings. At pragmatic boundaries, knowledge is tied to different interests, so coordination may require negotiation and transformation.

Bechky similarly shows that occupational groups develop distinct understandings of work. Boundary objects can help groups collaborate without complete agreement, but their usefulness depends on how they are interpreted and used. A master record or process object may therefore create a common reference while leaving disagreement about meaning, ownership, or acceptable action unresolved.

**Evidence boundary:** Technical consistency does not establish semantic agreement.

### 5. Formal architecture and situated adjustment coexist

Schmidt and Simone emphasise coordination mechanisms embedded in cooperative work. Faraj and Sproull focus on the coordination of expertise, while Faraj and Xiao show how protocols and situated action coexist in time-critical work. Jarzabkowski, Lê, and Feldman describe coordination as an ongoing accomplishment that responds to disruption and ambiguity.

These studies make it difficult to portray coordination as a finished property of system design. Formal arrangements can stabilise expectations and make work inspectable. Situated adjustment handles cases that were not fully anticipated, translates across expertise, and repairs failures. A strong account therefore studies how encoded arrangements invite, constrain, or redirect such adjustment.

**Section takeaway:** Standardisation and adjustment are not simple opposites. Organisations often need both.

### 6. What ERP research adds

ERP research illustrates how integration can produce both coordination capacity and new dependencies. Shared data and process logic can connect functions, while standard categories may create interpretive tensions or require local adaptation. Requirements and implementation studies also show that coordination problems are not exhausted by technical interfaces. Stakeholders must align terminology, responsibilities, and expectations.

The ERP-specific studies in the technical expansion are treated as contingent evidence, not universal laws. Their value is to demonstrate plausible mechanisms and tensions that can guide documentary coding and later empirical inquiry.

### 7. The contribution to this project

This stream supplies a disciplined bridge from software architecture to organisation theory. It permits analysis of enterprise software as an inspectable arrangement of dependencies, sequences, assignments, representations, gates, visibility, and exceptions.

The resulting claim is useful but bounded. The project can reconstruct a **codified coordination proposal**. It cannot infer mutual understanding, accepted responsibility, effective expertise use, or successful performance from architecture alone. Those are questions for implementation and practice evidence.

## Complete technical expansion

The following sections preserve the full scholarly review, its source qualifications, coding implications, and propositions. Each section begins with the coordination problem at issue, then connects the sources to the project and states the limit of the available evidence.

## Purpose and evidential boundary

This stream asks how enterprise software can be analysed as an arrangement for coordinating interdependent work. It does **not** assume that a workflow, data object, role, or alert produces coordination in practice. The defensible claim from reference artefacts is narrower: software can encode candidate dependencies, coordination mechanisms, visibility conditions, and escalation paths. Whether actors understand, accept, repair, or circumvent those arrangements requires implementation or practice evidence.

The review was rebuilt from the LeapSpace report rather than copied from it. The report is a useful discovery aid, but its citations include the uploaded prompt itself, two unresolved Scopus links, peripheral engineering studies, and recent papers that cannot anchor the theoretical lineage. Claims below therefore rest on independently checked publications. The accompanying [source assessment](Stream_02_Source_Assessment.md) records the access level for every source used.

## 1. What coordination theory explains

The first task is to identify what requires coordination. Malone and Crowston (1994) define coordination as managing dependencies among activities. The definition directs attention away from generic references to collaboration or communication and toward a three-part question:

1. What activities or actors depend on one another?
2. What kind of dependency connects them?
3. What mechanism manages that dependency?

This is especially productive for enterprise software because process models display ordered activity, shared resources, information transfers, and assignment structures. The definition is deliberately broad, however. If every technical link is coded as coordination, the concept loses discrimination. A documented relation must therefore identify both an organisational dependency and an encoded response to it.

This dependency-centred view complements classical organisation design. Thompson (1967) distinguishes pooled, sequential, and reciprocal interdependence. Mintzberg (1979) identifies mutual adjustment, direct supervision, and standardisation of work processes, outputs, and skills as broad coordinating mechanisms.

These are not competing taxonomies. Thompson characterises the pattern of interdependence. Mintzberg describes broad organisational means of coordination. Malone and Crowston add a finer mechanism-oriented question: which particular dependency is being managed, and how?

## 2. From dependencies to mechanisms

Useful dependency families for documentary coding are:

| Dependency family | Diagnostic question | Possible documentary trace | What the trace cannot establish |
|---|---|---|---|
| Flow or prerequisite | Must one activity or state precede another? | workflow sequence, status transition, prerequisite check | that the sequence is followed in practice |
| Fit or synchronisation | Must outputs, timing, or conditions align? | matching rule, scheduling field, reconciliation step | successful mutual adjustment |
| Shared resource | Do activities compete for or draw on the same resource? | allocation object, availability check, reservation | fair or effective allocation |
| Producer–consumer | Does one activity create information or material another requires? | document flow, hand-off, event/message | receipt, interpretation, or use |
| Task assignment | Who is expected or authorised to act? | role, worklist, responsibility rule | accepted responsibility or actual authority |
| Knowledge/expertise | Is specialised knowledge needed across a boundary? | expert role, collaboration object, exception routing | knowledge integration or shared understanding |

The table is a coding bridge, not a claim that these categories exhaust coordination. It keeps the analysis close to observable artefacts while allowing later comparison with organisational theory.

Identifying a mechanism is still not the same as demonstrating successful coordination. Okhuysen and Bechky (2009) organise coordination mechanisms into plans and rules, objects and representations, roles, routines, and proximity. Their principal advance is to separate these mechanisms from the integrative conditions they may help create: **accountability**, **predictability**, and **common understanding**.

This distinction prevents a common error in software research. A role field is evidence of encoded assignment, not accountability by itself. A workflow sequence may support predictability, but it does not prove that participants can anticipate one another. A shared record makes a representation available, but it does not prove common understanding.

For this project the three conditions should therefore be treated as propositions to test, not direct software observations:

| Integrative condition | Minimum evidence in software artefacts | Stronger evidence required beyond architecture |
|---|---|---|
| Accountability | visible assignment, ownership, status, or traceability | answerability, consequences, accepted responsibility |
| Predictability | explicit sequence, timing, trigger, or stable interface | actors’ reliable expectations and coordinated timing |
| Common understanding | shared representation, vocabulary, or context field | demonstrated aligned interpretation across groups |

## 3. Coordination is relational and epistemic

The dependency-mechanism approach explains how work is connected, but it does not by itself explain how people interpret what they exchange. **Epistemic coordination** concerns the knowledge, meanings, and expertise that actors must bring together in order to coordinate.

Formal mechanisms leave an important question unresolved: what social relations allow people to use them effectively? Gittell (2002) addresses this question through **relational coordination**. This form of coordination rests on mutually reinforcing communication and relationship dimensions, particularly where work is highly interdependent and uncertain.

The lesson for enterprise-software analysis is not that software contains relational coordination. It is that encoded work routing and shared information may interact with relationships that cannot be inferred from design documentation.

Faraj and Xiao (2006) then show why expertise and dialogue matter under uncertainty. In fast-response organisations, formal protocols coexist with expertise coordination and knowledge-rich communication. For this project, exception handling and escalation are therefore theoretically important. They may mark the point at which pre-specified coordination is judged insufficient.

An exception path still represents only a designed possibility. Whether it actually mobilises situated expertise remains an empirical question.

Bechky (2003) explains how occupational communities with different languages, locations of practice, and conceptions of a product can overcome misunderstandings by creating common ground. Objects can participate in that process, but access to the same object is not equivalent to shared understanding.

Carlile (2002, 2004) makes the problem more precise by distinguishing three increasingly demanding operations across knowledge boundaries. **Transfer** moves knowledge where differences are sufficiently understood. **Translation** develops a way to interpret different meanings. **Transformation** changes existing knowledge when novelty or conflicting interests prevent simple transfer or translation.

**Illustrative example:** A stable master-data object may support transfer. A semantic mapping may support translation. Contested definitions or interests may require transformation that a standard data model cannot settle.

These studies sharpen a crucial boundary: **shared data are not shared meaning**. Enterprise software may standardise categories and make work mutually visible while leaving interpretation, professional interests, and local knowledge unresolved.

## 4. Artefacts and representations as active coordination arrangements

The preceding literature establishes that objects can do more than store information. Coordination artefacts deserve their own analytical category because they can represent work, make dependencies visible, orient attention, preserve state, and provide a focal point for negotiation.

Zaitsev, Gal, and Tan (2020) analyse coordination artefacts in agile software development. Their study is valuable because it shows that an artefact's coordination role depends on use and changing project conditions, not simply on its technical presence.

For ERP reference architecture, candidate coordination artefacts include business objects, status records, approval histories, worklists, schedules, exception queues, process diagrams, analytical views, and notifications. Their possible functions should be coded separately:

- **representing** the current or intended state of work;
- **routing** an item or message between actors;
- **gating** an action until a condition is satisfied;
- **synchronising** activities, timing, or versions;
- **allocating** responsibility or a scarce resource;
- **alerting** an actor to deviation or required action;
- **recording** action for traceability or later review.

An artefact may perform several functions, and the same function may be realised by several artefacts. Coding should not infer the function from the artefact’s name; it should record the documented operation and its dependency target.

## 5. Coordinating as an accomplishment, not a finished structure

The next problem is temporal: coordination arrangements are not simply designed and then permanently achieved. Jarzabkowski, Lê, and Feldman (2012) study coordinating as an activity that is continually created and modified. Their process model follows cycles in which actors encounter disruption, notice what is missing, create new elements, form new patterns, and stabilise those patterns. Actors move between an abstract coordination mechanism and its performance.

This is a direct warning against equating a reference process with accomplished coordination.

Kellogg, Orlikowski, and Yates (2006) show how a **trading zone** can support cross-boundary coordination. A trading zone is a working space in which communities with different expertise and interests develop sufficient means of interaction without becoming identical. Temporal, technical, and political practices structure that interaction.

Together, these practice studies suggest that software-native mechanisms become consequential through situated performance. Gaps, breakdowns, negotiation, and repair can be constitutive parts of coordination rather than mere anomalies.

The project must therefore keep three levels separate:

1. **Encoded coordination:** dependencies and mechanisms documented in vendor artefacts.
2. **Implemented coordination:** configured organisational arrangements in an adopting organisation.
3. **Enacted coordinating:** situated accomplishment, adjustment, breakdown, repair, and workaround.

Paper 1 can make claims at the first level. It may formulate questions about the other two, but cannot answer them without different evidence.

## 6. What enterprise software can plausibly encode

Bringing the streams together yields five analytically distinct families:

| Encoded family | Organisational question | Typical evidence |
|---|---|---|
| Workflow and temporal ordering | In what order, under what conditions, and at what time should work proceed? | sequence, trigger, deadline, status transition |
| Responsibility and authority | Who may, must, or should act or decide? | business role, authorisation, approval rule, work assignment |
| Shared representations | What object or classification makes work visible across activities? | master/transaction data, document flow, semantic definition |
| Exception and repair routing | What happens when the normal path is inadequate or violated? | tolerance, block, alert, exception queue, escalation |
| Monitoring and traceability | How is progress, deviation, or prior action rendered observable? | status, log, KPI, audit trail, analytical view |

These are candidate mechanisms, not outcomes. “Approval required” is an encoded gate and allocation of decision opportunity; it does not prove substantive review. “Single source of truth” is vendor language unless consistency and interpretation are empirically demonstrated. An alert is a notification mechanism, not evidence that anyone noticed or acted.

### ERP-specific evidence and its limits

The ERP literature provides a bridge from general coordination theory to the empirical setting. It does not remove the project's inferential boundary.

Alsène (2007) studied sixteen work situations in four units of one Canadian mail and parcel organisation using SAP R/3. The accessible abstract reports that ERP contributions to coordination were diverse, variable in intensity, and not systematic. This supports a contingent question about when software participates in coordination. It does not support the general claim that ERP coordinates an enterprise. Only abstract-level access was available for this review.

Gosain, Lee, and Kim (2005) studied cross-functional coordination during four ERP implementations. Their abstract identifies three patterns for managing functional interdependencies: a planned, reference-model-oriented lean pattern; a richer pattern combining organising arrangements and cultural interventions; and a mediation pattern based on executive mandate or functional dominance. Because the object is ERP implementation rather than reference architecture itself, the study shows that technically similar projects may be accompanied by different organisational coordination patterns. It is not direct evidence about the organisational content encoded in SAP artefacts.

Daneva and Wieringa (2006) apply coordination theory to cross-organisational ERP requirements. Their framework is especially relevant because it makes built-in coordination and cooperation assumptions an explicit requirements problem and links those assumptions to a library of ERP-supported mechanisms. An institutional repository provides a full-text route. The paper concerns requirements alignment and inter-organisational settings, so its categories can inform the coding framework without being treated as validated findings for intra-organisational SAP reference processes.

Kelle and Akbulut (2005) examine ERP tools in supply-chain information sharing, cooperation, and cost optimisation. The publisher abstract states that ERP can support integration while also obstructing cooperation with business partners. This is a useful counterweight to one-directional integration claims. Its supply-chain and inventory focus, together with abstract-only access in this review, makes it an adjacent source rather than a foundation for the general framework.

Taken together, these studies support three bounded conclusions:

1. ERP systems can participate in dependency management.
2. Their contribution varies by work situation and surrounding organisational arrangements.
3. Integrated information and reference processes can introduce both coordination possibilities and constraints.

None establishes that a documented SAP S/4HANA feature produces coordination in an adopting organisation.

## 7. Governance, authority, and the limit of coordination theory

Coordination theory brings the analysis close to governance, but the two should not be collapsed. The LeapSpace report usefully points toward governance and decision rights, although it overstates their absence from coordination research. Coordination theory frequently addresses roles, accountability, allocation, and arrangements adjacent to control.

The more precise question for this project is how software structures distribute **decision opportunities, visibility, vetoes, obligations, and escalation rights**.

Coordination and governance overlap but are not synonymous. Coordination asks how interdependent activity is integrated. Governance asks who has the legitimate capacity to decide, set rules, allocate resources, and hold others to account. A workflow approval may do both, but the coding rationale must say which aspect is observed. Formal authorisation also cannot establish actual authority, discretion, or political acceptance.

## 8. Implications for the codebook

Each coordination observation should record:

1. the activities or actors connected;
2. the dependency type;
3. the encoded mechanism and exact operation;
4. the artefact or representation involved;
5. the assigned role or decision point, if any;
6. the information made visible or withheld;
7. the normal-path or exception-path status;
8. the proposed integrative condition, explicitly labelled as an interpretation;
9. a rival interpretation; and
10. the evidence location and confidence.

A claim should be rejected or narrowed when the artefact shows only co-presence, technical integration without an organisational dependency, a role label without documented action, or a purported outcome without implementation evidence.

## 9. Propositions for empirical analysis

The literature supports questions and bounded propositions, not findings:

- Where sequential dependencies are explicit, reference architectures are likely to encode more routing, gating, and status transitions than where interdependence is pooled.
- Reciprocal or knowledge-intensive dependencies may be less completely specifiable and may appear through exception, collaboration, or escalation facilities.
- Shared representations may increase visibility and transfer while leaving semantic differences and interests unresolved.
- Encoded accountability is more defensible where assignment, progress visibility, and traceability occur together than where only a role name is present.
- Exception structures may reveal the assumed boundary between standardised coordination and situated judgement.
- Cross-process variation in mechanisms should be explained by documented dependencies, not attributed automatically to “best practice.”

Each proposition must be tested against negative cases and rival explanations such as compliance, record keeping, technical integrity, or product convenience.

## 10. Synthesis and contribution

Coordination theory contributes the project’s central analytical move: reconstruct dependencies and the mechanisms intended to manage them. Organisation design supplies broad patterns of interdependence and coordination; the mechanism literature distinguishes devices from accountability, predictability, and common understanding; relational and knowledge-boundary research identifies what architecture alone cannot secure; practice research explains why coordination is continuously accomplished rather than installed.

The resulting contribution is intentionally bounded. Enterprise software can be studied as a **codified coordination proposal**: an inspectable arrangement of sequences, assignments, representations, gates, exceptions, and visibility. It is not the organisation itself, and its presence does not demonstrate coordinated performance. This boundary is what makes the documentary analysis both useful and credible.

## References used in this stream

Bechky (2003); Carlile (2002, 2004); Crowston (1997); Faraj and Sproull (2000); Faraj and Xiao (2006); Gittell (2002); Jarzabkowski, Lê, and Feldman (2012); Kellogg, Orlikowski, and Yates (2006); Malone and Crowston (1994); Mintzberg (1979); Okhuysen and Bechky (2009); Schmidt and Simone (1996); Thompson (1967); Zaitsev, Gal, and Tan (2020). Full records are maintained in `../references/references.bib`.

## Glossary for teaching and review

| Term | Working meaning in this project |
|---|---|
| Dependency | A relation in which an activity, actor, or output relies on another |
| Coordination mechanism | An arrangement intended to manage a dependency |
| Accountability | Clarity about responsibility, contribution, and progress |
| Predictability | The ability to anticipate tasks, timing, or others' actions |
| Common understanding | Sufficient shared interpretation to coordinate action |
| Boundary object | A representation that different groups can use despite differing perspectives |
| Knowledge boundary | A point at which differences in knowledge or interests complicate coordination |
| Relational coordination | Coordination supported by shared goals, shared knowledge, mutual respect, and communication |
| Expertise coordination | Recognising where expertise resides and bringing it into the work when needed |
| Situated adjustment | Context-sensitive adaptation during the performance of work |
| Codified coordination proposal | The project's term for the coordination arrangement represented in architecture or documentation |
