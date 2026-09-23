# Stream Four: Enterprise Systems, Implementation, and Transformation

## Evidence note

This review was developed from the project bibliography, verified publisher and repository records, official SAP documentation, and a critical audit of the supplied LeapSpace report. The LeapSpace report is a discovery aid, not scholarly evidence. It cited the uploaded prompt as evidence, did not retrieve the four foundational works it was asked to assess, and mixed relevant enterprise-systems research with unrelated implementation studies. No claim below relies on the report itself.

Access status matters. Several core claims below are supported by publisher abstracts and bibliographic records rather than complete article text. Those limits are recorded in the accompanying source assessment. Page-specific claims require checking against the exact copy used before publication.

## Part I: Learning guide

### 1. The practical problem

An enterprise system is not simply a large application. It offers an integrated set of data structures and process capabilities across organisational functions. Its attraction is also its organisational consequence: common data, shared process sequences, and cross-functional controls can reduce fragmentation, but they can also make one unit dependent on choices made elsewhere.

The central analytical problem is therefore not whether an organisation has installed ERP. It is how a packaged design moves through several distinct states:

1. **Encoded architecture:** the vendor's reference processes, data structures, roles, rules, workflows, and configuration possibilities.
2. **Implemented configuration:** the scope, settings, extensions, integrations, and organisational changes selected for a particular implementation.
3. **Enacted practice:** how people actually perform work with, around, or outside the configured system.
4. **Organisational outcome:** the operational, managerial, strategic, infrastructural, or organisational effects attributed to the system and its use.

These states are connected, but none proves the next. A reference process does not prove that a customer selected it. A configured workflow does not prove that users follow it. Use does not by itself prove benefit.

### 2. Five concepts to master

#### Enterprise integration

**Definition:** Integration is the linking of processes, data, and organisational units through a common enterprise system.

**Plain-language explanation:** Integration makes activities visible and consequential beyond the department in which they begin. A purchasing decision may affect inventory, liabilities, payment, and reporting through shared objects and transactions.

**Research use:** Volkoff, Strong, and Elmes (2005) show why integration must be analysed as differentiated relations among process and data elements rather than treated as a binary property.

**Evidence boundary:** The presence of common data or an integrated process design does not establish accurate data, effective coordination, or improved performance.

#### Standardisation

**Definition:** Standardisation reduces variation by prescribing common processes, categories, data definitions, or technical arrangements.

**Plain-language explanation:** A package can make different business units use the same recognised objects and process steps. This may improve comparability while restricting local variation.

**Research use:** Davenport (1998) treats enterprise systems as vehicles for integration and organisational redesign, while warning that embedded system logic may conflict with strategy or organisation. Standardisation should therefore be coded as an encoded or implemented arrangement, not presumed to be a benefit.

**Evidence boundary:** A standard reference path does not prove consistent enactment, and consistency does not prove suitability.

#### Fit and misfit

**Definition:** Fit concerns the relationship between packaged system capabilities and organisational requirements. Misfit is not one generic gap.

**Plain-language explanation:** A package may lack required functionality, impose unwanted data, alter roles, weaken a control, or conflict with organisational culture.

**Research use:** Strong and Volkoff (2010) identify six misfit domains: functionality, data, usability, role, control, and organisational culture. They distinguish deficiencies from impositions and fit as coverage from fit as enablement. This is more precise than treating fit as a single project score.

**Evidence boundary:** A documented mismatch does not determine the organisational response. Organisations may change the process, configure or extend the package, accept the mismatch, create a workaround, or abandon scope.

#### Configuration and customisation

**Definition:** Configuration selects among vendor-supported options. Extension adds functionality through supported interfaces or adjacent components. Modification changes core package behaviour. Terminology varies across sources and vendors.

**Plain-language explanation:** Not every departure from a default is the same. Choosing an available setting differs from building an extension or altering core code.

