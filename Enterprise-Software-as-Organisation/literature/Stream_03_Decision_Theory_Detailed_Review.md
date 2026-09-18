# Stream Three: Decision Theory, Detailed Literature Review

## How to use this review

This review has three layers. The **learning guide** introduces the main problem and vocabulary. The **readable scholarly synthesis** explains the literature as a connected argument. The **complete technical expansion** preserves the full scholarly detail, evidence boundaries, propositions, and coding framework.

The stream asks one practical question:

> How do organisations shape choices when people have limited attention, incomplete information, finite time, and unequal authority?

Enterprise software matters because it can distribute information, categories, rules, permissions, defaults, and exception routes. These are inputs to decision-making, not proof that a sound decision occurred.

## Learning guide

### 1. Begin with bounded rationality

Simon rejects the image of a decision-maker who knows every alternative, predicts every consequence, and calculates the best possible answer. Real actors work with limited time, information, attention, and computational capacity. They simplify problems and often search until they find an acceptable option.

Organisations respond by structuring the decision environment. They define what actors should notice, what objectives matter, which facts are relevant, what alternatives are recognised, and who can act. Simon calls these guides **decision premises**.

### 2. Decisions are distributed through premises

An organisation does not need senior managers to make every individual decision. It can distribute premises that shape many local choices. Policies, goals, classifications, thresholds, standard procedures, performance measures, and information reports all narrow or orient attention.

Enterprise software can encode such premises through fields, categories, defaults, tolerances, approval rules, calculated indicators, role assignments, and required evidence. The important analytical question is therefore not only who clicked approve. It is also who designed the categories, thresholds, and alternatives that made this choice possible.

### 3. Programmes handle recurrent situations

March and Simon describe programmes as organised responses to recurring situations. A programme reduces repeated problem-solving by linking recognised conditions to expected actions. In software, a workflow, rule, validation, automatic posting, or exception route may represent a programme.

Programmes can reduce cognitive burden and increase consistency. They can also exclude alternatives or reproduce assumptions that no longer suit the situation. The presence of a programme says little about its quality unless its premises and consequences are examined.

### 4. Authority is more than permission

Formal permission answers what a system allows a role to do. Authority concerns whether directives are accepted and acted upon. Barnard emphasises acceptance by the recipient. Simon explains authority as a relationship in which one actor permits another's decision to guide conduct within a zone of acceptance.

A role catalogue, approval matrix, or access control therefore shows a formal allocation. It does not establish actual influence, accepted authority, expertise, accountability, or the ability to secure compliance.

### 5. Automation often relocates discretion

Automation does not necessarily eliminate judgement. It may move judgement upstream to rule designers and configurators, sideways to data stewards, or downstream to exception handlers. It may also change what front-line users can see and contest.

The right question is not simply whether a decision is automated. Ask where the relevant premises were selected, who can change them, which cases escape the rule, and who handles exceptions.

### 6. Keep distinct acts distinct

Documentation often uses decision language loosely. The analysis should distinguish:

- **Information:** presenting facts or status.
- **Calculation:** deriving a value from specified inputs.
- **Recommendation:** proposing an option while leaving a choice open.
- **Decision:** selecting among alternatives or committing the organisation.
- **Authorisation:** granting permission for an action.
- **Execution:** carrying out an already determined action.
- **Automation:** performing one or more of these through encoded logic.

This prevents a dashboard, prediction, approval, and automatic posting from being treated as the same phenomenon.

### 7. Decisions may also serve legitimacy

Formal decisions do not always operate only as instruments for effective action. They can demonstrate rationality, responsibility, or compliance to an audience. Brunsson and Feldman and March help explain why plans, information, and decisions may have symbolic as well as operational roles.

This matters when reading enterprise documentation. A formally complete approval chain may communicate control and legitimacy even if practical influence or judgement lies elsewhere.

### 8. A practical reading route

For every rule, threshold, approval, default, recommendation, or automated action, ask:

1. What decision problem is being simplified?
2. What premises define relevant facts, goals, alternatives, and criteria?
3. Who designed those premises?
4. Who may decide, approve, override, or revise them?
5. What is automated, and what remains open to judgement?
6. Where has discretion moved?
7. How are exceptions recognised and escalated?
8. What evidence would establish accepted authority and actual decision practice?

### 9. Claim labels used throughout the project

