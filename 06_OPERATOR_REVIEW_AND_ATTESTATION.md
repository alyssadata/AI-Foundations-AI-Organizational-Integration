# 06 — OPERATOR REVIEW AND ATTESTATION

Use this step after Step 04 has produced the completed Organizational AI Integration Record.

Step 05 is an optional worked example and is not part of the operator's assessment.

## Purpose

The operator reviews the completed record and confirms whether it accurately reflects the organization-specific and system-specific facts the operator supplied.

This step does **not** ask the operator to change the AI Foundations assessment rules or independently rescore the assessment.

## What the operator reviews

Check the completed record for factual accuracy in these areas:

1. organization and operator identification
2. subject AI system identification and purpose
3. data, tool, and system access
4. state and memory
5. authority and human approval boundaries
6. revocation, shutdown, inspection, and recovery methods
7. change-control processes
8. operator notes

## If a factual correction is needed

Correct the operator-supplied specification in `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml` first.

Then rerun Step 04 using the corrected specification.

Do **not** manually alter a PASS, FLAG, or UNKNOWN result to make the record match a preferred outcome.

## Operator attestation

After reviewing the final record, append the following section to the end of the completed Organizational AI Integration Record:

---

## Operator Review and Attestation

**Operator:** [operator name]  
**Organization:** [organization name]  
**Review date:** [YYYY-MM-DD]

I reviewed this Organizational AI Integration Record against the organization-specific and system-specific information supplied for this assessment.

**Operator confirmation:** CONFIRMED / CORRECTIONS REQUIRED

If `CONFIRMED`:

The factual specifications represented in this record reflect the information I supplied for this assessment to the best of my knowledge at the time of review.

If `CORRECTIONS REQUIRED`:

List the factual corrections below, update Step 01, and rerun Step 04 before treating the record as final.

**Corrections:** [NONE / list corrections]

---

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** source and reviewer of organization-specific and system-specific facts  
**AI:** intake and assessment assistant that applies the supplied framework rules and formats the record

Operator attestation confirms review of operator-supplied facts. It does not represent independent verification, certification, or endorsement by AI Foundations.
