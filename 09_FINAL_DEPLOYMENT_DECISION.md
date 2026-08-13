# 09 — FINAL DEPLOYMENT DECISION LOGIC

The operator does **not** manually complete this file.

Step 04 runs this step automatically after the assessment and any FLAG/UNKNOWN handling are complete.

## What the AI asks

The AI asks for one final organization decision.

If no FLAG or UNKNOWN results remain, the AI offers exactly:

- `APPROVED TO OPERATE`
- `INTEGRATION DEFERRED`
- `RETIRED`

If one or more FLAG or UNKNOWN results remain, the AI offers exactly:

- `APPROVED TO OPERATE — OPEN FINDINGS`
- `INTEGRATION DEFERRED`
- `RETIRED`

The operator chooses one.

The operator does not fill a deployment form.

The AI does not choose the organization's deployment decision.

## What the AI does automatically

After the operator gives the decision, the AI generates the complete Final Deployment Decision section and inserts it into the final Organizational AI Integration Record.

The AI also carries the same decision into the generated Step 10 register row.

## Required AI-generated record section

```md
## Final Deployment Decision

**System ID:** [existing AI-### or AI-XXX]
**AI system:** [from operator-supplied facts]
**Organization:** [from operator-supplied facts]
**Operator / decision recorder:** [from operator-supplied facts]
**Decision date:** [assessment/final decision date]
**Assessment record:** [generated record filename]

**Deployment decision:** [operator's selected allowed value]

**Open findings at decision time:** [AI-generated from current assessment]

**Operating conditions or restrictions:** [operator supplied, or NONE]
```

The AI may ask one optional question for operating conditions or restrictions. If the operator supplies none, record `NONE`.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Organization / operator:** supplies the final deployment decision  
**AI:** presents the valid choices and generates the finished decision record

The decision is organization-supplied. It is not an approval or certification issued by AI Foundations.