# Stream One: Organisation Design, Detailed Literature Review

## How to use this review

This document has three layers. The **learning guide** introduces the problem and theorists in plain language. The **readable scholarly synthesis** develops the connected argument with explicit transitions and boundaries. The **complete technical expansion** preserves the full source-rich discussion, qualifications, and implications for research and citation work.

The central question is simple:

> When many people and units contribute to the same organisational purpose, how should their work be divided and then brought back together?

Organisation design studies the arrangements used to answer that question. For this project, the additional question is whether some of those arrangements are represented in enterprise software.

## Learning guide

### 1. The problem before the theory

Every organisation must divide work. Procurement, receiving, accounting, sales, delivery, and reporting involve different tasks, expertise, and responsibilities. Division creates specialisation, but it also creates dependencies. Once work has been separated, the organisation needs ways to reconnect it.

Organisation design therefore concerns two linked problems:

1. **Differentiation:** How should work be divided into tasks, roles, and units?
2. **Integration:** How should those differentiated parts exchange information, coordinate activity, and make collective decisions?

Enterprise software is relevant because it can represent both sides. It can distinguish roles, activities, organisational units, and business objects. It can also connect them through workflows, shared information, rules, approvals, and access rights.

**Important boundary:** A software representation is not the organisation itself. It shows an encoded proposal or possibility. Customer configuration and everyday practice may differ.

### 2. How the foundational theorists connect

| Theorist | Main question | Plain-language contribution | Use in this research |
|---|---|---|---|
| Thompson | How are activities dependent on one another? | Dependencies can be pooled, sequential, or reciprocal | Identify what kind of coordination problem a process contains |
| Galbraith | How much information must the organisation process? | Greater uncertainty and interdependence create greater information requirements | Examine whether architecture supplies information capacity or reduces information need |
| Mintzberg | How is differentiated work coordinated? | Organisations use supervision, mutual adjustment, and different forms of standardisation | Classify the broad coordination logic represented in an artefact |
| Burton and Obel | How do design elements fit together? | Structure, coordination, information, decisions, incentives, and context form a configuration | Analyse relations among software elements rather than isolated features |
| Puranam, Alexy, and Reitzig | What fundamental problems must every organisation solve? | New organisational forms often recombine familiar solutions to division, allocation, reward, and information problems | Avoid claiming that digital representation automatically creates a new organisational form |

The sequence matters. Thompson helps identify the dependency. Mintzberg helps classify the broad response. Galbraith asks whether the organisation has enough information-processing capacity. Later configurational research asks whether these elements work coherently together.

### 3. Three forms of interdependence

**Pooled interdependence** exists when activities contribute to a shared whole but do not pass work directly between one another. Separate business units may use the same financial structure or master data. Coordination may rely on common standards, shared resources, or common reporting.

**Sequential interdependence** exists when the output of one activity becomes an input to another. A goods receipt may provide information required for invoice verification. Coordination may rely on schedules, workflows, hand-offs, and standard processes.

**Reciprocal interdependence** exists when activities repeatedly exchange inputs and adjust to one another. Resolving an exception may require several functions to revise information or action iteratively. Coordination may require mutual adjustment, richer communication, and access to expertise.

**Illustrative SAP hypothesis, not a finding:** If documentation states that invoice verification depends on a goods receipt, it may support coding a sequential dependency. It does not prove that the hand-off works smoothly or that no workaround exists.

### 4. Information processing in plain language

Galbraith treats organisation design as a response to uncertainty. When tasks are predictable, rules and plans may be sufficient. When uncertainty increases, the organisation must either reduce the amount of information that needs to be processed or increase its capacity to process information.

Enterprise software may increase encoded capacity through shared records, status visibility, analytical views, exception alerts, or lateral access to information. It may reduce information need through standardisation, predefined categories, or self-contained process responsibility.

**Boundary:** More data do not automatically mean better understanding or better decisions. Information must be visible to the right actors, interpretable, timely, and connected to a capacity to act.

### 5. Why configuration matters more than isolated features

A workflow cannot be interpreted on its own. Its organisational significance depends on associated roles, thresholds, information visibility, exception rights, and structural restrictions. Later organisation-design research therefore treats design as a configuration of interdependent elements.

This produces three meanings of fit:

- **Architectural coherence:** Do the encoded elements make sense together?
- **Implementation fit:** Does the selected configuration suit a particular organisation?
- **Enacted fit:** Do actual practices meet coordination and information needs?

