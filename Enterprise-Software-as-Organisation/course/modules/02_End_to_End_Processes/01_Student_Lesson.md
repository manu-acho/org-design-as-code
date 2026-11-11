# End-to-End Processes: Follow the work, not the department

**Module 2 · Postgraduate · Week 2 · Student lesson draft**

[Module 1](../01_Enterprise_Software_and_Organisation/01_Student_Lesson.md) asked what a delivery number can prove. This lesson connects several actions and records without letting the diagram claim more than the evidence. A worked procurement reconstruction comes first, followed by an independent sales and shipping exercise. No prior SAP knowledge or formal process-modelling notation is required.

## 1. The invoice is not just Finance's problem

**Fictional opening.** A manufacturer needs packaging for a production run. Purchasing places an order, Receiving records the cartons that arrive, and Accounts Payable, the team responsible for handling supplier bills, enters the invoice. Each team can finish its own task while leaving the business problem unresolved. Purchasing may have ordered the correct item; Receiving may have recorded a partial receipt; the supplier may have billed the full order. Someone still needs to decide what the mismatch means and what should happen next.

An **end-to-end process** follows related work across the boundaries needed to reach a stated result. For the manufacturer, that might mean obtaining the packaging and settling the resulting liability, the amount the business owes the supplier. The analytical question sets the limits. A workshop on the invoice problem could begin with the purchase commitment and stop at the invoice disposition, such as recording it or holding it for review. A study of payment timing would need to go further.

```text
Purchasing                 Receiving                 Accounts Payable
Establish commitment  →   Record goods received  →  Review supplier claim
         What was agreed?       What was recorded?        What can proceed?

Invoice disposition is not settlement. Set the study boundary explicitly.
```

The arrows above orient the reader to a fictional story. They do not assert that all invoices use a receipt record or that every activity is compulsory. Part of learning to read process maps is recognising which arrows merely orient and which assert a specific dependency.

## 2. Use a small vocabulary consistently

**Posting** means recording a transaction in the system so that it takes effect in the relevant records. Posting a supplier invoice records it in the accounts; it does not mean the supplier has been paid. Posting a goods receipt records the receipt in the system; the record is not, by itself, evidence of the quality of the goods.

| Term | Working meaning | Example |
|---|---|---|
| Activity | Work performed by a person or system. Use a verb and an object. | Record goods receipt. |
| Event | Something that occurs at a point in time. | The receipt is recorded, or the goods physically arrive. Those are different events. |
| Actor, role and organisational unit | The actor performs the work; the role describes its responsibility; a unit groups work or defines a structural scope. | A named employee performs the represented Warehouse Clerk role at a plant. The reference need not identify the employee or their access. |
| Business object | A structured representation the process works on. | A purchase order, material document or supplier invoice. |
| State | A condition of an object at a particular point. | Posted or blocked for payment. These can describe different aspects of an invoice and are not synonyms for paid. |
| Handoff | Transfer of responsibility, information, a decision or an actionable object between activities. | An earlier purchase order supplies items for invoice entry. |
| Process instance or case | One occurrence of the work under a defined case boundary. | One order and its related work, or one invoice, depending on the question. |
| Outcome | The result we care about at a defined level. | A correct supplier settlement or fewer unresolved discrepancies, not merely an expected posting state. |

When a map shows “receipt”, ask whether it means physical arrival, the activity of checking the goods, or the record created after posting. When it shows “approved”, ask *what* was approved and what follows. Ambiguous labels can make two readers think they agree when they have different events in mind.

A **gateway** in a model expresses branching or joining logic. In this course, label the condition in plain language rather than drawing a diamond without explanation. A **variant** is a distinct permitted or observed route. An **exception** is a situation that needs different handling relative to an expected path; it may already have a designed route. An optional delivery split can be legitimate routine work, not an error. A discrepancy that prompts invoice reduction may be an exception with a documented response. “Optional” does not mean “uncontrolled”, and “exception” does not mean “outside the software”.

```text
An invoice arrives → Enter and check the invoice
    ├─ When an applicable routine path is supported → continue to the expected state
    ├─ When a documented exception condition applies → follow that branch
    └─ When the condition or next step is unknown → mark it; do not invent a route
```

## 3. Place the process in the wider business

A **process boundary** defines the work included for a question. An **organisational boundary** separates responsibilities, functions or organisations. A **system boundary** separates applications or technical components. One process can cross all three. Conversely, one application can contain several different processes. A sales order and a billing document can both live in the same product while still representing different work with different responsibilities.

The following is an orientation, not a catalogue of SAP functions. SAP's [end-to-end learning course](https://learning.sap.com/courses/exploring-end-to-end-business-processes-in-sap) uses broader names such as Source-to-Pay and Lead-to-Cash. Scope conventions vary. State the boundary rather than assuming readers use the same definition.

