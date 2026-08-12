# 08 — REASSESSMENT TRIGGERS

Use this step after the organization has completed its initial assessment and dispositioned any FLAG or UNKNOWN results.

## Purpose

An Organizational AI Integration Record describes a specific system under a specific set of operator-supplied conditions.

When those conditions materially change, the existing record may no longer describe the system being operated.

This step defines when the organization should update Step 01 and rerun the assessment.

## Reassessment is triggered when any of the following materially changes

### Model or provider

- underlying model
- model version
- model provider
- hosted versus local deployment
- system architecture that changes model behavior or access

### Instructions or organizational role

- system instructions
- operating instructions
- assigned purpose
- organizational role
- workflow responsibilities

### Data access

- new internal data access
- new external data access
- access to sensitive or restricted data
- expansion or removal of datasets, repositories, records, or knowledge sources

### Tool and system access

- new tools
- new APIs
- new internal systems
- new external services
- new credentials or permissions
- expanded write or execution capability

### Memory or persistent state

- persistent memory enabled or disabled
- memory scope changed
- cross-session state changed
- cross-user state changed
- retention, inspection, deletion, or recovery method changed

### Authority

- ability to communicate externally changes
- decision authority changes
- action authority changes
- ability to modify records or organizational state changes
- human approval boundaries change

### Control and recovery

- authority revocation method changes
- responsible control role changes
- shutdown method changes
- state inspection method changes
- recovery method changes

### Integration environment

- the AI is moved into a new department, workflow, product, business unit, or operating environment
- the same AI system is given materially different organizational responsibilities
- previously isolated AI becomes connected to persistent organizational systems or operational state

## What to do when a trigger occurs

1. Open `01_ORGANIZATIONAL_AI_INTEGRATION_SPEC.yaml`.
2. Update only the operator-supplied facts that changed.
3. Set a new assessment date.
4. Rerun Step 04 using the current Step 02 rules and Step 03 record template.
5. Complete Step 06 operator review again.
6. Complete Step 07 for any new FLAG or UNKNOWN results.
7. Preserve the prior completed record as the historical record of the earlier configuration.

Do not overwrite an older completed assessment record as though the earlier system state never existed.

## No-trigger case

If none of the assessed facts have materially changed, Step 08 does not itself require a new assessment.

An organization may still choose to reassess on its own schedule.

## Source and responsibility boundary

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Operator:** identifies and supplies factual changes to the organization-specific system configuration  
**AI:** may assist with updating the specification and rerunning the supplied assessment rules

AI Foundations defines the reassessment triggers and assessment structure. The operator remains responsible for identifying whether the deployed system or organizational conditions have materially changed.