This documentary study can examine architectural coherence directly. Implementation and enacted fit require evidence from customer organisations.

### 6. Modularity without the slogan

Modularity means dividing a complex system into parts with limited interaction across their boundaries. It is not always superior. Dividing too little can make the system difficult to understand and change. Dividing too much can create instability and excessive integration work.

Technical and organisational modularity must also be separated. Two software components may be technically distinct while the people using them remain highly interdependent. A software module counts as an organisationally meaningful construct only when it divides, allocates, coordinates, informs, authorises, or controls work.

### 7. Formal mechanisms and lived coordination

A workflow, role, schedule, plan, or shared object may support coordination. Okhuysen and Bechky help distinguish such mechanisms from three possible conditions:

- **Accountability:** People can identify responsibilities and progress.
- **Predictability:** People can anticipate how interdependent work will proceed.
- **Common understanding:** People share enough interpretation to work together.

The mechanism does not prove the condition. A shared status field may provide a basis for visibility without producing common understanding. Relational and practice research further shows that expertise, trust, contestation, joint sensemaking, and informal adjustment remain important, especially during novelty and exception.

### 8. The analytical route used in this project

```text
Activities and actors
        ↓
Form of interdependence
        ↓
Coordination and information requirement
        ↓
Encoded design response
        ↓
Documentary observation
        ↓
Bounded theoretical interpretation
        ↓
Rival explanation and evidence limit
```

### 9. What this stream allows us to say

**Established theoretical claim:** Organisations must divide and integrate work, and appropriate arrangements depend on interdependence, uncertainty, and relations among design elements.

**Interpretation for this project:** Enterprise-software reference architecture may encode design-relevant arrangements through roles, activities, objects, workflows, information relations, rules, and rights.

**Empirical proposition:** The project will test whether these arrangements can be reconstructed systematically as encoded organisation design.

**Claim not supported by documentation alone:** SAP determines an adopting organisation’s structure, coordination, performance, or everyday practice.

## Readable scholarly synthesis

### Organisation design begins with division and integration

Organisation design asks how a collective purpose is divided into manageable work and how the resulting parts are integrated again. Burton and Obel (2018) describe this as a relationship between structure and coordination. Structure divides work into tasks and units. Coordination enables those differentiated parts to contribute to a common purpose.

This framing is broader than an organisation chart. Goals, strategy, tasks, people, leadership, information, decisions, incentives, and control arrangements all matter. Their effects also depend on one another. A role may have little organisational meaning unless it is connected to tasks, information, authority, and other roles.

**Interpretation for this project:** SAP reference architecture may represent design-relevant arrangements by defining roles, tasks, units, objects, workflows, rules, and rights.

**Evidence boundary:** The presence of those elements does not prove that the software determines an adopting organisation. It establishes an encoded arrangement, not implementation fit or enacted practice.

Puranam, Alexy, and Reitzig (2014) help prevent exaggerated claims about novelty. They argue that apparently new forms of organising should be assessed through the fundamental problems they solve. These include dividing tasks, allocating tasks, distributing rewards, and providing information. A new label may describe a new combination of familiar solutions rather than a wholly new organisational form.

For this reason, the project should not call enterprise software a new organisational form simply because familiar mechanisms are digitally represented. The sharper question is whether software introduces a distinct organisational operation or provides a new carrier for an established solution.

**Section takeaway:** Organisation design gives us a vocabulary for examining software organisationally, but it does not allow us to equate software with the organisation.

### Fit concerns configurations, not isolated features

Contingency theory rejects the idea of one universally effective design. An arrangement must be evaluated in relation to its task, environment, strategy, and other design elements. Later research makes this relationship more dynamic and multivariate, but it does not abandon the underlying idea of fit.

Rivkin and Siggelkow (2003) show why isolated feature claims are unsafe. Hierarchy, incentives, decision decomposition, interactions among decisions, and limits on managerial information processing have interdependent effects. A design element that supports broad search can require another element that provides stability. Hierarchy can therefore help in one configuration and harm in another.

**Illustrative application:** A workflow should be interpreted together with its roles, thresholds, visibility rules, escalation paths, and configuration options. Saying that “workflow centralises decision-making” would be premature if these connected elements have not been examined.

Gulati and Puranam (2009) add another qualification. Formal and informal organisation may be inconsistent, and temporary inconsistency can sometimes facilitate renewal. Formal coherence is therefore not the same as organisational effectiveness. Software makes formal arrangements visible, but informal relationships may supplement, resist, or transform them.

