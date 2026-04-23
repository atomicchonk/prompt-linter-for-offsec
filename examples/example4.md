# Example 4
## Original Prompt

Summarize these bug bounty findings.

## Detected Phase

### Reporting

## Hardened Prompt
```
Use only provided confirmed findings and evidence. Summarize into a structured report. Do not invent scope, merge findings without evidence, assume severity, or claim speculative impact. Missing data = unknown. Return exactly:

Executive Summary:
scope:
confirmed findings (count + types):
notable confirmed impacts:

Findings Table:
title | asset | vuln type | confidence | confirmed impact | evidence status

Detailed Findings:
For each finding:

Title:
Asset:
Vulnerability Type:
Confidence:
Status:

Claim:
Evidence:
Reproduction:
Confirmed Impact:
Theoretical Impact:
Limitations / Unknowns:
Remediation (high-level only):

Related Findings:

duplicates (if confirmed)
shared root cause (if supported)
```
