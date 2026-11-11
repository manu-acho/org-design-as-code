# Case GC-J58-01: An approval, a substitute and a missing explanation

**Documentary evidence and fictional workshop brief · Module 8 · Draft for teaching review**

An approval record names the user account that recorded the action. Can it show that the review was independent? Compare how an accounting entry can be approved, forwarded, returned for changes or posted directly in separate SAP procedures. Then test what an approval record can establish in the fictional Cedar Distribution exercise. No SAP login is required.

## A. Documentary evidence

| Card | What the registered procedure represents | Locator |
|---|---|---|
| A · J58-W08-05 | The requester submits for verification before posting. The processor approves, and posting is the expected result in this example. | VER purpose and requester steps 3 to 7; APP processor steps 1 to 4. |
| B · J58-W08-06 | One procedure enables the approval posting-authorisation check as a scenario option. The forwarding procedure records a note and describes a company-code posting-authorisation check on the proposed new processor. | AUT purpose and steps 1 to 3; FWD purpose and steps 3 to 6. |
| C · J58-W08-07 | Rejection returns the entry with a reason. The requester checks the history, edits and resubmits. | REJ purpose and steps 1 to 3; EDT steps 3 to 4. |
| D · J58-W08-01 | A separate direct posting example represents posting debit and credit lines with dates, period, company code, accounts and assignments. The cited sequence does not show submission for verification. | PST steps 1 to 5. |

These are separate procedures, not a trace of one entry. They do not establish actual segregation, universal verification, enabled controls in a particular tenant, override permission or an accountability forum. A posting-authorisation check is not, by itself, proof that the substitute has independent business authority. Card D is a counterexample to treating the verification branch as the only represented route, not evidence that a client entry in scope for verification can bypass it.

## B. Fictional client: Cedar Distribution

Cedar's stipulated policy requires independent review of material close adjustments within scope before posting. A preparer must not approve their own entry. The assigned reviewer is unavailable. The client has not settled who can substitute, how that right is verified, or who reviews emergency departures. The workshop is about designing and testing those rules, not making an accounting determination.

Below is an **invented partial extract**, not an SAP screen, schema or expected system output. It deliberately omits version history, policy and evidence references.

| Time | Entry | Recorded account | Event |
|---|---|---|---|
| 16:20 | C-17 | PREP-A | Submitted for review |
| 16:42 | C-17 | REV-B | Forwarded for review |
| 16:58 | C-17 | REV-C | Approved |
| 16:59 | C-17 | BATCH-D | Posting recorded |

The extract shows different account labels, not proven distinct people or independent review. It does not prove the records refer to the same version of the entry, what the reviewer saw, whether the forwarding rule was checked or why approval was appropriate. Treat “adequate independent review” and “a procedural acknowledgement with little scrutiny” as rival interpretations.

**Workshop challenge:** Compare forwarding to an independent authorised substitute, holding and escalating, and a narrowly specified departure from an otherwise applicable requirement. The prohibition on self-approval is not negotiable in this exercise. If the proposed departure does not change a rule, it is not an override. If no eligible reviewer is available, explain the safe alternative.

Use the [exercise](../exercises/M08_Test_a_Control_and_Trace.md) before reading the worked reasoning.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Accounting and Financial Close (J58) (2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