**Research use:** Brehm, Heinzl, and Markus (2001) replace the simple configuration-versus-modification binary with a spectrum of tailoring choices whose maintenance and upgrade implications differ. Singh and Pekkola's (2021) systematic review confirms that packaged systems embody process assumptions and that customisation research remains fragmented across disciplines. Together, these sources provide a useful starting vocabulary, subject to SAP-specific verification.

**Evidence boundary:** The existence of an option does not establish that a customer selected it. Public-cloud restrictions and supported extensibility patterns must be documented for the relevant product and release.

#### Implementation lifecycle

**Definition:** Implementation is a temporally extended process of decision, project work, stabilisation, use, and further development.

**Plain-language explanation:** Go-live is neither the beginning nor the end. Choices before contracting affect scope; project decisions shape configuration; the shakedown period reveals problems; later work adapts or expands the system.

**Research use:** Markus and Tanis (2000) organise the enterprise-system experience into chartering, project, shakedown, and onward-and-upward phases. Robey, Ross, and Boudreau (2002) explain implementation through learning and the management of knowledge barriers. Boudreau and Robey (2005) show that post-implementation users may initially resist and later reinvent system use through improvised learning.

**Evidence boundary:** A lifecycle model orders analytical attention. It does not guarantee a linear sequence or define success uniformly across time and stakeholders.

### 3. A short reading route

1. Read Davenport (1998) for the organisational stakes of integrated packages.
2. Read Markus and Tanis (2000) for the lifecycle and success problem.
3. Read Soh, Kien, and Tay-Yap (2000), Hong and Kim (2002), and Strong and Volkoff (2010) for progressively sharper accounts of fit and misfit.
4. Read Robey, Ross, and Boudreau (2002) and Boudreau and Robey (2005) for learning, resistance, and reinvention.
5. Read Volkoff, Strong, and Elmes (2005) for integration as an organisational phenomenon.
6. Read Singh and Pekkola (2021) for the customisation evidence base and its limits.
7. Read current official SAP material only after this foundation, to identify what SAP currently calls Fit-to-Standard and how it describes the Explore and Realize phases.

### 4. Concept summary

| Concept | What it means | Use in this project | Boundary |
|---|---|---|---|
| Reference architecture | Vendor-provided process, data, role, rule, and configuration design | Primary object of documentary analysis | Not a customer implementation |
| Integration | Linking of process, data, and organisational units | Identify encoded dependencies and shared objects | Does not establish coordination quality |
| Standardisation | Reduction of variation through common designs | Identify prescribed categories, sequences, and controls | Does not establish enacted uniformity |
| Fit | Relationship between package and organisational requirements | Classify possible areas of alignment | Cannot be inferred without organisational requirements |
| Misfit | Deficiency or imposition across several domains | Anticipate implementation choices and tensions | Not observable from vendor architecture alone |
| Configuration | Selection among supported options | Locate bounded implementation discretion | Option availability does not prove selection |
| Extension | Added functionality through supported mechanisms | Record where reference design permits supplementation | Does not establish actual extension use |
| Enactment | Situated use and adaptation | Defines a later empirical level | Cannot be recovered from reference documentation |
| Outcome | Effects attributed to implementation and use | Defines a claim requiring independent evidence | Deployment alone is not an outcome |

## Part II: Readable scholarly synthesis

### 5. Enterprise systems join technical integration to organisational design

Davenport (1998) supplied the field's enduring starting point: enterprise systems promise to replace fragmented information arrangements with integrated packages, but adopting the package also imports a particular logic of processes and information. Management must therefore decide whether that logic fits the organisation rather than delegate the decision to technologists. This is not yet a theory of architecture as organisation design, but it makes the architecture consequential.

Later research disaggregates the general promise of integration. Volkoff, Strong, and Elmes (2005) distinguish process and data integration and examine relations among organisational units with different interdependencies. Their contribution prevents the project from coding every shared object as the same kind of integration. The analytical question becomes: what is connected, through which object or sequence, across which boundary, and with what encoded consequences?

