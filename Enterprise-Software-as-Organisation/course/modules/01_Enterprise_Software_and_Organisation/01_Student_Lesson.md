# Enterprise Software and Organisation: What is being designed besides the software?

**Module 1 · Postgraduate · Week 1 · Student lesson draft**

The course begins with a question that applies to any business system: when people see different information or can take different actions, how does the system arrange their work? A shortage is one example of an **exception**, a situation that needs a different response from the usual one. SAP is the main documented case, not a prerequisite or the limit of the argument.

## 1. Start with six bottles of milk

**Fictional example.** A customer orders six bottles of milk for home delivery. A grocery employee finds only four on the shelf. The customer sees one order, but several groups have to act. Someone needs to pick the goods, someone may need to ask about a substitute, someone needs to know what will go on the vehicle, and someone needs to make sure the final bill reflects the agreed order.

Suppose the store has two possible policies. In the first, pickers may substitute an equivalent product within stated limits if the customer has opted in. In the second, a service team must contact the customer before any substitution. The same shortage triggers different work. The first policy needs reliable product equivalence and a usable record of consent. The second needs a **handoff**, the passing of work or information from one task to another. Here the picker sends the shortage to service, and service returns the customer's decision. This route also needs a deadline and a rule for no reply. If the vehicle is due to leave, the store must decide whether to wait, send four bottles or escalate the decision to someone who can resolve it. These are design options in the illustration, not facts about SAP or a real retailer.

```text
Order for six → Picker finds four → How should the shortage be handled?
    ├─ Design A: picker applies agreed limits and recorded consent
    └─ Design B: service team asks the customer and returns a decision
Both designs still need a way to inform dispatch and final billing.
```

Neither design is simply “more digital”. Each allocates responsibility, sets limits on decisions and creates different dependencies. In Design A, the picker needs trustworthy information at the point of work. In Design B, dispatch may depend on a response the service team cannot guarantee before the vehicle leaves. If you improve the screen without addressing those relationships, you may speed up a step without solving the coordination problem.

**First study pause.** Who can report what is physically available? Who can consent to the substitute? Who needs the outcome before acting? Those may be three different actors. The same screen does not make the answers the same.

## 2. What is an enterprise system?

**Enterprise software** supports work that matters across an organisation. **Enterprise resource planning (ERP)** is a class of systems that supports and connects core operations such as purchasing, sales, inventory and finance. SAP's [ERP overview](https://www.sap.com/resources/what-is-erp) offers the vendor's orientation to those functions. The point here is not that every organisation has one system or one perfectly consistent record. It is that data and actions in one part of the business can have consequences in another.

In this course, **SAP** is the vendor. **SAP S/4HANA Cloud Public Edition** is the particular product and deployment setting studied in the principal reference cases. A **scope item** is a named segment of reference business-process content, such as Sell from Stock (BD9). A **release** identifies a version context, and a **localisation** identifies country- or region-specific context. Product, release, scope item and localisation belong in the evidence note because similarly named procedures need not behave identically in every setting. No knowledge of SAP menus or certification is assumed.

A **business object** is a structured representation of something the organisation works with, such as a sales order or an invoice. **Master data** describe entities reused across transactions, such as a product or a customer. **Transaction records** describe particular business commitments, events or entries. The same product identifier might appear on hundreds of orders, but each order has its own quantities and conditions. A **role** describes a position in the work, such as shipping specialist. That is not the same as the individual occupying it, the individual's technical permissions or their authority to decide.

```text
Shared descriptions: customer, product, organisational unit
                              ↓ used by
Transaction records: order → delivery-related record → invoice
                              ↑ acted on by
People and system logic in defined roles, rules and states
```

The diagram is a generic illustration, not a universal document chain. **Data integration** is about how records are shared, linked or kept consistent. **Process integration** is about how work is connected, such as one activity providing the value the next needs or a decision allowing an action to proceed. Two teams can use the same product record without sharing the same workflow. Two systems can support one process if the handoff between them is reliable. Integration is therefore a question about the relationship, not simply a count of applications.

