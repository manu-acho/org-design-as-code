# Organisation Design: Dividing work and bringing it back together

**Module 3 · Postgraduate · Student lesson · Draft for review**

**Study route:** Part I is for Week 3 and Part II for Week 4. Bring the bounded map from [Module 2](../02_End_to_End_Processes/01_Student_Lesson.md) to examine what changes when the same work is divided or assigned differently. No SAP configuration knowledge is needed. The [reading pack](../../reading-packs/M03_Organisation_Design.md) refreshes activities, roles, records and boundaries.

## Part I. Why dividing work creates a design problem

### Begin with the invoice, not the organisation chart

**Illustrative example.** A manufacturer needs to pay a supplier. Purchasing agreed the quantities and prices. Receiving knows what arrived. Accounts Payable has the invoice and has to decide how to record it under the applicable procedure. Each function knows something the others may need. Dividing work makes specialisation possible; it also creates the problem of connecting those contributions.

That is the starting point for organisation design. **Differentiation** is the division of collective work into tasks, roles or units. **Integration** is the work of bringing those contributions together so they serve a common purpose. An organisation chart may show that Purchasing and Accounts Payable are separate units. It does not show which purchasing facts Accounts Payable can use, how an error is returned, or who can decide what to do if a reference is missing. The design includes those arrangements too.

**Illustrative transfer.** A university can separate the academic decision to admit a student from the administration of enrolment. That is differentiation. The registrar needs a reliable record of the admission decision and its conditions to enrol the student. Providing that record and a way to resolve missing information is integration. The two activities can remain distinct even when they share an application.

**Division and integration in the illustrative invoice example**

```text
DIVIDE THE WORK                         RECONNECT THE CONTRIBUTIONS
Purchasing  → records agreed terms ────┐
Receiving   → records receipt ─────────┼→ Facts available to invoice review
Supplier    → submits the invoice ─────┘          ↓
                                     Accounts Payable checks and records
```

The arrows show possible information links in an invented example. They do not assert that all three inputs are mandatory in a SAP procedure. That is a question for evidence, and the second half of the lesson will give you a counterexample.

### Separate the task from its allocation

It matters whether a design changes **what must be done** or **who does it**. Checking a quantity and approving a discrepancy are two different tasks. Giving both to one role changes task allocation; combining them into a single operation changes how the work is divided. Puranam, Alexy and Reitzig (2014) distinguish task division and allocation from information provision and reward provision. Their distinction gives us four questions to ask about a design, even if the evidence only answers some of them. A reference procedure might identify a task and its role without saying anything about the person's incentives or how their performance is evaluated. [Puranam, Alexy and Reitzig](https://doi.org/10.5465/amr.2011.0436)

