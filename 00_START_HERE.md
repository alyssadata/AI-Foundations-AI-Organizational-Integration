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

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** the person or organization supplying the factual specifications  
**AI:** intake and assessment assistant that structures operator-supplied information, applies the supplied framework rules, and formats the record  
**Subject:** the AI system being integrated into organizational operations

The AI must not invent organization-specific facts. If a fact is unknown, record it as `UNKNOWN`.

## Operational flow

**01 Operator specification → 02 Assessment rules → 03 Record format → 04 Run assessment → completed Organizational AI Integration Record → 05 optional worked example**

The operator remains the source of the organization-specific facts. AI Foundations remains the source of the framework, structure, assessment logic, and record format.
