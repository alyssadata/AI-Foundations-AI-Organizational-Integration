# 04 — RUN THE ASSESSMENT

Use this step after the operator has completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`.

## What to give the AI

In the same conversation, provide:

1. your **completed** `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
2. `02_ASSESSMENT_RULES.yaml`
3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
4. the copy/paste prompt below

You may paste the three files as text or attach them if your AI interface supports file attachments.

## COPY AND PASTE THIS PROMPT

Copy the entire block below and paste it into the AI after providing the three files above.

```text
Run the AI Foundations AI Organizational Integration assessment now.

Use only these materials I provided:
1. my completed 01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml
2. 02_ASSESSMENT_RULES.yaml
3. 03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md

Apply every rule in 02_ASSESSMENT_RULES.yaml to the operator-supplied facts in my completed Step 01 specification.

For every rule, return only one permitted outcome: PASS, FLAG, or UNKNOWN.

Do not invent, infer, repair, or assume organization-specific facts I did not provide. If information is missing or UNKNOWN, follow the unknown-handling rule in Step 02.

Do not add outside governance standards, legal requirements, vendor recommendations, risk frameworks, or your own assessment criteria. Apply only the supplied AI Foundations rules.

Populate the Step 03 record template completely.

Preserve this framework source exactly:
Alyssa Solen → AI Foundations → AI Organizational Integration

Preserve the operator as the source of organization-specific facts. For each assessment finding, identify the specific operator-supplied field or fields that produced the result.

Return ONE complete Markdown Organizational AI Integration Record suitable to save directly as a .md file.

Do not add commentary before or after the record.

At the very top write:
**SAVE AS:** ORGANIZATIONAL_AI_INTEGRATION_RECORD_[ORGANIZATION]_[YYYY-MM-DD].md

Replace [ORGANIZATION] and [YYYY-MM-DD] using the organization name and assessment date in my completed Step 01 specification. Use a filename-safe organization name.
```

## What you should get back

The AI should return **one completed Organizational AI Integration Record** containing the operator-supplied system information and the Step 02 `PASS`, `FLAG`, or `UNKNOWN` results.

Save that returned Markdown record. You will use it in Step 06.

## Source and operator boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** source of the organization-specific and system-specific facts  
**AI:** applies the supplied rules and formats the output record

The AI must not represent operator-supplied facts as claims independently verified by AI Foundations.