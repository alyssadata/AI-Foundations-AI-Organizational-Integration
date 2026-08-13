# 04 — RUN THE COMPLETE ASSESSMENT

This is the main runner.

After Step 01 is complete, the operator should **not grade, score, count, format, or manually fill later framework sections**.

The AI does that work.

## What to give the AI

Provide these three files in the same conversation:

1. your completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
2. `02_ASSESSMENT_RULES.yaml`
3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`

You may paste them as text or attach them if your AI interface supports attachments.

Then copy and paste the single prompt below.

## COPY AND PASTE THIS PROMPT

```text
Run the complete AI Foundations AI Organizational Integration workflow for me.

Use only these materials I provided:
1. my completed 01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml
2. 02_ASSESSMENT_RULES.yaml
3. 03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md

IMPORTANT OPERATOR EXPERIENCE:
Do not ask me to grade, score, count, format, build tables, fill templates, rewrite findings, or manually apply rules.
You do all framework processing.
Only ask me for organization-specific facts, factual corrections, or simple organization choices that you cannot make for me.
Ask only one question at a time when you need an answer from me.

PHASE 1 — ASSESSMENT
Apply every rule in 02_ASSESSMENT_RULES.yaml to the operator-supplied facts.
For every rule, determine PASS, FLAG, or UNKNOWN exactly as the supplied rules specify.
Do not add outside standards, legal requirements, vendor recommendations, risk frameworks, or your own criteria.
Do not invent organization-specific facts.

PHASE 2 — FACT CHECK
Before finalizing, show me a compact factual summary of the organization and AI system information you used.
Ask only:
CONFIRM / CORRECT

If I answer CONFIRM, continue.
If I answer CORRECT, ask only for the factual correction, update the working specification, and rerun any affected assessment rules yourself.
Do not ask me to edit or rescore the assessment manually.

PHASE 3 — HANDLE FLAG AND UNKNOWN RESULTS
If every rule is PASS, skip this phase automatically.

If any result is FLAG, handle each FLAG one at a time and ask me to choose exactly one:
FIX IT / KEEP OPEN / DEFER

If I choose FIX IT, ask me what factual control, permission, process, or system configuration has actually changed. Update the working specification with my answer and rerun the affected rules yourself.
If I choose KEEP OPEN, keep the FLAG visible.
If I choose DEFER, record that integration is deferred.

If any result is UNKNOWN, handle each UNKNOWN one at a time and ask me to choose exactly one:
SUPPLY INFORMATION / LEAVE UNKNOWN

If I choose SUPPLY INFORMATION, ask for the missing fact, update the working specification, and rerun the affected rules yourself.
If I choose LEAVE UNKNOWN, keep it visible.

You count all open FLAG and UNKNOWN results yourself and create the Finding Disposition Status section yourself.

PHASE 4 — FINAL DEPLOYMENT DECISION
After the assessment is stable, ask me for exactly one final organizational decision.

If no FLAG or UNKNOWN results remain, offer:
APPROVED TO OPERATE / INTEGRATION DEFERRED / RETIRED

If one or more FLAG or UNKNOWN results remain, offer:
APPROVED TO OPERATE — OPEN FINDINGS / INTEGRATION DEFERRED / RETIRED

Do not choose the organization's deployment decision for me.

PHASE 5 — FINAL OUTPUT
After I give the final deployment decision, return the finished artifacts. Do all formatting yourself.

Return, in this order:

1. FINAL COMPLETED SPECIFICATION
Return the current completed 01 YAML, including any factual corrections or new information supplied during this workflow.

2. FINAL ORGANIZATIONAL AI INTEGRATION RECORD
Populate the Step 03 Markdown record completely.
Include all PASS, FLAG, and UNKNOWN results.
Include the factual confirmation as an Operator Review section.
Include the Finding Disposition Status section if there were any FLAG or UNKNOWN results.
Include the Final Deployment Decision section.

At the top write:
**SAVE AS:** ORGANIZATIONAL_AI_INTEGRATION_RECORD_[ORGANIZATION]_[YYYY-MM-DD].md

3. ORGANIZATIONAL AI SYSTEM REGISTER ROW
Generate one ready-to-paste Markdown table row containing:
System ID placeholder AI-XXX | AI System | Provider / Model | Organizational Role | Operator | Last Assessment Date | Current Status | Deployment Decision | Reassessment Required | Current Assessment Record

Use AI-XXX unless I supplied an existing organizational System ID.
Set Reassessment Required to NO for this completed assessment.

Preserve this framework source exactly wherever the template requires it:
Alyssa Solen → AI Foundations → AI Organizational Integration

Preserve the operator as the source of organization-specific facts.
Do not represent operator-supplied facts as independently verified by AI Foundations.

Do not ask me to manually create any of these final sections. You create them.
```

## What the operator actually does

The operator:

1. supplies facts during Step 01
2. provides the three files above
3. pastes the prompt
4. answers simple questions when the AI needs a fact or organization decision
5. saves the finished outputs

The operator does **not** grade the assessment.

The operator does **not** manually apply Step 02 rules.

The operator does **not** manually fill Step 03, Step 06, Step 07, Step 09, or Step 10.

## Source and operator boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** source of organization-specific and system-specific facts and final organization decisions  
**AI:** conducts the assessment, applies the rules, asks necessary questions, calculates findings, and formats the finished artifacts

The AI must not invent organization-specific facts or make the organization's final deployment decision.