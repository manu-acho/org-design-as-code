# Case EO-BD9-01: A delivery number is not a delivery to the customer

**Introductory documentary case · Module 1 · Draft for teaching review**

A shipping team creates a delivery record. What does that show about the goods, and what is still unknown? Compare how the earlier sales order helps the team select work with how a confirmed quantity is used to prepare a bill. The cards summarise two SAP procedures, not two steps observed on one order. No SAP account or prior experience is needed.

**Key terms:** A *shipping point* is an organisational element used for shipping; here it helps select the work. A *sales document* is the earlier record referred to in Card A. *Billing* is the preparation of the charge or invoice, not evidence that a customer paid it.

| Card | What the source represents | Exact locator |
|---|---|---|
| A · BD9-W08-08 | Shipping uses a shipping point, planned date and earlier sales document as selection inputs for delivery creation. The procedure expects a delivery record and a number in its log. | DEL, Create Delivery steps 1 to 5. |
| B · BD9-W08-12 | In an optional proof-of-delivery procedure, a quantity deviation and reason can be entered. The confirmed quantity is used in billing. | POD steps 3 to 8. |

The procedures and their expected results do not establish physical fulfilment, actual customer behaviour, technical permission by shipping point, or compulsory receipt confirmation before every billing transaction. The fictional grocery example in the lesson is independent of these cards.

Use the [annotation exercise](../exercises/M01_Annotate_a_Reference_Artefact.md); then compare your reasoning with the worked answers.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Sell from Stock (BD9) (SAP Help links specify 2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
