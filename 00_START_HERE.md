# START HERE — AI Organizational Integration

This repository is designed so the operator does **not** grade, score, calculate, build tables, or manually complete assessment forms.

**The AI does the framework work.**

The operator supplies organization-specific facts and simple organization choices when asked.

## THE EASY WORKFLOW

You personally use only **Step 01** and **Step 04** for a normal assessment.

### 1 — Tell the AI about the system

Open [`01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`](01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml).

Copy the whole file into the AI.

The AI asks you for the missing facts one question at a time.

Answer the questions. If you do not know something, say `UNKNOWN`.

The AI returns the completed Step 01 specification.

### 2 — Let the AI do the entire assessment

Open [`04_RUN_ASSESSMENT.md`](04_RUN_ASSESSMENT.md).

Give the AI:

- your completed Step 01 specification
- [`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml)
- [`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md)

Then copy the **one prompt** in Step 04 and paste it into the AI.

From there, the AI runs the rest of the workflow.

## What the AI does for you

The AI:

- applies every assessment rule
- determines every `PASS`, `FLAG`, and `UNKNOWN`
- creates the assessment record
- asks you only to confirm or correct the facts it used
- handles every FLAG or UNKNOWN one at a time
- reruns rules when you supply corrected or new facts
- counts open findings
- creates the finding-disposition section
- asks for the final organization deployment choice
- creates the final deployment-decision section
- creates the ready-to-paste organizational system-register row

## What you do NOT do

You do **not**:

- score the assessment
- decide whether a rule is PASS or FLAG
- count findings
- fill the record template
- build a disposition table
- write the operator-review section
- write the deployment-decision section
- build the register row

The AI does those things from the framework rules and the facts you supply.

## What the other numbered files are

[`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml) — rules the AI applies. You do not score them.

[`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md) — output structure the AI fills.

[`05_EXAMPLE_COMPLETED_ASSESSMENT.md`](05_EXAMPLE_COMPLETED_ASSESSMENT.md) — fictional example only.

[`06_OPERATOR_REVIEW_AND_ATTESTATION.md`](06_OPERATOR_REVIEW_AND_ATTESTATION.md) — fact-confirmation logic Step 04 runs automatically.

[`07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md`](07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md) — FLAG/UNKNOWN handling logic Step 04 runs automatically.

[`08_REASSESSMENT_TRIGGERS.md`](08_REASSESSMENT_TRIGGERS.md) — used later if the system changes; the AI applies the triggers.

[`09_FINAL_DEPLOYMENT_DECISION.md`](09_FINAL_DEPLOYMENT_DECISION.md) — deployment-decision logic Step 04 runs automatically.

[`10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md`](10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md) — register-output logic Step 04 uses to generate the finished row.

## In one line

**Paste Step 01 → answer factual questions → paste Step 04 → answer simple choices → receive finished outputs.**

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator / organization:** supplies organization-specific facts and organization decisions  
**AI:** conducts intake, applies rules, calculates assessment outcomes, handles workflow logic, and formats all finished artifacts  
**Subject:** the AI system being assessed

The AI must not invent organization-specific facts or make the organization's final deployment decision.