**Project interpretation:** SAP reference architecture can be analysed as a designed field of possible integration. The evidence may show shared objects, required sequence, common data, or cross-functional visibility. It cannot show that integration was configured successfully or produced a desired result.

### 6. Packaged software contains generic assumptions, not neutral capacity

Packaged enterprise systems must serve more than one organisation. Their designs therefore generalise processes, data, roles, and controls. Soh, Kien, and Tay-Yap (2000) show that these generalisations can conflict with company, sector, or country requirements. Hong and Kim (2002), using survey data from 34 organisations, find that implementation success is associated with organisational fit and implementation contingencies. The study supports the importance of mutual adaptation but should not be converted into a universal causal law.

Strong and Volkoff (2010) provide the most useful architecture-facing elaboration. Their three-year qualitative study treats the enterprise system as an artefact whose effects become visible through misfits. Functionality, data, usability, roles, control, and organisational culture can each contain deficiencies or unwanted impositions. This directs documentary analysis toward more than functions. An architecture may distribute roles, mandate data, expose or suppress controls, and privilege particular classifications.

The distinction also disciplines novelty claims. Enterprise-systems scholarship already recognises embedded organisational structures. The research gap is therefore not the discovery that software contains assumptions. A stronger gap concerns a reproducible method for reconstructing those assumptions from controlled vendor reference artefacts before observing a customer implementation.

### 7. Implementation is a sequence of organisational choices

Markus and Tanis (2000) frame the enterprise-system experience as a lifecycle rather than a single adoption event. The chartering phase establishes the business case, package, scope, and project conditions. The project phase builds and configures. Shakedown covers transition and stabilisation. Onward and upward covers maintenance, enhancement, and benefit development. Success may differ by phase, stakeholder, and measure.

Robey, Ross, and Boudreau (2002) place organisational learning at the centre of implementation. Implementations confront knowledge barriers between old and new work, between functions, and between organisational and package knowledge. Their dialectical account matters because configuration is not merely a technical translation of settled requirements. It is a contested learning process through which requirements, package possibilities, and organisational commitments become mutually adjusted.

Boudreau and Robey (2005) move the analysis beyond implementation into use. Their interpretive case study of a government agency reports initial avoidance and later reinvention through improvised learning. The result is a decisive boundary for this project: even an integrated system described as constraining cannot determine enactment.

### 8. Misfit opens several adaptation routes

A misfit may be answered by organisational adaptation, package adaptation, or a combination. Soh and Sia's analysis of so-called vanilla implementations shows that few organisations simply accept a package without modification. Strong and Volkoff explain why the choice is multidimensional. A role imposition, for example, raises different questions from a missing report or unusable field.

Singh and Pekkola (2021) show that the customisation literature remains scattered and often generic. Their review supports a basic differentiation among configuration, extension, and modification, but it also demonstrates that the evidence base does not yet justify simple rules about when or how much to customise. Cloud delivery further changes the feasible set because the vendor controls more of the core and update cycle.

**Proposition:** Reference architecture defines a structured space of implementation discretion rather than a single prescribed organisation. The empirical task is to identify the available choices and their conditions without assuming which choice a customer makes.

### 9. Outcomes require separate evidence

Enterprise-system benefit claims cover multiple levels. Shang and Seddon (2002) distinguish operational, managerial, strategic, IT-infrastructure, and organisational benefit dimensions. Their evidence includes vendor-reported cases and manager interviews, so the framework is valuable for classification but should not be treated as proof that enterprise systems generally cause each benefit.

Gattiker and Goodhue (2005) sharpen the contingency argument after go-live. Their survey of 111 manufacturing plants links plant-level outcomes to interdependence and differentiation, with customisation and elapsed time also included. The study is valuable because it refuses a single enterprise-wide outcome and locates effects at a specified organisational level. Its results remain contingent on its manufacturing sample, measures, and model.

