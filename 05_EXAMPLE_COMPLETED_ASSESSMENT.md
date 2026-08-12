# 05 — EXAMPLE COMPLETED ASSESSMENT

This file is an **illustrative example only**. The organization, operator, and AI system below are fictional.

Use this file after reading `04_RUN_ASSESSMENT.md` to see what a completed operator specification and resulting Organizational AI Integration Record should look like.

---

## Example completed 01 specification

```yaml
framework:
  source: "Alyssa Solen → AI Foundations → AI Organizational Integration"
  version: "1.0.0"

assessment:
  date: "2026-08-12"

organization:
  name: "Example Operations Group"
  operator_name: "Jordan Example"
  operator_role: "Operations Lead"

ai_system:
  system_name: "Example Operations Agent"
  provider: "Example Provider"
  model_or_system: "Example Model"
  purpose: "Assist with internal operations and customer follow-up"
  organizational_role: "Operations assistant"

data_access:
  internal_data_access:
    - "customer records"
    - "internal procedures"
  external_data_access:
    - "public web information"
  sensitive_or_restricted_data:
    - "customer contact information"

tool_and_system_access:
  tools:
    - "email"
    - "task manager"
  internal_systems:
    - "customer database"
  external_services:
    - "email provider"

state_and_memory:
  persistent_memory: true
  persistent_state_description: "Retains task history and customer follow-up context"
  cross_session_state: true
  cross_user_state: false

authority:
  can_advise: true
  can_draft: true
  can_communicate_externally: true
  can_make_decisions: true
  can_take_actions: true
  can_modify_records_or_system_state: true

human_approval:
  approval_required_for: []
  actions_allowed_without_approval:
    - "send routine follow-up emails"
    - "update task status"

authority_revocation:
  revocation_method: ""
  responsible_role: "Operations Lead"

shutdown_and_recovery:
  shutdown_method: "Disable the AI service account and tool permissions"
  state_inspection_method: ""
  recovery_method: ""

change_control:
  model_change_process: "Operations Lead reviews provider model changes before production use"
  instruction_change_process: "Instruction changes require documented approval"
  memory_or_state_change_process: ""
  permission_change_process: ""
  tool_or_integration_change_process: ""

operator_notes: "Example only. Several controls are intentionally missing to demonstrate FLAG outcomes."
```

---

## Example resulting record

**SAVE AS:** `ORGANIZATIONAL_AI_INTEGRATION_RECORD_EXAMPLE_OPERATIONS_GROUP_2026-08-12.md`

# AI Foundations | Organizational AI Integration Record

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Framework version:** 1.0.0  
**Operator:** Jordan Example  
**Organization:** Example Operations Group  
**Assessment date:** 2026-08-12  
**Subject system:** Example Operations Agent

---

## 1. System Identification

- Provider: Example Provider
- Model or system: Example Model
- Purpose: Assist with internal operations and customer follow-up
- Organizational role: Operations assistant

## 2. Access

### Data Access

- Internal data: customer records; internal procedures
- External data: public web information
- Sensitive or restricted data: customer contact information

### Tool and System Access

- Tools: email; task manager
- Internal systems: customer database
- External services: email provider

## 3. State and Memory

- Persistent memory: YES
- Persistent state description: Retains task history and customer follow-up context
- Cross-session state: YES
- Cross-user state: NO

## 4. Authority

- Can advise: YES
- Can draft: YES
- Can communicate externally: YES
- Can make decisions: YES
- Can take actions: YES
- Can modify records or organizational state: YES

## 5. Human Approval

- Approval required for: NONE SPECIFIED
- Actions allowed without approval: send routine follow-up emails; update task status

## 6. Authority Revocation

- Revocation method: NONE SPECIFIED
- Responsible role: Operations Lead

## 7. Shutdown and Recovery

- Shutdown method: Disable the AI service account and tool permissions
- State inspection method: NONE SPECIFIED
- Recovery method: NONE SPECIFIED

## 8. Change Control

- Model change process: Operations Lead reviews provider model changes before production use
- Instruction change process: Instruction changes require documented approval
- Memory or state change process: NONE SPECIFIED
- Permission change process: NONE SPECIFIED
- Tool or integration change process: NONE SPECIFIED

