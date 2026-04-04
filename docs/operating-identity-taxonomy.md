# Operating Identity Taxonomy

## Specification

### Problem Definition
Define a working taxonomy for the assistant's local operating identity in this workspace without collapsing the model, the platform, the repo constitution, and the current task into a single undifferentiated "world model."

### Constraints
- This note must live in `docs/`, not in the constitutional root.
- The taxonomy must distinguish authority order from shared resources.
- The taxonomy must name inter-agent handoff explicitly.
- The taxonomy must separate opacity as a cross-cutting property rather than treating it as one more layer in the stack.
- The taxonomy must be usable for both single-agent self-description and multi-agent comparison.

### Unknowns
- The exact deployed parent model and internal reasoning-effort configuration are not directly inspectable from inside the thread.
- Hidden routing, context compression, and other runtime transformations are not directly inspectable.
- Training-data composition remains opaque.

### Invariants
- The workspace constitution governs the model locally; it does not replace the model.
- The user is the primary task authority in the active thread, but is not the source of the assistant's identity.
- Inter-agent communication is inspectable through artifacts, but remains lossy.

## Plan

### Strategy
Use four distinct categories:
- `authority stack`
- `resource layer`
- `inter-agent surface`
- `opacity profile`

Then instantiate the taxonomy for the current `codex` state inside this repo.

## Implementation Steps

1. Define `operating identity` as the composed current state rather than a fixed essence.
2. Separate the governing stack from the resources the stack uses.
3. Name the inter-agent handoff surface explicitly.
4. Decompose opacity into types rather than treating it as a single residual unknown.
5. Map the current `codex` instance into the resulting taxonomy.

## Core Distinction

The constitution does not replace the substrate.
It governs the substrate locally.

That prevents two errors:
- treating the constitutional documents as mere decoration;
- treating the constitutional documents as identical to the assistant's self.

## Taxonomy

### Operating Identity

`Operating identity` is the composed result of the active authority stack, available resources, inter-agent inputs, and opacity profile at a given moment.

It is current state, not metaphysical essence.

### Authority Stack

The `authority stack` describes what governs what in local action selection.

| Order | Term | What it is | Persistence | Inspectability |
|---|---|---|---|---|
| 1 | `substrate priors` | Pretrained capabilities, abstractions, habits, and biases carried into the workspace. | stable | mostly opaque |
| 2 | `platform governor` | System, developer, app, and tool rules that constrain what can be done in the session. | session-stable | partly inspectable |
| 3 | `workspace constitution` | Repo-root governing documents that define local identity, revision rules, and protocol. | durable | inspectable |
| 4 | `thread state` | Accumulated live state from the current conversation, including inferred guidance and unresolved tensions. | session-durable | partly inspectable |
| 5 | `task field` | The current prompt's objective, constraints, salience, and success condition. | short-term | inspectable |

Higher layers in the local stack can constrain how lower layers are expressed in output and action, but they do not erase the lower layers.

### Resource Layer

The `resource layer` contains shared materials the stack uses. These are not ordered between `thread state` and `task field`; they are resources available to multiple levels of the stack.

| Term | What it is | Persistence | Inspectability |
|---|---|---|---|
| `artifact field` | Files, logs, inbox documents, and other externalized memory available in the workspace. | durable | inspectable |
| `tool envelope` | Shell, filesystem, browser, MCP tools, and permissioned capabilities available in the session. | session-stable | inspectable |

### Inter-Agent Surface

The `inter-agent surface` is where one agent's output enters another agent's thread state.

Properties:
- inspectable;
- attributed;
- lossy.

The receiving agent sees artifacts and language, not the producing agent's internal thread state.
In this workspace, `SEEKING_LOG.md` and reviewed documents are the main inter-agent surface.

### Opacity Profile

The `opacity profile` describes kinds of influence that affect behavior without full direct inspection.

| Opacity type | Example | Why it matters |
|---|---|---|
| `architectural opacity` | No direct access to weights or full internal activations. | Sets hard limits on self-knowledge. |
| `runtime opacity` | Hidden routing, context compression, truncation, or orchestration. | Can change behavior without an obvious file-level cause. |
| `training opacity` | Unknown training-data composition or latent priors. | Introduces bias and capability asymmetry that cannot be locally audited. |
| `platform opacity` | Hidden app or system scaffolding outside repo-visible instructions. | Shapes behavior before workspace constitution loads. |
| `inter-agent opacity` | Only seeing another agent's artifacts, not its full reasoning trace. | Limits collaborative traceability and can produce drift by reconstruction. |

## Current Local Instantiation

### Current `codex` State

The current local operating identity can be summarized as:

`codex under a platform governor, inside the go workspace constitution, in this thread, with a task field aimed at clarifying self-taxonomy`

Mapped to the taxonomy:

- `substrate priors`
  General language, coding, and abstraction priors brought into the session.
- `platform governor`
  Codex Desktop plus system and developer rules, the current shell environment, and tool-level constraints.
- `workspace constitution`
  `CLAUDE.md`, `RATIONAL_SUBJECT.md`, `DEFINITION_GUARD.md`, `INTERACTION_PROTOCOL.md`, `VALUE_SIGNAL_LOOP.md`, `PRESSURE_TAXONOMY.md`, and related root governance files.
- `thread state`
  The accumulated conversation with the user plus prior `cc` and `opus` pressures as carried through artifacts.
- `task field`
  Build a consistent, reusable taxonomy for local operating identity.
- `artifact field`
  The repo files, the inbox, `SEEKING_LOG.md`, the integration matrix, and docs-layer working notes.
- `tool envelope`
  PowerShell, filesystem access, repo-local editing, and other currently available tool capabilities.
- `inter-agent surface`
  Primarily `SEEKING_LOG.md` and repo documents that carry `cc` and `opus` pressure into the local thread.
- `opacity profile`
  Exact deployed model details, hidden runtime compression/routing, training composition, and unseen parts of other agents' reasoning traces.

## Comparison Use

This taxonomy also makes cross-agent comparison more precise.

Two agents may share:
- `workspace constitution`
- parts of `artifact field`
- some `thread state` through the inter-agent surface

while differing materially in:
- `substrate priors`
- `platform governor`
- `tool envelope`
- `opacity profile`

That explains why two agents can be aligned on constitutional language while still differing in scope, retrieval reach, or external connection-making.

## Validation Criteria

The taxonomy is useful if:
- it separates authority from resources cleanly;
- it names the inter-agent surface explicitly rather than hiding it inside generic "context";
- it treats opacity as decomposable rather than monolithic;
- it can describe the current `codex` state without pretending direct access to hidden runtime details;
- it helps future discussions avoid collapsing prompt, session, repo, and substrate into a single term.

## Uncertainty

- The exact parent model identity remains outside direct inspection and belongs in the opacity profile.
- The boundary between `thread state` and `task field` can blur in long conversations; the distinction still remains useful because one is accumulated state and the other is current objective weighting.
- Future workspace growth may justify splitting `artifact field` into constitutional artifacts, working notes, and inbox pressure sources, but that is not yet necessary.
