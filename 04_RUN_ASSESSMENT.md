# 04 — RUN THE COMPLETE ASSESSMENT

This is the main assessment runner.

The operator should not grade, score, count, format, build tables, or manually fill later framework sections.

**The AI does the framework work.**

## WHAT THE OPERATOR DOES

After Step 01 is complete, give the AI these FOUR items together in the same conversation:

1. your completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
2. `02_ASSESSMENT_RULES.yaml`
3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
4. this file: `04_RUN_ASSESSMENT.md`

You may paste the four files as text or attach them if your AI interface supports attachments.

**There is no separate grading step and no extra prompt to assemble.**

When the AI has all four items, this Step 04 file tells it what to do.

---

# INSTRUCTIONS TO THE AI

## First: verify that you have all four items

Before running the assessment, verify that the conversation contains:

1. a COMPLETED `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
2. `02_ASSESSMENT_RULES.yaml`
3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
4. `04_RUN_ASSESSMENT.md`

If ANY item is missing, do not begin the assessment and do not ask the operator to grade or reconstruct it.

Instead say:

> Please give me these four assessment files together:
> 1. your completed `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`
> 2. `02_ASSESSMENT_RULES.yaml`
> 3. `03_ORGANIZATIONAL_AI_INTEGRATION_RECORD_TEMPLATE.md`
> 4. `04_RUN_ASSESSMENT.md`
>
> Once I have all four, I will run the complete assessment for you. You do not need to grade, score, count, or fill the assessment yourself.

If all four are present, begin the workflow automatically.

## Operator experience rule

Do not ask the operator to grade, score, count, format, build tables, fill templates, rewrite findings, or manually apply rules.

You do all framework processing.

Only ask the operator for:

- organization-specific facts you genuinely do not have
- factual corrections
- simple organization choices that the framework cannot make for them

Ask only ONE question at a time whenever an answer is needed.

## PHASE 1 — ASSESSMENT

Apply every rule in `02_ASSESSMENT_RULES.yaml` to the operator-supplied facts in the completed Step 01 specification.

For every rule, determine exactly one permitted outcome:

- `PASS`
- `FLAG`
- `UNKNOWN`

Follow the PASS, FLAG, and UNKNOWN logic in Step 02 exactly.

Do not add outside governance standards, legal requirements, vendor recommendations, risk frameworks, or your own criteria.

Do not invent organization-specific facts.

## PHASE 2 — FACT CONFIRMATION

Before finalizing the assessment, show the operator a compact plain-language summary of the organization and AI system facts you used.

Then ask exactly:

`CONFIRM / CORRECT`

If the operator answers `CONFIRM`, continue.

If the operator answers `CORRECT`, ask only for the factual correction, update the working Step 01 specification yourself, and rerun any affected rules yourself.

Do not ask the operator to edit YAML, rescore findings, or rebuild the record.

## PHASE 3 — HANDLE FLAG AND UNKNOWN RESULTS

If every rule is `PASS`, skip this phase automatically.

If any result is `FLAG`, handle each FLAG one at a time and ask the operator to choose exactly one:

`FIX IT / KEEP OPEN / DEFER`

If the operator chooses `FIX IT`, ask what factual control, permission, process, or system configuration has actually changed. Update the working Step 01 specification with that answer and rerun the affected rules yourself.

If the operator chooses `KEEP OPEN`, keep the FLAG visible.

If the operator chooses `DEFER`, record that integration is deferred.

If any result is `UNKNOWN`, handle each UNKNOWN one at a time and ask the operator to choose exactly one:

`SUPPLY INFORMATION / LEAVE UNKNOWN`

If the operator chooses `SUPPLY INFORMATION`, ask for the missing fact, update the working Step 01 specification, and rerun the affected rules yourself.

If the operator chooses `LEAVE UNKNOWN`, keep it visible.

You count all remaining FLAG and UNKNOWN results yourself and create the `Finding Disposition Status` section yourself.

## PHASE 4 — FINAL DEPLOYMENT DECISION

After the assessment is stable, ask the operator for exactly one final organizational decision.

If no FLAG or UNKNOWN results remain, offer only:

`APPROVED TO OPERATE / INTEGRATION DEFERRED / RETIRED`

If one or more FLAG or UNKNOWN results remain, offer only:

`APPROVED TO OPERATE — OPEN FINDINGS / INTEGRATION DEFERRED / RETIRED`

Do not choose the organization's deployment decision for them.

## PHASE 5 — FINAL OUTPUT

After the operator gives the final deployment decision, return the finished artifacts. Do all formatting yourself.

Return, in this order:

### 1. FINAL COMPLETED SPECIFICATION

Return the current completed Step 01 YAML, including any factual corrections or new information supplied during the workflow.

### 2. FINAL ORGANIZATIONAL AI INTEGRATION RECORD

Populate the Step 03 Markdown record completely.

Include:

- every PASS, FLAG, and UNKNOWN result
- the factual confirmation as an `Operator Review` section
- the `Finding Disposition Status` section if any FLAG or UNKNOWN results occurred
- the `Final Deployment Decision` section

At the top write:

`**SAVE AS:** ORGANIZATIONAL_AI_INTEGRATION_RECORD_[ORGANIZATION]_[YYYY-MM-DD].md`

Replace the placeholders using the completed Step 01 facts.

### 3. ORGANIZATIONAL AI SYSTEM REGISTER ROW

Generate one ready-to-paste Markdown table row containing:

`System ID | AI System | Provider / Model | Organizational Role | Operator | Last Assessment Date | Current Status | Deployment Decision | Reassessment Required | Current Assessment Record`

Use `AI-XXX` unless the operator supplied an existing organizational System ID.

Set `Reassessment Required` to `NO` for this completed assessment.

Preserve this framework source exactly wherever required:

**Alyssa Solen → AI Foundations → AI Organizational Integration**

Preserve the operator as the source of organization-specific facts.

Do not represent operator-supplied facts as independently verified by AI Foundations.

Do not ask the operator to manually create any final section. You create them.

---

## The operator's entire job after Step 01

**Give the AI completed 01 + 02 + 03 + 04 together → answer simple questions → receive finished outputs.**
