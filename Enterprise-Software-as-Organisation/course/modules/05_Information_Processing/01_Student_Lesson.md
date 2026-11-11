# Information Processing: Who can turn a result into action?

**Module 5 · Postgraduate · Week 7 · Student lesson draft**

[Module 4](../04_Coordination_and_Interdependence/01_Student_Lesson.md) asked what one task needs from another. This lesson asks what it takes to make that input useful. An **information bottleneck** is a point where necessary information fails to reach the right person, arrive in a usable form or support timely action. The lesson diagnoses one such problem, considers responses and explains what a reference procedure can show about the organisation's ability to act.

## 1. Begin with the decision, not the dashboard

**Fictional opening.** At a food distributor, Finance is checking and finalising its accounts for the month. This is the **month-end close**. The team sees an unusual balance, the amount shown in an account. The accountant does not know whether it reflects a timing difference, such as a transaction recorded in the following month, a mistake in the accounting entry, or a change in how the local team classifies entries. The local team knows what happened but has not seen the result. The close lead needs a decision before the reporting deadline. Giving the lead another copy of the same number does not answer any of those questions.

The teams depend on one another for different things. Central Finance can identify that a balance needs attention. The local team can explain the underlying transaction. Someone needs to decide whether to correct the entry, accept a timing difference or escalate the unresolved case. These tasks need not sit with one person. They do need to be connected.

```text
Central Finance has a signal     → Which balance should we investigate?
Local Finance has context        → What happened and what does the signal mean?
A named role has a decision      → Who can correct, accept or escalate?
```

The bottleneck could be transmission, interpretation or authority. The remedy depends on which it is. Start with the decision and the evidence it requires. Work backwards to the representation, the source and the people who know what happened.

## 2. Galbraith: match the work's information needs to the organisation's capacity

