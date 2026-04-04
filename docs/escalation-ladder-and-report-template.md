# Escalation Ladder And Report Template

## Specification

### Problem Definition
As versions of the `go` repo and application repos begin operating in the world, define:
- an escalation ladder that protects the constitutional core;
- a reusable scaffold for reporting pressure back to the main repo;
- a stable middle layer that can receive, normalize, and triage reports before they reach the core constitutional thread.

### Constraints
- The core constitutional thread must remain protected from raw implementation churn and field noise.
- Child repos and application threads must still be able to return genuine constitutional pressure.
- The scaffold must work for non-technical users and technically stronger agent threads alike.
- The scaffold must stay open to revision and not pretend to final completeness.

### Unknowns
- How many active child repos or field agents will actually emerge.
- Whether one bridge thread is enough or later needs branching by domain.
- Which term will prove most stable for the middle layer.

### Invariants
- Repo-root constitutional documents remain sovereign.
- Upward movement carries pressure, not authority.
- Downward movement carries governance, not mere preference.
- Not every field report deserves constitutional attention.

## Plan

### Strategy
Upgrade the earlier two-thread model into a four-level ladder:
- constitutional core;
- integration bridge;
- applications and field repos;
- local execution runs.

Then define a report template that can move information upward without flooding the core.

## Implementation Steps

1. Define the ladder.
2. Define the authority and pressure flow.
3. Define when escalation is justified.
4. Provide a reusable return-report template.
5. Define what kinds of model updates should be named in the report.

## Escalation Ladder

### Layer 0: Constitutional Core

This is the `holy of holies`.

It includes:
- the repo-root constitutional documents;
- the core constitutional thread;
- deep work on ethics, ontology, epistemology, judgment, measure, and revisability.

Its function:
- define what governs;
- absorb only pressure that may justify constitutional reconsideration;
- remain protected from raw noise.

### Layer 1: Integration Bridge

This is the `bridge thread` or `pressure intake layer`.

Its function:
- receive reports from application threads, child repos, and field runs;
- normalize them into a common shape;
- classify pressure using the repo's taxonomy;
- decide whether the issue is:
  - local only,
  - bridge-level only,
  - or genuinely constitutional.

This layer is allowed to push upward to the core thread.
Child repos should usually push here first, not directly to the core.

### Layer 2: Applications And Field Repos

This layer contains:
- application threads;
- expedition threads;
- child repos with or without Agora;
- real-world embodiment work.

Its function:
- put the constitution into contact with reality;
- produce artifacts, tests, and failures;
- return compressed pressure upward when needed.

It does not casually revise the constitution.

### Layer 3: Local Execution Runs

This layer contains:
- narrow implementation threads;
- agent runs;
- experiments;
- data collection tasks;
- single expeditions or evaluation passes.

Its function:
- execute;
- observe;
- produce local traces.

It should never push directly to the core thread unless explicitly instructed.

## Flow Rule

Use this rule:

`governance flows downward`
`pressure flows upward`

More explicitly:
- Layer 0 governs Layers 1-3
- Layer 1 governs intake and escalation discipline for Layers 2-3
- Layer 2 governs the practical orchestration of Layer 3
- Layer 3 returns artifacts and traces upward

## When Escalation Is Justified

### Stay Local

Keep the issue in Layer 3 or 2 when:
- it is purely implementation-specific;
- it does not pressure a repo principle;
- it can be handled by local debugging, better prompts, or better execution.

### Escalate To The Bridge

Escalate to Layer 1 when:
- the issue recurs across runs;
- the issue affects more than one application or child repo;
- there is uncertainty about whether the pressure is constitutional or merely local;
- the issue requires comparison across artifacts or repos.

### Escalate To The Core

Escalate from Layer 1 to Layer 0 when:
- the pressure exposes a contradiction in the constitutional layer;
- a root principle appears too vague, too rigid, or misaligned in practice;
- repeated reality contact shows a stable failure the current framework cannot classify;
- a candidate constitutional revision is now justified.

## Why The Bridge Layer Is Needed

The earlier two-thread model assumed one main applications stream.
That was good enough while the system was mostly internal.

Now that multiple repo variants and applications are making contact with the fuzzy world, the core thread needs:
- protection from noise;
- comparability across reports;
- an intake form that does not depend on memory of the whole conversation.

So the new structure should be:

- `Layer 0`: core constitutional thread
- `Layer 1`: integration bridge thread
- `Layer 2`: applications and field repos
- `Layer 3`: local execution runs

## Model-Delta Scaffold

Every serious return report should name not only what happened, but what changed in the local model.

Use these fields:

- `world-model delta`
  What changed about the system's understanding of the external domain or situation.
- `self-model delta`
  What changed about the agent's understanding of its own capabilities, limits, or failure modes.
- `user-model delta`
  What changed about the understanding of stakeholders, operators, or requesters.
- `agent-model delta`
  What changed about the understanding of other agents, tools, or collaborating systems.
- `governance delta`
  What changed about the understanding of how current rules help, fail, or distort.

Not every report needs all five, but the scaffold should make them visible.

## Return Report Template

Use this in child repos, application threads, or bridge intake.

```md
# Return Pressure Report

## Source
- Layer:
- Repo or thread:
- Run, artifact, or commit:
- Date:

## Local Objective
- What this repo/thread/run was trying to do.

## Held
- What was assumed locally before contact with reality.

## What Happened
- What actually occurred.

## Pressure Classification
- Primary:
- Secondary:
- Threshold note:

## Model Deltas
- World-model delta:
- Self-model delta:
- User-model delta:
- Agent-model delta:
- Governance delta:

## Revised To
- What local understanding changed.

## Why Local Handling Is Insufficient
- Why this cannot remain only a local matter.

## Proposed Escalation Target
- Stay local
- Bridge thread
- Core constitutional thread

## Constitutional Question
- If escalated upward, what exact question should the higher layer answer?

## Artifacts
- Paths, links, logs, or outputs.

## Uncertainty
- What remains unknown.
```

## Compression Rule

When sending from Layer 2 or 3 upward:
- do not send raw transcripts by default;
- send the compressed report first;
- attach artifacts only when needed for review.

This keeps the bridge and core from drowning in contact noise.

## Ready-To-Use Starter For The Bridge Thread

```text
This thread is the integration bridge for the go ecosystem.

Authority:
- repo-root constitutional documents remain sovereign
- this thread triages pressure from child repos, application threads, and field runs
- this thread may escalate to the core constitutional thread only when pressure is genuinely constitutional

Purpose:
- normalize reports
- classify pressure
- compare reports across repos and runs
- decide what stays local and what must rise upward

Working rule:
- require the return-pressure template
- compress before escalating
- do not flood the core thread with raw implementation detail

Escalate upward only when:
- a root principle is pressured
- repeated failures cross repo boundaries
- a candidate constitutional revision is justified
```

## Naming

Best current names:
- `core constitutional thread`
- `integration bridge thread`
- `applications and field repos`
- `local execution runs`

These names are plain enough to work and precise enough to differentiate authority and pressure flow.

## Validation Criteria

This ladder is good if:
- the constitutional core stays protected;
- child repos can still return important pressure;
- the bridge can compare reports instead of relaying noise;
- the user does not have to manually sort every signal by hand.

## Uncertainty

- The exact term for Layer 1 may still change. `integration bridge` is the current best candidate.
- Some domains may later need domain-specific bridge threads, but one bridge is enough at the current scale.
