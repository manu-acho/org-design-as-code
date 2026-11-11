# Coordination and Interdependence: What does the next task need?

**Module 4 · Postgraduate · Student lesson · Draft for review**

**Study route:** Part I is for Week 5 and Part II for Week 6. [Module 3](../03_Organisation_Design/01_Student_Lesson.md) explained how work is divided and brought back together. This lesson makes a statement such as “Sales and Logistics need to coordinate” specific enough to check. **Interdependence** means that what one activity can do depends on work or resources beyond that activity. For example, dispatch needs quantities from picking, while two shipments may need the same loading bay.

## Part I. Identify the dependency before choosing a mechanism

### Begin with a delivery that cannot wait

**Illustrative scenario.** A customer needs 100 units by Friday. Sales has recorded the request. The shipping team needs to know which order to fulfil, which items are available, and when the vehicle can leave. Another shipment needs the same loading slot. The customer also needs to accept a partial delivery if the full quantity cannot arrive. All of these are coordination problems, but they are not the same problem.

The order and its items can help identify the work. They cannot allocate the loading slot unless the design does something to resolve the competing demands. A schedule may reserve the slot, but it does not answer whether the customer accepts a partial shipment. That requires a different decision and potentially a different actor. Describing all of these as integration conceals what each team needs from the others.

**Three questions inside one shipment**

```text
Sales records the order ──────→ Shipping needs to identify the work.
Two shipments need one bay ───→ Someone or some rule allocates the slot.
Full shipment is not possible → A decision is needed on the partial delivery.
```