Outcomes also unfold over time. Stabilisation costs may precede operational gains, while later organisational effects depend on use, complementary change, and benefit management. A documentary study of reference architecture can therefore propose outcome-relevant mechanisms, but it cannot report realised benefits.

### 10. Cloud ERP and Fit-to-Standard require a narrower claim

The supplied LeapSpace report overstates the independent scholarly evidence on contemporary SAP public-cloud implementation. The SciSpace report identifies two stronger cloud-ERP studies, but they still do not establish the organisational effects of SAP S/4HANA Cloud Public Edition. Peng and Gala (2014) derive potential benefits and barriers from interviews with 16 ERP and cloud consultants. Bjelland and Haddara (2018) study update processes across 10 Norwegian client organisations and one cloud ERP vendor. The latter supports a bounded claim that cloud delivery can move update timing toward the vendor and make post-implementation change more iterative. Neither study evaluates SAP Fit-to-Standard or proves that every public-cloud customer lacks release discretion.

Current SAP documentation describes SAP Activate as a six-phase framework. During Explore, teams review preconfigured processes in a starter system, document requirements not covered by standard processes, and identify configuration decisions. During Realize, teams configure, build, test, and validate. This establishes SAP's current official method and vocabulary. It does not establish how projects enact the method or whether it succeeds.

The defensible inference is narrower. Fit-to-Standard makes reference content an explicit starting point for requirements discussion. This is directly relevant to the project because it gives reference architecture an observable implementation role. Whether the approach reduces customisation, changes power, accelerates delivery, or improves outcomes remains an empirical question.

## Part III: Complete technical expansion

### 11. Levels of analysis

Enterprise-systems research operates at several levels that must be coded separately:

- the package and its encoded structures;
- the implementation project and its decisions;
- the configured organisational system;
- the user, group, process, business unit, or organisation enacting it;
- the outcomes measured at a particular time.

The LeapSpace report blurred these levels when it used unrelated studies of healthcare, policing, and port decarbonisation to support a claim about macro, meso, and micro enterprise-system implementation. Those sources were retrieved through the word "implementation," not through conceptual relevance, and are excluded.

### 12. The architecture and the implementation choice set

The architecture contains both prescriptions and alternatives. Reference processes define a standard path. Configuration points expose choices. Extension mechanisms permit supplementation. Integrations connect other systems. Access and role designs distribute possible action. Master-data structures define recognised entities and attributes.

Documentary coding should therefore record:

1. the reference arrangement;
2. whether an alternative is explicitly available;
3. the mechanism of variation, such as configuration or extension;
4. any documented precondition or restriction;
5. the organisational dimension affected;
6. the evidence level.

It should not label a reference arrangement a misfit because misfit requires comparison with a particular organisation's requirement. It may instead code a **potential fit dimension**, such as role, data, control, or functionality.

Pollock, Procter, and Williams (2003) add the vendor side of this relationship. Their three-year ethnography follows an ERP module as a supplier translates between generic software and specific university settings. The concept of an artefact biography shows that reference architecture is not produced once and then merely implemented. It is repeatedly made generic through interactions among vendors and adopters. Kallinikos (2004) complements this account by analysing ERP packages as organisational forms that proceduralise operations and roles. These contributions strengthen the case for studying architecture directly, while also weakening any claim that it is a timeless or context-free object.

### 13. Fit and response matrix

| Misfit domain | Encoded evidence that may be observed | Possible implementation response | What cannot be inferred |
|---|---|---|---|
| Functionality | Required and unsupported activities, scope boundaries | Adopt, extend, integrate, modify, or change process | Customer requirement or chosen response |
| Data | Required fields, structures, relationships, classifications | Map, cleanse, migrate, extend, or accept | Data quality in use |
| Usability | Interface sequence and required interaction | Training, adaptation, alternate interface | Experienced usability |
| Role | Business roles and allocated activities | Reallocate work, redesign role, adjust access | Actual responsibility or accepted authority |
| Control | Validation, approval, restriction, and audit features | Configure threshold, add control, redesign process | Control effectiveness or accountability |
| Culture | No direct documentary observation from architecture alone | Organisational change or local adaptation | Cultural fit from vendor documentation |