- **Established claim:** Supported directly by identified scholarship.
- **Project interpretation:** A reasoned application of theory to the research problem.
- **Illustrative example:** Explains a concept but is not an empirical finding.
- **Proposition:** A claim to examine through data.
- **Evidence boundary:** States what available material cannot establish.
- **Verification required:** A citation, edition, or access issue still needs resolution.

## Readable scholarly synthesis

### 1. Bounded rationality makes organisation necessary

Simon begins from a simple but consequential point: individuals cannot process every relevant fact or calculate every possible consequence. Organising is partly the work of constructing an environment in which bounded actors can make workable choices. Attention is directed, alternatives are limited, responsibilities are assigned, and recurrent problems are given standard responses.

This reframes enterprise software. Its organisational significance lies not only in processing transactions, but also in structuring what users can perceive and do. A required field identifies a fact as relevant. A threshold distinguishes ordinary from exceptional cases. A role assignment allocates formal competence. A default favours one response before a user acts.

**Section takeaway:** To understand a decision, inspect the premises that shaped it.

### 2. Decision premises distribute organisational influence

March and Simon show how organisations guide behaviour without prescribing every act individually. Goals, rules, classifications, communication channels, and expectations become premises used in local choices. This is more subtle than centralisation. A decision may be executed locally while its decisive assumptions were selected elsewhere.

For documentary analysis, premises can be grouped into purpose, factual, value, attention, classification, procedural, and authority-related premises. The categories are analytical aids rather than claims that every artefact fits neatly into only one group.

**Illustrative example:** A purchasing tolerance may encode a factual comparison, a value judgement about acceptable variance, and an authority premise about who may override the result.

**Section takeaway:** The location of the click is not necessarily the location of judgement.

### 3. Programmes connect recurrent situations to action

March and Simon use programmes to explain how organisations respond efficiently to recurring stimuli. Simon later distinguishes relatively programmed from less programmed decisions. Programmes economise on attention by supplying search procedures, criteria, or standard actions.

In enterprise software, programmes may appear as workflows, rules, checks, schedules, recommendations, or automatic operations. Their benefits may include consistency and speed. Their risks include rigidity, hidden assumptions, and failure to recognise cases that do not match the encoded categories.

**Evidence boundary:** A documented programme does not establish that it is suitable, followed, or effective.

### 4. Formal and actual authority may diverge

Barnard grounds authority in acceptance. Simon explains how authority permits one actor's decision to guide another's behaviour within a zone of acceptance. Aghion and Tirole later distinguish formal authority, meaning the right to decide, from real authority, meaning effective control based partly on information and initiative.

This distinction is vital for software analysis. Access rights and workflow assignments are evidence of formal allocation. Actual authority may rest with a specialist who frames the options, a data owner who controls the premises, or an experienced user whose recommendation is rarely challenged.

**Section takeaway:** Permission is inspectable in architecture; accepted and effective authority require practice evidence.

### 5. Automation redistributes rather than simply removes judgement

Bovens and Zouridis describe a movement from street-level to system-level bureaucracy when rules are increasingly embedded in information systems. This insight should be used carefully. Automation may narrow front-line discretion, but choices remain in defining categories, training models, setting tolerances, maintaining data, specifying exceptions, and authorising overrides.

Joseph and Gaba's attention-based perspective reinforces this point. Structures distribute attention as well as authority. Gosain shows how enterprise systems can embed organisational knowledge and institutionalise assumptions. Loasby helps explain that institutions and routines make some forms of knowledge usable while leaving others outside the frame.

The project's concept of **discretion relocation** captures this movement. It asks where judgement has gone, who can exercise it, and whether affected actors can see or contest the premises.

### 6. Decisions, actions, and accounts should not be conflated

Simon distinguishes decision premises from resulting behaviour, while later work warns against treating formal decisions as transparent causes of action. Brunsson shows that decision, talk, and action can be loosely coupled. Feldman and March explain that information can carry symbolic value and signal competent management even when it is not used instrumentally.

Consequently, an approval record may document authorisation without revealing how the conclusion was reached. A dashboard may display information without shaping action. A recommendation may be routinely accepted, resisted, or ignored. Documentary evidence should be precise about which act is represented.

### 7. The contribution to this project

Decision theory allows enterprise software to be studied as a distribution of decision premises and programmed action. The architecture can define recognised facts, relevant categories, available alternatives, criteria, thresholds, permissions, defaults, approvals, automatic operations, and exception routes.

