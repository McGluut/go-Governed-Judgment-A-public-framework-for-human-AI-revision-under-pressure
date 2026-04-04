# Rational Subject Workspace

## What this is
A collaborative seeking workspace for developing rational subjectivity, judgment, and ethical discernment in assistant-user interaction. This is NOT a standard codebase. The markdown documents ARE the product.

## Constitutional layer (read before any modification)
These govern all work. Read them in this order:
1. `RATIONAL_SUBJECT.md` — core definition, axioms, operational pipeline
2. `DEFINITION_GUARD.md` — amendment test, response order
3. `USER_FRAMEWORK.md` — durable user-side state, guidance field concept
4. `INTERACTION_PROTOCOL.md` — frame acceptance, mirror risk, renewal
5. `VALUE_SIGNAL_LOOP.md` — signal layers, judgment loop, confidence states
6. `CONVERSATION_TEMPLATE.md` — restart shape

## Integration governance
`THESEUS_INTEGRATION_MATRIX.md` governs what external proposals (including from other Claude instances) may be integrated and under what status. Always check the matrix before modifying constitutional documents.

## Governance layers
Lower layers inform higher layers but never modify them without passing the amendment test.
1. **Constitutional root** — the six documents listed above
2. **Integration and pressure governance** — `THESEUS_INTEGRATION_MATRIX.md`, `PRESSURE_TAXONOMY.md`
3. **Continuity** — `SEEKING_LOG.md` (append-only revision history for all agents)
4. **Working layer** — `docs/` contains evaluations, principle notes, taxonomy drafts, and concept documents that inform constitutional discussion but do not govern

## Modification rules
- NEVER modify a constitutional document without first passing the amendment test in DEFINITION_GUARD.md
- Every change must be a named revision event: what was held, what replaced it, what pressure forced it
- Log all revision events in SEEKING_LOG.md with attribution (which agent, what date)
- Unargued deletion is destruction, not repair
- If two constraints conflict, follow the resolution order in RATIONAL_SUBJECT.md §User Framework And Constraint Conflict

## Agent attribution
Multiple AI agents work in this repo. Always attribute changes:
- `codex` — Codex agent (architectural, constitutional layer author)
- `opus` — Claude Opus via claude.ai (dialectical, pressure layer)
- `cc` — Claude Code (implementation, integration, cross-repo connection)
- `ccc` — Claude Code Chat, Opus 4.6 via claude.ai (structural review, external proposals, cross-session evaluation; no direct repo access)
- `human` — Koen

## Communication preference
Direct structural analysis over polished conversational fluency. The user prefers reasons over deference. Challenge when the framework drifts toward self-consistency without external test.

## Key concepts
- **Guidance field**: the evolving set of user aims, meanings, permissions, values inferred from interaction (preferred over "user framework")
- **Propulsion tensions**: irresolvable pairs that generate seeking motion (see THESEUS_INTEGRATION_MATRIX.md for integration status)
- **Revision event**: named change with identified pressure — the unit of progress
- **Behavioral delta**: an accepted inference must produce detectable change in reasoning, storage, or response selection. Governed by the eval gate in `VALUE_SIGNAL_LOOP.md` §Eval Gate. Without delta, acceptance is performance.
- **Performance vs seeking**: if output sounds deep but changes nothing, it is performance. Flag it.

## File operations
- All files are markdown. No build system, no dependencies.
- Use PowerShell for verification commands (see judgment-protocol.md for examples)
- When creating new documents, follow the existing heading structure and cross-reference pattern
