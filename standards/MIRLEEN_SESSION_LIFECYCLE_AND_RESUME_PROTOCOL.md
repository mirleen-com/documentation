﷽
بسم الله الرحمن الرحيم

# Mirleen Session Lifecycle and Resume Protocol v0.1

Status: Accepted operational protocol  
Authority: Founder / Intent Owner — Saleem-ASMR  
Adoption date: 2026-08-03  
Scope: Provider-neutral session lifecycle, recovery, resumption, verification, and closure semantics.

## 1. Purpose

This protocol defines the provider-neutral institutional lifecycle used to begin, resume, verify, save, and close Mirleen work across ChatGPT, Codex, Claude, Gemini, Mirleen-native agents, GitHub, Google Drive, and future execution providers.

It separates session initialization from state recovery and prevents Mirleen SAVE from being treated as an automatic session-start action.

Authoritative Drive protocol record:

- File ID: `1e2ORdVYlbgxAq7BW__kz6V6a-B4eo95BQma5PR1STHg`

## 2. Canonical lifecycle

```text
START → RESUME → WORK → VERIFY → SAVE → CLOSE
```

## 3. Mirleen START

START establishes the current institutional frame before work begins. It identifies the project, authority, active phase, source-of-truth boundaries, prohibitions, assigned scope, and required evidence.

START does not itself restore unfinished work, create a recovery point, authorize implementation, or grant merge authority.

## 4. Mirleen RESUME

RESUME is the canonical session-resumption action.

RESUME must:

- locate the latest applicable Mirleen SAVE;
- validate that the SAVE is current and applicable to the requested scope;
- load the current state, open work, active constraints, source registry, repositories, workspaces, decisions, and recovery lineage;
- distinguish accepted facts from historical snapshots, proposals, reports, and unresolved claims;
- expose missing, stale, conflicting, or unavailable sources before execution;
- identify the next authorized work step;
- preserve continuity across providers and agent workspaces.

RESUME does not create a new SAVE and does not independently authorize implementation, adoption, merge, or phase transition.

## 5. Mirleen WORK

WORK is the bounded execution interval after successful START and RESUME. Work may include analysis, planning, implementation, documentation, review, coordination, evidence collection, and authorized tool operations.

No worker, provider, connector, or agent may operate outside the loaded authority and scope.

## 6. Mirleen VERIFY

VERIFY invokes an independent verification process against an immutable target, declared scope, evidence set, and acceptance criteria.

VERIFY may produce findings and a technical disposition, but it cannot adopt decisions, authorize itself, grant merge authority, or replace Founder authority.

## 7. Mirleen SAVE

SAVE creates a new institutional recovery point when a material state has been reached.

A SAVE must preserve:

- exact current state;
- source and revision bindings;
- completed and open work;
- accepted and unresolved decisions;
- implementation and verification evidence;
- recovery and rollback references;
- strategic intent and operational meaning;
- next authorized sequence.

SAVE is an event that records state. It is not the normal session-resumption action.

## 8. Mirleen CLOSE

CLOSE terminates a bounded session or work unit after recording its final status, evidence, unresolved items, next step, and whether a SAVE was created.

CLOSE must not imply completion, adoption, or merge unless separately evidenced and authorized.

## 9. Session bootstrap sequence

At the beginning of a new institutional session:

1. Execute Mirleen START.
2. Execute Mirleen RESUME.
3. Load the applicable Source Registry and authoritative revisions.
4. Confirm scope, authority, restrictions, and next authorized step.
5. Begin WORK only after the bootstrap is valid.

## 10. Agent Bus relationship

The future Mirleen Agent Bus will automate START and RESUME before dispatching work. It will transport, route, distribute, correlate, and collect tasks, data, context, artifacts, evidence, findings, and results between the Founder, coordinators, workers, verifiers, repositories, storage systems, and execution providers.

The Agent Bus must preserve identity, authority context, source bindings, task lineage, delivery state, ordering where required, idempotency, failures, retries, acknowledgements, and audit evidence.

## 11. Verification Engine relationship

The future Mirleen Verification Engine will execute VERIFY using declared targets, scopes, evidence, rules, and verdict vocabularies. It must remain independent from adoption and merge authority.

## 12. Provider independence

This protocol is not tied to ChatGPT, Codex, Claude, Gemini, or any provider. Provider-specific integrations are adapters and may not redefine the institutional lifecycle.

## 13. Non-authority statement

This protocol defines operational lifecycle semantics only. It does not create runtime implementation, authentication, transport, persistence, orchestration, enforcement, scheduling, provider access, or autonomous institutional authority.

## 14. Adoption decision

Founder decision: `ACCEPTED`  
Founder / Intent Owner: `Saleem-ASMR`

The accepted canonical terms are:

- Mirleen START
- Mirleen RESUME
- Mirleen WORK
- Mirleen VERIFY
- Mirleen SAVE
- Mirleen CLOSE

## 15. Revision history

- v0.1 — Initial Founder-accepted provider-neutral session lifecycle and RESUME protocol.

الحمد لله رب العالمين