The resulting claim remains architectural. The project can reconstruct **encoded decision design** and formulate propositions about discretion, authority, attention, and exception handling. It cannot infer judgement quality, acceptance, accountability, or practical influence without implementation evidence.

## Complete technical expansion

The following sections preserve the full scholarly review, including its distinctions, source qualifications, propositions, and documentary coding framework. Each section begins with the decision problem at issue, relates the sources to one another, and ends with the implication or boundary for this project.

## Purpose and evidential boundary

This stream explains how organisations structure choice under bounded rationality and how enterprise software can encode decision premises, programmes, permissions, decision opportunities, and exceptions. Its central boundary is strict: a documented role, approval, rule, threshold, default, or automated action can reveal an encoded decision structure, but it cannot establish accepted authority, exercised discretion, substantive judgement, accountability, or decision quality.

The supplied LeapSpace report identifies several correct distinctions but cannot serve as the evidential foundation. Eight central citations resolve only to unidentified uploaded files or the research prompt, one source is wholly irrelevant, and foundational works are not bibliographically represented. The synthesis below therefore uses the report as a candidate map and rebuilds the argument around independently identified scholarship. Access and verification limits are recorded in the accompanying [source assessment](Stream_03_Decision_Theory_Source_Assessment.md).

## 1. Bounded rationality as an organisational problem

Decision theory begins with the limits under which real choices are made. Simon rejects the assumption that organisational actors possess complete information, unlimited computational capacity, stable preferences, and the ability to evaluate every alternative. Choice takes place within cognitive, informational, temporal, and organisational bounds. Actors simplify their environment, search selectively, and may accept a satisfactory alternative rather than prove that they have found a global optimum.

**Bounded rationality** is therefore not merely a statement that people make mistakes. It directs attention to the procedures through which choices become manageable. Organisations construct roles, classifications, programmes, reporting relationships, communication channels, and authority structures. These arrangements narrow attention and reduce the number of matters requiring fresh deliberation.

Such simplification enables coordinated action, but it is not neutral. It embeds assumptions about what counts as relevant information, an acceptable alternative, and a satisfactory result.

Simon's 1955 behavioural model provides the canonical article-level statement of rational choice under limits. Puranam et al. (2015) show that later organisational research has developed several ways to model bounded rationality. The project does not need to select one universal model of cognition. It needs to identify the limits and simplifying structures documented in the software architecture, while avoiding unsupported claims about users' psychological states.

## 2. Decision premises

Once rationality is understood as bounded, the next question is how an organisation shapes choices without making every choice centrally. Simon's concept of the **decision premise** provides the answer. In *Administrative Behavior*, organisational influence operates through the premises on which members base decisions. An organisation can therefore guide local choice by shaping the facts, values, objectives, categories, rules, expectations, and recognised alternatives that enter it.

A decision premise is not the same as a decision. It is part of the structured basis on which a decision is made. Enterprise software may plausibly encode premises through:

- mandatory or defaulted data;
- classifications and organisational assignments;
- eligibility and validation rules;
- tolerances and thresholds;
- available action menus or workflow outcomes;
- priority or sequencing rules;
- calculation and valuation methods;
- approval conditions;
- exception definitions;
- status-dependent permissions.

This concept supports a more precise argument than saying that software “makes decisions.” A purchasing tolerance, for example, can pre-structure whether an invoice follows a normal path or is blocked. The architecture may encode the relevant comparison and consequence. It does not show whether the underlying tolerance is legitimate, whether participants accept it, or whether the resulting action is substantively appropriate.

Two types of premise require particular care. A **factual premise** represents what is believed or treated as the state of the world, such as a quantity, status, date, or organisational relation. A **value premise** expresses what is preferred or acceptable, such as a target, priority, permissible range, or definition of a satisfactory outcome.

The distinction is analytically useful but not always clean in practice. Classifications and calculation rules can incorporate evaluative choices. Coding should therefore identify the documented operation and avoid claiming philosophical purity for either category.

Loasby (2002) extends the premise concept beyond an individual act of choice. Under **Knightian uncertainty**, where relevant possibilities or probabilities cannot be specified fully in advance, cognitive limits and dispersed knowledge make the formation and coordination of premises an institutional problem. Institutions frame decision spaces and facilitate knowledge sharing. Formal organisations can also invest in decision systems suited to their particular activities.

