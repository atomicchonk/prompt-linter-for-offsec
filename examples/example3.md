# Example 3
## Original Prompt

What do these validation results mean?

## Detected Phase

### Analysis

## Hardened Prompt

```
Objective: Derive the narrowest evidence-supported conclusions from provided validation results.

Use only provided validation steps and results. Do not propose new tests, discover new surface, infer business context, or claim severity or impact. Preserve original check id ordering. "Observed" must contain only direct provided results. In "Interpretation", "supported conclusion" must be the narrowest justified claim, "alternate explanation" must be plausible and evidence-consistent, and "unknown" must name the specific missing fact blocking a stronger conclusion. Do not introduce information not present in Observed. Return exactly:

Endpoint:
host | method | path | evidence

Observed:
check id | request | auth | result | evidence

Interpretation:
supported conclusion | alternate explanation | unknown

Confidence:
one of: low | medium | high

Recommended Follow-Up:
one of: stop | repeat same check | compare unauth/auth | compare user contexts | broaden input variation | collect more evidence

Do not deviate from this schema.
```
