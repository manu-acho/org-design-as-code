# Knowledge Boundaries: One purchase order, different versions of the problem

**Module 6 · Postgraduate · Week 8 · Student lesson draft**

[Module 5](../05_Information_Processing/01_Student_Lesson.md) distinguished having information from being able to act on it. This lesson takes the next step. What happens when the information reaches the right people, but each understands it through a different kind of work? And what happens when they understand one another perfectly but still disagree about what should happen?

## 1. Three departments agree on the number and still cannot proceed

**Fictional scenario.** A food manufacturer orders 100 cartons of packaging. At the dock, 100 cartons are counted, but 12 show visible damage and are set aside. The supplier invoices all 100. Purchasing says, “We ordered 100.” Receiving says, “We counted 100.” Accounts Payable says, “The invoice claims 100.” All three may be right. None of those statements tells the business how many cartons it should accept for use or pay for.

```text
Purchasing       100 ordered  → What did we agree to buy?
Receiving        100 counted  → What arrived, and what was set aside?
Accounts Payable 100 invoiced → What is the supplier claiming?

Same number ≠ same event ≠ same decision
```

The purchase order gives the teams a common point of reference. It does not collapse a commercial commitment, a physical event, a quality judgement and a payment decision into one fact. In this example, even subtracting 12 from 100 only gives a count of cartons not set aside at the dock. It does not establish the quantity ultimately accepted or payable. The distinction matters for enterprise-system design: a field can be correct in the context where it was produced and misleading in a different one.

A **knowledge boundary** is a point where groups cannot simply use one another's knowledge as if they did the same work. The groups have different experience, vocabulary or interests. Those differences are often useful. Receiving can spot physical damage that an invoice processor cannot see; Accounts Payable understands the conditions for processing a claim. The aim is to make enough of that specialised knowledge usable across the boundary without expecting everyone to become an expert in every function.

## 2. Carlile: diagnose the boundary before prescribing the fix