| Domain | Orientation | Reference window in this research |
|---|---|---|
| Procure-to-Pay (P2P) | Obtain goods or services and handle the supplier liability and payment. Source-to-Pay may also encompass sourcing and supplier selection before operational procurement. | J45, selected stock procurement and invoice procedures. Payment is a neighbouring scope, not an analysed J45 run. |
| Order-to-Cash (O2C) | Take and fulfil an order, bill and collect what is owed. Lead-to-Cash may include earlier opportunity or sales activity. | BD9, selected order, delivery and billing procedures. Cash collection is not demonstrated by an invoice. |
| Record-to-Report (R2R) | Record, reconcile and close accounts, then produce financial information. | J58, selected general ledger and close procedures, not the whole reporting or assurance landscape. |
| Recruit-to-Retire | Cover a person's employment lifecycle, from recruitment and onboarding through employment changes and eventual departure. | Orientation only here. It is not a fourth case comparable to the three Swiss references. |

SAP's course also introduces Design-to-Operate. It matters because production needs and stock decisions can shape what a business procures or promises, but it is not an additional empirical case in this module. In this course **R2R means Record-to-Report**; we spell out Recruit-to-Retire.

```text
Business landscape: procurement ↔ inventory/operations ↔ sales
                           ↘ accounting and close ↙
People and responsibilities are relevant throughout.

This shows possible interfaces, not the lineage of a single transaction.
```

A **process architecture** organises related processes and their interfaces. A payment process appearing next to an invoice process tells us where to investigate next. It does not tell us which data crossed, how a blocked item was treated, or whether a payment occurred. Map an actual handoff only when the evidence supports the relation on both sides or explicitly states how one side is used.

## 4. Choose the artefact that can answer the question