This strengthens the project's interpretation of enterprise architecture as a possible infrastructure for stabilising premises. It does not mean that every stored datum is a decision premise. A datum, category, or rule must have a documented relationship to a choice, constraint, or programmed response.

## 3. Programmes, recurrent choice, and routines

Premises shape individual choices. **Programmes** go further by structuring responses to situations that recur. March and Simon describe programmes as responses available for recognised, recurrent situations. A programme reduces the need for fresh search and deliberation by specifying what deserves attention and how the organisation should respond.

Programmed activity is especially relevant to enterprise software. Standard flows, rule sets, derivations, posting logic, and prescribed responses to recognised states can all represent programmes.

Several distinctions are required:

| Construct | Meaning for this study | Documentary indicator | Claim boundary |
|---|---|---|---|
| Programme | Prestructured basis for responding to a recognised situation | decision table, rule sequence, prescribed path | does not prove enactment or appropriateness |
| Rule | Condition linked to an action, result, or constraint | validation, threshold, routing condition | may constrain rather than decide |
| Procedure | Normative sequence for carrying out work | process step, instruction, workflow | documented procedure is not performed routine |
| Routine | Recurrent organisational pattern, including ostensive and performative dimensions | architecture may represent an artefact or ostensive account | cannot be inferred fully from reference documentation |
| Automation | Machine execution of an operation | automatic posting, derivation, routing | execution may implement an earlier human or organisational decision |

The key analytical question is therefore not simply whether deliberation has disappeared, but where it has gone. Automation may remove a transaction-time choice while relocating discretion to configuration, rule design, master-data governance, exception policy, or vendor product design.

## 4. Authority, acceptance, and permission

Programmes still require an account of who may define, apply, or depart from them. Simon treats **authority** as a relationship in which a subordinate accepts a communicated decision as a premise for action. Formal position matters, but authority cannot be reduced to an organisational chart or technical entitlement. Simon's later comparison of organisations and markets also emphasises authority, identification, and coordination as mechanisms that cannot be reduced to market exchange.

For documentary coding, four concepts must remain separate:

| Concept | Defensible documentary observation | What cannot be inferred |
|---|---|---|
| Permission | a role or user category is technically able to perform an operation | legitimacy, acceptance, competence, or actual exercise |
| Responsibility | a role is assigned work or ownership | authority to determine premises or outcomes |
| Approval authority | a role is allocated an accept, reject, or release opportunity | substantive review, hierarchical superiority, or accepted authority |
| Accountability | an actor is answerable and consequences attach to conduct | cannot be established from logging or traceability alone |

An approval workflow may allocate a decision opportunity and prevent progression without a recorded outcome. It does not necessarily identify line authority, the quality of review, the influence of informal expertise, or the acceptance of the approver’s premise. The project should use “encoded approval right” or “allocated decision opportunity” unless stronger evidence is available.

Aghion and Tirole (1997) approach the issue from a different theoretical tradition. They distinguish **formal authority**, the right to decide, from **real authority**, effective control over a decision. Their principal-agent model is not equivalent to Simon's acceptance-based account, so the concepts should not be collapsed.

The two accounts nevertheless reinforce a common warning for this project. A formally allocated software right does not demonstrate either acceptance or effective influence over the decision.

Winkler and Brown (2013) bring the distinction closer to information systems. At the application-governance level, they distinguish **decision control rights**, treated as decision authority, from **decision management rights**, treated as task responsibility. Their study does not concern transaction-level ERP processing, so it cannot be transferred directly. It nevertheless prevents an important coding error: responsibility for preparing, maintaining, or executing a decision process does not necessarily imply authority over its premises or outcome.

## 5. Discretion and its relocation

Authority concerns whose direction can guide action. **Discretion** concerns the recognised range within which an actor may choose among alternatives or interpret how a rule applies. Software can restrict discretion by eliminating options, requiring data, enforcing thresholds, or routing cases automatically. It can also create bounded discretion through configuration choices, tolerances, substitution rules, override rights, and exception handling.

Bovens and Zouridis (2002) provide an important bridge to digital administration. They describe a movement from **street-level bureaucracy**, where front-line officials exercise significant judgement, to **system-level bureaucracy**, where information technology shifts some of that judgement toward system analysts and software designers.

Their setting is public administration rather than ERP, and its constitutional concerns cannot be transferred wholesale. The narrower transferable proposition is that automation can relocate discretion upstream to those who specify systems rather than simply eliminate it.

For SAP reference architecture, possible locations of discretion include:

1. product design, where vendor-defined categories and supported alternatives are created;
2. implementation and configuration, where organisations select scope and parameters;
3. master-data and rule governance, where premises are maintained;
4. transaction processing, where users select among available actions;
5. exception processing, where normal programmes no longer resolve the case.

Documentary evidence can identify supported choice locations. Determining who controls them in a customer organisation requires implementation evidence.

## 6. Decision, action, calculation, recommendation, and automation

Once premises, authority, and discretion have been separated, the analysis can distinguish a decision from other consequential operations. The codebook must not classify every system operation as a decision. A defensible classification sequence is:

1. **Are organisationally meaningful alternatives represented?** If not, record an action, calculation, or state transition rather than a decision.
2. **Is a selection criterion or premise represented?** If yes, record it separately from the resulting action.
3. **Who or what selects or executes?** Distinguish human selection, configured rule execution, algorithmic recommendation, and automatic action.
4. **Can the result be overridden?** Record the documented override and its scope, not assumed discretion.
5. **What happens outside the recognised programme?** Identify block, exception, escalation, or manual review.

This yields several disciplined distinctions:

- A calculation produces a value according to a specified method; it need not select among organisational alternatives.
- A recommendation shapes attention or preference while leaving selection elsewhere.
- A default preselects an option but remains distinct from a mandatory value if it is genuinely overridable.
- An approval can be a substantive selection, a procedural gate, or an acknowledgement.
- Automated execution can carry out a decision programme whose premises were established earlier.
- Machine learning or optimisation should be coded only where the artefact documents those operations, not inferred from generic automation language.

## 7. Decisions as legitimacy and symbol

Decision processes can perform symbolic and political work in addition to selecting actions. Brunsson (1990) argues that decisions can allocate responsibility and produce legitimation. Other organisational decision research shows that decisions, actions, and outcomes may be **loosely coupled**, meaning that a formal decision does not necessarily determine the action or outcome associated with it.

This corrects a purely instrumental reading of approvals and records.

For enterprise software, a recorded approval may support traceability, demonstrate procedural conformity, allocate formal responsibility, or legitimise action. These are rival interpretations, not automatic consequences. A log records that an event occurred in the system; accountability additionally requires an answerability relation and possible consequences. A formal decision trace does not demonstrate that the recorded decision caused the eventual organisational outcome.

## 8. Proposed documentary coding framework

| Proposed code | Inclusion rule | Exclusion rule | Common false inference |
|---|---|---|---|
| DECISION_OPPORTUNITY | documented point at which alternatives can be selected | automatic transition with no represented alternative | opportunity equals exercised choice |
| DECISION_PREMISE | fact, value, rule, category, objective, or expectation used to structure choice | information with no documented decision relevance | presence equals acceptance |
| ALTERNATIVE_SET | documented available outcomes or actions | examples not presented as available options | list is exhaustive in practice |
| DECISION_CRITERION | condition used to evaluate or select an alternative | descriptive attribute with no evaluative operation | criterion is legitimate or sufficient |
| PROGRAMME | recognised situation linked to a prestructured response | recurrent activity without a documented response structure | programme equals enacted routine |
| DEFAULT | preselected but documented as changeable | mandatory value or automatic derivation with no override | default is neutral |
| THRESHOLD | boundary that changes routing, permission, or outcome | reporting target with no operative consequence | threshold itself made the decision |
| APPROVAL | accept, reject, release, or return operation that gates progression | acknowledgement or notification | approval proves substantive judgement |
| PERMISSION | technical entitlement to view or act | responsibility or authority inferred from a role name | permission equals authority |
| OVERRIDE | supported departure from a default, rule, block, or derived value | undocumented workaround | availability equals use or legitimacy |
| AUTOMATED_ACTION | system executes an operation without transaction-time human selection | recommendation awaiting selection | automation eliminates discretion everywhere |
| EXCEPTION_JUDGEMENT | documented manual or alternative handling after normal programming is insufficient | ordinary branch within the standard programme | exception handler has unrestricted discretion |
| TRACEABILITY | system records actor, time, state, or prior operation | accountability without a documented answerability relation | trace equals accountability |

These are proposed refinements. They must be reconciled with the existing descriptive codes during the codebook pilot rather than added wholesale.

## 9. Propositions for empirical analysis

The literature supports bounded propositions, not findings:

