# Literature Map

## Architecture of the review

The review uses organisation design, coordination, and information processing as the explanatory core. Enterprise-systems research establishes the phenomenon and the dominance of implementation-centred questions. Decision theory clarifies authority and premises; routines and sociomateriality guard against conflating encoded logic with practice; infrastructure studies sensitise the analysis to installed bases and classification. These literatures are positioned, not amalgamated.

| Stream | Foundational authors and works | Core concepts | Later development and relevance | Tensions and gap |
|---|---|---|---|---|
| Organisation design | Thompson (1967); Galbraith (1973, 1977); Mintzberg (1979) | Interdependence, uncertainty, information processing, coordination mechanisms, structural configuration | Contingency and information-processing approaches explain why arrangements vary with task demands | Built for organisations, not for reconstructing organisational assumptions in software architecture |
| Coordination theory | Malone and Crowston (1994); Okhuysen and Bechky (2009) | Managing dependencies; accountability, predictability and common understanding | Mechanism-centred vocabularies enable fine-grained analysis across settings | Broad definitions risk calling every software relation “coordination” |
| Decision theory | Simon (1947/1997); March and Simon (1958/1993) | Bounded rationality, decision premises, authority, programmes | Rules and information systems can distribute premises rather than only decisions | Formal permissions do not establish actual authority or judgement |
| Enterprise systems | Davenport (1998); Markus and Tanis (2000); Soh, Kien and Tay-Yap (2000); Boudreau and Robey (2005) | Integration, process standardisation, enterprise-system experience cycle, misfit, improvisation | Research documents transformation, drift, adaptation, and institutional effects | Architecture is often treated as input to implementation rather than an organisational artefact in its own right |
| Routines | Feldman and Pentland (2003) | Ostensive and performative aspects; artefacts | Artefacts can shape and represent routines without determining performances | Reference process is neither ostensive routine nor enacted performance; category boundaries require care |
| Technology and organisation | Orlikowski (1992, 2000); Leonardi (2011) | Duality of technology, practice lens, materiality, affordance and constraint | Corrects deterministic readings and foregrounds relations between material features and human agency | Paper 1 deliberately brackets enactment; it must state what documentary evidence cannot show |
| Digital infrastructure | Star and Ruhleder (1996); Bowker and Star (1999); Hanseth and Lyytinen (2010); Tilson, Lyytinen and Sørensen (2010) | Relational infrastructure, classification, installed base, generativity | Shows how standards and classifications organise distributed work over time | ERP reference architecture is more bounded than infrastructure, but may participate in one |
| Governance and control | Ouchi (1979); Eisenhardt (1985) | Behaviour/output control, markets, bureaucracies, clans, agency | Useful for separating encoded monitoring, rules, and outcomes | Control categories can obscure decision rights and information visibility; governance needs its own coding family |

## Conceptual overlaps and disciplined separations

Standardisation of work may be both a Mintzbergian coordination mechanism and an Ouchian behaviour control. Coding may record both, but analysis must state which question each answers. A shared master-data object may coordinate pooled activity and provide information-processing capacity; it is not automatically a governance mechanism. Access restrictions govern visibility and action but do not demonstrate accountability unless consequences or answerability are documented.

The main gap is a level-of-analysis gap. Enterprise-systems studies show what happens during and after implementation; organisation-design theories explain organisational arrangements; technology-in-practice studies explain enactment. Less developed is a reproducible method for moving from vendor reference artefacts to a bounded reconstruction of encoded organisation. This project addresses that gap while using routines and sociomaterial research to police its claims.

The organisation-design stream has now been developed separately in [Stream One: Organisation Design, Detailed Literature Review](literature/Stream_01_Organisation_Design_Detailed_Review.md). Its accompanying [LeapSpace source audit](literature/Stream_01_LeapSpace_Source_Audit.md) records which supplied sources were retained, narrowed, relocated, or excluded.

## Priority reading route

Read Thompson, Galbraith, and Mintzberg before coding the pilot, producing construct memos that distinguish dependency, coordination, and information capacity. Then read Malone and Crowston and Okhuysen and Bechky to test the mechanism vocabulary. Enterprise-systems readings position the contribution; routines, sociomateriality, and infrastructure readings supply boundary conditions. Full bibliographic records and verification flags are maintained in `references/references.bib` and the operational sequence in `literature/Reading_List.md`.
