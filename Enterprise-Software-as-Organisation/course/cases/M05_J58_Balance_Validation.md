# Case IP-J58-01: A result is missing. What does that mean?

**Documentary evidence and fictional workshop brief · Module 5 · Draft for teaching review**

An accountant cannot see a result they expected. Was the check never run, or does the screen hide the result? Part A distinguishes what the accounting checks cover from what a reviewer can see. Part B asks how a fictional company could follow up on what it finds. The cards describe SAP's reference procedures; the company's policy is not part of them. No SAP login is needed.

## A. Documentary evidence

| Evidence card | What the registered procedure supports | Locator |
|---|---|---|
| A · J58-W08-14 | The scheduling example selects a rule group and accounting context, including ledger, currency, fiscal year and period. These inputs specify the intended scope; they do not show a completed job. | JOB steps 3 to 6; the companion rule setup RUL is background, not evidence that a run occurred. |
| B · J58-W08-15 | The results example looks up a validation result by company code and ledger, lets the accountant inspect rule detail, and provides a way to reveal successful checks not shown by default. | RES steps 3 to 6. |

The references do not provide a same-run execution trace, a customer's role assignments or permissions, evidence of what anyone noticed, or a documented transition from result inspection to posting control or close sign-off.

## B. Fictional client brief

**Company:** Northbank Foods, a fictional distributor. Local Finance has access to supporting entries; Central Finance reviews material exceptions across the group. The close lead is responsible for sign-off. The purpose of validation in this exercise is to direct follow-up, not to certify that the accounts are correct.

**Current arrangement:** A central reviewer can see a flagged balance and asks the local team for context by email. Replies may identify the balance but omit the fiscal period or review owner. A group summary does not reliably tell the close lead whether a local review is complete.

**Client requirement:** Before sign-off, the close lead must see material exceptions that remain open, their owners and their escalation status. The lead should not receive restricted supporting entries. Local Finance can investigate, but the client has not yet agreed who can close a case or what qualifies as material.

**Workshop challenge:** One accountant reports that an expected result is absent from the initial view. Another can see a flag but has no evidence of follow-up. Diagnose these as separate problems. For the missing result, distinguish what the run included from what the reviewer can see. For follow-up, identify the owner, the information they need and one thing you would test before recommending a solution.

Use the [formative exercise](../exercises/M05_Trace_Information_to_Action.md). After attempting it, compare your reasoning with the worked answer.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Accounting and Financial Close (J58) (2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