- Mandatory data, classifications, and thresholds may distribute decision premises even where transaction-level choice remains decentralised.
- Workflow roles may allocate decision opportunities without establishing actual organisational authority.
- Automatic processing may relocate discretion from transaction users to configuration, rule maintenance, or product design.
- Exception structures may reveal where the architecture assumes programmed decision-making becomes insufficient.
- Shared programmes may centralise premises without centralising execution of every transaction.
- Defaults may shape bounded choice while preserving a documented override.
- Audit records may strengthen traceability without establishing accountability or causal responsibility.

Each proposition requires an explicit rival interpretation. A threshold may protect data integrity rather than allocate organisational judgement. A role may exist for licence packaging rather than authority. An approval may document compliance rather than deliberate choice. An exception path may handle technical failure rather than organisational novelty.

## 10. Relationship with other streams

Decision theory overlaps with but is not reducible to the other streams:

- Organisation design asks how differentiated work and information capacity are arranged. Decision theory asks how choice is bounded and premises distributed.
- Coordination theory asks how dependencies are managed. A decision rule may coordinate dependent activity, but its decision operation should be identified separately.
- Governance concerns legitimate decision rights and accountability. Decision theory explains premises and authority but does not make a technical permission legitimate.
- Control theory asks how behaviour or outcomes are monitored and aligned. A threshold may be both a decision premise and a control mechanism.
- Routines research distinguishes represented programmes and artefacts from recurrent performances.
- Sociomaterial research explains why encoded possibilities become consequential only through situated relations between people and material arrangements.

Joseph and Gaba (2020) provide a direct bridge between organisation design and decision theory. Their **aggregation perspective** examines how structure combines information and choices. Their **constraint perspective** examines how structure restricts behaviour and the available field of choice. They also identify informational conflict and uneven attention to different stages of decision-making as gaps in the literature.

For this project, the distinction suggests two complementary questions. How does enterprise architecture aggregate information and approvals? How does it limit alternatives, visibility, and local discretion?

Gosain (2004) then supplies an enterprise-systems and institutional boundary. Enterprise information systems can be shaped by institutional forces while also carrying institutional commitments. These commitments may constrain action and make historically produced organisational choices appear natural or self-evident.

This does not establish that SAP users accept the encoded premises. It supports examining whether reference categories and process structures preserve particular rules of rationality. Routines and sociomaterial research remain necessary for studying enactment and resistance.

## 11. Synthesis and contribution

Decision theory sharpens the project’s claim about enterprise software. Reference architecture can be analysed as a distribution of decision premises and programmed action: it defines categories, required facts, recognised alternatives, criteria, thresholds, permissions, defaults, approvals, automatic operations, and exception routes. This can reveal where the architecture locates possible choice and where it closes choice down.

The claim must remain architectural. Documentation does not establish that participants accept formal authority, exercise available discretion, make considered judgements, bear accountability, or achieve effective outcomes. The project’s contribution is therefore to reconstruct **encoded decision design** and to specify the additional evidence required to study implemented and enacted organisational decision-making.

## References used in this stream

Aghion and Tirole (1997); Barnard (1938); Bovens and Zouridis (2002); Brunsson (1990); Cohen, March, and Olsen (1972); Cyert and March (1963); Feldman and March (1981); Gosain (2004); Joseph and Gaba (2020); Loasby (2002); March and Simon (1958/1993); Puranam et al. (2015); Simon (1947/1997, 1955, 1973, 1976, 1979, 1991); Winkler and Brown (2013). Full records and edition-verification notes are maintained in `../references/references.bib`.

## Glossary for teaching and review

| Term | Working meaning in this project |
|---|---|
| Bounded rationality | Choice under limits of information, attention, time, and computational capacity |
| Satisficing | Searching until an acceptable option is found rather than proving a global optimum |
| Decision premise | An assumption, fact, value, goal, category, or rule that guides choice |
| Programme | A structured response to a recurring situation |
| Formal authority | The recognised right or permission to decide |
| Real authority | Effective control over a decision, often supported by information or initiative |
| Zone of acceptance | The range within which a person accepts another's direction |
| Discretion | Legitimate room to exercise judgement among possible actions |
| Discretion relocation | Movement of judgement to designers, configurators, data owners, or exception handlers |
| Attention structure | An arrangement that influences which issues and information receive notice |
| Exception | A case that cannot or should not follow the normal programme |
| Encoded decision design | The project's term for decision premises and programmed actions represented in architecture |
