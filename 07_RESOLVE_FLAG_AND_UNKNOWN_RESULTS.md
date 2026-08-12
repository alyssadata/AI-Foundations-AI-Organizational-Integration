# 07 — HANDLE FLAG AND UNKNOWN RESULTS

Use this step only if the completed Organizational AI Integration Record contains one or more `FLAG` or `UNKNOWN` results.

If every result is `PASS`, skip Step 07 and continue to Step 09.

## What this step does

For each non-PASS result, the organization makes one simple choice.

### If the result is FLAG

Choose one:

- `FIX IT` — the organization will change the relevant control, permission, process, or system configuration.
- `KEEP OPEN` — the organization is not fixing it now and wants the finding to remain visible.
- `DEFER` — the organization does not want to proceed with this integration yet.

### If the result is UNKNOWN

Choose one:

- `SUPPLY INFORMATION` — provide the missing factual information.
- `LEAVE UNKNOWN` — the information is not currently available.

## Easiest way to do Step 07

Paste your completed Organizational AI Integration Record into the AI.

Then copy and paste this prompt:

```text
Help me complete Step 07 of the AI Foundations AI Organizational Integration framework.

Read the completed Organizational AI Integration Record I provided.

Find every result marked FLAG or UNKNOWN.

Ask me about them one at a time.

For each FLAG, ask me to choose exactly one:
FIX IT / KEEP OPEN / DEFER

For each UNKNOWN, ask me to choose exactly one:
SUPPLY INFORMATION / LEAVE UNKNOWN

If I choose FIX IT or SUPPLY INFORMATION, ask me for the factual change or missing information. Do not invent it.

When we are finished, return one Markdown section titled:
## Finding Disposition Status

For each FLAG or UNKNOWN, include:
- Rule ID
- Current outcome
- My chosen action
- Any factual update I supplied

At the end include:
- Open FLAG results: [number]
- Open UNKNOWN results: [number]
- Integration disposition: PROCEED / PROCEED WITH OPEN FINDINGS / DEFER

Do not change any PASS, FLAG, or UNKNOWN result yourself.
Do not invent organization-specific facts or decisions.
```

## Important

If you choose `FIX IT` or `SUPPLY INFORMATION` and the organization actually changes a fact, control, permission, process, or system configuration:

1. update Step 01 with the new factual information
2. rerun Step 04
3. use the new assessment result

Do not manually change a `FLAG` to `PASS` or an `UNKNOWN` to another outcome.

## What comes out of Step 07

One short `Finding Disposition Status` section that records what the organization decided to do about each non-PASS result.

That section can be appended to the completed Organizational AI Integration Record.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Organization / operator:** supplies the facts and chooses what to do about each finding  
**AI:** asks the questions, records the operator's choices, and formats the result

The AI must not invent organization-specific facts, remediation actions, or deployment decisions.