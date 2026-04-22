# Prompt Hardening for Offensive Workflows

A Codex Skill that rewrites rough AI prompts used in authorized offensive security workflows to reduce hallucination, constrain assumptions, and keep outputs grounded in observed evidence.

---

## Why this exists

AI is becoming part of offensive security workflows, but most prompts are:

* too vague
* overly assumptive
* prone to hallucinated conclusions
* not structured for validation

This leads to:

* false positives
* wasted time
* misleading analysis
* overconfident outputs

This skill helps operators **engineer their prompts**, not just write them.

---

## What it does

Given a rough prompt, this skill rewrites it to:

* anchor on observed evidence
* prevent assumed authentication or access
* separate facts from inferences and speculation
* enforce scope and authorization constraints
* bias toward minimal, testable validation steps
* require uncertainty to be stated clearly

---

## Example

### Before

What can I do with these endpoints?

### After

Using only the observed endpoints, parameters, and responses provided below, identify plausible security testing directions for an authorized assessment. Do not assume additional routes, authenticated functionality, internal access, or business logic not directly evidenced.

Group your answer into:

1. Observed attack surface
2. Likely validation targets
3. Assumptions requiring confirmation

Prioritize concise, testable next steps and clearly state any uncertainty.

---

## Best used for

* Bug bounty workflows
* Internal authorized testing
* Recon triage
* Web/API analysis
* Findings validation
* Note cleanup

---

## Not for

* Unauthorized testing
* Exploit automation
* Payload generation against real targets

---

## Usage

Provide:

* your rough prompt
* context (optional)
* observed evidence (optional)

The skill returns:

* a hardened prompt
* a short explanation of improvements

---

## Philosophy

> AI should assist operators, not mislead them.

This project focuses on:

* signal over noise
* validation over speculation
* control over convenience

---

## License

GNU GPL-3