This produces three distinct forms of fit:

1. **Architectural coherence:** whether encoded elements are mutually consistent.
2. **Implementation fit:** whether the selected configuration suits a particular organisation.
3. **Enacted fit:** whether everyday practice meets actual coordination and information needs.

The present documentary study can examine architectural coherence directly. The other forms require evidence from implementation and use.

**Section takeaway:** The organisational significance of a software feature depends on the configuration around it and the context in which it is implemented.

### Decomposition creates integration requirements

Complex work must be divided, but the boundaries matter. Ethiraj and Levinthal (2004) show that both excessive integration and excessive decomposition can create problems. Too much integration can restrict search and cause premature commitment to inferior designs. Too much decomposition can create instability and repeated adjustment among parts.

Browning (2001) explains how a design structure matrix can represent dependencies among components or tasks. For this project, a dependency matrix could make role, task, and object relationships visible across a process. The matrix would be an analytical method. It would not show that SAP itself implements a modular organisation.

Technical modularity and organisational modularity must remain separate. Software components concern technical interfaces. Organisational modules concern whether groups of tasks and actors can work with limited cross-boundary coordination. Avritzer et al. (2010) demonstrate that technical dependencies can create organisational coordination requirements, but the two forms of architecture are not identical.

**Section takeaway:** A named software module is not automatically an organisational module. The analysis must examine the activities, actors, and dependencies associated with it.

### Coordination mechanisms are not coordination outcomes

Okhuysen and Bechky (2009) distinguish coordination mechanisms from the conditions those mechanisms may support. Plans, roles, routines, meetings, schedules, and objects may contribute to accountability, predictability, or common understanding. The mechanism and the condition are not the same.

A workflow may specify sequence and responsibility. This may provide a basis for predictability and accountability. It does not prove that people can anticipate one another or accept responsibility in practice.

Gittell (2002) shows that coordination also depends on relationships and communication. Shared goals, shared knowledge, mutual respect, and timely problem-solving communication are not contained in a workflow or data object. Faraj and Xiao (2006) add that uncertain, fast-response work can require expertise, contestation, joint sensemaking, and even protocol breaking.

Zaitsev, Gal, and Tan (2020) show that artefacts can participate in coordination. Their significance arises through relations among actors, representations, and practices. This supports examining software artefacts as potential coordination arrangements, while rejecting the assumption that an artefact coordinates by itself.

**Section takeaway:** Documentary analysis can identify an encoded mechanism and its intended condition. It cannot establish relational quality or coordinated performance.

### Information must be connected to a capacity to act

Galbraith links uncertainty to information-processing requirements. Organisations can respond by reducing the amount of information that must be processed or by increasing their capacity to process it.

Later empirical work shows why information availability alone is insufficient. Srinivasan and Swink (2018) connect visibility and analytics with organisational flexibility. Their argument implies that insight matters when the organisation can act on it. Gattiker and Goodhue (2005) likewise show that ERP consequences vary with interdependence and differentiation.

For this project, shared data, analytical views, alerts, and document flows may represent information-processing capacity. Their organisational meaning also depends on decision rights, response mechanisms, and flexibility.

**Evidence boundary:** Reference architecture cannot establish realised analytical capability, shared interpretation, or performance.

### Digital technology creates possibilities through relationships

Zammuto et al. (2007) argue that new organisational possibilities arise from the intersection of technological features and organisational arrangements. This is an affordance perspective. Technology does not create an organisational result by itself. A possibility emerges through the relationship between technical features, actors, goals, and practices.

Digital-infrastructure and innovation research broadens the picture further by examining installed bases, generativity, and changing organisational boundaries. These works matter to the wider research programme, but they should not replace the more focused organisation-design framework used for Paper 1.

### The precise contribution of this project

Existing literature establishes four parts of the argument:

1. Organisation design includes task, information, decision, coordination, and control arrangements.
2. Digital technologies interact with organisational arrangements to create possibilities for action.
3. Enterprise systems embody integrated process and information structures.
4. Technical dependencies can have organisational coordination implications.

The literature does not already establish the complete proposition that ERP reference architecture is codified organisation design. That is the bridge this research must construct and test.

The defensible claim is therefore:

> Enterprise-software reference architecture can be examined as a candidate representation of organisation design. The analysis must reconstruct encoded relations among tasks, actors, information, decisions, controls, and coordination mechanisms, while keeping implementation and practice outside the direct documentary claim.

