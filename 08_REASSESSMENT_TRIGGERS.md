# 08 — REASSESSMENT TRIGGER LOGIC

The operator does **not** manually grade reassessment triggers.

Use this file later, after an AI system has already been assessed, when something about the system may have changed.

## Easiest use

Give the AI:

1. the prior completed Organizational AI Integration Record
2. the current facts or description of what changed
3. this Step 08 file

Then ask:

```text
Apply Step 08 to the prior assessment record and the current facts I supplied.
Tell me whether reassessment is REQUIRED or NOT REQUIRED under these triggers.
Identify the specific changed facts that triggered the result.
Do not invent changes I did not supply.
If reassessment is required, tell me to rerun the Step 04 complete workflow using the updated facts.
```

## Reassessment is REQUIRED when any of these materially changes

- underlying model, model version, provider, hosting, or system architecture
- system instructions, operating instructions, purpose, organizational role, or workflow responsibilities
- internal, external, sensitive, or restricted data access
- tools, APIs, internal systems, external services, credentials, permissions, write access, or execution capability
- persistent memory, memory scope, cross-session state, cross-user state, retention, inspection, deletion, or recovery
- external communication authority, decision authority, action authority, record/state modification authority, or human approval boundaries
- authority revocation, responsible control role, shutdown, state inspection, or recovery methods
- department, workflow, product, business unit, operating environment, or materially different organizational responsibilities
- movement from an isolated AI tool into persistent organizational systems or operational state

## If reassessment is REQUIRED

The AI should:

1. identify which operator-supplied facts changed
2. carry those current facts into a new working Step 01 specification
3. rerun the complete Step 04 workflow
4. generate a new assessment record
5. preserve the prior record as historical evidence of the earlier configuration
6. generate an updated Step 10 register row

The operator does not manually rescore the old record.

## If reassessment is NOT REQUIRED

The prior assessment remains current under Step 08 unless the organization chooses to reassess anyway.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** supplies the facts about what changed  
**AI:** compares those supplied changes against the Step 08 triggers and formats the result

The AI must not invent system changes that the operator did not supply.