### 14. Lifecycle implications for evidence collection

Reference documentation is mainly evidence about encoded architecture. Implementation methods identify expected project activities. Configuration records would evidence implemented choices. Interviews, observation, logs, and local work instructions would be needed for enactment. Performance and organisational claims require outcome measures and an appropriate research design.

This produces an evidence chain:

> Reference artefact -> documented choice space -> customer implementation evidence -> enactment evidence -> outcome evidence

The project currently addresses the first two links. Later studies may extend the chain, but Paper 1 must not write those later links as findings.

### 15. Implications for the analytical framework

This literature adds five necessary constructs:

- **reference arrangement:** the vendor-provided process, role, data, rule, or control design;
- **variation mechanism:** configuration, extension, integration, modification, or organisational change;
- **implementation decision:** a documented selection within or beyond the reference design;
- **potential fit dimension:** the organisational requirement domain affected by an encoded arrangement;
- **evidence transition:** the additional evidence needed to move from encoded design to configuration, enactment, or outcome.

### 16. Relationship with neighbouring literatures

Enterprise-systems research establishes the phenomenon, lifecycle, fit problem, and adaptation choices. It does not fully explain recurrent performance, situated sociomaterial enactment, infrastructure evolution, legitimate governance, or process-representation semantics. Those questions require the separate reviews of routines, technology and materiality, digital infrastructure, governance and accountability, and business-process management.

### 17. Strongest defensible gap

The literature does not permit the claim that enterprise architecture has been ignored. Davenport, Soh and colleagues, Brehm and colleagues, Pollock and colleagues, Kallinikos, Strong and Volkoff, and the customisation literature all recognise embedded process and organisational assumptions.

The defensible gap is methodological and level-specific:

> Enterprise-systems research richly explains implementation, fit, adaptation, and use, but offers less guidance for systematically reconstructing encoded organisational logic from release-controlled vendor reference artefacts before examining a customer configuration or enacted practice.

The project can contribute a reproducible documentary method and a bounded vocabulary for that reconstruction. Its novelty will depend on demonstrating that the method reveals relations that existing process, fit, and implementation frameworks do not capture adequately.

### 18. Claims discipline

The project may claim that:

- enterprise systems integrate process and data through packaged designs;
- packaged designs embody assumptions that may fit or misfit organisational requirements;
- implementation involves lifecycle choices, learning, configuration, adaptation, and stabilisation;
- reference architecture can be studied as an organisational artefact;
- official SAP methodology makes reference processes an explicit object of Fit-to-Standard discussion.

The project must not claim from reference documents alone that:

- SAP standardises an adopting organisation;
- Fit-to-Standard eliminates discretion or customisation;
- configuration options were selected;
- users follow the reference process;
- controls are effective or legitimate;
- implementation produces transformation or performance improvement;
- SAP's method is enacted as officially described.

## Part IV: Audit conclusion

The LeapSpace report located 33 named external sources plus four prompt-upload entries and two absent numbers in its reference sequence. Four prompt citations are rejected as evidence. At least four external sources are plainly off-topic for this review, and several others are adjacent, practitioner-oriented, or too weakly accessed to support the claims assigned to them. The report's confidence rating of "Medium" is rejected because the core source assessment used opaque internal identifiers and the foundational works were not actually retrieved.

This curated review retains the LeapSpace report's useful leads to Volkoff, Strong, and Elmes (2005), Wang et al. (2007), Singh and Pekkola (2021), and limited SAP implementation literature. The subsequent SciSpace report contributed important additional leads on tailoring, artefact biography, information packages, post-implementation contingency, cloud updates, and cloud-adoption dilemmas. Both reports remain discovery aids. The argument has been rebuilt around independently identified scholarship, and the accompanying assessment records each decision.
