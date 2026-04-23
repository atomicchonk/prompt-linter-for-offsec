# Example 1
## Original Prompt

Find all endpoints on this target.

## Detected Phase

### Recon

## Hardened Prompt

```
Rewrite only from provided target data. Extract and normalize surface. Do not interpret behavior, prioritize targets, infer workflows, assume auth, or expand scope. Missing data = unknown. Return exactly:

Surface:
host | method | path | evidence

Inputs:
parameter | location | evidence

Auth Signals:
signal | evidence

Unknowns:
item | missing evidence
```
