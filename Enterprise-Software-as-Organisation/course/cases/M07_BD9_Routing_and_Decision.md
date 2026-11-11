# Case DT-BD9-01: The amount routes the order. Who decides?

**Documentary evidence and fictional workshop brief · Module 7 · Draft for teaching review**

A rule sends a sales order to a reviewer. It does not tell the reviewer whether to accept it, reject it or return it for changes. Part A separates those decisions in the SAP procedures. Part B asks what a fictional distributor should do when an order falls below the usual amount threshold but involves an unusual delivery promise. No SAP login is needed.

## A. Documentary evidence

| Evidence card | What the registered procedure represents | Locator |
|---|---|---|
| A · BD9-W08-04 | An ordered setup example has an amount-conditioned workflow for net value above CHF 1,000 with a Level 2 release step, and another definition without conditions with a Level 1 release step. | WF steps 1 to 10. |
| B · BD9-W08-05 | The represented Sales Manager receives an approval task and can choose release, rejection or rework and submit the decision. | AP steps 1 to 5; ROL, Sales Manager row. |
| C · BD9-W08-06 | A documented rework path allows Internal Sales to handle a returned order. The change example describes a conditional return to approval, not an unconditional restart. | RW note; NT steps 1 to 4; CHG steps 1 to 5. |

The cards summarise procedures and expected effects, not a transaction trace. Do not infer a universal threshold, sequential Level 1 and Level 2 approvals, automatic approval of the unconditioned case, a credit decision, an override or actual customer authority from these cards. Do not combine the change example with the setup example to reconstruct a single effective threshold.

## B. Fictional client: Ridgeway Distribution

Ridgeway proposes a simplified policy for the exercise: orders **strictly above CHF 1,000** go to a senior reviewer and the other in-scope orders go to a standard reviewer. This classroom policy explicitly specifies the equality case. It is not a claim about the live execution of the SAP example. An unusual delivery commitment may require input from a planner, but the client has not decided whether the planner advises, must concur or has the right to decide.

| Order | Facts supplied for the workshop |
|---|---|
| A | CHF 999.99, routine delivery. |
| B | CHF 1,000.00, routine delivery. |
| C | CHF 1,000.01, routine delivery. |
| D | CHF 980, new customer and unusual delivery commitment. |
| E | CHF 1,020, unusual delivery commitment. |
| F | CHF 980, delivery commitment not yet known. |

For D, E and F, record what the amount rule would do separately from what the proposed target should do. If the client has not decided an expected route or right, label it unresolved. As a follow-up test, imagine D is changed after a rework request. Decide what policy would require review again. Do not assume the change restarts an SAP workflow.

Use the [exercise](../exercises/M07_Trace_a_Decision_Programme.md), then compare your work with the worked reasoning.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Sell from Stock (BD9) (SAP Help links specify 2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
