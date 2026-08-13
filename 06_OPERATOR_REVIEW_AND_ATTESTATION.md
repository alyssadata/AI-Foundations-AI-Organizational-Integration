# 06 — FACT CONFIRMATION LOGIC

The operator does **not** manually complete this file.

Step 04 runs this step automatically.

## What happens

After the AI applies the assessment rules, it shows the operator a compact summary of the organization-specific and system-specific facts it used.

The AI asks only:

`CONFIRM / CORRECT`

### If the operator answers CONFIRM

The AI records an Operator Review section in the final Organizational AI Integration Record.

### If the operator answers CORRECT

The AI asks only for the factual correction, updates the working specification, reruns any affected rules, and then asks for confirmation again.

The operator does not edit PASS, FLAG, or UNKNOWN results.

The operator does not create or paste an attestation block.

## Required AI-generated record section

The AI creates this section automatically after confirmation:

```md
## Operator Review

**Operator:** [operator name]
**Organization:** [organization name]
**Review date:** [YYYY-MM-DD]
**Operator confirmation:** CONFIRMED

The operator confirmed that the organization-specific and system-specific facts represented in this record reflect the information supplied for this assessment to the best of the operator's knowledge at the time of review.
```

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** source and confirmer of organization-specific and system-specific facts  
**AI:** presents the fact summary, records corrections, reruns affected rules, and generates the review section

This is a confirmation of operator-supplied facts, not independent verification by AI Foundations.