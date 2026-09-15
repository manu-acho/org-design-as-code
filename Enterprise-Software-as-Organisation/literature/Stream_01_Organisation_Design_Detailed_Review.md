# Stream One: Organisation Design, Detailed Literature Review

## Purpose and evidential scope

This review develops the organisation-design stream for the research programme on enterprise software as codified organisation design. Claims are based on verified bibliographic records and, where accessible, publishers' abstracts or full texts. The review deliberately separates organisation-design scholarship from adjacent work on coordination, enterprise systems, digital infrastructure, and work design. Those adjacent streams matter, but moving a paper into “organisation design” merely because it discusses technology or coordination would obscure rather than strengthen the theoretical argument.

Post-2000 research did not replace a classic Thompson–Galbraith–Mintzberg framework with a single new, modular or digital paradigm. It developed several partially connected lines of work: multi-contingency fit and misfit; configurational complementarity among design elements; decomposition and modularity under complex interdependence; process- and practice-based accounts of coordination; and renewed attention to the organisational possibilities associated with digital technologies. These developments make organisation design more dynamic and relational. Only some of them, however, directly support the claim that organisation is encoded in software.

## 1. What organisation design explains

Organisation design concerns the deliberate or emergent arrangement of task division and task integration in pursuit of a collective purpose. Burton and Obel (2018) express the core problem as fit between **structure**, which divides a larger purpose into tasks and units, and **coordination**, which makes those differentiated parts work in concert. Their multi-contingency view broadens design beyond the organisation chart: goals, strategy, structure and tasks interact with leadership, people and work processes, while coordination is accomplished through control, decision, information and incentive systems. This is a useful contemporary restatement of the classical problem rather than a rejection of it.

The distinction between division and integration is directly relevant to enterprise software. A reference architecture can differentiate organisational units, roles, tasks and business objects, then connect them through workflows, information systems, rules and rights. Burton and Obel therefore justify asking whether an architecture contains design-relevant arrangements. They do not establish that any documented software feature is an organisation design or that a package determines an adopting organisation. Their framework is a theory of organisational design fit, not a theory of software encoding.

Puranam, Alexy and Reitzig (2014) provide a second useful foundation. They ask what is genuinely new about new forms of organising and argue that novelty should be assessed through fundamental problems of organising rather than labels. Their account directs attention to task division, task allocation, reward distribution and information provision, and to bundles of solutions to those problems. A supposedly novel form may combine familiar elements in a novel bundle without requiring wholly new organisation theory. This is important for the present programme: “software-defined organisation” should not be asserted as a new organisational form merely because its mechanisms are digitally represented. The theoretical task is to identify which old organising problems are solved by which configurations, and then determine whether software introduces a distinct operation or only a new carrier.

Together, these perspectives suggest an analytical definition: organisation design is the arrangement of differentiated tasks and actors plus the mechanisms of information, decision, control, incentive and interaction through which their interdependencies are managed. This definition is broad enough to include digitally mediated arrangements but narrow enough to exclude technology that has no organisational operation.

## 2. Contingency after 2000: from simple fit to interdependent design configurations

### 2.1 Continuity of the contingency argument

The core contingency claim remains that the appropriateness of a design depends upon features of the context and task. Post-2000 work commonly makes the fit relation more multivariate, dynamic, and internally interdependent; it does not abolish it. Burton, DeSanctis and Obel's multi-contingency approach treats design components as an interconnected system and diagnoses misfits among environment, strategy, configuration, task, people, leadership, coordination, control and incentives. Burton and Obel (2018) additionally argue for design rules based on empirical observation, simulation and experimentation, especially where novel organisational conditions make backward-looking prescription unreliable.

This creates two implications. First, no isolated design variable should be expected to have a stable effect across contexts. Second, internal coherence among design components matters alongside fit with the environment. For enterprise software, this discourages claims such as “workflow centralises decision-making” without examining the workflow's relation to role design, thresholds, structural restrictions, information visibility, exception rights and local configuration.

### 2.2 Complementarity and inconsistency among design elements

Rivkin and Siggelkow (2003) examine interdependencies among a vertical hierarchy, incentives, the decomposition of decisions, interactions among decisions, and managerial information-processing limits. Their agent-based model is organised around a tension between broad search for good configurations and stability once good decisions are discovered. Sets of design elements may promote search or stability, and elements that promote one can increase the value of offsetting elements that provide the other. Vertical hierarchy is therefore neither uniformly beneficial nor redundant: its effect depends upon a configuration and can be detrimental under some conditions.

