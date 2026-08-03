﷽
بسم الله الرحمن الرحيم

# Mirleen Coordination Architecture and Orchestrator Direction v0.1

**Status:** FOUNDER-ACCEPTED ARCHITECTURAL DIRECTION  
**Authority:** Founder / Intent Owner — Saleem-ASMR  
**Scope:** Architectural direction only; no runtime implementation or Phase 3 authorization.  
**Authoritative Drive record:** `1jVdh56Is790cv1FKFOpcM7BEb9pWDe3wvu7jhw3wtUM`

## 1. Purpose

This document preserves the accepted architectural direction for the post-Phase-2.5 evolution of Mirleen. It records how Mirleen is intended to coordinate agents, evidence, verification, workflow, providers, and Founder decision gates without conflating architecture with implementation.

## 2. Architectural direction

Mirleen shall evolve toward a provider-neutral institutional coordination architecture composed of:

- Mirleen Orchestrator
- Inter-Agent Bus
- Verification Engine
- Agent Identity and Workspace Registry
- Workflow Engine
- Provider Adapters

These components are architecturally related but remain separately governable. Acceptance of this direction does not mean that any runtime, protocol, adapter, scheduler, transport, persistence layer, or autonomous authority has been implemented or authorized.

## 3. Mirleen Orchestrator

The Mirleen Orchestrator is the coordination component responsible for directing the institutional workflow. It is not a Worker and is not itself an authority source.

Its intended responsibilities are:

- receive a Founder-authorized objective;
- load START and RESUME context;
- identify the current SAVE, source registry, active repositories, workspaces, and constraints;
- decompose approved work into bounded tasks;
- submit tasks and context through the Inter-Agent Bus;
- track assignments, acknowledgements, outputs, corrections, and verification state;
- route outputs to the Verification Engine;
- request Founder decisions at material authority gates;
- preserve provenance, exact revisions, and institutional history;
- coordinate closure and creation of a new SAVE when authorized.

The Orchestrator must not:

- invent institutional authority;
- ratify ADRs, standards, or policies;
- approve its own output;
- merge code without explicit authorization;
- bypass independent verification;
- silently modify task scope;
- conceal evidence, uncertainty, conflicts, or failures.

## 4. Inter-Agent Bus

The Inter-Agent Bus is the provider-neutral communication, distribution, collection, and artifact-exchange fabric between the Founder, Orchestrator, Workers, Reviewers, Architects, Verifiers, external tools, and Mirleen-native agents.

Its intended responsibilities include:

- task and message envelopes;
- source manifests and immutable revision references;
- distribution of approved inputs to one or more agents;
- transfer of artifacts, reports, claims, evidence, findings, and correction requests;
- acknowledgements and delivery state;
- retries, failure handling, and dead-letter handling;
- correlation of requests, responses, tasks, and verification runs;
- lineage, provenance, and audit references;
- provider-independent identity and role references;
- aggregation of distributed results;
- routing to reconciliation and independent verification;
- reducing or eliminating Founder copy-and-paste.

Communication through the Bus does not itself grant authority, certification, acceptance, adoption, merge eligibility, or permission to act outside an assigned scope.

## 5. Verification Engine

The Verification Engine is the governed system for preparing, executing, recording, and closing independent verification processes.

Its intended responsibilities include:

- START and CLOSE gates;
- verification requests and scopes;
- exact source and revision pinning;
- evidence intake and classification;
- claim-to-source locators;
- findings, severities, conflicts, and blockers;
- protected-scope checks;
- reproducible command and test evidence;
- verdict vocabulary and eligibility rules;
- correction and re-verification cycles;
- independent Final Verifier separation;
- audit, recovery, and historical evidence preservation.

The Verification Engine may determine technical or evidentiary eligibility within its authorized scope, but it must not grant Founder adoption, ratification, merge authority, or autonomous institutional authority.

## 6. Agent Identity and Workspace Registry

The registry shall provide provider-neutral references for:

- stable agent identity;
- role and role history;
- provider and provider-instance mapping;
- workspace or session continuity;
- certification and qualification status;
- assignment history;
- lifecycle state;
- verifier independence;
- suspension, remediation, replacement, and succession;
- non-reuse of retired identities.

Workspace or conversation names are operational identifiers and must remain separate from identity proof and authority grants.

## 7. Workflow Engine

The Workflow Engine shall model the governed lifecycle of institutional and coding work:

```text
START → RESUME → PLAN → ASSIGN → EXECUTE → COLLECT → RECONCILE
→ VERIFY → CORRECT → REVERIFY → FOUNDER GATE
→ MERGE OR ADOPT → SAVE → CLOSE
```

The exact state model, transition rules, cancellation, retries, leasing, concurrency, and recovery semantics remain future contract work.

## 8. Provider Adapters

Provider Adapters may connect Mirleen to:

- OpenAI ChatGPT;
- OpenAI Codex;
- Anthropic Claude;
- Google Gemini;
- GitHub;
- Google Drive;
- future providers;
- Mirleen-native agents.

Adapters must remain subordinate to Mirleen contracts, authority rules, evidence requirements, and audit boundaries. No provider-specific capability may redefine the institutional model.

## 9. Direction of control

```text
Founder / Intent Owner
        ↓
Mirleen Orchestrator
        ↓
Inter-Agent Bus
        ↓
Workers / Reviewers / Architects / Coordinators
        ↓
Artifact and Evidence Collection
        ↓
Reconciliation
        ↓
Verification Engine and Independent Final Verifier
        ↓
Founder Decision Gate
        ↓
Authorized Merge / Adoption / SAVE / CLOSE
```

## 10. Relationship to mirleen-server

`mirleen-com/mirleen-server` is the planned governed application and execution boundary for this future architecture. It may eventually host or compose the Orchestrator, Bus, Verification Engine, registries, workflow components, audit composition, and provider adapters.

This direction does not authorize runtime implementation. Implementation requires separately approved contracts, plans, verification, recovery points, and Founder decisions.

## 11. Recommended planning gate

Recommended planning label:

**Phase 2.75 — Verification and Agent Coordination Foundation**

This label remains a planning recommendation unless separately adopted. Suggested order:

1. Verification Engine boundaries and contracts.
2. Agent Identity and Workspace Registry boundaries.
3. Inter-Agent Bus boundaries and contracts.
4. Orchestrator responsibilities and ports.
5. Workflow Engine state and transition contracts.
6. Provider Adapter boundaries.
7. Independent architectural and authority review.
8. Founder disposition.
9. Contract-only implementation after authorization.

## 12. Current status

- Architectural direction: **ACCEPTED**
- Mirleen Orchestrator: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Inter-Agent Bus: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Verification Engine: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Agent Identity and Workspace Registry: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Workflow Engine: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Provider Adapters: **ARCHITECTURALLY ACCEPTED / NOT IMPLEMENTED**
- Phase 3: **NOT AUTHORIZED**

الحمد لله رب العالمين