In [Galbraith's information-processing view](https://jaygalbraith.com/wp-content/uploads/2024/03/infoprocess1974.pdf), task uncertainty matters because some decisions cannot be settled before the work begins. New information appears during execution and may require people to change plans, schedules or priorities. For a given performance requirement, more uncertainty generally means more information must be processed during the task. This is not a claim that an uncertain business must collect every possible data point. It is about what people must find out and resolve to do the work.

An **information-processing requirement** is what must be established, shared and interpreted for work to proceed at the expected standard. **Information-processing capacity** is the ability to do that in time. It includes people, decision arrangements and communication, as well as systems. A database may hold a million records and still fail to put the right evidence in front of the right person before the deadline.

When cases are predictable, rules and plans handle a wide range of routine decisions. Hierarchical referral deals with exceptions outside that range. But if rules no longer cover much of what happens, too many exceptions may reach the same decision point. A manager's inbox can then become the limiting resource, even if every message arrives instantly.

```text
Routine case ──────→ Rule or plan covers it ────→ Work continues
Unsettled case ────→ Someone must decide ───────→ Exception reaches reviewer
Many unsettled cases at once ──────────────────→ Review capacity may be exceeded
```

Galbraith distinguishes two broad responses. **Reduce the requirement** so fewer issues need to be resolved in the first place, or **increase capacity** so the organisation can handle issues it still needs to resolve. Neither response is free.

| Design response | Illustrative example at the distributor | What it could cost or leave unresolved |
|---|---|---|
| Build in slack | Allow a buffer between local review and group reporting, so late evidence does not force immediate replanning. | A longer calendar may delay reporting. It does not correct a recurring source-data defect. |
| Make tasks more self-contained | Give a local unit the relevant records, expertise and a defined remit to resolve routine timing differences. | Expertise may be duplicated, and issues with group-wide consequences still need cross-unit review. |
| Improve vertical information systems | Give the close lead a structured summary with the affected period, balance and scope, instead of separate spreadsheets and email threads. | A shorter report may remove context. More frequent reports can create more work for the same reviewer. |
| Create lateral relations | Arrange direct contact between Central and Local Finance for unusual items, with clear ownership of the follow-up. | Joint review takes staff time. It needs a route for unresolved disputes. |

To see the distinction, consider a second distributor with three sites that compete for one finance specialist's time. If every small timing difference must be sent to that specialist, demand for their attention grows. Providing a clearer review queue increases capacity only if it helps the specialist resolve cases more effectively; the decisions still arrive. Equipping local teams to handle specified routine cases can reduce demand on the shared specialist, but transfers work and requires clarity about the limits of local authority. The right comparison considers both where the work goes and whether that part of the organisation can handle it.

**Worked comparison.** Suppose the close must still finish on Friday. One proposal is to add a day of buffer before the deadline by moving local review earlier. Another is to bring the local and central accountants together for 20 minutes every morning. The first is useful if evidence is reliably available earlier and the extra time absorbs variation. The second is useful if the unresolved questions need dialogue. If the underlying transaction is not recorded until Thursday, moving a meeting to Tuesday does not make the facts available sooner. If the data are already timely but ambiguous, widening the calendar alone may only delay the same conversation.

```text
Same symptom: review cases pile up
  ├─ Reduce demand: local teams resolve specified routine cases
  └─ Increase capacity: central and local reviewers jointly interpret difficult cases
Design check: where does the work go, and what still needs escalation?
```

This extends the previous module. A queue or a handoff is a **mechanism**. Galbraith's question is whether the arrangement can handle the amount and kind of work it receives. The coordination question remains whether the mechanism could support accountability, predictability or common understanding. Neither establishes that any of these conditions, or a better outcome, has been observed.

## 3. Trace information from the event to a possible action

The useful unit of analysis is a path, not the inventory of reports. Start with the event or state that matters. Identify how it is recorded, who can see it and what judgement it is meant to support. Then ask who is expected, permitted and able to act. These are different claims.

```text
Event or state → Representation → Visibility → Interpretation → Possible action
                    What was       Who can     What does it     Who can decide
                    recorded?      see it?     mean here?       or intervene?
```

**Availability** means the information exists in the relevant record or result. **Visibility** concerns whether a particular actor can retrieve or see it, including whether it appears in their working view. **Attention** concerns whether that actor notices and prioritises it. **Interpretation** concerns whether they understand what it means for the decision. **Ability to act** concerns whether they can do anything appropriate with it, given their role, authority, access, time and resources. The sequence is a diagnostic aid; real cases can loop back as actors request better evidence.

An access restriction and a display default can both make an item absent from someone's screen. They are not the same. A default filter changes what appears first to someone who can still reveal the item. A permission restriction changes what the person can access or do. A search that returns no result may also use the wrong scope. To distinguish these possibilities, check the query, the view and the actor separately. Do not infer permissions from a filter, or actual attention from a notification.

**Worked example.** Suppose a central accountant sees “12 items to review” in a fictional close dashboard. The local accountant sees one balance and a list of underlying entries. The first view supports prioritisation; the second supports diagnosis. If the twelve items are all different manifestations of one upstream issue, the central count may exaggerate the number of independent problems. If only the local team can see the supporting records, the central reviewer may need an explanation, not wider access to every entry. Limited visibility can be deliberate and appropriate. The question is whether a reliable route exists to bring sufficient evidence to the decision maker.

```text
Same underlying records
  ├─ Summary view → Triage: which matter needs attention first?
  └─ Detailed view → Diagnosis: which entries explain the balance?
Neither view alone tells us who may correct it.
```

This is why the number of reports is a poor measure of capacity. Capacity can grow when the same evidence is easier to interpret or when a knowledgeable actor can respond sooner. It can fall when alerts compete for attention, when a summary hides the applicable scope, or when a role can see a problem but cannot get it resolved. In supply-chain research, [Srinivasan and Swink (2018)](https://doi.org/10.1111/poms.12746) report associations among visibility, analytics capability and flexibility to act. Their study gives us a reason to ask about these capabilities together. It is not proof that a particular SAP report, dashboard or role improves performance.

## 4. Documentary case: what ran, what appears and what follows?

**Swiss SAP S/4HANA Cloud Public Edition reference case, Accounting and Financial Close (J58).** The two [case cards](../../cases/M05_J58_Balance_Validation.md) concern **balance validation**, the checking of balances against defined rules. A **rule group** is a set of checks selected together. The **accounting context** narrows where the checks apply, for example to a particular ledger, the collection of accounting records being checked, and a particular reporting period. The registered scheduling procedure uses these selections to define the validation run. The results procedure describes a role viewing results and opening rule-level detail. Successful rules can be revealed even when they are not displayed by default. Neither procedure records a client closing its books.

```text
Rule group + accounting context → Define what the validation run covers
Result selection + default view → Define what the reviewer initially sees
Review and follow-up decision   → Require a separate responsibility and evidence
```

The two cards document complementary functions, not an observed run followed through to resolution. A rule not visible initially may still have been evaluated. But revealing successful checks does not prove that every intended rule was selected, that the job ran in the right context or that the underlying records are correct in every respect. A rule result is conditional on the rule and the data it evaluated. It is not a universal statement about the accounts.

Consider two analysts looking for the same apparently missing result. One suspects that a filter hides a success. The other suspects the rule was outside the job's scope. The documentary case tells us both distinctions matter. To settle the issue in a particular implementation, check what the job was instructed to evaluate, what it actually executed, and which view the analyst opened. If the result appears after the display changes, that supports the view explanation for this case. If the rule was never in the selected group, no display change can reveal a result from that run. A third possibility is that the analyst's access is restricted; the case does not establish whether that is true.

| Evidence available | Defensible reading | Overreach |
|---|---|---|
| Job settings show a rule group and accounting context | The reference design provides a way to delimit a validation run. | All relevant balances and rules were checked. |
| The result view lets the reviewer show successful checks and inspect rule detail | The design provides selective visibility and a route to more detail. | A hidden result was not processed, or every reviewer can see every result. |
| A result is available for inspection | A represented reviewer can examine information relevant to follow-up. | The result blocks posting, authorises correction or signs off the close. |

A plausible rival is that the default is merely a display convenience. The documentary evidence cannot tell us whether it actually changes behaviour. It does support a narrower observation: the initial view distinguishes which results are surfaced and which require further action to reveal. Whether that distinction directs attention in practice depends on what reviewers look at, what they must document and how they respond under time pressure. A walkthrough with comparable normal and exception cases could test that.

## 5. Architecture studio: turn a missing handoff into a design question

**Fictional design exercise, not SAP configuration guidance.** At the distributor, central Finance reviews results but cannot tell whether a local team investigated a flagged balance. The client wants significant exceptions reviewed before sign-off, the formal approval to finish the close. Local supporting detail should remain available only to the roles that need it.

A **baseline and target comparison** separates the current arrangement from a proposed one. Here, the baseline is a flagged balance without reliable evidence of follow-up. The target is a view that tells the close lead which cases remain open and who owns them. The missing link between flag and follow-up is a **gap** to investigate. TOGAF is an enterprise architecture framework. The Open Group places gap analysis and stakeholder management among the techniques used with the [TOGAF Architecture Development Method](https://help.opengroup.org/hc/en-us/articles/32127544219026-Competency-to-Role-Mapping-TOGAF-Enterprise-Architecture-Practitioner). This classroom exercise applies only that narrow idea.

```text
Client baseline → Proposed target → Gap to investigate → Testable requirement
SAP reference evidence informs the comparison; it does not define the target.
```

| Lens | Baseline, as stipulated by the fictional brief | Proposed target and gap |
|---|---|---|
| Business | Central Finance sees results; local teams investigate; the close lead cannot see ownership or progress. | Name a reviewer for each in-scope case and an escalation owner. Decide who may close a case, and who may sign off the period. |
| Data and information | The result and local explanation cannot reliably be connected in the close lead's view. | Specify a common case reference, validation scope, review status and concise disposition. Decide which details can be shared and which must stay restricted. |
| Implementation question | The SAP evidence documents scoped validation and a results view. | Verify whether the selected solution supports the desired follow-up, access rules and traceability. Do not assume these are delivered by J58. |

The gap is not automatically “we need another SAP app”. It may be missing ownership, a missing link between records, unclear visibility rules or a combination of those. Two defensible options are a controlled follow-up process that refers to existing results, and a more integrated case route if the required capabilities are verified. Compare which roles would use each option, what data must cross the boundary and how failure would be detected. A short pilot can test the requirement before a project assumes the proposed design works.

**Consulting checkpoint.** Keep three statements separate in the workshop record. *Supported by the reference:* the procedure represents a scoped run and a results view. *Potential fit to test:* the results view may give the nominated reviewer enough detail to start investigating an in-scope flag. *Unresolved requirement:* the lead needs reliable ownership and follow-up status before sign-off. An unresolved requirement is not proof of a product limitation. It tells the team what to demonstrate, investigate or decide with the client next. We will return to this distinction in the [SAP Activate and Transformation module](../09_SAP_Activate_and_Transformation/README.md).

**A testable requirement:** Before sign-off, the close lead can identify unresolved material exceptions in scope, the assigned reviewer and the escalation status without opening restricted supporting entries. Define “material” and “in scope” with the client. In a test, include one flagged case with a review pending, one reviewed case, and a user who should not see local evidence. An automated gate is not part of the documented SAP behaviour here; if the client needs one, record it as a separate requirement to investigate.

## 6. Bring the distinction into the next module

1. When does a new report increase capacity, and when does it merely move work into another inbox?
2. How would you distinguish an excluded validation rule, a hidden success and an access restriction?
3. What does a displayed result establish? What would you need to establish that someone took responsibility for it?
4. In the fictional client case, name a change that reduces central review demand and one that increases capacity. Who takes on the work each change creates?
5. Can two teams agree on which balance they see but disagree on what it means or how to respond? Give a concrete example.

Complete the [information path and gap exercise](../../exercises/M05_Trace_Information_to_Action.md) before reading the worked answer. [Module 6](../06_Knowledge_Boundaries/README.md) takes up the last question: when a record crosses a functional boundary, what can the recipient understand from the record alone, and what requires further translation or negotiation?