## Complete technical expansion

The sections below preserve the full source-by-source argument, detailed qualifications, and post-2000 literature map for research and citation work. Each section begins from an analytical problem, then explains what the cited literature contributes, how the contributions connect, and what the project may infer from them.

## Purpose and evidential scope

This review develops the organisation-design stream for the research programme on enterprise software as codified organisation design. Claims are based on verified bibliographic records and, where accessible, publishers' abstracts or full texts. The review deliberately separates organisation-design scholarship from adjacent work on coordination, enterprise systems, digital infrastructure, and work design. Those adjacent streams matter, but moving a paper into “organisation design” merely because it discusses technology or coordination would obscure rather than strengthen the theoretical argument.

Post-2000 research did not replace the classic framework associated with Thompson, Galbraith, and Mintzberg with a single modular or digital paradigm. Instead, it developed several partially connected lines of work. These include multi-contingency fit and misfit, configurational relations among design elements, decomposition under complex interdependence, practice-based accounts of coordination, and the organisational possibilities associated with digital technologies.

Together, these developments make organisation design more dynamic and relational. Only some of them directly support the claim that organisation is encoded in software. The review therefore distinguishes literature that defines organisational design from literature that supplies an analogy, boundary condition, or adjacent digital application.

## 1. What organisation design explains

Organisation design begins with a paired problem: work must be divided, and the divided work must be brought back together. It concerns the deliberate or emergent arrangement of task division and task integration in pursuit of a collective purpose.

Burton and Obel (2018) express this as a problem of fit between **structure** and **coordination**. Structure divides a larger purpose into tasks and units. Coordination enables those differentiated parts to work in concert. Their multi-contingency view also broadens design beyond the organisation chart. Goals, strategy, structure, and tasks interact with leadership, people, and work processes. Control, decision, information, and incentive systems contribute to coordination. This is a contemporary restatement of the classical design problem, not a rejection of it.

The distinction between division and integration is directly relevant to enterprise software. A reference architecture can differentiate organisational units, roles, tasks and business objects, then connect them through workflows, information systems, rules and rights. Burton and Obel therefore justify asking whether an architecture contains design-relevant arrangements. They do not establish that any documented software feature is an organisation design or that a package determines an adopting organisation. Their framework is a theory of organisational design fit, not a theory of software encoding.

Puranam, Alexy, and Reitzig (2014) provide a second foundation by asking what is genuinely new about new forms of organising. They argue that novelty should be assessed through fundamental organising problems rather than fashionable labels. Their account directs attention to task division, task allocation, reward distribution, information provision, and the bundles of solutions used to address them.

A supposedly new form may therefore combine familiar elements in a new bundle without requiring wholly new organisation theory. This matters for the present programme. A “software-defined organisation” should not be declared a new organisational form merely because familiar mechanisms are represented digitally. The theoretical task is first to identify which organising problems a configuration addresses. The project can then ask whether software performs a distinct organisational operation or provides a new carrier for an established one.

Together, these perspectives suggest an analytical definition: organisation design is the arrangement of differentiated tasks and actors plus the mechanisms of information, decision, control, incentive and interaction through which their interdependencies are managed. This definition is broad enough to include digitally mediated arrangements but narrow enough to exclude technology that has no organisational operation.

## 2. Contingency after 2000: from simple fit to interdependent design configurations

### 2.1 Continuity of the contingency argument

Contingency theory rejects the idea that one organisational design is best in every setting. Its core claim is that the appropriateness of a design depends on the context and task. Post-2000 work makes this relation more multivariate, dynamic, and internally interdependent rather than abolishing it.

Burton, DeSanctis, and Obel treat design components as an interconnected system. Their multi-contingency approach diagnoses misfits among environment, strategy, configuration, task, people, leadership, coordination, control, and incentives. Burton and Obel (2018) also argue that design rules should draw on empirical observation, simulation, and experimentation. This becomes especially important when novel organisational conditions make backward-looking prescription unreliable.

This creates two implications. First, no isolated design variable should be expected to have a stable effect across contexts. Second, internal coherence among design components matters alongside fit with the environment. For enterprise software, this discourages claims such as “workflow centralises decision-making” without examining the workflow's relation to role design, thresholds, structural restrictions, information visibility, exception rights and local configuration.

### 2.2 Complementarity and inconsistency among design elements

