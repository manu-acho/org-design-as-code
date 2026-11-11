# Governance and Control: The entry was approved. What does that prove?

**Module 8 · Postgraduate · Week 10 · Student lesson draft**

[Module 7](../07_Decision_Theory/01_Student_Lesson.md) asked who shaped the choice before the approver clicked. This lesson asks who can constrain the choice, what makes it possible to challenge, and what evidence would show that a control worked. It uses a documented SAP procedure for reviewing accounting entries and a separate fictional close exercise.

## 1. A perfectly plausible approval record

**Fictional opening.** A distributor is finalising its accounts for the month. An **adjustment**, an accounting entry that corrects or updates an amount, is submitted and approved. The **workflow history**, a record of steps taken, gives a user, an action and a time. The close lead asks why the adjustment was approved. The team can show who clicked, but cannot say what evidence they saw, whether they had the right to decide for that accounting unit (identified by a **company code**), or who was expected to challenge a weak explanation.

Compare two possible stories. In the first, the reviewer independently assesses the evidence and asks the preparer to explain a discrepancy before approving. In the second, the reviewer approves on the strength of a colleague's instruction without seeing the underlying evidence. Both could leave a similar approval record. That does not make the record useless. It makes it evidence of a narrower fact than the close lead needs.

```text
Recorded approval → Evidence that a decision was recorded
Delegated right   → Evidence about who was entitled to decide
Review of reasons → Evidence about whether the decision could be challenged
```

**Governance** concerns how the organisation allocates decision rights, defines limits and provides for oversight and challenge. **Control** concerns arrangements intended to bring actions or results into line with a standard. They intersect: governance can decide who owns a control and can change it; a control may require that a particular step takes place before another is possible.

## 2. Give each governance claim its own evidence

| Concept | Plain-language question | Evidence to look for |
|---|---|---|
| Permission | Can this user technically perform the action? | Configuration, role assignments and a controlled access test. |
| Responsibility | Who is expected to carry out or follow up the work? | Assignment, role description and an escalation route. |
| Formal authority | Who has the right to decide in this scope? | Policy, delegation and its limits. |
| Real authority | Who effectively shapes the choice? | Decision histories, access to information and accounts of how recommendations were handled. |
| Traceability | Can the relevant action, state or rationale be reconstructed? | Linked records, history and adequate provenance. |
| Accountability | Who must explain their conduct to whom, and what can that forum do? | An obligation to explain, a forum able to question and judge, and possible consequences. |

A person can be responsible for preparing a journal without being authorised to approve it. An approver can have a technical permission outside their policy remit. A person with the formal right can still defer to a colleague who controls the relevant information. None of those possibilities can be settled from a role name alone.

**Segregation of duties** separates responsibilities that should not be exercised by the same person in the relevant circumstances. For example, a fictional policy might prohibit preparing and approving the same material adjustment. A process diagram showing two role labels represents a separation of tasks; it does not establish that two distinct users are assigned, that the restriction is enforced on the same entry, or that a substitute route preserves it. Those are specific things to verify.

```text
Two roles in a procedure
    → Check who is assigned in the selected implementation
    → Test the same-entry restriction, including alternate routes
    → Observe whether review actually operates independently
```

## 3. Diagnose how a control is meant to work

