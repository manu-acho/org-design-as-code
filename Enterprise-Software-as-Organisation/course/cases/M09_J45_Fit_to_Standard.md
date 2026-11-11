# Case FTS-J45-01: One invoice process for two plants?

**Documentary evidence and fictional client brief · Module 9 · Draft for teaching review**

Alpine Pack Foods wants two plants to use a common way of handling supplier invoices without losing independent review. The SAP cards show that a payment block can hold an invoice back from payment and that a separate procedure can remove it. The workshop asks whether those actions are enough to meet the fictional client's requirement, and what the team would need to test before deciding. No SAP account, source downloads or screenshots are needed.

## A. Reference walk-through cards

| Card | What the reference represents | Exact locator and boundary |
|---|---|---|
| A · J45-W07-16 | On the PO-referenced route, the earlier purchase order supplies invoice items; the procedure represents further checks and expected posting. | IVA steps 1 to 8 and 10 to 12. This is not proof of mandatory three-way matching, independent review or payment. |
| B · J45-W07-17 | One procedure represents manual blocking at item level. Another starts with a payment-blocked invoice and represents a release action. | IVA step 9; REL steps 1 to 5. Separate examples, not a trace of one invoice. No automatic mismatch block, same-entry segregation or actual payment is demonstrated. |
| C · J45-W07-19 | An optional no-PO/GR-reference route uses accounting inputs and represents checks before posting. | NOP steps 1 to 8. The example does not establish when a particular client should allow the route or what its full production controls would be. |

The facilitator talks through the summaries rather than opening a live system. This is a guided reading of the reference evidence, not a product demonstration or a record of one invoice.

## B. Fictional client: Alpine Pack Foods

Alpine Pack Foods is a fictional Swiss packaged-food manufacturer with two plants. It is preparing a new Public Edition implementation. The workshop scope begins with entering a supplier invoice and ends with its posting or block and release disposition. Payment execution is downstream and out of scope, but the payment team needs to know which items are eligible for further processing. Purchase order and receipt facts are upstream inputs, not redesign targets in this session.

**Current arrangements.** Plant North often asks the buyer to obtain Receiving's explanation before Accounts Payable acts. Plant South uses a supervisor email to approve release. Both may refer to the same discrepancy as “not received” even when one means that no delivery arrived and the other means inspection is pending. Neither plant wants an unexplained payment release. These practices and requirements are invented, not findings from J45.

| ID | Requirement or preference | Who can confirm it? |
|---|---|---|
| FTS-01 | Reuse PO information where the purchase order exists, while allowing Accounts Payable to verify invoice data. | Accounts Payable process owner and Purchasing. |
| FTS-02 | For in-scope disputed invoices that are payment-blocked, the original entrant must not release the block. An eligible independent reviewer must be able to review and act. If none is available, retain the block and escalate. | Finance control owner; security and functional leads verify feasibility. |
| FTS-03 | Allow a legitimate no-PO invoice only where the client's approved coverage rule permits it. Do not use the alternative to avoid controls on an invoice that should follow the disputed-PO route. | Accounts Payable process owner and Finance control owner. The exact coverage categories remain open. |
| FTS-04 | Reconcile existing blocked items at cutover and give every unresolved item an owner and evidence route. An item must not become eligible merely because the system changes. | Data and cutover lead, payment team and Finance control owner. |
| FTS-05 | A supervisor asks to retain Plant South's email template. The client has not agreed that email itself is required. | Supervisor and control owner: identify what the message actually achieves. |

## C. Transaction cards and workshop roles

| Card | Fictional facts for discussion |
|---|---|
| N1 · Routine PO invoice | Invoice for 100 units with a valid PO reference; receipt evidence is available and there is no stated dispute. |
| N2 · Disputed PO invoice | Invoice claims 100; only 88 are confirmed accepted in the fictional case. Assume a payment block has already been recorded for the exercise. Do not infer the difference created it. |
| N3 · Legitimate no-PO candidate | A stipulated authorised non-PO charge for the exercise. The broader coverage rule and applicable checks still require client confirmation. |
| N4 · Attempted alternate route | The preparer tries to handle N2 without the PO reference. The dispute and the policy obligation have not changed. |
| N5 · Cutover item | A legacy blocked invoice has a pending Receiving explanation and no confirmed owner in the target arrangement. |

Assign a facilitator, a scribe, and voices for Accounts Payable, Purchasing/Receiving, Finance control and technical delivery. Combine roles in a small class. The facilitator describes the standard; the process and control owners explain the business requirement; the technical lead states what still needs verification. The scribe must not turn a suggestion into an approved decision.

Proceed to the [workshop exercise](../exercises/M09_Run_a_Fit_to_Standard_Workshop.md). Open the worked outputs after making a first attempt.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Procurement of Direct Materials (J45) (2608.1). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
