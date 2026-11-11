# Comparative Process Analysis: When is a recurring pattern really the same?

**Module 10 · Postgraduate · Week 12 · Student lesson draft**

A purchase order supplies information to an invoice. A confirmed delivery quantity is used in billing. An earlier clearing document identifies which accounting items were linked and marked as cleared, so that the clearing can be undone. Are these three examples of the same organisational mechanism, or do the records do different jobs?

The capstone builds three small comparisons, looks deliberately for a case that does not fit, and asks what claim can survive that challenge. The goal is to explain a relationship, not list features or go beyond the evidence. The [evidence cards](../../cases/M10_Three_Processes_Comparative_Dossier.md) and [comparative studio](../../exercises/M10_Test_a_Cross_Process_Pattern.md) are sufficient to take part without SAP access.

## 1. Compare a relationship, not an entire department or process

The comparison uses selected Swiss reference procedures from three areas: J45 for procurement of direct materials, BD9 for sell from stock, and J58 for accounting and financial close. They represent parts of **Procure-to-Pay (P2P)**, **Order-to-Cash (O2C)** and **Record-to-Report (R2R)**. The three names indicate the business area. They do not make these complete models of everything the organisation does.

| Case | Window in this lesson | What stays outside |
|---|---|---|
| J45 · P2P | Purchase-order rework and selected supplier invoice routes. | Full purchasing coverage, payment runs and observed supplier behaviour. |
| BD9 · O2C | Sales-order rework, selection for delivery creation and optional proof of delivery. | Cash collection, customer-level credit decisions and an observed fulfilment history. |
| J58 · R2R | Journal submission, rejection, direct posting and selected clearing procedures. | Full close, statutory reporting and assurance about the accounts. |

The cases share a vendor, product context and release family, but they do not form one observed chain. The examples do not show that a specific J45 purchase or BD9 sale ended in a specific J58 entry. Nor are the cases a representative sample of customer organisations. The point of comparing different business functions is to test whether an operation recurs across different objects and purposes **within the reference corpus**. Shared platform conventions are a reason to take a technical or documentation rival seriously, not evidence of independent replications across vendors.

```text
J45 branch        BD9 branch        J58 branch
     ↓                 ↓                 ↓
Reconstruct each actor, operation, object and consequence first
                       ↓
Compare the same analytical question across the separate branches
```

## 2. Make the unit of comparison small enough to check

Start with a **segment**: a documented action, rule, relationship or change of state, with a precise source location. An overview may show that invoicing follows earlier work. It takes a more specific step to show that the earlier order supplies invoice items or identifies the record to be acted on. The research method calls this the **granularity gate**: the evidence must be detailed enough to support the claim being made.

Use four questions for each segment:

1. **Who or what acts?** Name the represented role or logic without inferring the actual person, permissions or authority.
2. **What operation is represented, and on what object?** Say *populates invoice items*, *selects delivery work* or *targets a clearing arrangement*. Avoid relying on an app or field name alone.
3. **What does the later activity need from the earlier one?** Distinguish a value, an identifiable object, a state, a decision or another prerequisite.
4. **What would change if the input or condition differed?** Use documented options where available. Otherwise frame the difference as an inference or test, not an observed failure.

In the [coding manual](../../../08_Coding_Manual.md), a **candidate software organisational primitive** is an identifiable and reusable type of operation that does something consequential for the organisation of work. A rule that routes a review, a reference that supplies values and an action that changes a state can be candidates. A screen title or reused field label is not enough. Name the operation, its target and the scope in which it matters before deciding how broadly to describe it.

Keep the levels separate. At the **micro** level, an operation makes a particular value available for a later task. At the **process** level, that operation may work with other roles, checks and exception routes. At a broader **cross-process** level, you can test for recurrence, but a recurrent micro operation does not mean the full process arrangements are equivalent. For example, copying data forward and making release contingent on independent review are different claims, even if both occur around the same invoice.

```text
Source segment → Descriptive observation → Proposed operation and relation
               → Within-case configuration → Cross-case pattern → Bounded claim
Do not skip directly from the feature label to the last box.
```

## 3. Worked example: three ways an earlier record matters