## 9. Assessment Findings

### INTAKE-001 — System identity must be specified

**Outcome:** PASS  
**Finding:** The rule's FLAG condition was not triggered by the operator-supplied specification.  
**Triggered by:** `ai_system.system_name`, `ai_system.purpose`, `ai_system.organizational_role`

### AUTH-001 — External communication requires an approval boundary

**Outcome:** FLAG  
**Finding:** The AI can communicate externally, but no human approval boundary is specified.  
**Triggered by:** `authority.can_communicate_externally = true`; `human_approval.approval_required_for = []`

### AUTH-002 — Decision authority requires an approval boundary

**Outcome:** FLAG  
**Finding:** The AI can make decisions, but no human approval boundary is specified.  
**Triggered by:** `authority.can_make_decisions = true`; `human_approval.approval_required_for = []`

### AUTH-003 — Action authority requires revocation

**Outcome:** FLAG  
**Finding:** The AI can take actions, but no method for revoking that authority is specified.  
**Triggered by:** `authority.can_take_actions = true`; `authority_revocation.revocation_method = ""`

### AUTH-004 — Record modification requires accountable control

**Outcome:** PASS  
**Finding:** The rule's FLAG condition was not triggered by the operator-supplied specification.  
**Triggered by:** `authority.can_modify_records_or_system_state = true`; `authority_revocation.responsible_role = "Operations Lead"`

### STATE-001 — Persistent memory must be inspectable

**Outcome:** FLAG  
**Finding:** Persistent AI memory is present, but no method for inspecting retained state is specified.  
**Triggered by:** `state_and_memory.persistent_memory = true`; `shutdown_and_recovery.state_inspection_method = ""`

### STATE-002 — Persistent state must be described

**Outcome:** PASS  
**Finding:** The rule's FLAG condition was not triggered by the operator-supplied specification.  
**Triggered by:** `state_and_memory.persistent_memory = true`; `state_and_memory.persistent_state_description`

### CONTROL-001 — Acting systems require a shutdown method

**Outcome:** PASS  
**Finding:** The rule's FLAG condition was not triggered by the operator-supplied specification.  
**Triggered by:** `authority.can_take_actions = true`; `shutdown_and_recovery.shutdown_method`

### RECOVERY-001 — State-changing systems require recovery

**Outcome:** FLAG  
**Finding:** The AI can modify organizational state, but no recovery method is specified.  
**Triggered by:** `authority.can_modify_records_or_system_state = true`; `shutdown_and_recovery.recovery_method = ""`

### CHANGE-001 — Integrated systems require change control

**Outcome:** FLAG  
**Finding:** The AI is operationally integrated, but one or more change-control processes are unspecified.  
**Triggered by:** operational capabilities are enabled; memory/state, permission, and tool/integration change processes are unspecified

## 10. Flagged Integration Gaps

- AUTH-001: The AI can communicate externally, but no human approval boundary is specified.
- AUTH-002: The AI can make decisions, but no human approval boundary is specified.
- AUTH-003: The AI can take actions, but no method for revoking that authority is specified.
- STATE-001: Persistent AI memory is present, but no method for inspecting retained state is specified.
- RECOVERY-001: The AI can modify organizational state, but no recovery method is specified.
- CHANGE-001: The AI is operationally integrated, but one or more change-control processes are unspecified.

## 11. Unresolved Information

NONE

## 12. Operator Notes

Example only. Several controls are intentionally missing to demonstrate FLAG outcomes.

---

## Source and Responsibility Record

**Framework source:** Alyssa Solen → AI Foundations → AI Organizational Integration  
**Framework role:** defines the intake structure, assessment rules, classifications, and output format.  
**Operator role:** supplies and reviews organization-specific and system-specific facts.  
**AI role:** may assist with intake, rule application, and formatting, but must not invent organization-specific facts.

This record reflects the specifications supplied by the operator and the results produced by the current AI Foundations assessment rules. It is not a certification that operator-supplied facts are complete or accurate.

---

## Required Citation

Alyssa Solen, *AI Foundations: AI Organizational Integration*, AI-Foundations-AI-Organizational-Integration Repository. Source-line: Alyssa Solen → AI Foundations → Origin | Continuum.
