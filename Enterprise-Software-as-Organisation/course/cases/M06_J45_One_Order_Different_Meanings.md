# Case KB-J45-01: One order line, four different questions

**Documentary evidence and fictional workshop brief · Module 6 · Draft for teaching review**

A buyer, a warehouse clerk and an invoice processor can refer to the same purchase order while answering different questions. First examine what the order supplies to invoice entry. Then use the fictional damaged-delivery scenario to work out what each team knows and what still needs deciding. No SAP account is needed.

## A. Documentary evidence: what the purchase order supplies

| Field | Record |
|---|---|
| Evidence ID and scope | J45-W07-16, IVA steps 1 to 8 and 10 to 12. This card concerns PO-referenced supplier invoice entry and represented checks, not end-to-end payment. |
| Observation | The earlier purchase order reference populates invoice items. The procedure represents checks of amounts, quantities and taxes. |
| Interpretation and rival | Item population supports a stronger transfer claim than lookup alone. The order can still be just a structured input in this procedure; there is no evidence here that people use it to negotiate meanings or resolve a dispute. |
| Limits | No customer transaction trace, inspection, agreement, payment decision or universal three-way matching claim. The procedure title refers to PO/GR, but the coded entry step uses a PO reference. |

## B. Fictional client: Alder Foods

Alder Foods orders **100 cartons** of packaging on one purchase order line. Receiving physically counts **100**. It sets aside **12** because of visible damage. The supplier invoices **100**. The plant says it needs **90 usable cartons** by tomorrow. No inspection outcome, accepted quantity or payable quantity is stipulated. These numbers and roles are teaching inputs, not values or behaviour copied from an SAP script.

| Role | What the role knows | Question to take to the group |
|---|---|---|
| Purchasing | What was ordered and what was communicated to the supplier. | What can we ask the supplier to confirm, replace or dispute? |
| Receiving | What arrived, what was counted and what was set aside. | Can we link the physical event and the observation to the right line? |
| Quality | How to inspect the material; the inspection has not concluded. | What evidence would let us say the cartons are usable? |
| Accounts Payable | What the supplier claims and what invoice evidence has been presented. | Which client rule and authorisation would justify the next action? |

**Facilitator constraint:** Compare waiting for inspection with investigating whether an undisputed portion could be treated separately. Do not select a payment result by arithmetic. The client must establish who can decide, what can be considered undisputed, and what the configured system can support. If there is insufficient evidence, recording an unresolved decision is a valid workshop result.

Proceed to the [exercise](../exercises/M06_Analyse_a_Shared_Object.md). Use the worked reasoning only after making a first attempt.

**Reference scope:** Swiss SAP S/4HANA Cloud Public Edition, Procurement of Direct Materials (J45) (2608.1). The cards summarise the reference procedures. See the [source-locator table](../../figures/Table_07_Findings_Source_Locators.md) for official sources.