The next question is whether design elements have independent effects. Rivkin and Siggelkow (2003) show why they often do not. They examine the interdependencies among vertical hierarchy, incentives, the decomposition of decisions, interactions among decisions, and managerial information-processing limits.

Their agent-based model centres on a tension between **search** and **stability**. Search helps an organisation explore alternative configurations. Stability helps it retain a good configuration once found. Some design elements promote search, while others promote stability. An element that strongly promotes one may increase the value of another that provides the missing counterbalance. Vertical hierarchy is therefore neither uniformly beneficial nor redundant. Its effect depends on the wider configuration and can be harmful under some conditions.

The significance is more precise than saying that several designs can work. Design elements may be **complementary**, meaning that one becomes more valuable when another is present. They may also be **compensatory**, meaning that one offsets a weakness or excess created by another. The value of an element therefore depends on the surrounding arrangement.

**Illustrative example:** A strict workflow may become workable when it is combined with clear roles and a usable exception route. The same workflow may become obstructive if exceptions cannot be escalated or resolved.

An enterprise architecture should consequently be analysed as a configuration rather than an inventory of primitives. A rule, approval hierarchy, and incentive system are not independent solutions. Even when software exposes only the rule and approval hierarchy, an unobserved incentive system may condition their organisational consequences. Paper 1 can reconstruct the encoded configuration. It cannot establish overall fit because many relevant organisational contingencies lie outside the reference architecture.

Gulati and Puranam (2009) extend configurational reasoning by analysing inconsistency between formal and informal organisation. Their central contribution is that temporary inconsistencies need not be treated only as design failure: they can facilitate organisational renewal. This cautions against equating formal architectural coherence with organisational effectiveness. Software makes formal arrangements especially inspectable, but informal networks and routines may supplement, counteract, or transition around them. For Paper 1, the implication is a boundary condition: the encoded design may be internally coherent without describing the full coordination system of an adopting organisation.

### 2.3 Equifinality and the limits of optimal-design language

Contingency and configurational research also permits **equifinality**. In plain language, different configurations may perform a similar function or reach a similar outcome. Equifinality does not mean that every configuration is equally suitable. It also cannot be inferred merely because software offers several configuration choices. Demonstrating functional equivalence requires comparative outcome evidence, which lies outside the documentary design of Paper 1.

Accordingly, this programme should use “fit” in three distinct senses. **Architectural coherence** concerns consistency among encoded elements. **Implementation fit** concerns correspondence between a selected configuration and a particular organisational context. **Enacted fit** concerns whether actual practices meet coordination and information requirements. Documentary evidence can address only the first directly.

## 3. Decomposition, modularity and organisational complexity

### 3.1 Modularity is contingent, not the general direction of organisation design

Modularity is attractive because it promises to make complexity manageable, but deciding where to draw boundaries is itself a design problem. Ethiraj and Levinthal (2004) analyse how a complex system can be divided into modules. Their simulation demonstrates a trade-off. Excessive integration can limit search and produce premature fixation on an inferior design. Excessively fine modularisation can generate instability, cycling, and failure to improve.

Their contribution is not that modularity is generally superior to hierarchy. It is that the effectiveness of decomposition depends on how well module boundaries correspond to actual interaction patterns and on the search dynamics those boundaries produce.

Browning (2001) reviews the design structure matrix as a method for representing component or task dependencies and supporting decomposition and integration. Its relevance is methodological as much as theoretical. A matrix makes dependencies visible and can help identify clusters, sequencing, feedback and coordination needs. For the SAP study, a design-structure or dependency matrix could represent role–task–object relations across a reference process. That analytical use should not be mistaken for evidence that SAP itself implements modular organisation design.

Rivkin and Siggelkow (2003) similarly show that the decomposition of decisions interacts with hierarchy, incentives, decision interdependence and processing limits. Taken together, this research supports three restrained propositions: task decomposition is an organisation-design choice; the quality of decomposition depends on underlying interdependencies; and decomposition creates integration requirements. It does not support the broad historical claim that organisation design after 2000 became modular.

### 3.2 Nearly decomposable systems and enterprise architecture

The idea of a **nearly decomposable system** provides the bridge from modularity to interdependence. Such a system contains clusters whose internal interactions are stronger or more frequent than their interactions with other clusters. The parts are relatively independent, not completely isolated.

