# Kering Workstream Data

This directory contains blank workstream-specific registers. It must not contain SAP corpus records or unregistered raw participant data.

## Templates

- `Source_Register_Template.csv` records source identity, version, provenance, access, and inclusion decisions.
- `Evidence_Log_Template.csv` records traceable evidence segments, descriptive observations, interpretations, rivals, and claim limits.

Create dated working copies only after the feasibility boundary has been frozen. Sensitive field data will require a separate approved storage arrangement and must not be added to this repository by default.

The repository ignores `data/raw/`, `data/interviews/`, and `data/consent/` within every empirical workstream. A workstream-level `private/` directory is also ignored. These exclusions reduce accidental tracking but do not replace encryption, access control, retention limits, or an approved research-data plan.
