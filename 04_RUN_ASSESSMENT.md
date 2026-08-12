# 04 — RUN THE ASSESSMENT

Use this step after the operator has completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`.

## What to provide to the AI

In one conversation, provide the AI with:

1. the **completed** `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
2. `02_ASSESSMENT_RULES.yaml`
3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
4. the execution instruction below

## Execution instruction

Copy and paste this instruction into the AI:

> Run the AI Foundations AI Organizational Integration assessment using the completed operator specification, the assessment rules, and the record template I provided.
>
> Apply every rule in `02_ASSESSMENT_RULES.yaml` to the operator-supplied facts in the completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`.
>
> For each rule, return only the outcome permitted by the framework: `PASS`, `FLAG`, or `UNKNOWN`.
>
> Do not invent, infer, repair, or assume organization-specific facts that the operator did not provide. If a required fact is missing or recorded as `UNKNOWN`, follow the unknown-handling rule in `02_ASSESSMENT_RULES.yaml`.
>
> Do not add outside governance standards, legal requirements, vendor recommendations, risk frameworks, or your own assessment criteria. Apply only the supplied AI Foundations assessment rules.
>
> Populate `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md` completely. Preserve the framework source exactly as written. Preserve the operator as the source of organization-specific facts. Identify the specific operator-supplied fields that triggered each finding.
>
> Return one complete Markdown record suitable to save directly as a `.md` file. Do not return commentary before or after the record.
>
> At the top of the record, add:
>
> `**SAVE AS:** ORGANIZATIONAL_AI_INTEGRATION_RECORD_[ORGANIZATION]_[YYYY-MM-DD].md`
>
> Replace `[ORGANIZATION]` and `[YYYY-MM-DD]` using the supplied organization name and assessment date. Use a filename-safe organization name.

## Required output

The AI must return **one completed Organizational AI Integration Record** based on:

**AI Foundations framework + operator-supplied specifications + current assessment rules**

The completed record is the assessment artifact.

## Source and operator boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** source of the organization-specific and system-specific facts  
**AI:** applies the supplied rules and formats the output record

The AI must not represent operator-supplied facts as claims independently verified by AI Foundations.