The significance is not simply that “several designs can work”. More precisely, design elements have **complementary and compensatory relations**, so the marginal value of one depends on the presence of others. An enterprise architecture should consequently be analysed as a configuration rather than an inventory of primitives. A rule, approval hierarchy, and incentive are not independent solutions; even where the software exposes only the first two, the unobserved incentive system may condition their organisational consequences. Paper 1 can reconstruct the encoded configuration, but it cannot establish overall fit because many relevant organisational contingencies lie outside the reference architecture.

Gulati and Puranam (2009) extend configurational reasoning by analysing inconsistency between formal and informal organisation. Their central contribution is that temporary inconsistencies need not be treated only as design failure: they can facilitate organisational renewal. This cautions against equating formal architectural coherence with organisational effectiveness. Software makes formal arrangements especially inspectable, but informal networks and routines may supplement, counteract, or transition around them. For Paper 1, the implication is a boundary condition: the encoded design may be internally coherent without describing the full coordination system of an adopting organisation.

### 2.3 Equifinality and the limits of optimal-design language

Contingency and configurational research permits **equifinality**: different configurations may perform similar functions or reach similar outcomes. It does not imply that any configuration is equally suitable. Nor can equifinality be inferred from the mere availability of configuration choices in software. Demonstrating functional equivalence requires comparative outcome evidence, which is outside the documentary design of Paper 1.

Accordingly, this programme should use “fit” in three distinct senses. **Architectural coherence** concerns consistency among encoded elements. **Implementation fit** concerns correspondence between a selected configuration and a particular organisational context. **Enacted fit** concerns whether actual practices meet coordination and information requirements. Documentary evidence can address only the first directly.

## 3. Decomposition, modularity and organisational complexity

### 3.1 Modularity is contingent, not the general direction of organisation design

Ethiraj and Levinthal (2004) analyse the problem of identifying an appropriate modularisation of a complex system. Their simulation demonstrates a trade-off: excessive integration can produce limited search and premature fixation on inferior designs, whereas excessively fine modularisation can generate instability, cycling, and failure to improve. The contribution is therefore not that modularity is generally superior to hierarchy. It is that the effectiveness of decomposition depends upon how module boundaries correspond to interaction structures and upon the search dynamics generated by those boundaries.

Browning (2001) reviews the design structure matrix as a method for representing component or task dependencies and supporting decomposition and integration. Its relevance is methodological as much as theoretical. A matrix makes dependencies visible and can help identify clusters, sequencing, feedback and coordination needs. For the SAP study, a design-structure or dependency matrix could represent role–task–object relations across a reference process. That analytical use should not be mistaken for evidence that SAP itself implements modular organisation design.

Rivkin and Siggelkow (2003) similarly show that the decomposition of decisions interacts with hierarchy, incentives, decision interdependence and processing limits. Taken together, this research supports three restrained propositions: task decomposition is an organisation-design choice; the quality of decomposition depends on underlying interdependencies; and decomposition creates integration requirements. It does not support the broad historical claim that organisation design after 2000 became modular.

### 3.2 Nearly decomposable systems and enterprise architecture

Enterprise software invites a modular reading because it contains process domains, components, roles, services and data objects. Yet technical modularity and organisational modularity are analytically distinct. Technical modules concern interfaces and dependencies among software components. Organisational modules concern the degree to which groups of tasks and actors can operate with limited cross-boundary coordination. The two may align, but Avritzer et al. (2010) show the converse problem in global software development: software-architectural dependencies have coordination implications for geographically distributed work. Architecture can shape the need for organisational communication without being identical to organisational structure.

This distinction is central to “software organisational primitives”. A primitive should not qualify because it is a technical module. It qualifies only where its operation divides, allocates, coordinates, informs, authorises or controls organisationally meaningful work.

## 4. Coordination as mechanisms, conditions and situated practice

### 4.1 From structural devices to integrative conditions

Okhuysen and Bechky (2009) define coordination as interaction that integrates interdependent tasks. Their review organises a heterogeneous literature by distinguishing coordination mechanisms, such as routines, plans, schedules, roles and meetings, from three integrative conditions they can produce: accountability, predictability and common understanding. This is a major refinement for architectural analysis because it prevents the mechanism from being confused with its intended integrative effect.

A workflow is an encoded mechanism. It may support predictability by specifying sequence, accountability by assigning a task, and common understanding by displaying shared status. Documentary analysis can establish the mechanism and sometimes its intended condition. It cannot establish that users actually experience predictability or common understanding. This difference should be built into coding language: “provides an encoded basis for accountability” is defensible where assignment and trace are explicit; “creates accountability” requires evidence of organisational enactment.