Burton and Obel (2018) focus on the fit between structure and coordination. Their starting point is not whether a particular division of work is good by itself, but whether the way the parts are connected suits how the work has been divided. Apply that to the invoice. Allocating invoice entry to Accounts Payable does not remove its dependence on facts produced elsewhere. A design needs a way to supply, verify or replace those facts. The structure tells us who has a task; the coordination arrangement tells us how that task can draw on other work. [Burton and Obel](https://link.springer.com/article/10.1186/s41469-018-0029-2)

**Four questions about a design**

```text
Division     What tasks make up the collective work?
Allocation   Who is expected to perform each task?
Information  What does each actor need, and where does it come from?
Rewards      What motivates or reinforces the required contribution?

Reference procedure  → may describe tasks, actors and information
                     → does not by itself establish incentives in practice
```

### Worked comparison: changing who does the work is not changing the work

**Hypothetical scenario.** Two plants buy the same components. An invoice arrives for 100 units, but Receiving has recorded only 80. For this illustration, assume the organisation wants two things done: establish what happened to the other 20, and decide how to treat the invoice. It also wants the decision recorded so the next person can understand it.

In the first design, a plant buyer gathers the delivery facts and a central Accounts Payable reviewer decides how to handle the invoice. In the second, a central exception team gathers the facts, and the same type of reviewer still makes the decision. The work has been **reallocated**: the investigation moved. It has not been **redivided**: gathering facts and deciding what to do remain separate tasks. A third design could give the investigation and the decision to one role while keeping them as two distinct steps. That changes allocation too. The analytical question is not how many people are named, but where the boundaries between tasks and responsibilities sit.

**Keep the tasks constant; change the performer**

```text
Task                         Design A                  Design B
Establish the receipt facts  Plant buyer               Central exception team
Decide how to handle claim   AP reviewer               AP reviewer
Record the decision          AP reviewer               AP reviewer

What changes: who investigates.
What remains: a reviewer needs the investigation result before deciding.
```

Now imagine that the investigation itself is split. A receiving specialist checks what was recorded, while Purchasing checks whether the balance was agreed for a later delivery. That is a change in **division**, not just an assignment of the same investigation to someone else. It may give each part to someone closer to the evidence, but it creates a new integration task: somebody must bring together the receipt and purchasing accounts. If the two accounts disagree, the design must provide a way to handle that disagreement. A chart that only assigns responsibility does not answer that question.

The fourth question from Puranam and colleagues, reward provision, is useful here even if it cannot be answered from a process script. Suppose the investigation team is measured only on how quickly it closes a ticket, while the reviewer needs a well-supported explanation. Those measures *could* pull in different directions. That is a hypothetical design risk, not an inference from the fact that a ticket or a reviewer exists. To examine it, ask how staff are actually evaluated and what happens when speed and evidential quality conflict.

**Try it.** If management moves exception investigation from each plant to a central team, name one dependency that remains and one information problem the move might introduce. A defensible answer is that the reviewer still needs the investigation result, but the central team might need a way to ask local staff about a receipt it cannot inspect directly. The possible information problem follows from the arrangement; it is not an observed result.

### A handoff is a relationship, not just the next step

A **dependency** exists when one activity needs an output, resource, decision or state associated with another. Two steps can appear in that order on a diagram without the later one taking anything from the earlier one. To identify the relationship, ask what the later activity needs and how it receives it. In the opening illustration, Purchasing may create a record of agreed terms. If Accounts Payable uses that record, the design connects the two tasks through its content. If the record is only displayed for navigation, its role in the handoff is different.

A **coordination mechanism** is a way of managing a dependency, for example by standardising what a record contains, routing an exception, or making a decision available to the next actor. Identifying the mechanism is not the same as showing that coordination succeeded. A record can be available and still be incomplete, contested or misunderstood. Module 4 will distinguish forms of interdependence and mechanisms more precisely. Here, the goal is to name the tasks and describe what connects them.

**Diagnostic contrast**

```text
Chronology alone     A is listed before B. What, if anything, crosses?
Documented handoff   A produces information → B uses it for a specified task.
Observed outcome     Separate evidence is needed to show what actually happened.
```

### Worked comparison: same record, three different jobs

**Illustrative example.** An invoice reviewer sees a PO number in each of three invented designs. In the first, the number is displayed beside the invoice, but the reviewer does not need to use it. In the second, the reviewer uses it to locate an order whose terms need correcting. In the third, entering the number brings ordered quantities into the invoice task. The field can look identical in all three designs. The organisational analysis changes when the field does different work.

```text
Visible number      → Earlier record can be inspected.
Selection reference → The order is identified as the target of a correction.
Operative reference → Earlier order values become inputs to invoice entry.
```

Ask what would stop, change or require another input if the number were missing. This is a question to put to the evidence, not a reason to assume that a system would fail. On the first design, the later task may proceed without the display. On the second, the correct target has to be found another way, if that is possible. On the third, the values must come from some other input if the route permits it. This is why we examine alternatives: they show whether the dependency belongs to a particular arrangement rather than to the business outcome in general.

**Week 3 practice.** Return to the illustrative manufacturer. Write one sentence naming the work divided between Purchasing and Accounts Payable, one naming a possible dependency, and one naming something you would need to verify before calling it a mandatory handoff. If you cannot name an input or consequence, you have described a sequence, not yet a dependency.

## Part II. Why a configuration matters more than a feature

### Fit is a question about relationships

A **configuration**, in the organisation-design sense used here, is a set of design choices considered together: tasks, roles, information, rules and ways of dealing with exceptions. Do not confuse it with **customer system configuration**, which is the particular arrangement selected and set up in an implementation. A software feature can contribute to several different organisational configurations, depending on what it acts on and how it connects to other operations.

**Contingency** means that the suitability of an arrangement depends on conditions, rather than on a universal best design. **Fit** concerns how well choices work together or suit those conditions. **Complementarity** is a more demanding idea: two choices reinforce each other's contribution under the conditions being considered. Two settings being present together is not evidence of complementarity. To argue that they reinforce each other, explain the connection and identify what evidence would support it.

**Hypothetical comparison.** Consider requiring an upstream reference on every invoice. Where suitable purchase records are available and maintained, a reference rule and reliable data could reinforce each other. Where an authorised transaction has no procurement record, the same rule could make legitimate work difficult unless another route is available. These are design hypotheses. The lesson has not measured data quality, delays or control outcomes.

**One rule, different supporting conditions**

```text
Require a purchasing reference
        ├→ Suitable reference exists → Inspect the referenced route and its checks
        └→ No suitable reference     → Inspect any authorised alternative or gap

Judge the rule together with data availability, responsibilities and exception paths.
```

**Equifinality** is the possibility that different arrangements can achieve a comparable result under stated conditions. The word *comparable* matters. Two routes can both reach a status called posted without producing identical accounting entries, risks, effort or organisational outcomes. The case lets us compare a shared *type* of documented result and different dependencies. It does not demonstrate equal performance.

### Worked comparison: fit is not the same as complementarity

**Hypothetical scenario.** Imagine two changes to invoice work. Change A is a rule that requires a PO reference for ordinary stock purchases. Change B is a stewardship routine in which named staff resolve incomplete or outdated order records before the invoice arrives. Each change has a purpose. The rule connects the invoice to an earlier purchasing record. Stewardship aims to make that record usable. The point of the example is to ask whether introducing either change makes the other more valuable, not to assume that two desirable practices automatically reinforce each other.

| | No stewardship routine | Stewardship routine in place |
|---|---|---|
| **No required reference** | Invoice entry can use other inputs under the assumed policy. | Order data may improve, but invoice entry does not necessarily use it. |
| **Required reference** | The link can be present while the linked data are incomplete. | The rule is more likely to expose usable upstream data, if stewardship works. |

The table suggests a **complementarity hypothesis**: stewardship may add more value to invoice work when that work actually uses the maintained record. To test it, define a result, such as the proportion of ordinary stock invoices whose reference supplies usable data, then examine how it varies across the arrangements. Keep legitimate no-reference cases separate. Otherwise a change in case mix can masquerade as improvement. No figures are asserted here; the table describes what a comparison would need to distinguish.

**Fit** poses a broader question. Even if the two choices reinforce one another for ordinary stock purchases, the design may be unsuitable for authorised expenses with no purchasing record. That is a contingency problem: the value of the arrangement changes with the kind of work it must accommodate. One design might retain a tightly scoped reference rule and a separately governed alternative. The design question is then what counts as an eligible exception, which checks apply, and who can act. There is no universal ranking unless the objective, conditions and evidence have been specified.

### Technical modularity does not guarantee independent work

**Technical modularity** concerns how system components are separated and connected through interfaces. **Organisational modularity** concerns how work is divided into units or activities that can operate with some independence. The boundaries need not coincide. Two software areas may share an object on which two groups rely, or separate applications may be tied together by a handoff that is organisationally demanding.

Ethiraj and Levinthal (2004) use simulation to examine design choices in complex systems. Their study helps explain why the question is not simply whether to break a system into more pieces. Decomposing a system can make local changes easier to explore; separating strongly interdependent parts can leave coordination problems unresolved. Their findings concern modelled conditions, not an evaluation of SAP or the performance of any team. The implication for our analysis is to ask which dependencies remain when a boundary is drawn. [Ethiraj and Levinthal](https://doi.org/10.1287/mnsc.1030.0145)

**Different boundaries in the illustrative invoice example**

```text
Technical question       What components and interfaces handle the data?
Organisational question  Who produces the data, who uses it, and who fixes errors?
                          ↓
Do not infer the second answer from the first.
```

### Transfer example: a different application does not remove a handoff

**Illustrative example, not SAP evidence.** A maintenance provider replaces its dispatch application but keeps its billing application. Billing still needs a record of the work completed at the customer site. The two applications are technically separate. The technicians and billing team are not thereby organisationally independent: one team's work still supplies evidence the other needs.

```text
Dispatch application  │  Interface: completed-work record  │ Billing application
                      │                                      │
Technician records ───┴──── work, date and completion ───────┴→ Billing uses record
                                       │
                                       └→ If incomplete, who corrects or confirms it?
```

Now consider the opposite arrangement. Both teams use one application, but the technician records completion under a separate responsibility and Billing can work only once it has the record. The technical boundary changed. The organisational dependency did not. To analyse either design, ask whether the information needed at the boundary is explicit, how often the work requires clarification, and who has to resolve an incomplete record. Those questions connect the technical interface to the organisation of work. They do not presume that tighter integration or more separation is always preferable.

### Worked example: two J45 invoice routes

**Verified documentary example, based on registered case evidence.** In the Swiss J45 procedure with a purchase-order reference, Accounts Payable enters an earlier PO and the procedure expects invoice items to be populated. The accountant still checks the invoice and posts under the documented conditions. In the separately documented optional procedure without a PO or goods receipt reference, the accountant supplies accounting inputs, including general ledger, cost-centre and tax details as applicable in the example. The route still includes consistency and tolerance checks before posting. See the [student case and exact source locators](../../cases/M03_J45_Invoice_Routes.md).

**Compare what each route takes as input**

```text
A · PO reference → Invoice items populated → Checks → Expected posting
B · Accounting inputs without PO/GR ref.  → Checks → Expected posting

Same broad result: a posted invoice.
Different dependency: what the later task takes from prior procurement work.
Separate reference examples, not two treatments of one observed invoice.
```

Here is the reasoning. First, the source describes different inputs. Second, the PO route shows an identifiable dependency: the earlier purchasing record supplies information used in a later task. Third, the alternative tests the scope of the claim. We cannot say that all invoices depend on a PO. We can say that this referenced route uses purchasing data and that the optional route obtains its inputs differently. One rival is that the PO reference is only a convenience. If it merely opened the right screen, that interpretation might be enough. The fact that it populates items is stronger evidence of a role in the later task. It still does not show that the route is faster, preferred, or more effective.

Notice what the feature label leaves out. Calling both routes invoice processing tells us little about which data the accountant needs to supply and what earlier work the system can reuse. Calling one route controlled and the other uncontrolled is also wrong: both represent checks. The useful unit of comparison is the arrangement of records, responsibilities and checks, not whether the application has a particular feature.

**From source step to bounded claim**

| Move | What to write for the J45 case |
|---|---|
| Describe | In the referenced route, entering the earlier PO populates items. In the no-reference route, the accountant supplies accounting inputs. |
| Interpret | One arrangement makes upstream purchasing data an input to later work. The other uses a different basis for recording the invoice. |
| Challenge | Could the PO number merely locate a record? Item population is the documentary detail that distinguishes an input from a simple lookup. |
| Bound | The alternative weakens a claim of universal PO dependence. It does not show that the two routes have identical consequences or that either works better in practice. |

An organisation-design argument works in both directions. It can explain the relationship without SAP labels: in one route, an activity relies on information previously produced by another; in the second, the later activity uses inputs supplied differently. It can also return to the evidence card and identify the step that justifies the interpretation. Without both moves, the analysis is either too abstract to check or too descriptive to explain the arrangement.

### Three questions that require different evidence

| Question | Meaning | Evidence you would look for |
|---|---|---|
| **Architectural coherence** | Do the represented inputs, activities and consequences fit together for the specified route? | Reference procedures, conditions and expected states, including alternatives. |
| **Implementation fit** | Does the selected and configured arrangement meet the needs and constraints of a particular organisation? | Requirements and decisions, configuration records, and relevant tests. |
| **Enacted fit** | How does that arrangement work with the practices through which people carry out and adapt the work? | Observed work, interviews and relevant transaction or exception traces. |

These are distinct questions, not three stages automatically demonstrated by a diagram. A coherent route can be a poor choice for a particular organisation. A configured design can also be used differently from how it was intended. The case supplies documentary evidence for a comparison of represented arrangements. It does not show whether a customer selected either route or whether either delivered better results.

### Worked comparison: three ways to investigate the same problem

**Hypothetical scenario.** A project team is concerned that invoices without a purchasing reference may be difficult to process. The same concern suggests three different investigations.

First, read the reference procedures. Is there a represented no-reference route, what does it require, and what is the expected result? That is an architectural question. It does not ask whether the organisation should select that route. Second, inspect a customer's requirements, design decision and test evidence. Did the project choose a route that covers the relevant categories of invoices and exceptions? That is an implementation-fit question. A successful test may support a narrow conclusion about the scenario tested. It does not tell us whether the scenario represents all everyday cases.

Third, observe how people handle invoices during work. They may use the selected route, ask colleagues to repair a record, defer the case, or handle an exception outside the visible workflow. These are possibilities, not observations about any customer. To find out which occurs, look for contemporaneous case traces and compare them with what staff say and do. That is an enacted-fit question. If the aim is to establish whether the arrangement improves payment timeliness or control, define the outcome and gather additional evidence rather than inferring it from any of these three levels alone.

### Check your understanding

1. What does an organisation chart leave unexplained in the opening example?
2. What would show that a reference supplies data rather than merely identifies or displays a record?
3. What remains comparable between the two J45 routes, and what must not be called equivalent?
4. A project says its new invoice design fits local work because the reference script posts successfully. Which of the three questions has it not answered, and what would you ask for?
5. A new team now performs an existing investigation. What additional change would make this a change in task division as well as allocation?
6. In the maintenance example, what would convince you that the teams no longer depend on one another for the same information?

Then complete the [two-route design exercise](../../exercises/M03_Compare_Invoice_Arrangements.md). Your task is not to choose a universal best design. It is to make the trade-off and the evidence boundary explicit.

Bring one supported handoff from your two-route comparison into [Module 4](../04_Coordination_and_Interdependence/README.md), where you will diagnose the kind of dependency it creates.