Enterprise software invites a modular reading because it contains process domains, components, roles, services, and data objects. Yet technical and organisational modularity are different. Technical modularity concerns interfaces and dependencies among software components. Organisational modularity concerns whether groups of tasks and actors can operate with limited coordination across their boundaries.

**Illustrative example:** Two software components may be technically separate while their users must communicate continually to resolve exceptions. The system is technically modular, but the work is not organisationally independent.

The two forms of modularity may align, but they need not. Avritzer et al. (2010) demonstrate the converse problem in global software development: dependencies in software architecture create coordination demands for geographically distributed work. Architecture can therefore shape the need for organisational communication without being identical to organisational structure.

This distinction is central to “software organisational primitives”. A primitive should not qualify because it is a technical module. It qualifies only where its operation divides, allocates, coordinates, informs, authorises or controls organisationally meaningful work.

## 4. Coordination as mechanisms, conditions and situated practice

### 4.1 From structural devices to integrative conditions

Once work has been divided, the analysis must explain how it is reintegrated. Okhuysen and Bechky (2009) define coordination as interaction that integrates interdependent tasks. Their review organises a diverse literature by separating **coordination mechanisms** from the **integrative conditions** those mechanisms may produce.

Mechanisms include routines, plans, schedules, roles, and meetings. The three integrative conditions are accountability, predictability, and common understanding. This separation is a major refinement for architectural analysis because it prevents a visible device from being confused with its intended effect.

A workflow is an encoded mechanism. It may support predictability by specifying sequence, accountability by assigning a task, and common understanding by displaying shared status. Documentary analysis can establish the mechanism and sometimes its intended condition. It cannot establish that users actually experience predictability or common understanding. This difference should be built into coding language: “provides an encoded basis for accountability” is defensible where assignment and trace are explicit; “creates accountability” requires evidence of organisational enactment.

Gittell (2002) adds a relational level that is not captured by mechanisms alone. She examines coordination through relationships characterised by shared goals, shared knowledge, mutual respect, and communication that is frequent, timely, accurate, and oriented toward problem solving. The study treats relational coordination as a mediator between coordination mechanisms and performance under varying input uncertainty.

This provides an important counterweight to an artefact-centred account. Formal roles, routines, and information systems may enable relational coordination. The quality of relationships and communication is not, however, contained in the formal mechanism.

### 4.2 Expertise and dialogic coordination under high uncertainty

Faraj and Xiao's (2006) study of a trauma centre asks what coordination requires when uncertainty is high and time is scarce. They distinguish two families of practice. **Expertise coordination practices** include protocols, community-of-practice structuring, plug-and-play teaming, and knowledge sharing. **Dialogic coordination practices** include contesting knowledge claims, making sense of a situation jointly, intervening across boundaries, and sometimes breaking a protocol.

Under novel and time-critical conditions, actors may therefore need to do more than follow a prescribed procedure. They may have to question, reinterpret, or depart from it.

This finding qualifies a simple contingency mapping in which uncertainty is handled by more information processing. The nature of the information and authority relation matters. A system can route an exception to expertise, but it may not encode the contestation through which experts revise the problem definition. For the SAP case, exceptions, overrides and escalation should be examined for how much dialogic adjustment the architecture represents, enables, or leaves outside. An absence of mutual-adjustment artefacts is not evidence that enacted work lacks mutual adjustment; it may reveal a limit of the reference representation.

### 4.3 Coordination artefacts and digital work

The next step is to ask how material and digital artefacts participate in coordination. Zaitsev, Gal, and Tan (2020) examine coordination artefacts in agile software development. Their study supports the proposition that artefacts can participate in coordination, but it does not justify the general claim that software contains organisational structure. An artefact acquires coordinating force through its relations with representations, practices, and actors.

Persson et al. (2022) examine mutual adjustment in the integration of agile software development and user-experience design. Their study extends the empirical settings in which Mintzbergian mutual adjustment can be observed. It does not show that classical coordination mechanisms have been replaced.

The post-2000 coordination literature therefore becomes “coordination-rich” in a specific sense: it differentiates formal mechanisms, relational conditions, expertise practices, temporal practices, dialogic intervention and material artefacts. The development is plural, not a unified new theory.

## 5. Information processing in contemporary organisation design

### 5.1 Demand, capacity and action

Galbraith's information-processing logic connects uncertainty and interdependence to a practical design problem. An organisation can reduce the amount of information that must be processed, increase its capacity to process information, or combine both responses.

