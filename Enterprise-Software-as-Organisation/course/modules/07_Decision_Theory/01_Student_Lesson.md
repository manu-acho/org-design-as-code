# Decision Theory: Who decided before the approver clicked?

**Module 7 · Postgraduate · Week 9 · Student lesson draft**

[Module 6](../06_Knowledge_Boundaries/01_Student_Lesson.md) asked what happens when people share a record but give it different meanings. This lesson asks what happens once the problem is understood: who defines the criteria, who receives the case, which alternatives are available, and who can depart from the normal rule?

## 1. Two orders cross the same desk

**Fictional opening.** A distributor receives two orders. One is worth CHF 980 and comes from a new customer who needs an unusual delivery commitment. The other is worth CHF 1,020 and comes from a regular customer buying familiar goods. The company's proposed policy sends orders above CHF 1,000 to a senior reviewer and other orders to a standard reviewer. It does not yet say what to do with unusual delivery commitments.

The policy can sort the two orders consistently by value. It cannot tell us that the more expensive one is riskier, or that the standard reviewer can resolve the unusual commitment. Those are different judgements. When the reviewer opens an order, several choices have already been made: the organisation chose a monetary trigger, selected the people who receive each category, and decided which actions the reviewers can take.

```text
Policy owner chooses a criterion → Rule sorts the case → Reviewer chooses a response
         What counts?                  Who sees it?            What happens next?
```

The question is not just “who approved it?” It is also “who shaped the decision that was available to the approver?”

## 2. Simon: make choices under real limits

**Bounded rationality** means decision makers work with limits on information, time, attention and computational ability. Simon's [1955 article](https://digitalcollections.library.cmu.edu/node/48694) starts from what a person can actually learn and evaluate, rather than assuming they know all alternatives and consequences. **Satisficing** is one possible response: search for an option that meets an acceptable standard instead of trying to prove that it is the best of all possible options. This is not the same as being careless. It can be a reasonable way to act when searching further has costs.

Consider a replacement supplier for tomorrow's production run. A buyer could check whether each candidate can deliver by morning, meet the packaging specification and stay within the approved price. Finding a supplier that meets all three criteria might be enough to stop searching. This would be satisficing if those criteria define acceptability and the search stops there. If the buyer evaluates all eligible suppliers and selects the lowest price, that is a different procedure, even if the same supplier wins. A system log showing the final selection alone could not tell us which search happened.

```text
Need a replacement supplier → Define an acceptable option → Search the available set
    ├─ An option meets the criteria → May stop without ranking every supplier
    └─ None meets the criteria     → Search further, escalate or revisit the criteria
```

The organisation can make that search easier by supplying approved vendor records, specifications, deadlines and a route for exceptions. It can also make good alternatives hard to see if it narrows the list too far. Bounded rationality helps explain why such simplifications exist; it does not tell us which simplification is appropriate in every setting, or let us infer an individual user's reasoning from a screen.

## 3. A premise is something a choice is made from

In the fictional order example, **net value** is the order amount before applicable tax. The comparison depends on which amount the rule is configured to use. A **threshold** is the cut-off that changes the route: under the fictional policy, an amount strictly above CHF 1,000 sends the order to senior review.

In Simon's *Administrative Behavior*, an organisation can influence decisions by supplying **decision premises**: facts, goals, criteria and assumptions that guide a choice. The point is that the person making a local decision need not be the person who decided what counts as relevant evidence or an acceptable outcome. The [shared decision-theory review](../../../literature/Stream_03_Decision_Theory_Detailed_Review.md) develops the distinction between factual and value premises.

| Premise or input | Example in the fictional order policy | Question to ask |
|---|---|---|
| Factual premise | The order record shows a net value of CHF 1,020. | Which value was recorded, when, and on what basis? Could it be stale or wrong? |
| Value premise | Larger financial commitments should receive more senior review. | Why is extra scrutiny desirable? What other objectives might compete with it? |
| Operational rule | If the order is in scope and its net value is above CHF 1,000, send it to the senior reviewer. | Who set the trigger, how does it handle equality, and what happens outside scope? |
| Available response | A reviewer may send an unclear order back for more information. | Does the reviewer have the information, permission and authority to choose another response? |

