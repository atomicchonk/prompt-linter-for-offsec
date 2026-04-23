# Prompt Linter for Offensive Security

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![AI](https://img.shields.io/badge/AI-assisted-blue)
![Security](https://img.shields.io/badge/Security-Offensive-orange)
![Type](https://img.shields.io/badge/Type-Codex%20Skill-purple)
![Status](https://img.shields.io/badge/Status-Active-success)

<img width="447" height="280" alt="image" src="https://github.com/user-attachments/assets/ddabee89-c6d0-4718-bead-f0047bb511c3" /> 

---




A minimal Codex skill that rewrites vague prompts into **deterministic, phase-correct prompts** for security workflows.

Enabling operators to get the most "bang-for-their-buck" in terms of tokens and output.

---

## What it does

* Detects the phase: **Recon, Validation, Analysis, Reporting**
* Rewrites your prompt into a **structured, constrained version**
* Enforces:

  * evidence-only reasoning
  * strict scope
  * reproducible outputs
  * fixed schemas

---

## Why use it

AI in offsec tends to:

* hallucinate endpoints or behavior
* assume access or context
* mix multiple tasks into one step

This fixes that by forcing **clean, single-purpose prompts**.

---

## Phases

| Phase      | Purpose           |
| ---------- | ----------------- |
| Recon      | Extract surface   |
| Validation | Confirm behavior  |
| Analysis   | Interpret results |
| Reporting  | Present findings  |

Each phase outputs a **strict schema** (no freeform text).

---

## Example

**Input**

```
enumerate endpoints and test for issues
```

**Output**

```
Detected Phase
Recon

Hardened Prompt
Extract and normalize only provided surface. No assumptions. Return:

Surface:
host | method | path | evidence
```

---

## Reporting formats

Default: **generic**

Optional:

* `HackerOne`
* `Bugcrowd`

---

## Design principles

* **Deterministic** → same structure every time
* **Evidence-first** → no guessing
* **Minimal** → no extra sections
* **Composable** → outputs chain cleanly

---

## What this is NOT

* not a scanner
* not a vuln finder
* not an agent framework

It only:

> rewrites prompts so AI behaves predictably

---

## TL;DR

* one skill
* one job
* no hallucinations
* clean outputs

Use it when your prompts are messy and your results aren’t reliable.