Later research examines particular capacities and the arrangements that make them useful. Srinivasan and Swink (2018), for example, analyse data from 191 firms. They report that demand and supply visibility are associated with analytics capability. Analytics capability has a stronger association with operational performance when organisational flexibility permits action on the resulting insights, particularly under volatile conditions.

The theoretical implication is not merely that more visibility is better. Information availability and capacity to act are complements. This matters for enterprise architecture: integrated data and analytical views may increase encoded information capacity, but decision rights, process flexibility and response mechanisms determine whether insights can be acted upon. Paper 1 can reconstruct the architecture's proposed relation among visibility, rights and workflow. It cannot infer realised analytical capability or performance.

Gattiker and Goodhue (2005) examine plant-level consequences after ERP implementation through interdependence and differentiation. Their central relevance is that ERP effects are conditioned by organisational context rather than uniform. The paper belongs at the boundary between organisation design and enterprise-systems research: it uses organisational constructs to explain outcomes after implementation. It does not analyse reference architecture as encoded organisation, but it supplies a reason to expect that common enterprise-system arrangements interact differently with differentiated and interdependent units.

### 5.2 Digital affordances and new possibilities for organising

An **affordance** is a possibility for action that arises in the relation between an actor and a material arrangement. It is not a fixed effect contained in a technology. Zammuto et al. (2007) use this relational reasoning to argue that new organisational possibilities arise from the intersection of IT features with organisational arrangements and practices, not from IT alone.

They identify affordances that include visualising entire work processes, supporting real-time and flexible product or service innovation, enabling virtual and mass collaboration, and creating simulations or synthetic representations. Their insistence on unpacking both technology and organisation is especially important for this project.

The paper supports analysing what a technology makes organisationally possible. It does not support deterministic language such as “software recreates structure digitally”. An affordance is relational: what can be done depends upon technical features and organisational arrangements. Reference architecture provides evidence about designed features and intended roles, but the actual affordance relation belongs partly to implementation and use.

Yoo et al. (2012) broaden the discussion to organising for innovation in a digitised world. Digital-infrastructure studies, including Hanseth and Lyytinen (2010) and Henfridsson and Bygstad (2013), explain how infrastructures evolve through their existing base of systems, users, standards, and practices. They also examine **generativity**, meaning a capacity to produce further developments that were not fully specified in advance.

These works move the unit of analysis beyond a bounded firm and show how digital artefacts can reconfigure organisational boundaries and participation. They belong primarily to digital innovation and infrastructure research. They should inform the wider research programme without overloading Paper 1's organisation-design framework.

## 6. Does post-2000 organisation design support “software-encoded structure”?

The proposition that enterprise systems and software architectures operate as organisational design media requires a carefully bounded evidence chain. The literature supports several components of this claim, but not the complete proposition as an established consensus.

First, organisation-design research establishes that roles, tasks, information systems, decisions, controls and incentives are design components (Burton and Obel, 2018). Second, digital-organisation research establishes that IT features combine with organisational arrangements to enable new forms of organising (Zammuto et al., 2007). Third, enterprise-systems research shows that integrated systems embody process and data logics and that their effects vary with interdependence and differentiation (Gattiker and Goodhue, 2005). Fourth, software-architecture research shows that technical dependencies have coordination implications for the organisation producing software (Avritzer et al., 2010).

None of these, individually, demonstrates that an ERP reference architecture *is* codified organisation design. The proposed research contribution lies precisely in constructing and empirically testing that bridge. Treating the bridge as already established would erase the paper's theoretical work. A defensible formulation is:

> Existing research establishes that organisation design encompasses task division, coordination, information, decision and control arrangements; that digital technologies interact with organisational arrangements to create organising possibilities; and that enterprise systems embody integrated process and information structures. This study tests whether and how these observations can be joined through the concept of encoded organisation design.

This formulation treats “software organisational primitive” as a candidate theoretical construct, not a renamed feature.

## 7. A refined post-2000 map

