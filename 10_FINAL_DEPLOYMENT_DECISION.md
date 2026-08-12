# 10 — FINAL DEPLOYMENT DECISION

Use this step after the operator has completed Steps 06 and 07 for the current assessment record.

## Purpose

This step records the organization's final operating decision for the assessed AI system.

The assessment findings do not make the deployment decision automatically. The organization remains responsible for deciding whether and under what conditions the system will operate.

## Allowed deployment decisions

Record exactly one:

- `APPROVED TO OPERATE`
- `APPROVED TO OPERATE — OPEN FINDINGS`
- `INTEGRATION DEFERRED`
- `RETIRED`

### APPROVED TO OPERATE

Use when the organization has completed its assessment and chooses to operate the system without unresolved findings it is treating as open.

### APPROVED TO OPERATE — OPEN FINDINGS

Use when the organization chooses to operate the system while one or more Step 07 findings remain explicitly open.

The open findings must remain recorded in the completed Organizational AI Integration Record.

### INTEGRATION DEFERRED

Use when the organization decides the system should not enter or continue the intended integration state at this time.

### RETIRED

Use when the organization has ended operation of the assessed system or configuration.

## Final Deployment Decision Record

Append the following section to the completed Organizational AI Integration Record:

---

## Final Deployment Decision

**System ID:** [AI-### from Step 09]  
**AI system:** [system name]  
**Organization:** [organization name]  
**Operator / decision recorder:** [name]  
**Decision date:** [YYYY-MM-DD]  
**Assessment record:** [current record filename or location]

**Deployment decision:** APPROVED TO OPERATE / APPROVED TO OPERATE — OPEN FINDINGS / INTEGRATION DEFERRED / RETIRED

**Open findings at decision time:** [NONE / list rule IDs and findings]

**Operating conditions or restrictions:** [NONE / operator-supplied conditions]

**Decision notes:** [optional operator-supplied notes]

---

## Register update

After recording the decision:

1. update the system's row in `09_ORGANIZATIONAL_AI_SYSTEM_REGISTER.md`
2. record the current deployment decision
3. confirm the register points to the current completed assessment record
4. preserve all prior assessment and decision records

If a Step 08 reassessment trigger occurs after approval, mark reassessment as required and run the assessment cycle again before treating the previous decision as current for the changed configuration.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Organization / operator:** owns and records the final deployment decision  
**AI:** may format the decision record from operator-supplied information but must not choose, infer, or invent the organization's deployment decision

The final deployment decision is an organization-supplied decision recorded under the AI Foundations AI Organizational Integration framework. It is not an approval, certification, or deployment decision issued by AI Foundations.