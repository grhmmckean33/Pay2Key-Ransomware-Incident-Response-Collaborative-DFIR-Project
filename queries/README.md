# KQL Reconstructions for My Scope-Assessment Workstream

These queries demonstrate how I would implement the three-check methodology used in my assigned scope-assessment workstream within Microsoft Defender XDR Advanced Hunting.

**Evidence limitation:** the supplied client-ready report does not contain the original technical appendices, raw telemetry or original case queries. These files are transparent portfolio reconstructions, not verbatim investigation evidence.

## How each query supports my role

1. `01-file-presence-hunt.kql` — tests whether suspicious artefacts are present across candidate devices.
2. `02-process-execution-validation.kql` — confirms whether an artefact executed and captures account, command-line, hash and parent-process context.
3. `03-network-correlation.kql` — checks whether the suspicious process or host communicated with external infrastructure.
4. `04-host-scope-matrix.kql` — brings the three checks together to support a host-level decision and identify evidence gaps.

## Analytical principles

- Do not declare a host compromised from file presence alone.
- Do not describe a host as definitively clean because one query returned no results.
- Correlate timestamps, devices, accounts, processes, hashes and remote endpoints.
- Escalate artefacts that do not fit the working attribution.
- Record telemetry limitations and the precise wording of each conclusion.

Before running these queries, confirm authorisation, set the approved timeframe, and replace example indicators and device names with values appropriate to the environment.
