﷽
بسم الله الرحمن الرحيم

# Mirleen Agent Workspace Naming Convention v0.1

- **Status:** ACCEPTED OPERATIONAL CONVENTION
- **Classification:** Provider-neutral workspace convention
- **Founder / Intent Owner:** Saleem-ASMR
- **Acceptance date:** 2026-08-03
- **Authoritative Drive convention:** `1182ShL6LdBJ5WgOJcFwy_vDCpHApn7_UuGcrbnTzdrM`
- **Founder acceptance decision:** `16BBBYTBwdm-8OrRE60m_MrmongHeJP-36bi1BKUFUjw`

## 1. Purpose

This convention establishes a stable, provider-neutral naming system for engineering conversations, agent sessions, reviews, verification threads, planning sessions, and operational workspaces used by Mirleen.

It reduces ambiguity as the number of workers, reviewers, verifiers, and supporting agents grows across multiple AI providers and future Mirleen-native agents.

## 2. Provider independence

The convention is not tied to ChatGPT, Codex, Claude, Gemini, or any other provider. These systems are execution providers only. Mirleen role identifiers remain stable when the underlying provider changes.

Provider names may be recorded as metadata when relevant, but they do not replace the institutional role identifier.

## 3. Canonical identifier format

`<PREFIX>-<SEQUENCE> — <DESCRIPTIVE TITLE>`

Examples:

- `WK-004 — Map Worker State`
- `FV-003 — Phase 2.5 Institutional Compliance`
- `RV-001 — Phase 2 Architecture Review`

The sequence uses at least three digits and is unique within its prefix category.

## 4. Canonical prefixes

- `WK` — Worker: implementation, bounded execution, transformation, or assigned production work.
- `FV` — Final Verifier: independent final verification with no implementation or adoption authority.
- `RV` — Reviewer: architecture, code, document, governance, or bounded review activity.
- `AR` — Architect: architecture exploration, boundary definition, and architectural proposals.
- `CR` — Coordinator: coordination, routing, dependency tracking, and work sequencing.
- `PLN` — Planning: planning, decomposition, roadmaps, and execution sequencing.
- `DOC` — Documentation: drafting, editing, structuring, or maintaining project documentation.
- `SEC` — Security: security analysis, threat review, security verification, or security planning.
- `OPS` — Operations: operational workflows, deployments, maintenance, incident handling, or environment administration.
- `RES` — Research: research, comparison, investigation, evidence collection, or exploratory analysis.

Additional prefixes require a documented convention revision. A new prefix must not silently redefine an existing role.

## 5. Numbering rules

1. Numbers are assigned sequentially within each prefix category.
2. An assigned identifier is never reused for a different conversation or agent identity.
3. Renaming a conversation does not change its institutional identifier.
4. Archived or retired sessions retain their original identifier.
5. Provider migration retains the identifier when institutional role and continuity remain the same.
6. A replacement or successor receives a new identifier unless continuity is explicitly preserved by an authorized decision.

## 6. Naming rules

1. The descriptive title states the bounded mission or subject.
2. Generic names such as `Worker`, `Verifier`, `New Chat`, or `Review` without a subject should be avoided.
3. Phase or milestone identifiers should be included when they materially distinguish the task.
4. Provider names appear only when the provider itself is relevant to the mission.
5. The identifier appears at the beginning of the name so it remains visible in narrow sidebars and lists.

## 7. Role and authority boundaries

A workspace name records role and identity; it does not grant authority.

- A `WK` identifier does not authorize unrestricted implementation.
- An `FV` identifier does not grant Founder adoption or merge authority.
- An `RV` identifier does not make findings authoritative without the applicable decision process.
- An `AR` identifier does not ratify an architectural proposal.
- A prefix never overrides the Constitution, Founder decisions, task envelopes, source manifests, repository protections, or verification gates.

## 8. Scope

This convention applies to:

- AI-agent conversations and threads;
- human-agent collaborative workspaces;
- temporary and persistent engineering sessions;
- external-provider agents;
- future Mirleen-native agents;
- session references used in reports, evidence records, handoffs, and recovery documents.

It does not define identifiers for repositories, packages, files, ADRs, policies, contracts, artifacts, tasks, commits, branches, pull requests, workflow runs, or institutional objects governed by another specification.

## 9. Initial operational registry

- `WK-000 — Bootstrap Mirleen Server`
- `WK-001 — Define Decomposition`
- `WK-002 — Define Output Evidence`
- `WK-003 — Implement Records`
- `WK-004 — Map Worker State`
- `WK-005 — Define Canonical …`
- `WK-006 — Define Canonical …`
- `WK-007 — Authority Matrix`
- `WK-008 — Integrate Mirleen`
- `FV-001 — Mirleen Platform Final Verifier`
- `FV-002 — Independent Final Reconciliation`
- `FV-003 — Phase 2.5 Institutional Compliance`

Ellipses indicate titles that remain unresolved and must not be guessed.

## 10. Lifecycle and archival

A conversation or workspace may be active, paused, completed, superseded, retired, or archived. Lifecycle state is recorded separately from its stable identifier.

Deletion, archival, or provider migration must not erase evidence, decisions, or provenance required by Mirleen governance.

## 11. Future platform services

This convention may later inform a Mirleen Workspace Registry or Agent Registry. It does not define runtime registry behavior, identity proof, authentication, provider adapters, storage, synchronization, or automated naming enforcement.

Any executable implementation requires separate approved architecture and contracts.

## 12. Change control

This document is an operational convention, not a constitutional standard and not a runtime protocol.

Material changes to prefixes, identifier semantics, reuse rules, or authority boundaries require Founder review and a recorded revision. Routine title clarification that preserves the identifier and role may be performed without changing the convention itself.

الحمد لله رب العالمين
