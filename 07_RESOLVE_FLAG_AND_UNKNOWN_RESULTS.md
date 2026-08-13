# 07 — FLAG AND UNKNOWN HANDLING LOGIC

The operator does **not** manually complete this file.

Step 04 runs this step automatically.

If every assessment result is `PASS`, the AI skips Step 07.

## If the AI finds a FLAG

The AI handles FLAG results one at a time and asks the operator to choose only:

- `FIX IT`
- `KEEP OPEN`
- `DEFER`

The AI explains the finding in plain language before asking for the choice.

### FIX IT

The AI asks what factual control, permission, process, or system configuration has actually changed.

The operator supplies the fact.

The AI updates the working specification and reruns the affected assessment rules itself.

### KEEP OPEN

The AI keeps the FLAG visible in the final record.

### DEFER

The AI records that integration is deferred.

## If the AI finds an UNKNOWN

The AI handles UNKNOWN results one at a time and asks the operator to choose only:

- `SUPPLY INFORMATION`
- `LEAVE UNKNOWN`

### SUPPLY INFORMATION

The AI asks for the missing fact, updates the working specification, and reruns the affected rules itself.

### LEAVE UNKNOWN

The AI keeps the UNKNOWN visible in the final record.

## What the AI does automatically

The AI:

- identifies every FLAG and UNKNOWN
- explains each finding
- asks the choices one at a time
- records the operator's answers
- updates the working specification when new facts are supplied
- reruns affected rules
- counts remaining FLAG and UNKNOWN results
- determines whether the finding status is `PROCEED`, `PROCEED WITH OPEN FINDINGS`, or `DEFER` from the operator's choices
- generates the complete Finding Disposition Status section

The operator does not score, count, build a table, or write the disposition section.

## Required AI-generated record section

When Step 07 applies, the AI generates:

```md
## Finding Disposition Status

[one AI-formatted entry for each FLAG or UNKNOWN]

**Open FLAG results:** [AI calculated]
**Open UNKNOWN results:** [AI calculated]
**Integration disposition:** PROCEED / PROCEED WITH OPEN FINDINGS / DEFER
```

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** supplies organization-specific facts and simple organization choices  
**AI:** performs finding handling, rule reruns, counting, and formatting

The AI must not invent organization-specific facts or organization decisions.