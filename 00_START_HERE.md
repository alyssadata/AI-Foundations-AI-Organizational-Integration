# START HERE — AI Organizational Integration

## What this gives you

**This framework gives you a dated snapshot of where your organization is today with one AI system, where the current gaps or unknowns are, and a baseline you can reassess when the system changes.**

For the plain-language explanation of what the assessment does and what you receive at the end, see [`WHAT_THIS_IS_AND_WHAT_YOU_GET.md`](WHAT_THIS_IS_AND_WHAT_YOU_GET.md).

This repository is designed so the operator does **not** grade, score, calculate, build tables, or manually complete assessment forms.

**The AI does the framework work.**

The operator supplies organization-specific facts and simple organization choices when asked.

# THE WHOLE EXPERIENCE

There are only **two paste actions** in a normal assessment.

## PASTE 1 — Start the guided intake

Open [`01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`](01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml).

Copy the entire file and paste it into the AI.

The AI will:

- explain that it is guiding Step 01
- ask the missing questions ONE AT A TIME
- use plain language
- record `UNKNOWN` when the operator does not know an answer
- build the YAML itself
- return one completed Step 01 YAML specification

The operator only answers factual questions.

When Step 01 is finished, the AI is instructed to tell the operator:

> Step 01 is complete. Copy the completed YAML above.
> Next, give the AI these FOUR items together:
> 1. your completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
> 2. `02_ASSESSMENT_RULES.yaml`
> 3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
> 4. `04_RUN_ASSESSMENT.md`
> Step 04 will run the assessment for you. You do not grade or fill anything yourself.

## PASTE 2 — Give the AI 01 + 02 + 03 + 04 together

Provide these FOUR items together in the same conversation:

1. the completed Step 01 YAML returned by the AI
2. [`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml)
3. [`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md)
4. [`04_RUN_ASSESSMENT.md`](04_RUN_ASSESSMENT.md)

You may paste them as text or attach them if the AI interface supports attachments.

**You do not need to pull a separate prompt out of Step 04.**

Step 04 contains the runner instructions.

If the AI does not have all four items, Step 04 instructs it to stop and ask for the missing assessment files rather than making the operator figure out what to do.

Once all four are present, the AI runs the workflow automatically.

# WHAT THE AI DOES AFTER PASTE 2

The AI:

- applies every assessment rule
- determines every `PASS`, `FLAG`, and `UNKNOWN`
- checks the facts with the operator using `CONFIRM / CORRECT`
- handles FLAG findings one at a time using simple choices
- handles UNKNOWN findings one at a time using simple choices
- reruns affected rules after factual updates
- counts findings itself
- creates the finding-disposition section
- asks for the final organizational deployment choice
- creates the final deployment-decision section
- outputs the final completed Step 01 specification
- outputs the finished Organizational AI Integration Record
- outputs the ready-to-paste organizational system-register row

# WHAT THE OPERATOR DOES NOT DO

The operator does **not**:

- grade the assessment
- decide whether a rule is PASS, FLAG, or UNKNOWN
- manually apply Step 02
- manually fill Step 03
- count findings
- build tables
- write the Step 06 review section
- write the Step 07 disposition section
- write the Step 09 deployment section
- build the Step 10 register row

The operator only supplies facts and organization decisions the AI cannot legitimately invent.

# WHAT THE OTHER FILES ARE

[`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml) — assessment logic the AI applies.

[`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md) — output structure the AI fills.

[`05_EXAMPLE_COMPLETED_ASSESSMENT.md`](05_EXAMPLE_COMPLETED_ASSESSMENT.md) — fictional worked example only.

[`06_OPERATOR_REVIEW_AND_ATTESTATION.md`](06_OPERATOR_REVIEW_AND_ATTESTATION.md) — fact-confirmation logic Step 04 runs automatically.

[`07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md`](07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md) — finding-handling logic Step 04 runs automatically.

[`08_REASSESSMENT_TRIGGERS.md`](08_REASSESSMENT_TRIGGERS.md) — later reassessment logic if the system changes.

[`09_FINAL_DEPLOYMENT_DECISION.md`](09_FINAL_DEPLOYMENT_DECISION.md) — deployment-decision logic Step 04 runs automatically.

[`10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md`](10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md) — register-output structure Step 04 uses.

[`99_WRAP_UP_SUMMARY.md`](99_WRAP_UP_SUMMARY.md) — final summary of what the operator has in hand, what to save, and what to do if the system changes later.

# IN ONE LINE

**Paste 01 → answer questions → receive completed 01 → give completed 01 + 02 + 03 + 04 together → answer simple choices → receive finished outputs.**

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator / organization:** supplies organization-specific facts and organization decisions  
**AI:** conducts intake, applies rules, calculates assessment outcomes, guides the workflow, and formats finished artifacts  
**Subject:** the AI system being assessed

The AI must not invent organization-specific facts or make the organization's final deployment decision.
