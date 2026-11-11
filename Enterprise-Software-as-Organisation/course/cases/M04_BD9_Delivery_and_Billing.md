# Case CO-BD9-01: Selecting delivery work and supplying a billing quantity

**Documentary case · Module 4 · Draft for teaching review**

Two SAP reference procedures connect one activity to another through a record. The first concerns finding items to create a delivery. The second concerns a confirmed quantity used in billing. Analyse the two independently before comparing them.

The cards summarise separate procedures, not events observed on one order. The comparison is between identifying which work to do and supplying a value the next team uses.

## Evidence cards

| Card | What the procedure represents | Exact locator |
|---|---|---|
| A · BD9-W08-08 | Shipping uses shipping point, planned date and the earlier sales document to select work for delivery creation. The expected result is a delivery with a number in the delivery log. | [DEL: Create Delivery](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/create-delivery?locale=en-US&state=PRODUCTION&version=2608), Create Delivery steps 1 to 5. |
| B · BD9-W08-12 | In the optional proof-of-delivery route, Shipping can record a deviation and reason, then confirm and save. The confirmed quantities are used in billing. | [POD: Proof of Delivery (Optional)](https://help.sap.com/docs/s4hana-cloud-best-practices/sell-from-stock-bd9-ch/proof-of-delivery-optional?locale=en-US&state=PRODUCTION&version=2608), steps 3 to 8. |

The expected delivery record is not evidence of physical delivery. The documented use of confirmed quantity is not a universal prerequisite for billing. A shipping point used to select work is not on that basis an access restriction.

## Questions

1. What is the earlier activity or record, and what does the later activity do with it?
2. What is the mechanism in each card? How do selection criteria and a value used downstream differ?
3. What would distinguish an operative input from a record that is merely visible?
4. Name a condition each arrangement could support. What would you have to observe to show that it did?

Use the [formative exercise](../exercises/M04_Map_Coordination.md) for your submission. After attempting it, compare with the instructor reasoning.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Sell from Stock (BD9) (SAP Help links specify 2608). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
