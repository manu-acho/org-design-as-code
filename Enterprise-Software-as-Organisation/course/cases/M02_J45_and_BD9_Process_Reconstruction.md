# Case EP-CH-01: Reconstruct the documented process

**Documentary dossier · Module 2 · Draft for teaching review**

This dossier compares two examples of how work moves between teams. In procurement, a purchase order supplies information for recording goods received and entering a supplier invoice. In sales, an earlier order helps Shipping select work for delivery. Part A is worked through in the lesson. Part B is for independent practice.

The cards summarise SAP reference procedures and their expected results. They show how work is designed to proceed, not what happened in a particular company or transaction. No SAP login is needed.

## A. Worked dossier: J45, Procurement of Direct Materials

**Boundary:** selected procurement entry and purchase-order creation through receipt and supplier invoice procedures, with the neighbouring payment scope noted. This is not the entire P2P process.

| Card | Represented observation | Locator |
|---|---|---|
| A1 · J45-W07-02 | Purchasing selects a requisition, retains or assigns a source and creates a PO. The requisition is expected to show a PO-created status. | [CON: Convert Purchase Requisitions to Purchase Orders](https://help.sap.com/docs/s4hana-cloud-best-practices/procurement-of-direct-materials-j45-ch/convert-purchase-requisitions-to-purchase-orders?locale=en-US&state=PRODUCTION&version=2608.1), steps 3 to 8. |
| A2 · J45-W07-03 | A separate direct order example creates a stock-material PO without requisition conversion. | [DIR: Create Purchase Order](https://help.sap.com/docs/s4hana-cloud-best-practices/procurement-of-direct-materials-j45-ch/create-purchase-order?locale=en-US&state=PRODUCTION&version=2608.1), purpose and steps 1 to 4 and 7. |
| A3 · J45-W07-13 | The Warehouse Clerk uses the PO ID to load receipt data. The expected result of posting includes a material document identifier. | [GR: Post Goods Receipt](https://help.sap.com/docs/s4hana-cloud-best-practices/procurement-of-direct-materials-j45-ch/post-goods-receipt?locale=en-US&state=PRODUCTION&version=2608.1), steps 1 to 6. |
| A4 · J45-W07-16 | Accounts Payable uses the PO reference to populate invoice items, then checks the invoice. Posting is the expected result. | IVA steps 1 to 8 and 10 to 12 in the locator table. |
| A5 · J45-W07-18 | A separate invoice-reduction example addresses amounts and quantities above PO values. A companion procedure can retrieve and print a complaint letter. | IVB steps 4 to 11; LTR steps 3 to 5 in the locator table. |
| A6 · J45-W07-19 | The optional no-PO/GR-reference route uses accounting inputs and represents checks before posting. | NOP steps 1 to 8 in the locator table. |
| A7 · J45-W07-24 | The reference lists outgoing payment as a succeeding Accounts Payable process, J60. | SUC table, Accounts Payable J60 row; PUR overview in the locator table. |

A1 and A2 differ at order creation. A3 and A4 show different uses of an earlier PO, not a proven compulsory link from the material document to the invoice. A5 is a documented response under stated example conditions, not every mismatch. A7 identifies a boundary, not a payment.

## B. Independent dossier: BD9, Sell from Stock

**Boundary:** start with delivery creation using an earlier sales document; map selected outbound delivery and billing examples. Stop at the saved billing document and name the neighbouring Accounts Receivable scope.

| Card | Represented observation | Locator |
|---|---|---|
| B1 · BD9-W08-08 | Shipping uses the earlier sales document and shipping criteria to select work. The procedure expects a delivery and number in the log. | DEL, Create Delivery steps 1 to 5 in the locator table. |
| B2 · BD9-W08-09 | Shipping selects the outbound delivery and records picked quantity. The separate issue procedure represents posting goods issue. | [PCK: Execute Picking](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/execute-picking?locale=en-US&state=PRODUCTION&version=2608), steps 1 to 9; [GI: Post Goods Issue](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/post-goods-issue?locale=en-US&state=PRODUCTION&version=2608), procedure steps 1 to 4. |
| B3 · BD9-W08-11 | In an optional delivery split, selected items are assigned to a new delivery document; other items remain on the original. | [SPL: Split Outbound Delivery (Optional)](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/split-outbound-delivery-optional?locale=en-US&state=PRODUCTION&version=2608), steps 1 to 7. |
| B4 · BD9-W08-12 | On the optional proof-of-delivery route, a deviation and reason can be entered and the confirmed quantity is used for billing. | POD steps 3 to 8 in the locator table. |
| B5 · BD9-W08-13 | The billing example selects from a due list, creates a draft and saves a billing document. Its example turns automatic posting on. | [BIL: Create Billing Document](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/create-billing-document?locale=en-US&state=PRODUCTION&version=2608), Create Billing Document steps 1 to 6 and 10. |
| B6 · BD9-W08-18 | Accounts Receivable J59 is named as a succeeding scope. | SUC table, Accounts Receivable J59 row; PUR overview in the locator table. |

Use the [reconstruction exercise](../exercises/M02_Reconstruct_a_Process.md) before opening the worked answer.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Procurement of Direct Materials (J45) and Sell from Stock (BD9) (J45 procedures labelled 2608.1; BD9 SAP Help links specify 2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