Relational coordination research adds another level. Gittell (2002) examines coordination through relationships characterised by shared goals, shared knowledge, mutual respect, and communication that is frequent, timely, accurate and problem-solving. The study treats relational coordination as a mediator between coordination mechanisms and performance under varying input uncertainty. This provides a powerful counterweight to an artefact-centred account: formal roles, routines and information systems may enable relational coordination, but the quality of relationships and communication is not contained in the formal mechanism.

### 4.2 Expertise and dialogic coordination under high uncertainty

Faraj and Xiao's (2006) study of a trauma centre develops a practice perspective for fast-response organisations. They distinguish expertise coordination practices, including protocols, community-of-practice structuring, plug-and-play teaming and knowledge sharing, from dialogic coordination practices such as epistemic contestation, joint sensemaking, cross-boundary intervention and protocol breaking. Under novel and time-critical conditions, actors may need not merely to follow a protocol but to contest, reinterpret or break it.

This finding qualifies a simple contingency mapping in which uncertainty is handled by more information processing. The nature of the information and authority relation matters. A system can route an exception to expertise, but it may not encode the contestation through which experts revise the problem definition. For the SAP case, exceptions, overrides and escalation should be examined for how much dialogic adjustment the architecture represents, enables, or leaves outside. An absence of mutual-adjustment artefacts is not evidence that enacted work lacks mutual adjustment; it may reveal a limit of the reference representation.

### 4.3 Coordination artefacts and digital work

Zaitsev, Gal and Tan (2020) examine coordination artefacts in agile software development. The study is directly relevant to the proposition that artefacts can participate in coordination, but it should not be converted into a general claim that software contains organisation structure. An artefact acquires coordinating force through relations among representations, practices and actors. Likewise, Persson et al. (2022) show mutual adjustment in the integration of agile software development and user-experience design. These studies extend the empirical settings in which Mintzbergian mutual adjustment is observed; they do not show that classical coordination mechanisms have been replaced.

The post-2000 coordination literature therefore becomes “coordination-rich” in a specific sense: it differentiates formal mechanisms, relational conditions, expertise practices, temporal practices, dialogic intervention and material artefacts. The development is plural, not a unified new theory.

## 5. Information processing in contemporary organisation design

### 5.1 Demand, capacity and action

Galbraith's information-processing logic remains influential because it links uncertainty and interdependence to a design problem: either reduce the need to process information or increase processing capacity. Later work operationalises particular capacities and examines complementary organisational arrangements. Srinivasan and Swink (2018), for example, analyse data from 191 firms and report that demand and supply visibility are associated with analytics capability; analytics capability is more strongly associated with operational performance when organisational flexibility permits action on generated insights, particularly under volatile conditions.

The theoretical implication is not merely that more visibility is better. Information availability and capacity to act are complements. This matters for enterprise architecture: integrated data and analytical views may increase encoded information capacity, but decision rights, process flexibility and response mechanisms determine whether insights can be acted upon. Paper 1 can reconstruct the architecture's proposed relation among visibility, rights and workflow. It cannot infer realised analytical capability or performance.

Gattiker and Goodhue (2005) examine plant-level consequences after ERP implementation through interdependence and differentiation. Their central relevance is that ERP effects are conditioned by organisational context rather than uniform. The paper belongs at the boundary between organisation design and enterprise-systems research: it uses organisational constructs to explain outcomes after implementation. It does not analyse reference architecture as encoded organisation, but it supplies a reason to expect that common enterprise-system arrangements interact differently with differentiated and interdependent units.

### 5.2 Digital affordances and new possibilities for organising

Zammuto et al. (2007) argue that new organisational possibilities arise from the intersection of IT features with organisational arrangements and practices, not from IT alone. They identify affordances including visualising entire work processes, real-time and flexible product/service innovation, virtual collaboration, mass collaboration, and simulation or synthetic representation. Their insistence on unpacking both technology and organisation is especially important for this project.

The paper supports analysing what a technology makes organisationally possible. It does not support deterministic language such as “software recreates structure digitally”. An affordance is relational: what can be done depends upon technical features and organisational arrangements. Reference architecture provides evidence about designed features and intended roles, but the actual affordance relation belongs partly to implementation and use.

Yoo et al. (2012) locate organising for innovation in a digitised world, while digital-infrastructure studies such as Hanseth and Lyytinen (2010) and Henfridsson and Bygstad (2013) explain evolution, generativity and installed-base dynamics. These works broaden the unit beyond a bounded firm and show why digital artefacts can reconfigure boundaries and participation. They belong primarily to digital innovation/infrastructure streams. They should inform the macro research programme without overloading Paper 1's organisation-design framework.

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
