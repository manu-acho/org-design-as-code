# Case CP-CH-01: Three Swiss reference processes, two comparisons

**Documentary teaching dossier · Module 10 · Draft for teaching review**

Earlier records can supply invoice items, provide a quantity for billing or identify which accounting action to undo. Part A asks whether those records do the same job. Part B asks a different question: when work is returned for changes, does it always go through approval again? Use the first comparison as a worked example and the second for independent practice.

The cards summarise separate SAP procedures and expected results. They do not record tests run for this course or show one transaction across the three processes. Use the step locations to justify a claim. No SAP login is required.

## A. Worked comparison: earlier records and later actions

| Card | Documented observation | Locator |
|---|---|---|
| A1 · J45-W07-16 | The PO reference populates invoice items. The procedure represents checks before posting. | IVA steps 1 to 8 and 10 to 12. |
| A2 · BD9-W08-12 | On the optional proof-of-delivery route, the confirmed quantity is used in billing. | POD steps 3 to 8. |
| A3 · J58-W08-11 | The reset procedure uses the earlier clearing document number and company code. | RST steps 3 to 5. Do not use the automatic-clearing portion as proof of a same-instance reset. |
| A4 · J45-W07-19 | A separate optional invoice-entry procedure uses accounting inputs without a PO or GR reference and retains checks. | NOP steps 1 to 8. |
| A5 · BD9-W08-08 | Selection for delivery creation uses a sales-document reference and shipping criteria. | DEL, Create Delivery steps 1 to 5. |

Read the [worked comparison](../modules/10_Comparative_Process_Analysis/01_Student_Lesson.md#3-worked-example-three-ways-an-earlier-record-matters) after trying to classify each use of the earlier record yourself.

## B. Independent studio: returned work and what happens next

| Card | Documented observation | Locator |
|---|---|---|
| B1 · J45-W07-11 | Where rework is configured, the Purchasing Manager requests it with a reason. The procedure instructs the creator to edit the purchase order, but does not show creator-side completion. | RWK procedure introduction, steps 1 to 3 and closing instruction; RCF step 3 for configuration context. |
| B2 · BD9-W08-05 and BD9-W08-06 | The represented Sales Manager can request rework and submit comments. Internal Sales can respond in the inbox or change the sales order; the change procedure describes a conditional return to approval. | AP steps 1 to 5; RW note; NT steps 1 to 4; CHG steps 1 to 5. The related procedures do not demonstrate a completed transaction. |
| B3 · J58-W08-07 | A rejected verification request returns with a reason. The requester checks the history, edits and resubmits the journal entry. | REJ purpose and steps 1 to 3; EDT steps 3 to 4. This is not a reversal of a posted entry. |
| B4 · J58-W08-01 | A separate direct posting procedure represents journal posting without the verification submission shown in B3's branch. | PUR overview; PST steps 1 to 5. |

The B cards vary in what they show. Treat “creator is instructed to act”, “another role can respond or change”, and “requester edits and resubmits” as distinct evidence. Do not infer actual identity, reciprocal interdependence, realised correction or the effectiveness of governance. A direct posting route is a boundary contrast unless the claim covers that route.

Use the [studio brief](../exercises/M10_Test_a_Cross_Process_Pattern.md) before looking at the facilitator's worked defence.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Procurement of Direct Materials (J45), Sell from Stock (BD9) and Accounting and Financial Close (J58) (2608.1 for J45, 2608 in the BD9 SAP Help links, and 2608 for J58). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
