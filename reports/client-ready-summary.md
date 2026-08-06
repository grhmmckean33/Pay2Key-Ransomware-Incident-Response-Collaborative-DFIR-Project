# Graham McKean — Scope Assessment Contribution Summary

## My assignment

I worked as the **Scope Assessment Analyst** during a collaborative Pay2Key ransomware investigation. My task was to establish which systems were affected and to support each conclusion with defensible endpoint evidence.

## Method used

For each relevant host, I correlated:

1. suspicious file presence;
2. process execution and user/process context; and
3. network communication with suspicious infrastructure.

This prevented scope decisions from being based on a single indicator or alert.

## Key personal finding

During my review, I independently identified `Synaptics.exe` and `massscan_gui.exe` on the contractor workstation. These artefacts did not fit the expected Pay2Key activity. I escalated the mismatch, which contributed to separating additional actor activity and reduced the risk of incorrect attribution.

## Outcome

My work supported the host-by-host scope assessment, including confirmation of compromise on the Domain Controller and contractor workstation and the conclusion that five other systems showed no evidence of compromise in the available telemetry. My findings and limitations were incorporated into the collaborative incident report.

## Skills demonstrated

- Microsoft Defender XDR / Defender for Endpoint
- KQL and Advanced Hunting
- Incident scoping
- Evidence correlation
- Threat hunting
- Attribution discipline
- Escalation of anomalous findings
- Technical and stakeholder reporting

> This summary describes my contribution to a simulated team investigation. It does not claim ownership of work completed by the IR Lead or other analysts.
