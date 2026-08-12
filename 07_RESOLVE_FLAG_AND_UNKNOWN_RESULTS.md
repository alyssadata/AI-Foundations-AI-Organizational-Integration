# 07 — RESOLVE FLAG AND UNKNOWN RESULTS

Use this step after the operator has reviewed and attested to the completed Organizational AI Integration Record.

## Purpose

Step 07 gives the organization an explicit disposition for every assessment result that is not `PASS`.

A `FLAG` means the current operator-supplied specification triggers an integration gap under the current AI Foundations rule set.

An `UNKNOWN` means the current operator-supplied specification does not contain enough information to determine the rule outcome.

Neither result should disappear through manual editing.

## For every FLAG

Create one finding disposition entry:

### [RULE ID] — [Rule name]

**Current outcome:** FLAG  
**Finding:** [copy the finding from the completed record]  
**Triggered by:** [copy the triggering operator-supplied field(s)]  
**Operator disposition:** RESOLVE / ACCEPT AS OPEN / DO NOT INTEGRATE YET  
**Planned action:** [operator supplied]  
**Responsible role:** [operator supplied]  
**Target date:** [operator supplied or UNKNOWN]  
**Evidence of resolution:** [operator supplied or PENDING]

### If the disposition is RESOLVE

Update the relevant factual specification in Step 01 only after the organizational control, process, permission, or system configuration has actually changed.

Then rerun Step 04.

Do not change Step 01 merely to make a FLAG become PASS.

### If the disposition is ACCEPT AS OPEN

Keep the FLAG in the record and document why the organization is proceeding with the finding still open.

The outcome remains `FLAG`.

### If the disposition is DO NOT INTEGRATE YET

Record that the organization is deferring integration until the finding is addressed.

## For every UNKNOWN

Create one unresolved-information entry:

### [RULE ID] — [Rule name]

**Current outcome:** UNKNOWN  
**Missing or unresolved information:** [field or fact]  
**Responsible role:** [operator supplied]  
**Resolution path:** SUPPLY INFORMATION / REMAIN UNKNOWN  
**Target date:** [operator supplied or UNKNOWN]

If new factual information becomes available, update Step 01 and rerun Step 04.

Do not guess the missing fact.

## Final finding status

After all FLAG and UNKNOWN results have dispositions, add this section to the completed Organizational AI Integration Record:

---

## Finding Disposition Status

**Open FLAG results:** [number]  
**Open UNKNOWN results:** [number]  
**Resolved through updated specification and rerun:** [number]  
**Integration disposition:** PROCEED / PROCEED WITH OPEN FINDINGS / DEFER

**Operator rationale:** [operator supplied]

---

`PROCEED` means the operator is proceeding and the current assessment record contains no open FLAG or UNKNOWN results under the current rule set.

`PROCEED WITH OPEN FINDINGS` means the operator is proceeding while one or more FLAG or UNKNOWN results remain explicitly documented.

`DEFER` means the operator is not proceeding with integration at this time.

These are operator dispositions, not AI Foundations certifications of safety, legality, compliance, or fitness for deployment.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** owns organization-specific facts, remediation actions, and the final integration disposition  
**AI:** may structure the disposition record but must not invent remediation, responsible roles, evidence, or organizational decisions

AI Foundations supplies the framework and assessment logic. The organization remains responsible for its deployment decisions and factual representations.
