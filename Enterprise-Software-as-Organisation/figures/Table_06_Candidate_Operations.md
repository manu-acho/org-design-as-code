# Table 6. Candidate operations and what qualifies them

These categories are used for architectural interpretation, not a validated inventory. Evidence IDs resolve in [Table 7](Table_07_Findings_Source_Locators.md).

| Candidate operation | Qualifying relation | Example | Exclusion |
|---|---|---|---|
| Supply data or select an object | A later activity uses prior content or an identifier as an operative input. | J45-W07-16 supplies invoice items; J58-W08-11 identifies a clearing record. | Merely displaying a reference. |
| Route a task | A condition and recipient are specified for an object and path. | BD9-W08-04 sets conditions and recipient levels. | Treating a recipient as an effective permission or the order of definitions as a sequence of decisions. |
| Decide or change state | A decision or operation has a documented consequence for the object. | J58-W08-05 shows the expected approved-and-posted state. | Counting this as another independent replication of workflow routing. |
| Return work | A documented reason or instruction accompanies an exception route. | J45-W07-11 shows the request; J58-W08-07 shows resubmission. | Inferring completed rework or reciprocal adjustment from the request alone. |
| Scope an operation | A field is used to select or condition a task. | J45-W07-06 uses purchasing group; BD9-W08-08 uses shipping point. | Treating selection as an authorisation restriction. |
| Schedule execution | A defined task has timing or parameters distinct from execution. | BD9-W08-17 gives job options and logs; J58-W08-17 distinguishes run modes. | Inferring automatic productivity gains or universal human review. |
| Make an output inspectable | A recorded state or result is available for review. | J58-W08-15 shows rule-result inspection. | Inferring that a named actor intervened or was held accountable. |
