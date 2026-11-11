# SAP Activate and Transformation: When does a standard process fit?

**Module 9 · Postgraduate · Week 11 · Student lesson draft**

**Fictional opening.** Alpine Pack Foods is replacing two plants' invoice procedures with a shared process. At one plant, a buyer clears up delivery discrepancies by speaking to Receiving. At the other, Accounts Payable asks a supervisor before removing a **payment block**, a restriction that holds an invoice back from payment. Removing the block is a **release**. It does not mean the supplier has been paid. The project team can show that SAP represents a block and a release action. The finance lead asks, “Does that mean we can keep our independent-review rule?” The demonstration does not yet answer it.

This module moves from interpreting an architecture to making and verifying an implementation choice. The workshop compares a documented standard process with fictional client requirements, then follows an unresolved issue through decision, planned work, testing and operational review. It builds on [coordination](../04_Coordination_and_Interdependence/README.md), [knowledge boundaries](../06_Knowledge_Boundaries/README.md) and [governance](../08_Governance_and_Control/README.md). It is neither SAP exam preparation nor a configuration guide.

## 1. SAP Activate: a lifecycle, not just a workshop

**SAP Activate** is SAP's implementation method. Its **roadmap** organises work into phases, from considering the change through operating the new arrangement. SAP's [Public Edition roadmap orientation](https://learning.sap.com/courses/administrating-sap-s-4hana-cloud-public-edition/understanding-the-significance-of-sap-activate-roadmaps-for-the-administrator_f0dbeeb9-20a2-4b80-a602-e9fdbcb7edaa) describes six phases. The applicable roadmap depends on the product, deployment and project. Two terms help with the table: **playback** means showing stakeholders the configured behaviour and checking earlier assumptions; **cutover** means switching work to the new arrangement, including deciding how open items will be handled. The questions and outputs below are original teaching examples, not prescribed SAP deliverables.

| Phase | Question for Alpine Pack | What the next team needs |
|---|---|---|
| Discover | Why consolidate invoice handling, and what belongs in the initial scope? | An agreed purpose, candidate scope and a baseline for evaluating value. |
| Prepare | Who can speak for the two plants and make decisions? What evidence and environment are ready? | Scope boundaries, participants, example transactions, workshop access and governance. |
| Explore | What does the reference process cover? Which needs, values and decisions remain open? | A fit assessment and prioritised requirements with owners, evidence and next checks. |
| Realize | Does the chosen design work with the selected configuration, data, integrations and roles? | Configured increments, evidence from playback and testing, and unresolved defects or risks. |
| Deploy | Can the organisation switch over without losing ownership of open items? | Reconciled cutover data, trained roles, support handover and an explicit readiness decision. |
| Run | Are people using the intended route? What changes when the software or policy changes? | Operational evidence, support and improvement actions, and regression checks after relevant changes. |

The phases describe the direction of delivery; they do not mean every uncertainty is settled in Explore. A playback in Realize may reveal that an identifier is not available where the workshop assumed it would be. The team should revisit the requirement and its rationale, rather than quietly build a different solution. A **quality gate** is a point to evaluate whether the evidence is adequate to proceed. Completing a workshop does not by itself settle a high-risk design decision.

```text
Discover → Prepare → Explore → Realize → Deploy → Run
                      scope     playback   cutover   observe
                      + fit     + tests    + support + improve
                        ↑          |
                        └── New evidence may reopen a design decision
```

A **phase** asks when something needs to be decided or delivered. A **workstream** groups related work across time. In [SAP's methodology overview](https://learning.sap.com/courses/discovering-sap-activate-implementation-tools-and-methodology/describing-the-methodology-structure_d959f6fc-ebfc-4143-94b3-6b83a6339b8b), workstreams cover areas such as design and configuration, testing, integration, data management, solution adoption, and operations and support. These responsibilities need to meet around the same requirement. If an open invoice transfers at cutover but its underlying block or supporting reason cannot be reliably reconciled, that is not only a migration issue: it affects payment controls, process ownership, testing and support. Do not assume the objects or fields can be migrated unchanged. Investigate, reconcile, and agree the treatment before go-live.

## 2. What Fit-to-Standard does, and what it does not do

**Fit-to-Standard** starts by showing the standard process under consideration. The team then asks which client needs it meets, what settings are needed, and which requirements remain unresolved. For Alpine Pack, that means showing the documented release action before asking how independent review would be enforced. The workshop neither starts from a blank sheet nor promises to reproduce the current process.

SAP's [workshop guidance for Public Edition](https://learning.sap.com/courses/implementing-sap-s-4hana-cloud-public-edition/conducting-fit-to-standard-workshops_d2850fb4-a4e5-4e36-a366-de35b309a550) places these sessions in Explore. The **Starter System** is where the team demonstrates the standard process. Its demonstration roles are not the design for who can act in the live system. The **Business Driven Configuration Questionnaire (BDCQ)** collects the choices and values the team needs to set up the process. **SAP Cloud ALM** is where the guidance describes recording individual requirements against the relevant processes. Recording a requirement is not configuring the solution; the guidance places subsequent configuration work in SAP Central Business Configuration and the development environment.

```text
Before: scope + standard scenario + client cases + decision makers
   ↓
During: demonstrate → ask what happens in the client's case → record evidence and choices
   ↓
After: assign owner → confirm decision or investigate → refine backlog → test and play back
```

Preparation matters. Invite the people who know what happens at the dock, who interpret the invoice and who can agree a payment-control change. Ask for one routine example and one difficult case. Check which release, localisation and scope item the reference covers. Agree what the workshop can decide and what must go to a process or control owner. For an end-to-end question, bring the adjacent team rather than assuming its work is represented by one department's process.

Keep three entries separate in the decision record:

1. **Reference observation:** what the artefact or demonstration actually showed, in its scope.
2. **Client requirement:** the outcome, obligation or operating condition the client needs, with its owner and reason.
3. **Proposed disposition:** use the standard route, set a supported value, change work, investigate a gap, or pursue another agreed response. Record whether the choice is provisional, approved, or unresolved.

A request such as “keep our email approval” names a proposed solution. Ask what it does: does it summon the right reviewer, preserve an explanation, or prevent unauthorised release? The answer determines what must survive. Conversely, do not dismiss a site-specific practice just because it differs. It may compensate for an information gap, reflect a genuine constraint or do work not visible to the central team. Ask for a recent case and a responsible decision owner. This is the organisational design work behind the workshop.

## 3. Diagnose the fit, then choose how to respond

[Strong and Volkoff (2010)](https://aisel.aisnet.org/misq/vol34/iss4/8/) identify misfits across functionality, data, usability, role, control and organisational culture. They distinguish **deficiencies**, where something needed is missing, from **impositions**, where the system requires something unwanted. The table applies these concepts to fictional workshop questions. It does not claim all six problems occur at Alpine Pack or are limitations of SAP.

| Lens | Example question |
|---|---|
| Functionality | Is there a route for the needed action, or only for a superficially similar action? |
| Data | Can we link a decision to the correct invoice and receipt evidence? Is a mandatory category meaningful at both plants? |
| Usability | Can reviewers find the evidence before the deadline, or does the intended workflow add steps they cannot realistically complete? |
| Role | Who can investigate, recommend and release? Does the proposed assignment assume expertise the role does not have? |
| Control | Is approval before release required, and do normal, substitute and alternative routes preserve that rule? |
| Organisational culture | Will people raise uncertainty, or does a local norm reward closing a case quickly even when evidence is weak? |

Consider a discrepancy field labelled “not received”. At one plant this means nothing arrived. At the other it means goods arrived but acceptance is pending. A field exists, so a functionality-only review may say “fit”. The common category may instead impose a misleading representation. A translation exercise with Receiving and Accounts Payable could resolve the meaning before anyone requests a new field. If the teams agree on meaning but disagree about what evidence is enough to release payment, the remaining issue is governance, not terminology.

**The response depends on the requirement, not on who suggested it.** A mandatory policy, a business preference and an assumption are not equal. Verify the source of any claimed obligation. If teams disagree about whether a requirement is mandatory, log the decision and owner. A workshop gap is a difference to investigate; it is not necessarily a defect, a product limitation or permission to build.

| Candidate response | When to consider it | Question before committing |
|---|---|---|
| Adopt standard | The supported route appears to meet the stated need. | Do representative data, roles and exceptions support that assessment? |
| Configure | The product offers a supported setting or rule relevant to the requirement. | Is it supported in this release and scope, and who owns the value and change? |
| Adapt the organisation | A different handoff, responsibility or training approach preserves the needed outcome. | Who takes on the work, and is the new arrangement usable at both sites? |
| Integrate or extend | A material need remains after viable standard and process options have been assessed. | Is there an appropriate released interface or extension point, and who maintains and tests it? |
| Defer, reject or investigate | Evidence, authority or priority is missing, or the need can legitimately wait. | Who decides, what is the interim treatment and what would reopen the item? |

**Configuration** selects among supported options. **Extension** adds behaviour or information through an available mechanism. **Integration** connects work or data across systems and introduces another handoff to govern. None is synonymous with modifying the product core. SAP's [Public Edition extensibility overview](https://learning.sap.com/courses/administrating-sap-s-4hana-cloud-public-edition/introducing-extensibility-options_f2a7854e-77d7-4ae7-8fdb-c6c9a770366d) distinguishes key-user, developer and side-by-side approaches. Clean-core thinking asks how to preserve maintainability and upgradeability; it does not make a proposed extension safe simply because it is called side-by-side. Verify the interface, permissions, failure handling, ownership and regression burden. For example, an external review service is a poor substitute for a release control unless the integration can safely deal with missing, duplicate or late responses. Do not recommend an extension because a workshop participant asked for a screen.

## 4. Worked case: payment block is not independent release

Read the [J45 evidence cards and client brief](../../cases/M09_J45_Fit_to_Standard.md). On the Swiss PO-referenced invoice route, entering the earlier purchase order supplies invoice items and the procedure represents further checks. Another documented observation concerns a manual block and a separately documented release action on a payment-blocked invoice. An optional no-reference route instead uses accounting inputs and also represents checks. The cards are not one transaction trace. They do not show that a discrepancy always causes a block, that an independent person must release it, or that release causes payment.

```text
Reference shows              Client needs                 Workshop disposition
PO supplies invoice items  → PO-based entry             → Candidate standard fit
Block and release shown    → Independent release        → Role and control design to verify
No-reference route shown   → Keep it from bypassing rule  → Scope and negative test
```

**Follow FTS-02 from the initial question to a test.** The client says the person who entered an in-scope disputed invoice must not release its payment block. The reference provides a candidate control point, not the required independence. In the workshop, ask the Finance control owner which invoices and identities are in scope, how substitutes are delegated and what happens if no eligible reviewer is available. Ask the implementation team to demonstrate the available role and control behaviour in the selected landscape. A role name and an approval action are not sufficient.

**What a useful exchange sounds like, in the simulation:**

- **Facilitator:** “The reference shows a release action. What would make that action acceptable in your process?”
- **Finance control owner:** “For a disputed invoice in scope, the person who entered it must not be able to release the block.”
- **Technical lead:** “Then I need to test both identities on the same type of case. Showing that the reviewer can release it will not tell us whether the entrant can.”
- **Scribe, at readback:** “The policy need is confirmed in this exercise. Standard-based enforcement is a candidate. Feasibility is open, and Finance has not approved an alternative design.”

Record the need independently of its solution. For instance: “Prevent the original entrant from releasing a payment block on an in-scope disputed invoice, while allowing an eligible independent reviewer to release it after review.” A provisional design can use the standard block and release as a candidate, while keeping enforcement unresolved. If no supported implementation has been demonstrated, do not label the requirement fit or assign a build. First obtain an authoritative feasibility decision. If the client accepts a changed process, record the decision and any remaining exposure; do not silently downgrade a mandatory rule.

In Realize, use two distinct test identities against comparable in-scope blocked invoices. Give the eligible independent reviewer the evidence required by the agreed policy. Test that this reviewer can release the block and that the original entrant cannot. Inspect the resulting block state and the evidence linking the user, invoice and action. Check legitimate no-reference handling separately and test any feasible alternate route that might avoid the policy. A successful release does not establish payment, and a rejected click on one screen does not establish enforcement across every path.

## 5. Use TOGAF to connect the decision to the architecture

[The Open Group's TOGAF competency overview](https://help.opengroup.org/hc/en-us/articles/32127544219026-Competency-to-Role-Mapping-TOGAF-Enterprise-Architecture-Practitioner) includes stakeholder management, gap analysis, requirements management and planning transitions. Use those ideas to organise the decision; do not map TOGAF's Architecture Development Method phases one-for-one onto Activate phases. They answer different questions. SAP supplies a candidate process and delivery guidance. Architecture work connects a proposed change to the broader arrangement of roles, information and systems.

| Architecture question | Alpine Pack example |
|---|---|
| Baseline: how is work organised now? | Plants use different channels to ask for evidence and seek review. A release explanation may sit outside the invoice record. |
| Target: what should change? | A shared policy defines the covered disputes and independent reviewer. The release decision is linked to its evidence. |
| Gap: what is missing or uncertain? | The reference does not establish that the original entrant is prevented from releasing. The treatment of open blocked invoices at cutover also needs a decision. |
| Transition: what must happen first? | Confirm policy and owners, verify supported implementation, test with realistic roles and data, rehearse cutover, then monitor exceptions in Run. |

This comparison does not make the standard process the target architecture. It shows which elements of the target the standard may support and which depend on organisation, configuration or other systems. A sound handoff to the delivery team records the requirement, owner, evidence, dependency and acceptance condition. Avoid handing over a statement like “configure the SAP block” when the actual question is whether independent release can be assured.

## 6. From backlog to working change

A **backlog** is an ordered list of work and questions to resolve, not a list of approved builds. A high-risk feasibility investigation may outrank a well-understood configuration task. The exact tracking system is not the main issue. The important link is between the requirement, the decision and the evidence that will later support acceptance.

```text
Requirement → decision or open question → owned backlog item
           → configured increment or process change → playback and test
           → readiness decision → observation after go-live
```

For FTS-02, the first item is to confirm how independent release can be supported for the agreed scope. Keep this distinct from FTS-03, which concerns legitimate invoices without a purchase order. Confirm the coverage rule and map out the controls before using that route. The data and cutover team needs a separately owned action for old blocked items. A training item should teach users how to handle a discrepancy and escalate an unresolved case, not just where to click.

```text
Finance policy: covered cases and eligible reviewers
    ├─ Design + security: role and enforcement options
    ├─ Data + integration: usable evidence and continuity at cutover
    ├─ Testing: ordinary, prohibited and alternate-path cases
    └─ Adoption + support: role training, escalation and ownership in Run
```

In **playback**, show stakeholders the proposed configured behaviour and revisit earlier assumptions. In **user acceptance testing (UAT)**, have the business evaluate the agreed scenarios and acceptance criteria. Integration tests address cross-system handoffs; migration rehearsals and reconciliations address data continuity; regression tests check whether a change disturbed behaviour that should remain stable. A pass on one does not substitute for the others. Record what was tested, against which version and scope, and the resulting state. Keep defects, open policy decisions and approved scope changes distinct.

**Worked cutover check.** Take a fictional legacy blocked invoice with a pending Receiving explanation. Before cutover, confirm who owns it and agree whether it is carried forward or handled through a controlled alternative. Reconcile the item and its block disposition on both sides of the cutover. A total count can agree even if the wrong invoice lost its restriction. Check a sample by identifier and state, record unresolved items and assign support ownership. Do not infer that a particular migration mechanism transfers every artefact.

[Robey, Ross and Boudreau (2002)](https://www.tandfonline.com/doi/abs/10.1080/07421222.2002.11045713) distinguish learning to configure a package from learning to carry out changed work. Their ERP study is not an evaluation of contemporary SAP Public Edition. It helps explain why a successful technical test and a prepared organisation are different achievements. A reviewer may understand the release action and still be unable to obtain a timely explanation from Receiving. Plan for both forms of learning.

## 7. After go-live: design, fit, practice and outcomes

```text
Architectural coherence → Do the represented roles, data and actions fit together?
Implementation fit     → Does the selected design meet this client's requirements?
Enacted fit             → Can people make it work in normal and exceptional practice?
Outcomes                → Did a defined result change, and what else might explain it?
```

For implementation fit, collect the decision, configured settings or agreed process design, and test results. For enacted fit, sample ordinary, disputed and urgent cases, including cases that never progressed to release. Compare records with what people describe and do. For outcomes, define a baseline, the population and the measurement window. For example, shorter median time to release could reflect a smaller share of complex cases. Check the case mix and whether unresolved cases dropped out of the denominator before attributing the change to the project. A go-live decision is not a performance finding.

Now run the [Fit-to-Standard workshop](../../exercises/M09_Run_a_Fit_to_Standard_Workshop.md). Before looking at the worked answers, be able to explain: why a block is not proof of independent review, when a delta is not a build request, how a test distinguishes routing from enforcement, and what you would need to see after go-live to assess the change. [Module 10](../10_Comparative_Process_Analysis/README.md) will ask which of these patterns recur across different end-to-end processes.
