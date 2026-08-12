# START HERE — AI Organizational Integration

This repository provides a runnable organizational AI integration assessment.

## Do these files in order

### 01 — Complete the operator specification

Open [`01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`](01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml).

1. Copy the entire contents of that file.
2. Paste it into the AI system you want to use for the intake process.
3. Follow the interview. The AI should ask you for the missing organization- and system-specific facts section by section.
4. Review the completed specification before using it as assessment input.

### 02 — Apply the assessment rules

Use [`02_ASSESSMENT_RULES.yaml`](02_ASSESSMENT_RULES.yaml) against the completed operator specification.

The rules convert the operator-supplied specifications into explicit PASS, FLAG, or UNKNOWN findings.

### 03 — Generate the Organizational AI Integration Record

The standardized output record is the next stage of the workflow and will preserve the framework source, operator, system specifications, and assessment findings.

## Roles

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** the person or organization supplying the factual specifications  
**AI:** intake assistant that structures operator-supplied information  
**Subject:** the AI system being integrated into organizational operations

The AI must not invent organization-specific facts. If a fact is unknown, record it as `UNKNOWN`.

## Operational flow

**01 Operator specification → 02 Assessment rules → 03 Organizational AI Integration Record**

The operator remains the source of the organization-specific facts. AI Foundations remains the source of the framework, structure, and assessment logic.
