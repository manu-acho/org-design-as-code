# Stream Eight: Governance, Control, Accountability, and Decision Rights

## Scope and evidence boundary

This review separates four questions that enterprise-software analysis frequently collapses. Governance concerns the allocation and legitimation of rights. Decision-rights analysis concerns who is authorised to choose among alternatives. Control concerns attempts to direct conduct or outputs toward a standard. Accountability concerns a relationship in which an actor must explain or justify conduct to a forum that can judge and attach consequences.

The review draws on verified publisher records, complete accessible articles or manuscripts, and abstract-level evidence used only within its limits. A technical permission, workflow status, audit record, or approval step can provide evidence of a represented governance or control arrangement. It cannot by itself establish legitimate authority, exercised judgement, effective control, answerability, or accountability in practice.

## Part I: Learning guide

### 1. The practical problem

Enterprise systems contain many arrangements that appear to govern work: roles, authorisations, approval thresholds, blocks, validations, monitoring views, change histories, escalation paths, and reversals. It is tempting to call all of them “controls”. That vocabulary is too broad for analysis.

A required field can control data entry without allocating decision authority. An approval task can route a decision without showing that the assigned actor has accepted or legitimate authority. A change log can support traceability without creating any obligation to explain conduct. A dashboard can make deviation visible without producing intervention or consequence.

The central discipline is therefore:

> Identify separately the right, the standard, the observation, the judgement, the intervention, the answerability relation, and the consequence.

Only then should the arrangement be classified as governance, control, accountability, or some combination.

### 2. Concepts to master

#### Governance

Governance allocates and constrains legitimate rights to decide, act, monitor, change rules, and demand an account. It concerns the arrangement through which authority is constituted and exercised, not merely the technical ability to perform an action.

In enterprise software, governance may be represented through role design, organisational restrictions, workflow responsibility, configuration authority, release processes, segregation rules, and escalation structures. Documentary evidence establishes the formal representation. Legitimacy and practical authority require organisational evidence.

#### Decision rights

Jensen and Meckling (1992/1995) connect decision-right allocation with the distribution of knowledge. Specific knowledge can be costly to transfer, making it advantageous to move decision rights toward informed actors. Delegation also creates control costs where interests differ.

A decision right is therefore more than access. It concerns recognised authority to select among alternatives within a domain. Technical permission may be necessary for exercising that right, but it is neither sufficient nor always aligned with real authority.

#### Formal and real authority

Aghion and Tirole (1997) distinguish formal authority, the right to decide, from real authority, effective control over decisions. Real authority can depend on information, initiative, attention, and who develops the proposal that is likely to be accepted.

This distinction is decisive for workflow analysis. A manager may formally approve a purchase order while the substantive decision has already been shaped by rules, master data, requester choices, automated checks, and the information selected for review.

#### Organisational control

Ouchi (1979) begins from partially divergent objectives and the problem of cooperation. His framework differentiates market, bureaucratic, and clan mechanisms according to informational and social conditions. Eisenhardt (1985) develops the distinction between behaviour and outcome control, linking the choice to task programmability, measurability, information systems, and uncertainty.

Control should therefore be analysed as a relation among a controller, a controlled activity or output, a standard or objective, information about conduct or results, and some intervention or consequence. The presence of one component is not the complete control arrangement.

#### Accountability

Bovens (2007) defines accountability narrowly as a relationship between an actor and a forum. The actor is obliged to explain and justify conduct; the forum can question and judge; and consequences may follow. Lindberg (2013) similarly identifies an accountable agent, a domain, a principal or forum, rights to require information and justification, and sanctioning capacity.

Accountability is not synonymous with responsibility, transparency, traceability, liability, responsiveness, or control. These may support an accountability relation, but none establishes the whole relation alone.

#### Discretion

Discretion is the bounded space within which an actor may choose among permissible alternatives. Rules can reduce, relocate, or reshape discretion. They rarely eliminate it altogether. Bovens and Zouridis (2002) show how information and communication technologies can shift discretion from street-level officials toward system designers and system-level bureaucracies.

Enterprise automation may therefore move judgement into rule design, data classification, exception handling, monitoring, or override rather than simply remove human decision making.

### 3. Reading route

1. Read Ouchi (1979) for the organisational problem of control and the conditions supporting different mechanisms.
2. Read Eisenhardt (1985) for behaviour and outcome control under variation in task programmability, information, measurement cost, and uncertainty.
3. Read Kirsch (1996, 1997) for formal and informal control portfolios in information-systems work.
4. Read Jensen and Meckling (1992/1995) for knowledge and decision-right allocation.
5. Read Aghion and Tirole (1997) for formal and real authority.
6. Read Bovens (2007) and Lindberg (2013) for the components and limits of accountability.
7. Read Bovens and Zouridis (2002) for the redistribution of discretion through information systems.

