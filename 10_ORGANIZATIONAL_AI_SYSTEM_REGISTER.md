# 10 — ORGANIZATIONAL AI SYSTEM REGISTER OUTPUT

The operator does **not** manually build the register row.

Step 04 generates a ready-to-paste register row automatically after the final deployment decision is recorded.

## What the AI generates

For the completed assessment, the AI produces one Markdown table row with:

| System ID | AI System | Provider / Model | Organizational Role | Operator | Last Assessment Date | Current Status | Deployment Decision | Reassessment Required | Current Assessment Record |
|---|---|---|---|---|---|---|---|---|---|

The AI fills every value from the current completed assessment and final deployment decision.

If an existing System ID was supplied, use it.

If this is a new system and no System ID was supplied, use `AI-XXX` as a placeholder so the organization can assign its next sequential ID without rebuilding the row.

For a newly completed assessment, set `Reassessment Required` to `NO`.

## AI-derived Current Status

The AI derives `Current Status` from the final current record:

- no open FLAG or UNKNOWN results + approved → `ASSESSED — NO OPEN FLAGS`
- open FLAG result(s) → `ASSESSED — OPEN FLAG(S)`
- no open FLAG but one or more UNKNOWN results → `ASSESSED — UNKNOWN(S) REMAIN`
- deployment decision is deferred → `INTEGRATION DEFERRED`
- deployment decision is retired → `RETIRED`

The operator does not calculate this status.

## Reassessment

When Step 08 later identifies a material change, the AI should generate an updated register row with `Reassessment Required` set to `YES` until the new assessment is completed.

After reassessment, the AI generates a new current row pointing to the new assessment record.

Prior completed assessment records must remain preserved as historical records of earlier configurations.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator / organization:** supplies the underlying organization-specific facts and maintains its register  
**AI:** derives the register status from the completed framework record and generates the ready-to-paste row

The AI must not invent organization-specific facts, an existing System ID, or a deployment decision.