[Ouchi (1979)](https://doi.org/10.1287/mnsc.25.9.833) starts from an organisational problem: people must cooperate even when their objectives do not fully coincide. Control design depends partly on what can be assessed and which norms people share. For a close team, speed and independent scrutiny are both legitimate objectives, but optimising one can undermine the other. A procedure demanding an extra signature might slow the close without improving scrutiny if the signer has no usable evidence.

A **behaviour control** concerns how work is performed. A rule requiring independent review before posting is an example. An **outcome control** assesses the result against an agreed standard. A subsequent review of unresolved reconciliation differences can be an example if a standard and response are specified. Informal control can also matter, such as professional norms that encourage colleagues to raise uncertainty rather than treat a review as a formality. [Kirsch (1997)](https://doi.org/10.1287/isre.8.3.215) studied portfolios of formal and informal controls in systems-development projects. Her study motivates asking how controls work together; it is not evidence that a particular SAP finance control is effective.

```text
Standard → Observe evidence → Compare with the standard → Intervene if needed
                  ↑                                            ↓
                  └──────── Recheck the result or follow-up ────┘
```

Use that sequence as a diagnostic, not a requirement that every mechanism implements every step. A control can depend on several roles or systems. Define the standard before judging what the trace means:

| Component | Fictional close example | A failure to look for |
|---|---|---|
| Standard | Material adjustments within scope need independent review before posting. | Materiality or scope is undefined. |
| Observation | The reviewer sees the entry and supporting evidence. | A notification arrives but the evidence is inaccessible. |
| Comparison | Someone checks the applicable policy and the substance of the entry. | The task checks completion, not whether the review was adequate. |
| Intervention | An unresolved entry can be sent back, held or escalated under policy. | No authorised reviewer is available before the deadline. |
| Follow-up or consequence | A named forum follows unresolved issues and can require remediation. | A trace exists, but nobody can reopen or challenge the matter. |

Different controls operate at different times. A gate is **preventive** if it blocks a prohibited action before it occurs. A review is **detective** if it identifies a problem that may already exist. A correction is **corrective** if it changes the affected state or addresses the underlying issue. A pre-posting review can be a designed gate; it is not evidence of prevention on every path. The [Module 5 balance validation example](../../cases/M05_J58_Balance_Validation.md) represents review visibility, not a demonstrated gate over posting.

**Worked portfolio.** Imagine a close team adds a second approver after a series of poorly supported adjustments. If both reviewers see the same incomplete record and each assumes the other checked it, the extra signature does not fix the information problem. A better candidate arrangement could combine one properly informed independent review, a visible route for incomplete evidence, and a later check of how exceptions were handled. This is a design hypothesis. To evaluate it, compare which errors each mechanism can detect or prevent, where it depends on another mechanism, and how often it adds delay without changing a decision.

## 4. J58: distinguish approval, forwarding and rejection

The [Swiss J58 evidence cards](../../cases/M08_J58_Verification_and_Accountability.md) cover selected checks on **journal entries**, records that specify amounts to add to or subtract from the relevant accounts. For example, a correction might move an expense to the right account. In the approval example a requester submits an entry for verification before it is posted. The represented processor approves; posting is the expected result. In a separate example, forwarding changes the processor. The procedure describes a check of the proposed recipient's technical permission to post for that company code. A further procedure returns a rejected entry with a reason so the requester can review, edit and resubmit.

```text
Approval example:  Submitted, not yet posted → Processor approves → Expected posting
Forwarding example: A different processor is named → Posting-authorisation check described
Rejection example:  Reason returned → Requester reviews, edits and resubmits

Separate procedures, not one observed entry or a universal posting path.
```

These observations support a claim about **represented controls** on the named verification branch. The registered evidence also includes a separate option for approval posting-authorisation checking. A documented option is not proof that all checks are enabled in a customer's tenant. Forwarding is a change of recipient, not evidence of bypassing approval. Rejection and resubmission represent a pre-posting return path, not reversal of a posted entry. An effect documented on one branch does not establish the same effect on another.

An approval may be a substantive decision, a gate, an acknowledgement, or a way of signalling that a prescribed procedure took place. Those interpretations can coexist. In J58, the distinction between submission and expected posting after approval supports more than “someone received a notice”. The rejection procedure supports the availability of a represented intervention. Neither tells us how carefully a reviewer assessed the evidence, whether the same person performed both roles in practice, or whether a forum could challenge that review.

### Scope check: a separate posting route is not evidence of a bypass

The same Swiss J58 reference family includes a separate direct journal posting example (J58-W08-01, PST steps 1 to 5; see [case card D](../../cases/M08_J58_Verification_and_Accountability.md)). That procedure represents direct posting of debit and credit lines with the relevant accounting inputs. The cited direct example does not show the submission-for-verification step. This limits the claim we can make about the verification branch; it does not prove that an entry which *requires* independent verification can be posted directly to evade it.

```text
Verification example → Submit for review → Approval → Expected posting
Direct example       → Enter the journal and post under its own conditions
Scope test           → Which route can this entry use under the agreed policy and setup?
```

A **bypass** would mean avoiding a requirement that actually applies to the case. To test for one, start with the client's policy and select an entry that should require independent review. Then test whether an appropriately scoped user can post that entry through a different applicable path without the required review. Include an out-of-scope entry as a comparison: a legitimate direct posting for that case should not be reported as a bypass. Check the resulting posting state and entry identity, not just which options appear on screen. The procedures provide candidate paths for this question, not the answer for a particular tenant.

## 5. Traceability helps accountability, but does not create it

[Bovens (2007)](https://doi.org/10.1111/j.1468-0386.2007.00378.x) uses a narrow actor-forum conception of accountability. Applied here, ask who must give an account, to whom, about which conduct, and what the forum can do with the answer. This is a way to analyse a fictional or real governance arrangement, not a claim that an SAP workflow itself creates such a relationship. It is also more demanding than the coordination use of accountability in [Module 4](../04_Coordination_and_Interdependence/01_Student_Lesson.md), where making responsibilities apparent can help people coordinate.

```text
Trace:  Actor + action + time + context → Something to reconstruct
Accountability: Actor gives reasons → Forum questions and judges → Consequences may follow
```

Consequences need not be punitive. An authorised forum might require a correction, request further evidence or change a procedure. But an inbox history is not itself a forum, and requiring a reason field does not establish that anyone can ask a follow-up question. Conversely, the ability to question an actor does not mean the records are adequate. Trace quality and the strength of the relationship need separate assessment.

**Worked rival test.** Suppose a fictional trace shows one approval in the final minute of the reporting window. One analyst calls it a rubber stamp; another says the substantive review happened earlier in a meeting. Timing alone does not distinguish the stories. Evidence linked to this entry would help: what was available at review, who participated, what questions they raised and what changed before approval. An early review can be substantive and still poorly documented. A detailed log can coexist with little independent challenge.

**Illustrative transfer.** A university expense system may record who approved a claim. An accountability arrangement might also include an authorised finance panel that can request the receipt and reasons, question the approver and require follow-up if the claim was handled improperly. The same distinction holds whether approval is recorded in an ERP system, a dedicated expense tool or a shared register.

**Study pause:** For either example, state one supported observation and one piece of missing evidence.

### Worked example: from a trace to a challenge and follow-up

**Fictional oversight review.** Cedar's close oversight panel can require reviewers to explain an approval, examine its basis and ask the control owner for corrective action. It opens a review of entry C-17 using the [fictional history](../../cases/M08_J58_Verification_and_Accountability.md). The panel is an organisational forum, not a workflow or product feature.

| Stage | What happens in the simulation | Why the stage matters |
|---|---|---|
| Give an account | The panel asks the reviewer behind REV-C why approval was appropriate and requests the delegation and evidence they relied on. The reviewer says they checked a draft before the task was forwarded. | The trace identifies a recorded action. The obligation to explain brings in the reasons and records behind it. |
| Question | The panel asks whether that draft was the posted version and whether the substitute's remit covered the entry. The reviewer supplies the delegation, but the supporting record cannot be tied to the posted version. | The panel tests the explanation rather than treating either the approval or the reviewer's assurance as conclusive. |
| Judge | The panel finds the delegation supported but the review of the posted version unsubstantiated. It does not conclude that the entry was wrong or that the reviewer did no work. | A finding must say which standard the evidence does or does not support. |
| Require and check follow-up | The panel asks the control owner to arrange an independent review of the posted version, document the result and repair the link between evidence and entry versions. The panel checks completion before closing its finding. | The consequence is remediation, not automatic punishment. A retrospective review does not retroactively demonstrate that the pre-posting control operated as intended. |

If the panel could only receive the report, not request reasons, question them or require follow-up, the same history would support traceability but not the accountability arrangement described here. Conversely, an empowered panel cannot make a sound judgement from incomplete evidence alone. In a real study, check the forum's remit and how it exercised it in particular cases.

## 6. Consulting studio: design an exception without losing control

**Fictional client.** During close, the assigned reviewer is unavailable. The client wants time-sensitive adjustments to proceed without letting preparers approve their own entries. Compare two arrangements. One forwards the task to an authorised independent reviewer, preserving the same standard. The other would create a narrowly defined emergency departure from the normal rule. The second is an **override proposal** only if it changes an otherwise applicable rule. Neither proposal is a claim about what the SAP reference delivers.

```text
Reviewer unavailable
   ├─ Substitute review → Same standard, another authorised reviewer
   └─ Proposed override → Defined departure, named authority, reason and later review
Do not confuse reassignment with permission to bypass a control.
```

Ask first whether the routine standard can be preserved. If an emergency exception is justified, specify which requirement can be departed from and which cannot. In the fictional brief, the prohibition on self-approval stays in force. Define who grants the departure, what evidence is retained, what happens if no eligible person is available and who reviews the decision afterwards. A credible option may be to hold and escalate rather than weaken the rule. Compare how each proposal changes risk, workload and the ability to reconstruct a decision.

Use a small TOGAF-informed baseline-target-gap comparison, building on [Module 5](../05_Information_Processing/01_Student_Lesson.md). A missing independent substitute may be a delegation and availability gap. A weak review history may be an information and oversight gap. The gaps are related, but neither proves a product limitation. Test the chosen design with a normal approval, a proposed unauthorised substitute, an attempted self-approval and a returned entry that is edited. If an override remains in scope, test its eligibility, refusal, expiry or closure and follow-up as separate conditions.

```text
Reference documents → Designed gate, action or state
Configuration tests → Selected control works or fails under stated conditions
Evidence from use   → How review, exceptions and challenge actually operate
```

**Worked verification plan.** Suppose the selected configuration stops PREP-A from approving C-17 through the standard screen. That supports a narrow claim about the test user, entry and route. It does not tell us whether the same person can approve through a substitute assignment, whether the decision applies to the latest version, or whether another route is subject to the same policy. A stronger test uses an eligible reviewer as a positive comparison, deliberately attempts a prohibited action, and checks the resulting state. A disabled button is useful evidence, but it is weaker than showing that the prohibited state change did not occur through the relevant routes tested.

To study how the control operates over time, sample different kinds of cases: routine approvals, substitutions, returned entries and urgent cases. A sample consisting only of successful postings excludes the decisions the control may have stopped. For each case, distinguish whether a review happened, what it considered and how unresolved issues were handled. If the organisation claims the control reduced errors, that is a further claim requiring a defined outcome and a defensible comparison. A low count of recorded exceptions could mean the process improved, or that reviewers did not record them. Include the rival before treating the metric as evidence of success.

Complete the [control and accountability exercise](../../exercises/M08_Test_a_Control_and_Trace.md). Before moving on, explain why a two-role workflow is not proof of segregation, why an audit trace is not accountability, and why a documented check is not evidence of control effectiveness in use. [Module 9](../09_SAP_Activate_and_Transformation/README.md) will bring these questions into Fit-to-Standard and transformation work.
