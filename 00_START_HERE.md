# START HERE — AI Organizational Integration

This repository gives an organization a structured way to assess one AI system before or during organizational integration.

## What you actually do

You do **not** manually complete every numbered file.

### STEP 1 — Tell the AI about your system

Open [`01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`](01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml).

Copy the whole file into the AI you are using.

The AI will interview you one section at a time and return a completed YAML specification.

**Your job:** answer with facts about your organization and the AI system. If you do not know something, say `UNKNOWN`.

Save the completed specification.

---

### STEP 2 — Run the assessment

Open [`04_RUN_ASSESSMENT.md`](04_RUN_ASSESSMENT.md).

That file tells you exactly what to give the AI.

For the assessment, the AI uses:

- your completed Step 01 specification
- [`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml)
- [`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md)
- the execution instruction inside Step 04

**You do not manually score Step 02.**  
**You do not manually fill Step 03.**

The AI returns one completed Organizational AI Integration Record with `PASS`, `FLAG`, and `UNKNOWN` findings.

---

### STEP 3 — Check that the facts are right

Open [`06_OPERATOR_REVIEW_AND_ATTESTATION.md`](06_OPERATOR_REVIEW_AND_ATTESTATION.md).

Read the completed record and confirm that it accurately reflects the facts you supplied.

If a fact is wrong, correct Step 01 and rerun Step 04.

Do not manually change assessment results.

---

### STEP 4 — Deal with any FLAG or UNKNOWN results

If the record contains a `FLAG` or `UNKNOWN`, open [`07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md`](07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md).

For each result, decide what the organization will do.

If the organization changes a control or supplies missing information, update Step 01 and rerun Step 04.

---

### STEP 5 — Record the organization's decision

Open [`09_FINAL_DEPLOYMENT_DECISION.md`](09_FINAL_DEPLOYMENT_DECISION.md).

Choose and record one decision:

- `APPROVED TO OPERATE`
- `APPROVED TO OPERATE — OPEN FINDINGS`
- `INTEGRATION DEFERRED`
- `RETIRED`

The organization makes this decision. The AI does not make it for the organization.

---

### STEP 6 — Add the system to the organization register

Open [`10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md`](10_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md).

Add or update one row for the assessed AI system so the organization has a current inventory of its integrated AI systems and assessment records.

---

## Files you only use when needed

[`05_EXAMPLE_COMPLETED_ASSESSMENT.md`](05_EXAMPLE_COMPLETED_ASSESSMENT.md) is only an example. You do not have to complete it.

[`08_REASSESSMENT_TRIGGERS.md`](08_REASSESSMENT_TRIGGERS.md) is used later. If the model, provider, instructions, data access, tools, permissions, memory, authority, or other material system configuration changes, use Step 08 to determine whether the assessment must be run again.

---

## The whole workflow in one line

**Tell the AI what the system is → let the framework assess it → check the facts → address findings → make the deployment decision → record the system.**

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator / organization:** supplies the organization-specific facts and makes the deployment decision  
**AI:** conducts the intake, applies the supplied framework rules, and formats the record  
**Subject:** the AI system being assessed

The AI must not invent organization-specific facts.