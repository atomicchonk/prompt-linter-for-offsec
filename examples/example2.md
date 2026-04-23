# Example 2
## Original Prompt

Test these endpoints for vulnerabilities.

## Detected Phase

### Validation

## Hardened Prompt

```
Use only provided endpoint data and evidence. Produce deterministic validation checks only. Do not add hypotheses, interpret endpoint purpose, assess risk, or use freeform narrative. One row per minimal reproducible check. "request" must be a single minimal HTTP request or action. Return exactly:

Endpoint:
host | method | path | evidence

Checks:
check id | objective | request | auth | success | failure

Next Step:
one of: stop | retest with auth | compare contexts | expand input checks | need more evidence

Do not deviate from this schema.
```
