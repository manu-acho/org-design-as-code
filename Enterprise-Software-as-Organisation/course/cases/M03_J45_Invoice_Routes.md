# Case OD-J45-01: Two routes for recording a supplier invoice

**Documentary case · Module 3 · Draft for teaching review**

Accounts Payable needs to record a supplier invoice. In one reference procedure the accountant has a purchase-order reference. A separately documented optional procedure does not use a purchase order or goods receipt reference. This case asks what changes in the work, the information it uses and the checks it represents. It does not ask you to execute SAP transactions.

The cards summarise separate procedures rather than two ways of treating one observed invoice. A purchase order (PO) records what was ordered. A goods receipt (GR) records reported receipt. A general ledger (G/L) account classifies an accounting entry. A tolerance is a limit used to decide whether a difference is acceptable.

## Evidence cards

| Card | What the document represents | Exact source locator |
|---|---|---|
| A: J45-W07-16 | The accountant supplies an earlier purchase order. Its reference populates invoice items. The procedure checks amounts, quantities and taxes, checks balance against tolerance, simulates and posts. | [IVA: Option A, supplier invoice with PO/GR relation](https://help.sap.com/docs/s4hana-cloud-best-practices/procurement-of-direct-materials-j45-ch/option-create-supplier-invoice-with-po-gr-relation?locale=en-US&state=PRODUCTION&version=2608.1), steps 1 to 8 and 10 to 12. Step 4 is the PO-reference action. |
| B: J45-W07-19 | In the optional route the accountant provides G/L account items and cost-centre and tax details rather than a PO or GR reference. Consistency and tolerance checks precede posting. | [NOP: Supplier invoice without PO/GR (optional)](https://help.sap.com/docs/s4hana-cloud-best-practices/procurement-of-direct-materials-j45-ch/create-supplier-invoice-without-po-gr-optional?locale=en-US&state=PRODUCTION&version=2608.1), steps 1 to 8. |

The title of Card A does not establish that the purchase order, goods receipt and invoice must always be compared, a check known as a three-way match.

## Use the case

1. For each card, mark the actor, inputs, check and expected end state.
2. Identify what the second route changes and what it retains.
3. Test whether a reference is merely a convenient lookup or an input to the later task. Name the evidence that would distinguish the two readings.
4. Identify one claim you would refuse to make and explain what evidence is missing.

Use the [exercise](../exercises/M03_Compare_Invoice_Arrangements.md) for the submission format. The instructor guide contains the model reasoning and alternatives.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Procurement of Direct Materials (J45) (2608.1). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