[Carlile (2004)](https://people.bu.edu/carlile/docs/3-T%20Framework%20%28Carlile%29.pdf) distinguishes three progressively more demanding boundaries. At a **syntactic boundary**, actors can rely on sufficiently shared meanings and need a workable way to exchange information. **Transfer** is the appropriate response: move the information using an agreed representation. At a **semantic boundary**, actors give relevant terms or situations different meanings. **Translation** makes those meanings and their implications intelligible across groups. At a **pragmatic boundary**, a proposed change has different consequences for the groups. Understanding the difference is necessary but insufficient; **transformation** may require people to revise their knowledge, practices or commitments and agree on an arrangement they can work with.

Carlile also asks about **novelty**. An arrangement that works for familiar cases may be inadequate when something changes. People can already share a vocabulary for ordinary receipts but need to work out what that vocabulary means when there is visible damage, a late inspection or a disagreement with a supplier. The more demanding diagnosis does not make the simpler work disappear. A negotiated exception policy still needs reliable identifiers and meanings.

| What is getting in the way? | What to check | A proportionate response |
|---|---|---|
| Both teams agree what a quantity means, but the message cannot be tied to the right order line. | Can both trace the same identifier, item and unit? | **Transfer:** agree how to transmit and match the identifier and unit. |
| The message arrives, but “received” means physically counted to one group and accepted after inspection to another. | Can each team explain the other's meaning with a concrete case? | **Translation:** distinguish counted, set aside and accepted, with examples that connect the terms to work. |
| Both teams understand those states but disagree about whether to pay the undisputed part while the supplier investigates. | What costs, risks and commitments would each option create, and who can decide? | **Transformation:** negotiate a policy and revise the handoffs, evidence and responsibilities needed to apply it. |

```text
Can we match the record? ──no──→ Transfer problem
             yes
              ↓
Do meanings line up? ──────no──→ Translation problem
             yes
              ↓
Can we act on that meaning? ─no→ Check stakes, authority and practice
                                  before proposing transformation
```

This is a diagnostic sequence, not a rule that work always advances through three stages. A single exception can expose several boundaries. Start where the evidence is clearest. A failure to act might be caused by a missing permission rather than conflicting interests. A disagreement that sounds political might disappear once the teams realise they are talking about different deliveries. Conversely, a glossary will not settle a disagreement about which department carries the cost of replacing stock.

**Worked comparison.** Suppose Receiving and Accounts Payable agree that “counted” means cartons physically counted at the dock. One site reports quantities in cartons; another transmits the agreed equivalent in individual packs, with the conversion fixed and understood. A reliable conversion can solve that transfer problem. Now suppose the second site uses its quantity to mean cartons cleared by Quality. Converting units does not solve that problem. Even a perfectly converted number carries the wrong meaning for a user who assumes it describes a dock count. Finally, suppose everyone knows both counts but the operations lead wants to keep the line running and Finance wants to avoid paying for damaged goods. The issue is now how to organise competing responsibilities. A defensible arrangement may keep the same terminology but change who is consulted and what evidence is required before a decision.

## 3. Bechky and Carlile: how objects help people understand one another

In [Bechky's (2003) production-floor study](https://doi.org/10.1287/orsc.14.3.312.15162), engineers, technicians and assemblers brought different understandings to the same product. They had different language and places of work, and they encountered different aspects of the machine. In one episode, the lead assembler demonstrated the hand clearance needed to lift a pump so an engineer could see a constraint that mattered for fixture design. The demonstration linked the engineer's design work to the assembler's physical work. Rephrasing the assembler's comment had not done that job.

**Common ground** is enough mutually understood context to work on a problem together. It does not require identical expertise or agreement on the eventual decision. In the packaging example, Accounts Payable need not learn how to inspect cartons. It does need to know which event the count records, what the inspection can establish, and which question is still open.

[Carlile (2002)](https://doi.org/10.1287/orsc.13.4.442.2953) examines what objects can do at such boundaries. A **boundary object** is an object people use to work across groups despite their different perspectives. For example, a technician and a building manager might use the same floor plan to locate a faulty pipe and agree which rooms can stay open during repairs. It can give them something recognisable to refer to, help them surface differences, or support changes to what they know and do. Which job it performs depends on use. Calling a purchase order a boundary object because two people can open it is premature. It is a *candidate*: the question is whether people use it to compare their accounts of the work, expose a disagreement and coordinate a response.

```text
Commercial view     → One identifiable order line ← Physical receipt view
                                   ↑
                             Invoice claim

Shared point of reference → Compare differences → Agree what still needs deciding
```

A master record and a transaction object can serve different purposes. A material master can provide a shared identifier and unit conventions across many transactions. A purchase order line can anchor a discussion about one particular commitment. Neither establishes what happened at a dock. In a dispute about damage, the teams might need the order line, a receipt record and a physical demonstration or other permitted evidence of what arrived. If the representation omits a relevant distinction, adding a field may help, but only if people agree what event it denotes, who maintains it and how to handle corrections.

**Why interaction still matters.** [Gittell (2002)](https://doi.org/10.1287/mnsc.48.11.1408.268) studied coordination in patient care. The study helps explain why routines and relationships are not necessarily substitutes: a routine can support interaction. For enterprise-software analysis, the question is whether a shared record gives people a reliable way to consult the right expertise, not whether the record makes consultation unnecessary. The healthcare evidence does not establish how an SAP implementation works.

### Worked example: finding the specialist is not the same as getting an answer

[Faraj and Sproull (2000)](https://doi.org/10.1287/mnsc.46.12.1554.12072) distinguish recognising when expertise is needed, knowing where to find it and bringing it into the work. Their study is about software-development teams. Here, use the distinction to diagnose a fictional handoff, not to predict the performance of a finance or warehouse team.

At Alder Foods, Receiving knows which Quality specialist to call and sends the order number. The specialist still cannot assess the issue: the message does not identify the set-aside cartons or say when they can be inspected. Even if the specialist eventually completes the inspection, a private reply to Receiving may leave Accounts Payable unaware that its earlier information is out of date. Neither failure is fixed by a better staff directory.

```text
Receiving flags a case → Quality gets the line, affected cartons and decision deadline
      → Quality returns a scoped finding, or says inspection is still pending
      → Purchasing and Accounts Payable confirm what the finding does and does not settle
      → If the deadline cannot be met, the named owner escalates the unresolved decision
```

In this proposed design, Receiving identifies the case and the deadline; Quality assesses usability; Purchasing and Accounts Payable apply the finding within their own remit. Quality's response should say which cartons it covers, what was checked and what is still open. It need not expose every inspection detail to every recipient. If Quality cannot respond in time, the escalation preserves “pending” rather than silently turning it into “accepted”. This is an original handoff design, not a feature attributed to SAP.

**What would show common ground?** In a walkthrough, ask Accounts Payable to explain which stock the Quality finding covers and why it does not, by itself, establish what is payable. Ask Quality to explain which decision is waiting on its answer. Then change the example: Quality has inspected only half the set-aside cartons. If both roles can apply the distinction to that new case and keep the remainder unresolved, that is stronger evidence of shared understanding in the exercise than a delivered notification or a repeated definition. To make a claim about practice, compare real handoffs and exceptions as well.

## 4. Documentary case: follow what the purchase order supplies

**SAP reference evidence.** In the Swiss J45 purchase-order-referenced supplier invoice example, the procedure uses the earlier purchase order reference to populate invoice items. The invoice work still includes checks of amounts, quantities and taxes. See [the evidence card](../../cases/M06_J45_One_Order_Different_Meanings.md) for the source locator and release context. The procedure supports a claim about the transfer of structured information into the later task. It does not document the fictional damage incident, the meanings assigned by actual users or a universal three-way match.

```text
Documented path:  Prior purchase order → Invoice items populated → Checks
Research question: What does the information represent to each function?
Further evidence:  What did people understand, contest or change in a real case?
```

The distinction between **lookup** and **operative input** from Module 4 is useful again. If the order number merely helped the processor find an invoice, it could aid navigation without supplying any invoice values. Here the documented item population supports a stronger claim about transfer. It does not support a stronger claim about translation. To establish translation, one would have to see people or procedures explicitly relating meanings across contexts, such as distinguishing counted from accepted. To establish negotiated change, one would need evidence of the issue, alternatives, who could decide and what arrangement changed.

There is also a good rival interpretation of the boundary-object claim: the order may function only as a structured reference in the observed procedure. Its use in a conversation about damaged goods is possible, but not shown by the procedure. A paired walkthrough with Purchasing, Receiving and Accounts Payable could test whether it anchors a shared inquiry. Observe whether the participants can point to the relevant line, explain what the other teams' quantities represent and identify which evidence is missing. A smooth handoff in a routine case would not settle what happens under disagreement. Include an exception.

## 5. Workshop: make a disagreement visible before redesigning the process

**Fictional client.** In the [case brief](../../cases/M06_J45_One_Order_Different_Meanings.md), the plant needs 90 usable cartons by tomorrow, but only 88 were not set aside at the dock. Assume nothing about later inspection. The supplier asks to be paid for 100. Purchasing can contact the supplier, Receiving can report what arrived, Quality can assess the set-aside stock, and Accounts Payable can explain its invoice controls. The brief does not give any of those roles unilateral power to settle the whole issue.

An analyst who starts with “make the system use 88” is already making a policy decision. A better first move is to ask each role to explain what its number means, what it can verify, and what it cannot decide. Have the participants compare two proposals: wait for the inspection before deciding how to handle the invoice, or evaluate whether the undisputed portion can be processed separately under an agreed policy. Neither option is presented as a delivered SAP function. Each has consequences for payment timing, supplier relations, the production schedule and the evidence required for follow-up.

Separate the decision about replacing stock from the decision about the invoice. Purchasing may need to contact the supplier immediately to protect tomorrow's production schedule, even if Finance has to wait for inspection evidence. A single “exception resolved” status could conceal that one issue is settled and the other is not. Equally, more statuses will not help if no one is responsible for updating them. Ask which actors need to know about each decision and whether they need the same level of detail.

```text
Order line links the records
  ├─ Transfer: Do the order, receipt and invoice refer to the same item?
  ├─ Translation: Which count means ordered, counted, set aside or accepted?
  └─ Transformation: Who decides what to do while acceptance remains open?
```

**Light TOGAF bridge.** Record the current disagreement as a gap between the way the client works now and the way it needs to work. From a business-architecture perspective, specify responsibilities and the escalation decision. From an information perspective, specify which states must be distinguished and which evidence connects them to the order line. The [Open Group's Practitioner competency overview](https://help.opengroup.org/hc/en-us/articles/32127544219026-Competency-to-Role-Mapping-TOGAF-Enterprise-Architecture-Practitioner) places architecture development, stakeholder engagement and gap analysis in the toolkit. This is a short application of those ideas, not a TOGAF deliverable template.

A useful acceptance test begins with an order for 100, 100 cartons counted, 12 set aside and an invoice for 100. Ask whether Purchasing and Accounts Payable can identify the same item, explain why the figures are not interchangeable, and show who can resolve the open decision and what evidence is required. A negative case checks that an unresolved inspection is not treated as acceptance or automatically used to justify payment. The expected decision must come from agreed client policy, not from the lesson. A successful test would support a claim about the selected configuration under those test conditions. Repeated observation of day-to-day handling would be needed for a claim about enacted practice.

```text
Reference procedure → Shows how information is represented and passed
Configuration test  → Checks a proposed arrangement under stated conditions
Observed work       → Shows how people actually interpret and use the record
```

## 6. Transfer the method to a different process

**Illustrative example.** A sales team marks a customer order “complete” when it has been dispatched. A service team uses “complete” once the customer confirms receipt. Billing uses a different milestone to initiate its own work. A new report can send the status to all three groups faster, but it cannot tell them which event each group means. If the groups agree on the events but disagree about when to invoice a disputed shipment, a new status definition will not decide the policy. Compare this fictional example with the [Module 4 proof-of-delivery case](../../cases/M04_BD9_Delivery_and_Billing.md). The documented use of a confirmed quantity on an optional route is narrower than a claim about how a real company settles disputes.

Check your understanding:

1. Why might a conversion between cartons and packs be a transfer problem in one case but not another?
2. What would make the purchase order a candidate boundary object, and what evidence would show it functioning as one?
3. Give an example in which common ground improves but the disagreement remains.
4. Why does evidence of invoice-item population support transfer but not shared understanding or a universal matching rule?
5. What would you ask to distinguish a missing permission from a dispute over who should decide?

Complete the [shared-object exercise](../../exercises/M06_Analyse_a_Shared_Object.md) before reading the worked reasoning. In [Module 7](../07_Decision_Theory/README.md), we will ask how rules, information and authority shape the decisions people are in a position to make.
