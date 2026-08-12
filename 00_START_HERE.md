# START HERE — AI Organizational Integration

This repository provides a runnable organizational AI integration assessment.

## Do these files in order

### 01 — Complete the operator specification

Open [`01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`](01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml).

1. Copy the entire contents of that file.
2. Paste it into the AI system you want to use for the intake process.
3. Follow the interview. The AI should ask you for the missing organization- and system-specific facts section by section.
4. Review the completed specification before continuing.

### 02 — Assessment rules

Open [`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml).

These are the AI Foundations rules that will be applied to the completed operator specification. Do not rewrite them for the individual organization.

### 03 — Output record template

Open [`03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`](03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md).

This is the standardized record format the assessment will produce. The operator does not need to fill it manually.

### 04 — Run the assessment

Open [`04_RUN_ASSESSMENT.md`](04_RUN_ASSESSMENT.md).

Follow its execution instructions. Provide the AI with:

- the completed Step 01 specification
- Step 02 assessment rules
- Step 03 record template
- the Step 04 execution instruction

The AI applies the rules and returns one completed Organizational AI Integration Record in Markdown.

### 05 — Compare with the worked example

Open [`05_EXAMPLE_COMPLETED_ASSESSMENT.md`](05_EXAMPLE_COMPLETED_ASSESSMENT.md).

This is an optional fictional example showing a completed Step 01 specification and the resulting record, including both PASS and FLAG outcomes. It is a reference example only and is not operator input.

### 06 — Review and attest to the final record

Open [`06_OPERATOR_REVIEW_AND_ATTESTATION.md`](06_OPERATOR_REVIEW_AND_ATTESTATION.md).

Review the completed Organizational AI Integration Record against the facts you supplied.

If a factual correction is needed, correct Step 01 and rerun Step 04. Do not manually change assessment outcomes.

When the record is accurate, append the Step 06 operator attestation to the completed record.

### 07 — Resolve or disposition FLAG and UNKNOWN results

Open [`07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md`](07_RESOLVE_FLAG_AND_UNKNOWN_RESULTS.md).

For every `FLAG`, record whether the organization will resolve it, accept it as an open finding, or defer integration.

For every `UNKNOWN`, either supply the missing factual information or explicitly leave it unresolved.

If facts or controls change, update Step 01 and rerun Step 04. Do not manually change the assessment outcome.

Append the Step 07 Finding Disposition Status to the completed record.

### 08 — Reassess when the integrated system changes

Open [`08_REASSESSMENT_TRIGGERS.md`](08_REASSESSMENT_TRIGGERS.md).

Use Step 08 after the initial assessment to determine when the existing record no longer describes the system being operated.

A material change to the model, provider, instructions, role, data access, tools, permissions, memory, persistent state, authority, approval boundaries, shutdown, recovery, or integration environment triggers reassessment.

When a trigger occurs, update Step 01 and rerun Steps 04, 06, and 07. Preserve the prior completed record as the historical record of the earlier configuration.

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** the person or organization supplying and reviewing the factual specifications, making the final integration disposition, and identifying material system changes  
**AI:** intake and assessment assistant that structures operator-supplied information, applies the supplied framework rules, and formats the record  
**Subject:** the AI system being integrated into organizational operations

The AI must not invent organization-specific facts. If a fact is unknown, record it as `UNKNOWN`.

## Operational flow

**01 Operator specification → 02 Assessment rules → 03 Record format → 04 Run assessment → completed Organizational AI Integration Record → 05 optional worked example → 06 operator review and attestation → 07 finding resolution and integration disposition → 08 reassessment when material changes occur**

The operator remains the source and reviewer of the organization-specific facts and owns the final deployment decision. AI Foundations remains the source of the framework, structure, assessment logic, record format, and reassessment triggers.