A threshold is not simply a fact. The recorded amount is a factual input for the comparison. The choice to use value as a proxy for risk, and to set the cut-off there, expresses a policy judgement. A **default** is the outcome or option used when another condition or choice does not apply; a **fallback route** can send a case to a standard reviewer without approving it. Do not confuse either with evidence that the outcome was desirable.

**Worked contrast: preselected, mandatory or fallback?** In a fictional order review form, “Request more evidence” might be preselected but editable. That is a default that can influence attention without taking the choice away. A policy might instead require an exception category before submission. That is a mandatory input; it does not necessarily mandate *which* category is selected. A policy could go further and require a particular category under stated conditions. Finally, sending every in-scope order that matches no special routing condition to a standard reviewer is a fallback route. It decides where work goes, not how the order is disposed of. None of these examples describes a delivered SAP setting.

| Arrangement | What to test | What a passing test would establish |
|---|---|---|
| Editable preselection | Replace the suggested response with another allowed choice and submit. | The suggestion guides the choice without binding it. |
| Mandatory input or value | Try leaving the required field blank; if policy requires a particular value, also try submitting a different one. | The configured requirement is enforced for the cases tested. |
| Fallback route | Submit an in-scope case with no special condition and inspect both its queue and its decision state. | The case routes to the expected reviewer without the routing event itself constituting approval. |

**Worked comparison.** If “above CHF 1,000” means strictly greater than CHF 1,000, then CHF 1,000 exactly does not satisfy that condition. CHF 999.99 and CHF 1,000.01 straddle the rule even though the orders are very similar. That sharp difference is useful for testing the configuration, but it is not evidence of a sharp change in risk. A good workshop asks both whether the comparison works and whether the cut-off is defensible for the business.

## 4. Programmes and automation: locate the judgement, then trace the effect