### Study pause: dissect an approval

For one approval step, identify:

1. who may initiate it;
2. who is technically eligible to receive it;
3. who formally holds the decision right;
4. which information and premises shape the decision;
5. which conditions trigger, bypass, or terminate review;
6. what happens after approval, rejection, expiry, or rework;
7. who can override or change the rule;
8. who must later explain the decision, to whom, and with what consequence.

If the artefact shows only routing and status, do not call the complete arrangement accountable.

## Part II: Readable scholarly synthesis

### 4. Control begins with divergent objectives and limited information

Ouchi (1979) frames control as part of the organisational problem of obtaining cooperation among actors whose objectives are only partly congruent. Control arrangements depend on whether outputs can be measured, whether the transformation process is understood, and whether shared norms can support cooperation.

This framework prevents the assumption that more rules always produce better control. Behaviour control requires enough knowledge of desirable conduct to specify and observe it. Outcome control requires outputs that can be defined and measured. Clan or social control depends on processes of selection, socialisation, and shared understanding.

Enterprise systems can strengthen behaviour and output visibility by formalising steps, statuses, data requirements, and measures. They may also create false confidence where the recorded proxy is incomplete, the transformation is poorly understood, or actors orient toward the measure rather than the underlying objective.

### 5. Task conditions shape the choice of control

Eisenhardt (1985) integrates organisation theory with agency reasoning. Her empirical study links programmed tasks with behaviour-based control and associates less programmed tasks with outcome control or more elaborate information requirements. Measurement cost and uncertainty also matter.

The implication is not that an enterprise workflow should be labelled behaviour control whenever it contains prescribed steps. The analysis must establish what is monitored, how compliance is compared with a standard, and what follows. Likewise, a performance dashboard is not outcome control merely because it displays an indicator. The indicator must enter an arrangement of evaluation and consequence.

### 6. Control operates through portfolios

Kirsch (1996, 1997) extends control research into information-systems work. Behaviour, outcome, clan, and self-control can coexist. Stakeholders construct portfolios of overlapping and sometimes redundant mechanisms, with choices influenced by task characteristics, knowledge, role expectations, and available skills.

This portfolio view is well suited to enterprise software. One process may combine mandatory fields, workflow approvals, exception reports, performance targets, professional judgement, peer review, and self-monitoring. Coding each mechanism separately preserves the possibility that their combination is complementary, contradictory, or excessive.

### 7. Decision rights should follow knowledge, but delegation creates another problem

Jensen and Meckling argue that transferring knowledge and transferring decision rights are alternative organisational responses. Where relevant knowledge is specific and costly to move, decentralising rights may improve the use of knowledge. Yet decentralisation also increases the need for performance measurement and incentives because the actor's interests may not fully align with organisational objectives.

Enterprise software can alter both sides of this relation. Shared data and analytics can reduce some information-transfer costs. Standard rules can move premises to distributed actors. Workflow can route a decision toward a specialist. At the same time, central configuration can relocate decision authority upward or toward process owners and designers.

The resulting arrangement should be reconstructed empirically. A centralised technical rule may support decentralised execution, while a locally initiated transaction may remain tightly governed by central categories and thresholds.

### 8. Formal authority is not real authority

Aghion and Tirole's distinction explains why an organisational chart or workflow role cannot settle where effective judgement resides. An actor may hold the formal right to approve but lack the information, time, or initiative needed to shape the choice. Another actor may exercise real authority by developing the proposal and controlling the information on which approval relies.

In enterprise processes, real authority may be influenced by master-data specialists, configuration experts, requesters, automated decision rules, exception handlers, or analysts who frame the available options. This does not mean that formal approval is irrelevant. It means that a complete account must trace the production of decision premises as well as the final status change.

### 9. Accountability requires a relationship, not merely a record

Bovens (2007) provides a demanding test. There must be an identifiable actor and forum, an obligation to inform and justify, an opportunity for questioning and judgement, and possible consequences. Lindberg (2013) similarly preserves a domain of conduct and rights held by the principal or forum.

An audit trail can help identify actions and supply evidence. It does not itself ask questions, judge reasons, or impose consequences. A workflow history may support accountability when embedded in an organisational or legal forum, but traceability alone should be coded as an information mechanism.

This separation is crucial for enterprise software as organisation design. The architecture can represent the evidence infrastructure of accountability without representing the entire accountability institution.