[Davenport (1998)](https://hbr.org/1998/07/putting-the-enterprise-into-the-enterprise-system) makes the organisational issue visible: a packaged system brings its own assumptions about how data and processes are connected. The possibility of integration is attractive; the proposed way of organising work may still conflict with local needs. This is a conceptual starting point, not a prediction that adopting a package produces a particular benefit.

## 3. Read architecture as an arrangement of work

Here, **reference architecture** means the arrangement of work that can be reconstructed from vendor documentation. A process description might say when a task moves to another team; a role description might identify who handles it; a procedure might specify the record the team receives. These documents are **reference artefacts**: individual pieces of evidence about the design, alongside definitions, rules and descriptions of states. No single artefact describes the entire arrangement. Read together, they show how the design represents division of work, coordination, information, authority and exceptions.

| What to look for | Question about the work | Grocery example |
|---|---|---|
| Tasks and roles | Who does what, and who is expected to take over? | The picker reports a shortage; service may contact the customer. |
| Records and states | What does the next task know, and which condition matters? | Dispatch needs the final quantities, not just the original order. |
| Rules and decision rights | What is permitted or required, and who can decide? | Recorded consent and limits determine whether the picker may substitute. |
| Exceptions and follow-up | What happens when the normal route does not resolve the case? | If the customer does not reply, someone must decide how to proceed. |

**Codified organisation design** is the idea that some of these arrangements can be represented in data, rules and system operations. It does not mean the software contains the entire organisation or writes the outcome in advance. A manual discussion, professional judgement or local workaround can matter even if it is invisible to the system. Conversely, a rule that prevents an action can materially constrain people even if the documentation does not describe their experience. Both the technical operation and the organisational relation deserve attention.

**Worked contrast.** Imagine the customer order number appears on a dispatch screen. It could do three different jobs: help someone recognise the order, select the shipment the next task concerns, or supply quantities for the next action. To tell which, look for evidence of use. A display is not a selection rule, and a selection criterion is not proof of an access restriction. An input that supplies a value is stronger evidence of a dependency than an adjacent field on a screen.

```text
Same order number on a screen
    ├─ Displayed → a person may use it to recognise the order
    ├─ Used to select → it helps identify which record or task to act on
    └─ Used to supply values → the later task takes information from the earlier record
```

The course calls an identifiable, reusable and consequential operation a **candidate software organisational primitive**. Examples to test include routing a task, restricting an action and carrying a confirmed value forward. “Sales application” is too broad; “green icon” is too weak without an effect; “confirmed quantity used for billing on this route” is specific enough to examine. A candidate becomes worth comparing when it can be located in evidence and its organisational consequence is clear. The term is a research tool, not a claim that every system has a universal set of building blocks. [Module 10](../10_Comparative_Process_Analysis/README.md) will test that distinction across cases.

## 4. Do not collapse design, implementation, practice and outcomes

Four kinds of evidence about the grocery substitution support four different kinds of statement.

| Level | Example evidence | Conclusion it can support |
|---|---|---|
| Encoded or represented design | A reference procedure shows a substitute can be proposed and a response recorded. | The reference represents a candidate route. It does not show which retailer selected it. |
| Implemented configuration | A retailer's agreed requirements, settings and tests show when approval is required. | The selected design behaves as tested under stated conditions. That is not yet everyday use. |
| Enacted practice | Observed cases show staff calling customers, waiting for responses or adapting when time is short. | These actors handled these cases in particular ways. That does not alone establish an improvement. |
| Outcome | A defensible comparison examines incorrect substitutions and delivery delays before and after a change. | A measured difference can be reported. Attributing it to the change needs evidence about rival explanations. |

The project uses **architectural coherence**, **implementation fit** and **enacted fit** as three distinct questions. Do the represented elements work together logically in the branch? Does the selected arrangement suit the organisation's requirements and constraints? How does it actually work with day-to-day practice? These are not three levels of confidence in one conclusion. They are different questions with different evidence. A coherent design can fit one retailer and not another. A design that passes a test can still prove difficult to use under pressure.

**Worked comparison.** A reference design can consistently route every substitution to a service team and return the answer to dispatch. That is a coherent arrangement if the design also specifies what to do when the answer is late. It may fit a store with long delivery windows but not a store that dispatches every fifteen minutes. Even where tests show the agreed deadline and fallback work, observation might reveal that employees use a phone call not represented in the recorded workflow to clarify difficult cases. A study of enacted fit asks whether that extra practice helps the arrangement function or signals that the selected design misses something. None of these possibilities is a finding about a real retailer.

```text
Reference instruction   → What the design represents
Configuration and test   → What the organisation selected and verified
Case traces and fieldwork → How people used, adapted or avoided it
Outcome comparison       → What changed, and what might explain the change
```

### Why a procedure is not an organisational routine

[Feldman and Pentland (2003)](https://doi.org/10.2307/3556620) distinguish a routine's **ostensive** aspect, the general pattern participants can refer to, from its **performative** aspect, the specific actions of particular people in particular situations. A written procedure can guide or represent aspects of the general pattern; it is not the pattern in everyone's understanding and it is not an observation of performance. At the grocery store, a generic instruction may say to ask the customer. One employee may start the call before finishing the order; another may wait until all shortages are known. Those hypothetical variations show what a procedure alone cannot settle.

[Orlikowski's practice lens (2000)](https://doi.org/10.1287/orsc.11.4.404.14600) draws attention to patterns people enact through continuing use of technology. The question is not whether the software matters or people matter more. It is how the technical arrangement and ongoing practice relate in the cases observed. A preconfigured worklist can direct attention, but a particular team may still rely on conversation to interpret a difficult case. The conversation is not a claim about what all teams do; it is one possibility to investigate.

### Why one artefact is not an infrastructure

A delivery record is an **artefact**: an individual object that can be inspected. An **information infrastructure** is a wider, evolving arrangement of connected technologies and practices. [Hanseth and Lyytinen (2010)](https://doi.org/10.1057/jit.2009.19) theorise that wider level using the development of the Internet. The course borrows the distinction, not the claim that a single ERP product behaves like the Internet.

For example, a retailer may depend on existing product codes, partner messages, a transport system and older interfaces. That **installed base**, meaning what is already in place and used, can limit which changes are feasible. To argue that a delivery record has become part of a wider infrastructure, examine its connections, how the standards are maintained and how the arrangement changes over time. One process script can support a statement about a record or a handoff. It cannot settle a claim about the whole network, its evolution or who governs it.

## 5. First SAP reading: what does “create a delivery” show?

**Documentary example.** In the Swiss Sell from Stock reference case, SAP's represented delivery-creation procedure uses the earlier sales document together with shipping criteria to select work. The expected result includes a delivery record and its number in the log. An optional proof-of-delivery branch separately documents a confirmed quantity used in billing. See the [evidence cards](../../cases/M01_BD9_Reading_a_Reference_Artefact.md) for exact steps and source-access status. The two cards do not form a trace of one order. The fictional milk order does not describe this SAP procedure.

```text
Card A: prior sales document + shipping criteria → select work → expected delivery record
Card B: optional confirmation                    → confirmed quantity used in billing

Separate reference examples. A record is not proof that goods reached a customer.
```

Walk through Card A slowly:

1. **Observe.** The documented selection uses an earlier sales document with other criteria. The log entry is an expected result, not a record that this class ran the procedure.
2. **Interpret.** In this route, the earlier order helps connect Sales and Shipping by delimiting which work is selected. That is a specific information dependency.
3. **Consider a rival.** A technical identifier may be present simply to locate the relevant record. Here the documented selection tells us how it participates in the later task. The technical and organisational explanations can coexist; the latter identifies the relationship between the tasks.
4. **Bound.** The source does not establish which user could access a particular shipping point, which configuration a retailer chose, or whether a shipment physically reached anyone.

Now compare Card B. There the documented quantity does more than help find a record: it is used in a later activity. This supports a different, narrower inference. It does not show that every invoice is based on a receipt confirmation or that the teams understand deviations in the same way. The disciplined move is to say what the value does in the named branch, then stop.

**One usable finding:** “In the documented Swiss BD9 delivery-creation example, the earlier sales document helps select work for delivery creation. The expected delivery record does not establish physical fulfilment.” This is stronger than “SAP integrates everything”, because another person can verify it. It is more useful than “there is an order field”, because it names how the work is connected.

## 6. How to study the rest of the course

Start with the business problem, not the screen. Write down what the actors need from one another. Identify the actual operation. Then keep the observation, interpretation and evidence boundary visible in your notes. The method is the same whether you approach the course as a researcher, an operations student or a prospective SAP consultant.

For a consulting example, imagine a client asks whether a delivery log proves fulfilment. The reference can tell you what the expected log records. A configured demonstration can show the relevant state under the selected conditions. Confirmation of what the customer received would need separate evidence. A good consultant can explain the difference without needing to memorise every application name.

**Worked follow-up: turn a request into questions.** Suppose the client says, “We want one status called delivered, visible to every team.” Before endorsing the request, ask what the status should denote: a record was created, goods left the warehouse, or someone confirmed receipt. Ask who supplies that fact, who needs it, when they need it and whether a later correction is possible. The first question is about meaning; the next questions concern the arrangement of work. If the status is also meant to start billing, add a separate question about which action should follow and under what conditions. The request for a status is not yet a process design.

```text
"Show delivered"
    → Define the event
    → Identify who records and consumes it
    → Check what decisions or actions rely on it
    → Ask what happens when evidence is late or disputed
```

**Check your understanding:**

1. Why are the two substitution designs different organisational arrangements even if both use the same ERP?
2. When does a prior record supply an input rather than merely appear on screen?
3. What would you need to establish that a delivery rule was configured, used in practice, or improved an outcome?
4. Why are a written instruction, an observed routine and a wider information infrastructure different units of analysis?
5. Which BD9 observation supports a bounded claim, and which tempting inference should you refuse?

Complete the [first evidence annotation](../../exercises/M01_Annotate_a_Reference_Artefact.md) before opening the instructor answers. [Module 2](../02_End_to_End_Processes/README.md) will expand this from one evidence segment to a bounded process map.