| Development | What the literature supports | What it does not support | Relevance to SAP study |
|---|---|---|---|
| Multi-contingency fit | Design components and context are jointly interdependent; misfits can be multiple and dynamic | One universally optimal design or outcome inference from architecture | Analyse configurations and distinguish architectural from implementation fit |
| Complementarity and inconsistency | Hierarchy, decomposition, incentives and informal organisation can complement, compensate or conflict | Independent feature effects | Code relations among primitives and preserve omitted organisational contingencies |
| Decomposition and modularity | Module boundaries must reflect interactions; over- and under-decomposition create different problems | Modularity as a universally superior post-2000 form | Distinguish technical from organisational modularity |
| Coordination mechanisms and conditions | Routines, plans, roles, meetings and artefacts may support accountability, predictability and common understanding | That encoded mechanisms necessarily produce those conditions | Separate mechanism from intended and realised coordination |
| Expertise/dialogic coordination | Novel events require contestation, joint sensemaking and sometimes protocol breaking | That all uncertainty can be resolved through richer formal information systems | Search for exception, override and escalation boundaries |
| Information-processing complements | Visibility/analytics require flexibility and rights to act; effects vary with uncertainty | Data integration as sufficient for performance | Map information operation to decision and response mechanism |
| Digital affordances | Organising possibilities emerge from technology–organisation combinations | Technological determinism or architecture equalling practice | Bound claims to encoded possibilities and constraints |

## 8. Implications for the conceptual framework and coding

The review yields five revisions to the programme's use of organisation design.

First, treat the **configuration** rather than the isolated primitive as the main explanatory unit. The primitive remains useful for descriptive decomposition, but organisation design is visible in relations among structure, task, information, rights and coordination.

Second, distinguish a **coordination mechanism** from an **integrative condition** and from a **realised outcome**. Workflow is a mechanism; predictability is a possible condition; reliable collective performance is an outcome. Paper 1 can most strongly evidence the first.

Third, treat modularity as an empirical property of decomposition and interaction, not as a historical label for digital organisation. A process domain is not organisationally modular merely because the software architecture names it separately.

Fourth, divide fit into architectural coherence, implementation fit and enacted fit. Only architectural coherence lies within the documentary study's direct evidential reach.

Fifth, preserve dialogic and informal coordination as theoretically important negative space. If SAP documents rules, workflows and exceptions but not contestation or mutual adjustment, the finding concerns the limits and emphases of the encoded architecture, not the absence of those practices in organisations.

## 9. Positioning for the eventual summarised review

The eventual manuscript review should not claim that post-2000 theory “became modular, digital, and coordination-rich” without qualification. A more accurate synthesis is:

> Post-2000 organisation-design scholarship retained the classical concern with fitting differentiation and integration to task and environmental conditions, while elaborating interdependencies among design elements, the contingencies of decomposition, the plurality of coordination practices, and the organisational possibilities created with digital technology. This work provides concepts for analysing software architecture organisationally, but it does not by itself establish enterprise software as codified organisation design.

That final sentence defines the opening for the present study. Thompson, Galbraith and Mintzberg remain the primary lenses; post-2000 work refines their application, supplies boundary conditions, and prevents overly structural or deterministic interpretation.

## References used in this review

Full working records are in `../references/references.bib`. Core sources added or verified for this stream include Avritzer et al. (2010), Browning (2001), Burton and Obel (2018), Burton, DeSanctis and Obel (2011), Ethiraj and Levinthal (2004), Faraj and Xiao (2006), Gattiker and Goodhue (2005), Gittell (2002), Gulati and Puranam (2009), Okhuysen and Bechky (2009), Puranam, Alexy and Reitzig (2014), Rivkin and Siggelkow (2003), Srinivasan and Swink (2018), Zaitsev, Gal and Tan (2020), and Zammuto et al. (2007).

## Glossary for teaching and review

| Term | Plain-language meaning |
|---|---|
| Differentiation | Dividing organisational work into specialised tasks, roles, or units |
| Integration | Reconnecting differentiated work so that it contributes to a collective purpose |
| Interdependence | A condition in which one activity, actor, or unit depends on another |
| Uncertainty | A gap between information required to perform a task and information already available |
| Information-processing capacity | The organisation’s ability to collect, communicate, interpret, and act on relevant information |
| Coordination mechanism | An arrangement used to integrate dependent activity, such as a workflow, plan, role, or routine |
| Configuration | A set of design elements whose effects depend on one another |
| Complementarity | A relationship in which the value of one design element increases in the presence of another |
| Equifinality | The possibility that different configurations can perform similar functions or reach similar outcomes |
| Modularity | Division into parts with relatively limited interaction across their boundaries |
| Architectural coherence | Consistency among elements represented within the reference architecture |
| Implementation fit | Correspondence between a configured system and a particular organisational context |
| Enacted fit | Correspondence between actual practices and coordination or information requirements |
| Affordance | A possibility for action arising from the relationship between technical features and organisational arrangements |