### 10. Digital systems redistribute discretion

Bovens and Zouridis (2002) distinguish street-level, screen-level, and system-level bureaucracy. As decision rules become embedded in systems, some discretion can move away from front-line interaction toward those who design, maintain, and govern the system.

The same logic applies cautiously to enterprise software. A validation may remove one user's option while creating interpretive work for the person who classifies the exception. Automated routing may reduce local choice while increasing the importance of workflow conditions and role assignment. Standardisation may therefore redistribute discretion across time and organisational level.

The documentary study can identify where discretion appears to be represented, constrained, or relocated. It cannot establish how actors experience or exercise that discretion without field evidence.

## Part III: Complete technical expansion

### 11. Analytical distinctions

| Concept | Required elements | What is insufficient |
|---|---|---|
| Access right | Actor, resource or action, permission and scope | App assignment without effective restriction analysis |
| Decision right | Recognised authority, decision domain and alternatives | Technical ability to change a status |
| Control | Standard or objective, observation, comparison, controller or control logic, intervention or consequence | A rule, report, or metric in isolation |
| Accountability | Actor, domain, forum, obligation to explain, questioning, judgement and possible consequence | Traceability, transparency, responsibility label, or audit log alone |
| Segregation of duties | Incompatible activities, separation rule, assignment or transaction check, and response to conflict | Two differently named roles |
| Discretion | Actor, domain, available alternatives, constraints and override or escalation conditions | Absence of a documented rule |

### 12. Control-mechanism coding questions

For each candidate control, record:

1. the conduct, state, or output being controlled;
2. the standard, threshold, rule, plan, or expected state;
3. the information used to observe it;
4. whether comparison is automatic or performed by an actor;
5. the intervention, block, approval, escalation, correction, reward, or sanction;
6. the actor or logic authorised to intervene;
7. override and exception arrangements;
8. evidence of configuration and use; and
9. the possibility that the mechanism serves coordination or information rather than control.

### 13. Accountability coding questions

Do not code accountability unless the evidence identifies, or explicitly leaves open, the following:

- accountable actor or office;
- domain of conduct;
- forum or principal;
- obligation to provide information and reasons;
- capacity to question;
- capacity to judge;
- possible consequence; and
- basis of legitimacy.

Where only records and attribution are visible, code traceability or accountability support rather than accountability achieved.

### 14. Cross-stream boundaries

**Coordination:** An approval can coordinate sequential work, but control analysis asks which standard is enforced and governance analysis asks who may decide.

**Decision theory:** Stream Three explains premises, programmes, attention, and bounded rationality. Stream Eight adds legitimate rights, monitoring, judgement, and consequence.

**Infrastructure:** Stream Seven identifies standards and control points. Stream Eight asks who legitimately controls those points and who answers for their use.

**Routines and materiality:** Formal controls may be interpreted, combined, bypassed, or repaired in practice. Documentary control architecture is not evidence of effective control.

**Business-process management:** Process diagrams can locate approval and review steps, but they often omit legitimacy, informal control, sanction, and accountability forums.

### 15. Prohibited inferences

- Technical access is not legitimate authority.
- Formal authority is not necessarily real authority.
- Approval is not automatically accountability.
- Traceability is not answerability.
- A dashboard is not control without comparison and intervention.
- A validation is not proof of compliance.
- Two role templates do not prove segregation of duties.
- Automation does not eliminate discretion.
- A recorded user is not necessarily the organisational decision maker.
- An exception path does not establish that exceptions are handled effectively.
- Control presence does not prove control effectiveness or legitimacy.

### 16. Strongest defensible contribution

Stream Eight provides a disciplined way to reconstruct formal governance and control architecture without mistaking software capability for organisational accomplishment. It makes approvals, permissions, restrictions, validations, monitoring, escalation, override, audit, and configuration authority analytically comparable while preserving their differences.

For the documentary study, the strongest claim concerns represented allocations of access, decision processing, standards, observation, intervention, and accountability support. Claims about accepted authority, exercised judgement, answerability, legitimacy, compliance, and effective control require implementation and field evidence.

## Part IV: Audit conclusion

The verified literature supports six conclusions.

1. Control mechanisms depend on task knowledge, measurability, information, uncertainty, and social conditions.
2. Organisations commonly combine formal and informal controls rather than relying on one pure mode.
3. Decision-right allocation concerns the location of knowledge as well as incentive and control costs.
4. Formal and real authority can diverge.
5. Accountability requires explanation, questioning, judgement, and possible consequence, not merely a trace.
6. Enterprise software can redistribute discretion and provide control architecture without establishing effective or legitimate governance in practice.