[Malone and Crowston (1994)](https://crowston.syr.edu/sites/default/files/acmcs94.pdf) put dependencies between activities at the centre of coordination analysis. Apply that question here: what does each later task take from the earlier record, and what consequence does the source represent?

| Case and locator | Direct observation | Organisational reading and limit |
|---|---|---|
| J45-W07-16, IVA steps 1 to 8 and 10 to 12 | A PO reference populates invoice items. The processor still performs checks. | Purchasing data become input to later invoice work on this route. This does not show that a PO is required on all routes or that all supplied values are accepted unchecked. |
| BD9-W08-12, POD steps 3 to 8 | Confirmed quantities are used for billing on the optional proof-of-delivery route. | Shipping's confirmation supplies an operative billing value in this branch. It is not a universal requirement for billing or proof of successful delivery in practice. |
| J58-W08-11, RST steps 3 to 5 | The reset procedure uses the prior clearing document number and company code. | The earlier record identifies the clearing arrangement to which the action applies. This is not evidence that an earlier quantity is copied, or that the original journal entry is reversed. |

First test the narrow proposal: **all three transfer business values into the next activity**. J45 and BD9 support particular versions of that statement. J58 does not support it: the earlier reference helps identify the target of a corrective action. Now test a broader formulation: **an earlier record mediates a later action in each selected branch**. That is defensible if the comparison preserves the differences: supplying invoice items, supplying a confirmed quantity and identifying a prior state. The broader formulation is not permission to code them all as the same kind of transfer.

```text
Earlier record is used
  ├─ J45: supplies invoice items → the processor checks the resulting entries
  ├─ BD9: supplies confirmed quantity → billing uses it on the optional route
  └─ J58: identifies prior clearing → the reset acts on that arrangement
```

BD9 gives a useful contrast within the same case. In delivery creation, sales-document and shipping criteria help select work (BD9-W08-08). In proof of delivery, the confirmed quantity is used by billing (BD9-W08-12). A record can have more than one organisational use even within one scope item. In J45, the optional no-reference invoice procedure takes different accounting inputs (J45-W07-19). This does not eliminate checks or disprove the PO dependency on the referenced route. It rules out calling that dependency universal. In J58, direct posting is a separate example (J58-W08-01), not an alternative way to reset clearing; it bounds broad claims about accounting work rather than refuting the reset dependency.

**Rival: these are just identifiers or interface conventions.** A common form design might explain why a field appears. It cannot, by itself, account for the documented value use in J45 and BD9. For J58, the rival is more informative: an identifier is a technical means of selecting the correct object, and that technical role is compatible with the organisational reading that the correction is scoped to a particular earlier clearing arrangement. Do not claim to refute a technical explanation that is consistent with the evidence. State what the organisational interpretation adds: what work is made dependent on which earlier input or state.

**Bounded result:** In these selected Swiss reference branches, earlier records shape later action in different ways. PO items and confirmed quantities supply values in two cases; the clearing reference identifies the object of a corrective operation in the third. The evidence concerns represented dependencies, not measured efficiency, common understanding or the effectiveness of the controls.

## 4. A contrast is not always a counterexample

A **negative case** is evidence that would contradict a proposed claim if the claim applies to that case. To count as one, it must fall within the claim's scope. An authorised no-PO route is negative evidence against “all J45 supplier invoice entry requires a PO”; it is not negative evidence against “the PO-referenced route uses a prior PO”. A direct posting example does not refute a claim about how a journal entry behaves after being submitted to verification. Read the scope before naming the counterexample.

| What you found | How to handle it |
|---|---|
| The same operation has different documented effects in two branches. | Narrow the claim or distinguish variants. |
| A distinct in-scope route contradicts a universal claim. | Reject or rewrite the claim. |
| A superficially similar route concerns a different object or condition. | Use it as a contrast, not a disproof of the narrow claim. |
| The next step is not documented in the inspected material. | Mark it unknown. Do not turn missing evidence into evidence that the action is impossible. |

```text
Does this case fall inside the claim?
    no  → Use as a boundary contrast if informative
    yes → Does it show a different result, or is the evidence incomplete?
              Different → Reject, narrow or distinguish variants
              Incomplete → Mark unknown and state what would resolve it
```

Do not count repeated mentions as independent support. An overview, screenshot and instruction may all point to the same operation. Three titles using the word “approval” are not three observations of what approval does. Conversely, a well-located exception that changes what can happen is important even if it occurs only once in the corpus.

**Worked boundary check: a neighbouring process is not a demonstrated interface.** The registered J45 material lists Accounts Payable J60 as a succeeding process; BD9 lists Accounts Receivable J59. See J45-W07-24 and BD9-W08-18 in the [source-locator table](../../../figures/Table_07_Findings_Source_Locators.md). This tells us where the reference points next. It does not show which data crossed, the cardinality of the relation, how an exception was handled or whether any cash moved. Treat a neighbouring scope as a route for further inquiry. To claim a designed handoff, locate the input and output on both sides and explain the connection. To claim a same-instance link in practice, obtain appropriate linked records from an implementation. A shared vendor and similar identifiers are not enough.

## 5. Put the theory to work without forcing agreement

Begin with the operation. Then use a lens that answers a real question about it. Coordination theory asks which dependency is managed. Information processing asks what is made usable and for whom. Decision theory asks which facts or conditions shape a choice and who can depart from them. Governance asks who can act, who can intervene and what can be challenged. A strong comparison connects at least two lenses when they reveal different things. It need not invent an instance of every concept in every case.

For example, in BD9 a confirmed quantity can be evidence of an information dependency. It is not, without further evidence, proof that Shipping and Billing agree on what the confirmation means or that a particular person has formal authority to accept a deviation. In J58, a reset identifies an earlier accounting state and represents a corrective operation. Its existence does not establish the policy permitting its use or the independence of its review. You can ask the governance question even where the correct answer is “not shown here”.

Use the [analytical framework](../../../09_Analytical_Framework.md) to make a confidence judgement. Say what is well supported, which inference is plausible but weaker, and what the material cannot adjudicate. For example, the evidence can strongly support the difference between carrying a value and identifying a target. It is weaker for the claim that the same organisational purpose motivated both designs. It cannot tell us whether users rely on the represented path in everyday work. A useful confidence statement is tied to a particular claim, not a score for an entire case.

**Try a two-lens reconstruction.** In the optional BD9 proof-of-delivery procedure, separate the fact that a confirmed value feeds billing from the possibility of entering a deviation and reason. The first observation is about dependence: billing uses an input supplied earlier. The second is about represented discretion: Shipping can record a difference within the branch. Taken together, they suggest that this pathway can carry an adjusted representation forward rather than requiring the two tasks to start from the same unexamined quantity. They do not tell us who may settle a dispute or whether anyone used the option. To extend the claim, specify whether you need a source about access, a record of configuration, or an observation of practice. Each would answer a different question.

## 6. Independent studio: is a rework loop the same thing in all three cases?

Take this claim into the [studio exercise](../../exercises/M10_Test_a_Cross_Process_Pattern.md):

> Every documented return sends the same object back to its creator, and a revised object always re-enters approval.

Find the exact observation that supports or limits each part. Identify the initiating role, returned object, expected recipient, recorded reason or instruction, and represented continuation. Compare a purchase order, a sales order and a submitted journal entry. Do not join procedures into a single observed run. If a card says the creator should act but does not show the action, mark the completion unknown. If a step describes return only on a condition, preserve it in the claim.

Then test two alternative explanations. First, perhaps the recurrence is merely a common inbox convention. Ask what the source says happens after the notification. Second, perhaps every loop implies reciprocal interdependence. Ask whether the procedure shows mutual adjustment, or only a formal instruction and an opportunity for response. Do not look at the facilitator's worked reasoning before writing your own claim.

```text
Proposed common pattern → Best evidence per case → Strongest contrast or rival
                        → Retain, narrow or reject → Defend the revised claim
```

## 7. Defend the claim, then say what would change it

Use one comparison matrix and one clear claim in the oral defence. Start by naming the process and release boundary. Show the strongest step for your interpretation, then the hardest case for it. Explain what would make you change your mind. If someone asks why the pattern matters, say what it changes about who depends on whom, what is available for a decision or which action is possible. Do not answer by naming more SAP features.

| Question | Evidence that could answer it |
|---|---|
| Does the represented arrangement make sense within the selected branch? | Exact steps, conditions, expected states and relevant contrasts. |
| Did a particular organisation implement a suitable version? | Client requirements, design choices, configuration and scoped tests. |
| Do people actually handle the exception in the represented way? | Cases in use, records, observation and interviews across the involved functions. |
| Did the arrangement improve an outcome? | Defined measures, a relevant baseline or comparison, and a way to examine rival explanations. |

**Consulting transfer.** If the reference shows a return route, a Fit-to-Standard team can ask which condition should trigger it, who receives it and what counts as resolved. It cannot tell the client that rework will be faster. A TOGAF-informed gap statement can connect the current and desired responsibilities and information, but it is still a proposed design. Follow [Module 9](../09_SAP_Activate_and_Transformation/01_Student_Lesson.md) to convert that question into a requirement and a test rather than a claim about transformation success.

Before you submit, check: Can a reader locate every important observation? Is the difference between records supplying values and identifying a target clear? Did you try to disconfirm the claim? Did you distinguish unknown from absent? And can you explain what the comparison teaches without assuming that all SAP processes, releases or customers behave alike?

Complete the studio, then use the [comparative project brief](../../assessments/M10_Integrative_Comparative_Project.md) to plan the independent submission.