[Van der Aalst's BPM survey (2013)](https://doi.org/10.1155/2013/507984) distinguishes modelling, enactment, logging and analysis. These are related activities, not interchangeable evidence. A high-level model can communicate intended order. A procedure can supply a role, an input and an expected result. Configuration and test evidence answer what a client selected and how it behaved under stated conditions. A log can record events but may miss conversations, waiting, rejected attempts and work in other systems. An observed practice study can investigate those omissions. [Mendling, Reijers and van der Aalst (2010)](https://www.vdaalst.com/publications/p574.pdf) connect modelling choices to understandability and error risk. Use short verb-object labels and a visible boundary before adding detail.

**Business process management (BPM)** is broader than drawing models. It includes understanding, redesigning, implementing and monitoring processes over time. A **process model** is a selective representation for a purpose. An executable workflow is more than a descriptive model because its rules can affect which system transitions are possible, but it still need not capture the whole of human work. **Process mining** uses recorded events to discover, compare or enhance process models. These distinctions matter when a project compares a vendor reference model with customer data: each describes a different thing and may use a different unit of analysis.

| Artefact | Strong use | What it does not establish on its own |
|---|---|---|
| Reference overview or diagram | Orient to scope, roles and broad sequence. | Exact conditions, data use or actual behaviour. |
| Test procedure with expected result | Locate the represented action, input, branch and expected state. | That anyone ran it or obtained that result. |
| Client configuration and executed test | Show a selected arrangement and its behaviour in the tested conditions. | Day-to-day performance across all cases. |
| Event log | Analyse recorded events, times and object links. | Unrecorded actions, reasons or the whole work process. |
| Field observation and related records | Investigate how people performed or adapted work in context. | Generalisation beyond the studied cases without further evidence. |

**Worked log example.** A fictional log shows “delivery created” at 09:00 and “invoice saved” at 10:30. Those are recorded events, not a full account of what happened between them. If the identifiers cannot be linked, we cannot assume they concern the same order. Even with a link, the gap is elapsed time between recorded events, not necessarily work time. One order could have two deliveries; one delivery could be split. Flattening everything into one row can hide repetition, mix units of analysis and make a timing measure misleading. Start by defining what counts as a case and checking the object links.

## 5. Reconstruct J45 from records and actions

Open the [documentary dossier](../../cases/M02_J45_and_BD9_Process_Reconstruction.md). The worked case starts at a selected procurement request or direct order entry and ends at the expected invoice posting, with the neighbouring payment scope marked separately. We are reconstructing a **documented arrangement** from separate Swiss reference procedures, not replaying an observed order.

### Pass 1: mark the boundaries and actors

Purchasing creates the purchase order (PO). One procedure converts a **purchase requisition**, an internal request to buy something, into a PO; another creates a PO directly without converting a requisition. Warehouse work and Accounts Payable work are represented in separate procedures. The invoice is not the same business object as the PO or the **material document**, a system record of a stock movement such as receipt into inventory. These distinctions matter before any dependency is inferred.

### Pass 2: label each evidenced dependency

```text
Purchase requisition ── conversion example ──┐
Direct order entry ─── separate alternative ──┴→ Purchase order
     ├─ PO ID loads data for receipt posting → expected material document
     └─ PO reference populates invoice items → checks → expected invoice posting

The branches show uses of the PO across reference examples.
They do not establish concurrent execution or a compulsory receipt-to-invoice edge.
```

In J45-W07-13, the Warehouse Clerk uses the PO identifier to load receipt data. The expected material document is evidence of the represented result of posting, not the quality of a physical delivery. In J45-W07-16, Accounts Payable uses the PO reference to populate invoice items and carries out checks. These are two documented uses of the purchase order.

A **three-way match** compares the purchase order, the goods receipt and the supplier invoice, for example to check whether the quantities ordered, received and billed agree. The two documented uses of the PO do not establish that receipt data automatically supply invoice data, or that the three-way match is required or enforced on every route. The procedure title alone cannot supply the missing edge.

| Evidence move | What to write |
|---|---|
| Observation | The earlier PO supplies input in each named procedure. |
| Interpretation | Purchasing creates a record that later tasks depend on in different ways. |
| Rival or alternative | A PO identifier could merely locate a record. The documented loading or population supports the stronger claim that it supplies input here. |
| Limit | Separate procedures and expected results do not show a customer transaction or every possible branch. |

### Pass 3: represent a variation and an exception separately

The direct PO procedure challenges any claim that a requisition is mandatory for every purchase order in the scope. The optional no-PO/GR invoice procedure challenges a different claim, that every invoice needs a procurement reference. It still represents accounting inputs and checks. Neither alternative means controls disappear.

The invoice-reduction example is different again. It represents a response to an invoice amount and quantity above the PO values in that example. The companion procedure can produce a complaint letter from the invoice output. That output does not prove dispatch, acceptance or successful negotiation. Draw a boundary around the example rather than implying that all mismatches cause a reduction.

```text
Invoice entry in selected J45 examples
    ├─ PO referenced: supplies items; checks follow
    ├─ Optional no reference: accounting inputs; checks still apply
    └─ Separate mismatch example: reduction option + possible complaint output

Invoice processing in J45 ··· points to J60 as a succeeding payment scope
                             ··· does not demonstrate payment execution
```

### Pass 4: check what the map leaves unresolved

The cards leave four questions open: what made a particular purchase order eligible for approval; whether goods receipt preceded every invoice; whether the complaint was sent; and whether the two invoice routes are equally efficient or effective. These questions require additional sources. A plausible arrow is not evidence.

Write a bounded result: “In the selected Swiss J45 procedures, the purchase order is an input to represented goods receipt and to referenced invoice entry. Separate alternatives mean neither requisition conversion nor PO-referenced invoicing can be treated as universal. The dossier stops before execution of payment.” This is a process reconstruction, not a claim about implementation fit or enacted performance.

## 6. Reconstruct a different process yourself

In the shipping example, **goods issue** is the system record of stock leaving inventory for the shipment. It is not confirmation of customer receipt. A **delivery split** moves selected items to a new delivery record while others stay on the original. **Proof of delivery** concerns confirmation of what reached the customer; the dossier shows an optional procedure in which a confirmed quantity is used for billing. A **billing due list** identifies items presented for billing, not items already invoiced or paid.

In the [BD9 exercise](../../exercises/M02_Reconstruct_a_Process.md), start from delivery creation, identify the earlier order as an input, then trace the selected handling of the outbound delivery. Keep physical shipment, system goods issue, billing and cash separate. Show the optional delivery split or proof-of-delivery path only with its condition and effect. If a billing procedure starts from a due-list item, do not infer that the selected delivery in another card is the same item.

```text
Set the start and stop → Make an evidence row for each action
  → Draw supported links and mark optional branches
  → Name one missing link and one adjacent scope
  → Write a claim that matches the map
```

Ask another student to point at any arrow and tell you what it means: order of steps, reuse of information, transition of state or a neighbouring scope. If they cannot, label the arrow. If you cannot cite a source for it, mark it as a question.

**Before moving on:** Explain the difference between an optional variant and an exception. Show why “posted” is not the same as “paid”. Name two organisations or systems that could share work without sharing a screen. Explain why a single event log may not be enough to reconstruct a process. Then take your map into [Module 3](../03_Organisation_Design/README.md), where the question becomes why the work is divided and coordinated in this particular way.