Malone and Crowston (1994) treat coordination as the management of dependencies among activities. A **dependency** is a relationship that matters to performing the work, such as two shipments needing the same loading slot. A **mechanism** is an arrangement for managing it: in this case a schedule might reserve the slot. A rule, queue, record, role or interaction can also act as a mechanism. The distinction changes the order of analysis. What do the activities need from one another or in common? Only then does it make sense to ask how the arrangement addresses it. [Malone and Crowston](https://crowston.syr.edu/sites/default/files/acmcs94.pdf)

### Pooled, sequential and reciprocal interdependence

Thompson's classic distinction helps describe the **shape** of the relationship. In **pooled interdependence**, activities make separate contributions to a common whole or rely on a common pool without necessarily passing work directly between them. In **sequential interdependence**, one activity depends on an output or state produced by another. In **reciprocal interdependence**, the activities depend on one another's outputs or adjustments in both directions. These are ways of describing relationships, not labels for software features. See the [shared coordination review](../../../literature/Stream_02_Coordination_Theory_Detailed_Review.md#2-different-dependencies-require-different-responses) for the fuller treatment and source limits.

**Illustrative comparison: look for what is shared or passed**

```text
POOLED        Site A ──┐       Both contribute to a consolidated stock picture.
              Site B ──┴→ Pool Neither uses the other site's report directly.

SEQUENTIAL    Picked quantities → Dispatch prepares the shipment.
              Dispatch relies on a specified output of picking.

RECIPROCAL    Sales revises the delivery proposal ⇄ Logistics revises the plan.
              Each can need the other's updated contribution to continue.
```

Do not infer pooled dependence from use of the same application. Ask what shared pool or common result actually links the activities. Do not infer sequential dependence from chronology alone. Ask what the later task receives, selects or requires. Do not infer reciprocal dependence from a backward arrow. Ask which contributions are mutually contingent, and whether the source actually describes them. A prescribed return can have a clear purpose without documenting negotiation.

An entire process does not have to fit one label. Imagine two branches that independently report into one inventory position, then use that position to agree which can ship. Reporting contributes to the pool. The release decision depends on a resulting state. Resolving a conflict may involve reciprocal adjustments. Use the smallest relationship that explains the issue. Calling the whole process “reciprocal” would hide the differences.

### Use a second vocabulary to diagnose the coordination problem

Thompson's categories describe the pattern of dependence. Malone and Crowston help ask **what needs managing within that pattern**. One team produces information another consumes. Several teams need the same scarce resource. Separate outputs need to fit, or activities must be timed to coincide. Some work needs to reach an actor with the relevant responsibility or expertise. These questions are useful together, but do not force the two vocabularies into one-to-one correspondence.

| Problem to diagnose | Question to ask | A candidate mechanism |
|---|---|---|
| Flow or prerequisite | What prior output or state does the later work require? | A defined handoff or a stated precondition |
| Producer and consumer | What has to reach the next activity, when, and in what form? | A common record, output specification or notification |
| Shared resource | Which activities need the same limited resource? | A reservation, priority rule or allocation decision |
| Fit or synchronisation | Which outputs must be compatible, or which activities must align in time? | A reconciliation check, common specification or schedule |
| Task assignment or expertise | Who is expected to take the task, and what knowledge is needed? | A worklist, assignment rule or escalation to a specialist |

**Worked comparison.** The two shipments in the opening scenario could use a first-come allocation rule or a priority rule based on promised dates. Both mechanisms address the same scarce loading slot. They differ in the information required and in who can depart from the rule. First-come requires a usable arrival or booking sequence. A promised-date priority requires reliable commitments and a way to resolve ties or exceptions. If a manager allocates the slot instead, the dependency remains; the design locates more of the decision in a role rather than in a fixed rule.

```text
Two shipments → Need the same slot → Choose an allocation mechanism
                                      ├→ Queue: use booking sequence
                                      ├→ Priority: use agreed criteria
                                      └→ Named decision maker: weigh exceptions
```

None of these choices is shown to be best by the example. What matters for analysis is that the **dependency remains constant** while the mechanism, information needs and location of judgement change. Conversely, the same mechanism can address different dependencies. A schedule may allocate a bay to competing shipments, or it may synchronise a pick-up with loading. Ask what relation the schedule manages before calling it evidence of a particular kind of coordination.

### Check whether an input is actually usable

**Illustrative example.** Shipping sends Billing a quantity of 80. At first it looks as though the producer supplied what the consumer needed. Then Billing asks: 80 units picked, dispatched or received? The number arrived, but its meaning and the action it can support are still unclear. A producer-consumer relationship needs more than a transfer. Consider the object identity, timing, unit of measure, intended meaning, and whether the downstream actor can act on the value or correct it when necessary.

```text
Quantity sent → Quantity linked to the right item → Meaning established → Usable input
      A message can arrive without the later conditions being met.
```

**Week 5 practice.** Choose one arrow from the opening scenario. Rewrite it as: “Activity B depends on activity A for X, under condition Y.” Then propose a different mechanism for the same dependency. Identify one fact that would tell you whether the dependency exists in the documented procedure rather than in your interpretation of the drawing.

## Part II. Separate the mechanism from what it might achieve

### A workflow is a device, not a finding of coordination

Okhuysen and Bechky (2009) distinguish mechanisms such as plans and rules, representations, roles, routines and proximity from conditions those mechanisms can help create. **Accountability** here concerns whether responsibility for work is made apparent. **Predictability** concerns whether participants can anticipate what others will do. **Common understanding** concerns whether they have a sufficiently shared view of the work and how their contributions relate. These are not synonyms for coordination performance. This use of accountability is also narrower than a finding that an actor owes an account to a forum that can question and judge them, a distinction revisited in Module 8. [Okhuysen and Bechky](https://doi.org/10.5465/19416520903047533)

```text
Mechanism offered             Condition it may support        Further question
Role + task record        →   Accountability               →  Who takes responsibility?
Plan + schedule           →   Predictability               →  Can others plan on it?
Shared representation    →   Common understanding         →  Do meanings align?
                               None alone proves performance.
```

The middle column is where a good analysis becomes more careful. A role and an assignment may make responsibility visible without showing that anyone accepted it. A sequence can make a next step explicit without establishing that people can anticipate when it will happen. A shared status can offer a common reference without establishing agreement about what it means. These are testable propositions about how coordination might work, not findings implied by the design.

**Worked example.** Suppose a delivery board shows that an order is “ready”. Sales interprets that as “safe to promise”, Shipping as “eligible for picking”, and Billing as “not yet ready for invoicing”. This is an invented example. It illustrates why you would interview or observe the groups rather than infer shared meaning from a shared screen. If predictability is the issue, check whether participants can anticipate the next action and its timing. If the goal is fewer missed deliveries, define the outcome and gather evidence about delivery performance separately. A screenshot cannot do all three jobs.

### Documentary case: what the record actually does in BD9

**Verified documentary example, based on the registered Swiss case evidence.** The [BD9 evidence cards](../../cases/M04_BD9_Delivery_and_Billing.md) compare two separate procedures. In delivery creation, Shipping uses an earlier sales document and shipping criteria to select applicable items. The expected output is a delivery and a number in the delivery log. In the optional proof-of-delivery procedure, Shipping confirms and saves quantities, and the confirmed quantities are used in billing. Both examples connect earlier information to later work, but they do different jobs.

```text
A · Prior sales document + shipping criteria → Identify items for delivery creation
                                                  → Expected delivery in the log

B · Optional proof of delivery → Confirm and save quantities → Billing uses quantities

Independent reference examples. Not a trace of one transaction.
```

In A, the record and criteria help specify **which items** the later action concerns. The fact that the script expects a delivery number supports a claim about the represented document, not about goods physically reaching a customer. In B, the confirmed quantity is **a value the billing task uses**. This is evidence of a specific information dependency on the optional route, not of a universal billing prerequisite. Do not make B the next observed step after A just because the two are in the same scope item.

A plausible rival is that both references exist mainly because software needs identifiers and fields to function. That explanation is compatible with organisational significance. What makes the stronger interpretation defensible is not the existence of an identifier. It is the source's account of what each activity does with the information. A field displayed on a screen would not provide the same evidence.

| Analytical move | A: Delivery creation | B: Optional proof of delivery |
|---|---|---|
| Observe | Earlier sales document and shipping criteria are used in selection. | A confirmed quantity is used in billing. |
| Interpret | The reference helps delimit the work that can be selected for delivery creation. | A later task uses a value produced by earlier work on this route. |
| State the condition it might help | Participants could locate and prepare the appropriate delivery work more consistently. | Participants could use a more consistent quantity basis for billing. |
| Bound the claim | No observed fulfilment or proof of effective selection. | No proof of universal use, common understanding or effective billing. |

The third row contains hypotheses, not a result of the Swiss study. To examine the first, ask whether Shipping can reliably identify the right items across real cases. To examine the second, check whether people understand, trust and use the confirmed quantity, particularly when it differs from the shipped quantity. These questions need evidence beyond the reference procedures.

### Distinguish a formal return from situated adjustment

**Documentary contrast.** In Swiss J45, the documented purchasing-manager action can return a purchase order with a reason and instruct the creator to change it. The cited procedure does not show completion of the creator-side correction. In Swiss J58, a requester can check the rejection reason, edit a journal entry and resubmit it. That is evidence for a more complete formal return path in the cited procedures, not evidence that people negotiated or that a particular correction worked. These are separate cases and objects, not steps in one workflow. See the [public source locators](../../../figures/Table_07_Findings_Source_Locators.md) for J45-W07-11 and J58-W08-07.

```text
J45    Manager requests rework + reason → Creator instructed to edit
       The cited procedure stops before creator-side completion.

J58    Processor rejects + reason → Requester checks reason, edits and resubmits
       The cited procedure documents a return and resubmission path.
```

**Situated adjustment** is the work people do to make an arrangement function in a particular situation. Imagine that the purchasing manager's reason is “check the delivery date”, but the buyer has a supplier confirmation and the manager has a different production requirement. The rule can return the order. It cannot by itself establish how they resolve the conflict. They might settle it with a short conversation, ask Planning for an updated requirement, or reopen the supplier commitment. Each possibility requires different information. This scenario is illustrative; none of it is a finding from the two SAP examples.

Faraj and Xiao (2006) examine expertise and dialogue in a medical trauma centre. Their setting is not an ERP implementation, so the study does not tell us how SAP users behave. It gives us a useful question: when an exception cannot be resolved by a prescribed sequence alone, how does the organisation bring relevant expertise and different interpretations into the decision? A workflow can preserve a reason and create a route for action. A conversation can clarify what the reason means and what needs to change. The two mechanisms can coexist. An interview, observation or other appropriate record would be needed to learn how they were actually combined. [Faraj and Xiao, publisher abstract](https://doi.org/10.1287/mnsc.1060.0526)

### Worked comparison: investigate a breakdown without blaming the interface

**Illustrative scenario.** In a warehouse, Billing reports that partial deliveries repeatedly lead to invoice rework. The first proposal is to add an automated alert when a quantity changes. Before evaluating that proposal, identify the dependency. Which billing activity needs the quantity? Who is expected to confirm it? What is the difference between a new quantity and a correction to one already sent? If the wrong quantity is used, the breakdown could sit at several different points.

```text
Wrong quantity used for billing
        ├→ It never arrived: check the transmission or handoff.
        ├→ It arrived too late: check timing and the billing trigger.
        ├→ It meant something different: check interpretation and context.
        └→ It could not be corrected: check responsibility and ability to act.
```

An alert might help if the problem is attention. It might add noise if the information arrives on time but no one knows whether it means shipped or accepted. The right mechanism therefore depends on the rival explanations. A useful design discussion asks what evidence would discriminate among them. A message log can show when a value was sent. A case walkthrough can show which value a person used. Interviews or observation can clarify what the value meant to the teams. A comparison of invoice rework before and after a change would need a stable definition and comparable cases. It would still require care before attributing any improvement to the change alone.

Here we have moved from **architectural coherence** to a proposed investigation of work as performed. A reference path may specify a producer, an input and a consumer. Implementation evidence could show which path was selected and tested in a particular setting. Enactment evidence could show that people used it as intended, adapted it or relied on another channel. An analysis can stop at the first level and still be worthwhile, provided the wording stops there too.

### Transfer test: one mechanism, two different coordination problems

**Illustrative comparison.** Consider a hospital maintenance team using a queue. In one situation, the queue allocates a scarce technician between two jobs. In another, it delivers a fault report to the technician who knows the relevant equipment. The queue is visible in both. The first problem is allocation of limited capacity; the second is matching a task to expertise. A first-in rule could deal with one and be unsuitable for the other. Identify which claim would change if there were many technicians available but only one had the necessary knowledge.

An answer that names the underlying problem is stronger than “the queue coordinates both jobs”. It allows you to propose a mechanism and say why it fits the dependence. It also tells you what to inspect: priority criteria and waiting times in the first case; skill information, routing and access to advice in the second. The queue's existence alone tells us neither whether work is timely nor whether the right expertise was used.

### Check your understanding

1. Why does sharing an application not establish pooled interdependence?
2. What does a shipping-point filter show that a role assignment does not? What does it not show about who has permission?
3. Why are the BD9 delivery and billing examples two independent panels rather than one continuous process diagram?
4. What additional evidence would let you distinguish a documented rework path from actual mutual adjustment?
5. If an alert is added after a quantity change, identify the dependency it is meant to manage, one condition it might support, and a separate measure you would need to examine performance.

Then complete the [dependency, mechanism and condition exercise](../../exercises/M04_Map_Coordination.md). Bring one dependency and name what the next actor needs to know in time. [Module 5](../05_Information_Processing/README.md) asks whether the arrangement gives the actor usable information. [Module 6](../06_Knowledge_Boundaries/README.md) asks what happens when different groups give it different meanings.