In *[Organizations](https://www.wiley.com/en-us/organizations-2nd-edition-p-9780631186311)*, March and Simon help explain how organisations handle recurrent situations without starting from scratch each time. A **decision programme** supplies a repeatable response or search procedure for a recognised situation. It may specify what to check, where to send a case or what action follows. It does not have to predetermine the whole decision. A programme can deliberately route a case to someone who must exercise judgement.

Separate these operations when reading an enterprise workflow:

| Operation | Illustrative example | What it does not necessarily show |
|---|---|---|
| Calculation or classification | Compare the recorded amount with a threshold. | A business decision about whether to accept the order. |
| Recommendation | Suggest requesting more evidence. | Authority to require rework or to release the order. |
| Routing | Assign the case to a review queue. | The recipient's business authority, technical access or actual judgement. |
| Decision | Choose to release, reject or return the case. | That the expected system effect occurred. |
| Authorisation | Establish who may perform an action and within what scope. | That the authority was exercised or respected in practice. |
| Execution | Record the choice or perform the next permitted action. | That the executing system or person chose the policy. |

```text
Before the case  → Select premises, thresholds, roles and exception rules
During the case  → Classify, route, interpret, decide and record
After the choice → Execute the permitted action; verify the resulting state
```

Automation can occur at more than one point. A system might calculate a comparison and route automatically, while a person chooses the disposition. In another design, a prior authorisation might trigger automatic execution. That does not mean nobody exercised judgement: some of it may sit upstream in deciding the rule or downstream in handling unusual cases. Nor does every configuration choice imply unchecked discretion. The ability to change a value may be constrained by policy, testing and change approval.

**Exception versus override.** Returning an order for missing evidence uses a provided response. An **override** would allow someone to depart from an otherwise applicable rule under specified conditions. An override needs its own basis: eligibility, an authorised actor, a reason and a way to review its use. A rework branch, a configurable threshold and an override are three different things. If the source shows only rework, do not assume there is an override or invent its effect.

**Worked example: the same urgent order, three different responses.** Under a fictional policy, a reviewer returns an order because a delivery commitment is unverified. That is rework: the original rule still applies once the missing information arrives. If policy lets a designated manager make a one-time departure from the normal review requirement, that is an override. If the organisation instead changes the rule for all future orders of this class, that is a policy or configuration change. Each leaves a different trace. Look for the information requested in the first case, the authority and reason for departing in the second, and the revised rule and its effective date in the third. The fact that all three might eventually lead to a released order does not make them equivalent.

```text
Rework       → Supply or correct information; the applicable rule remains
Override     → Authorised departure for a particular case; record why
Rule change  → Revise the programme for the defined class of future cases
```

## 5. Documentary case: the threshold routes; the reviewer chooses

The [Swiss BD9 evidence cards](../../cases/M07_BD9_Routing_and_Decision.md) describe a sales-order workflow setup and the corresponding approval task. In the setup example, an ordered definition uses a net value above CHF 1,000 with a Level 2 release step. A second definition has no conditions and uses a Level 1 release step. In the approval procedure, the represented Sales Manager can choose release, rejection or rework. Read this as a configuration example and a represented choice, not as a live order trace or a universal SAP threshold.

```text
Setup example:    Ordered definitions, one amount condition and one unconditioned definition
Approval example: Represented reviewer chooses release, reject or request rework
Rework example:   Change and return to approval only where the documented conditions apply
```

The level names do not establish two approvals in succession. Nor does an unconditioned workflow definition mean “approved automatically”. It describes a workflow with a release step and no start condition in the example. The setup and change examples do not justify composing a single effective threshold for every path. Finally, the choice concerns the sales-order approval example, not a credit decision and not the end of Order-to-Cash.

One rival reading is that a workflow merely delivers a notification. Routing alone would support that narrow reading. The documented options and the instruction to submit a disposition support a stronger claim: the procedure represents a reviewer choice with different follow-up paths. It still cannot establish that a particular reviewer exercised independent judgement, that all intended restrictions were configured, or that the chosen action had its expected effect.

**Contrast with Record-to-Report.** The [J58 locators](../../../figures/Table_07_Findings_Source_Locators.md) identify an example in which a requester submits a journal entry for verification before posting, and posting is the expected result after the processor's approval (J58-W08-05). In a separate forwarding example, a posting-authorisation check is documented under stated conditions (J58-W08-06). These examples help distinguish choosing, routing, checking an entitlement and executing an action. They do not make the BD9 and J58 mechanisms equivalent or prove that any customer's approval checks are enabled.

### Worked automation trace: who sets the rule, who acts, what changes?

**Fictional policy.** Ridgeway's Finance team wants to reduce manual reconciliation work, meaning work to compare records and explain differences. An **open item** is an accounting item not yet cleared, such as an invoice still waiting to be matched to a payment. **Clearing** links relevant entries and changes their status from open to cleared; it is not itself a payment. Ridgeway authorises automatic clearing for a specified class of open items only when the company code, which identifies the accounting unit, and the account are in scope, the pair has the same unique reference and currency, and the two amounts offset exactly. A missing or duplicate reference goes to manual review. This is an invented policy, not an SAP algorithm or accounting recommendation.

```text
Policy owner approves eligibility → Configuration team implements and tests it
    → Run checks scope, reference, currency and amount
       ├─ One eligible pair → Clear it and record the resulting state
       └─ No eligible pair or ambiguous match → Leave open for review
```

Two in-scope items for +CHF 500 and -CHF 500, with the same unique reference, satisfy the stipulated rule if the other conditions also hold. Two items with the same amounts but a missing reference do not. The comparison classifies each candidate; clearing changes the state. A job marked complete would not show that either pair cleared. Test the individual items and the record that links them to the resulting state.

Judgement has moved, not vanished. The policy owner decides whether the eligibility test is acceptable. The configuration team implements changes under agreed approval; it does not thereby own the policy. An authorised data steward can investigate and correct an erroneous reference using source evidence. An exception reviewer can investigate an unresolved case, not silently relax the rule. These are roles in the fictional design. In a real implementation, verify who holds each right and which actions are technically available.

**What the SAP example adds.** The Swiss J58 procedure describes automatic clearing of qualifying items and generation of a clearing document. A separate reset procedure uses the earlier clearing document number and company code. Resetting clearing is not, by itself, reversal of the underlying journal entry. These procedures do not establish Ridgeway's fictional eligibility rules, data roles or exception route.

**Source:** J58-W08-11, ACL purpose and steps 1 to 3; RST steps 3 to 5 in the [source-locator table](../../../figures/Table_07_Findings_Source_Locators.md). This summary describes the reference procedures, not a clearing run observed in practice.

## 6. Permission is not effective authority

An approval button represents an available action in the procedure. **Technical permission** is whether an identified user can perform it under a particular setup. **Formal authority**, in [Aghion and Tirole's (1997) distinction](https://dash.harvard.edu/entities/publication/73120378-825e-6bd4-e053-0100007fdf3b), is the right to decide; **real authority** is effective control over the decision. Information and initiative can matter to that control. Simon's account of **accepted authority** asks a different question: whether another person's decision is accepted as a premise for action. Do not treat the two theories as interchangeable.

Imagine a manager has the formal right to approve orders, but an experienced planner is the only person who understands a delivery constraint. If the manager consistently defers to the planner's judgement, the planner may effectively shape that part of the decision. The planner's influence does not show that the planner has formal authority or permission to approve. Conversely, a manager may weigh the planner's recommendation and independently decide. The same approval log could be consistent with either interpretation.

```text
Who can click?       → Inspect configured authorisations and try a controlled negative test
Who should decide?   → Check the applicable policy and delegation
Who shaped the choice in practice? → Trace evidence, recommendations and responses in real cases
```

This is the link back to Modules 5 and 6. A manager may have the right to decide but lack usable information. A specialist may understand the issue but lack a formal route to influence it. Changing a role assignment is not a remedy for missing facts or conflicting definitions. Design the information path and the decision right together.

## 7. Consulting studio: test the edge case, not just the normal order

Return to the [fictional client brief](../../cases/M07_BD9_Routing_and_Decision.md). The current proposal routes by amount. The desired arrangement must also bring unusual delivery commitments to someone who can assess them. The SAP example does not establish that the client's requirement is implemented. First write down what counts as unusual, who can recognise it, what evidence the reviewer needs and whether the specialist advises or decides.

Use a small TOGAF-informed baseline-target-gap comparison, building on [Module 5](../05_Information_Processing/01_Student_Lesson.md). The gap might be a missing escalation responsibility, a missing indicator or an unclear combination rule when both amount and delivery conditions apply. One option is to have the standard reviewer seek advice before making a choice; another is to propose routing defined exceptions to a specialist reviewer. Which is better depends on whether the client needs advice, an independent decision or a veto. Both are proposed designs, not claims about delivered SAP functionality.

```text
Client policy → Required facts + decision owner → Candidate rule or handoff
             → Test normal, boundary and exception cases → Verify actual system effects
```

Test the amount rule just below, at and just above the cut-off. Test a low-value order with an unusual commitment and a case with both triggers. Ask what should happen when the indicator is unknown. Test whether a user outside the authorised role can act, and whether an edited case must be assessed again under the agreed policy. Specify the expected route and the expected decision state separately. If stakeholders have not agreed an expected result, record the open policy decision rather than treating the test as passed or failed.

Before moving on, explain why a configured route is not the same as an exercised decision, why a log can be useful without showing independent judgement, and why an exception is not necessarily an override. Then complete the [decision-programme exercise](../../exercises/M07_Trace_a_Decision_Programme.md). [Module 8](../08_Governance_and_Control/README.md) asks how organisations establish, challenge and review the use of these decisions.
