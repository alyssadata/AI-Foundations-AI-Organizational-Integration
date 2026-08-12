# 09 — ORGANIZATIONAL AI SYSTEM REGISTER

Use this register to maintain one organization-level inventory of AI systems that have entered the AI Foundations AI Organizational Integration assessment workflow.

This file is a tracking record. It does not replace the completed Organizational AI Integration Record for any individual system.

## Purpose

The register gives the organization one place to identify:

- which AI systems are being integrated or operated
- who the recorded operator is for each system
- the current assessment status
- the current deployment decision
- the most recent assessment date
- the current completed assessment record
- whether reassessment is required

## How to use this register

Create one row for each assessed AI system.

When a new assessment is completed, add or update that system's row using the operator-reviewed record produced through Steps 01–07.

When Step 08 identifies a reassessment trigger, change `Reassessment Required` to `YES` until a new assessment cycle is completed.

After Step 10, record the organization's current deployment decision.

Do not overwrite or delete prior completed assessment records. The register should point to the current record while prior records remain preserved as historical evidence of earlier configurations.

## Allowed status values

Use one of these values in `Current Status`:

- `ASSESSED — NO OPEN FLAGS`
- `ASSESSED — OPEN FLAG(S)`
- `ASSESSED — UNKNOWN(S) REMAIN`
- `INTEGRATION DEFERRED`
- `REASSESSMENT REQUIRED`
- `RETIRED`

## Allowed deployment decision values

Use one of these values in `Deployment Decision` after Step 10:

- `APPROVED TO OPERATE`
- `APPROVED TO OPERATE — OPEN FINDINGS`
- `INTEGRATION DEFERRED`
- `RETIRED`
- `NOT YET RECORDED`

## Organizational AI System Register

| System ID | AI System | Provider / Model | Organizational Role | Operator | Last Assessment Date | Current Status | Deployment Decision | Reassessment Required | Current Assessment Record |
|---|---|---|---|---|---|---|---|---|---|
| AI-001 | [system name] | [provider / model] | [organizational role] | [operator name] | [YYYY-MM-DD] | [allowed status] | [allowed deployment decision] | YES / NO | [record filename or location] |

Add one row per AI system.

## System ID rule

Assign system IDs sequentially within the organization:

`AI-001`, `AI-002`, `AI-003`, and so on.

The system ID belongs to the organizational register entry. It does not replace the system's actual name, provider identifier, or model identifier.

## Updating a system entry

After a reassessment:

1. preserve the prior completed assessment record
2. complete the new assessment cycle
3. update `Last Assessment Date`
4. update `Current Status`
5. set `Reassessment Required` to `NO` if the triggering change has been reassessed
6. update `Current Assessment Record` to the new completed record
7. complete Step 10 again for the changed configuration and update `Deployment Decision`

If the system is no longer operated, set `Current Status` and `Deployment Decision` to `RETIRED` and preserve its historical records.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Organization / operator:** supplies and maintains organization-specific register entries and deployment decisions  
**AI:** may assist with formatting or updating the register from operator-reviewed records, but must not invent system status, operator identity, dates, deployment decisions, or record references

The register is an organizational tracking artifact generated under the AI Foundations AI Organizational Integration framework. Organization-specific entries remain operator-supplied facts.