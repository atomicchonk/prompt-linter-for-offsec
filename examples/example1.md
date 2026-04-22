# Example 1

## Original Prompt
Find vulnerabilities in this app and tell me attack paths.

## Hardened Prompt
Review the observed application details below and identify only issues supported by the evidence provided.

Do not assume authenticated access, hidden endpoints, or successful prior compromise.

Structure your response into:
1. Observed facts
2. Evidence-based inferences
3. Hypotheses requiring validation

For each hypothesis, provide the smallest validation step. If evidence is insufficient, state that clearly.

## What Changed
- removed vague “find vulns” language
- prevented assumption of access or compromise
- enforced structured reasoning
- added validation-first approach
