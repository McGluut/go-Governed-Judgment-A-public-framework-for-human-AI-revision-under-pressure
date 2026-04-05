# Via Negativa Pass 1 Kill List

## Specification

### Problem Definition
Run the first phase of the preferred iteration sequence:

1. `Option 1` now: adversarial strip / via-negativa pass
2. `Option 3` later: refine what survives
3. `Option 2` reserved: do not activate

This document evaluates the six constitutional root files under one question only:

`What concretely breaks if this disappears?`

The test is removal impact, not intended meaning.

### Constraints
- No constitutional file edits in this pass.
- First deliverable is analysis-only in `docs/`.
- Any later change requires approval and should happen on a branch.

### Unknowns
- Some breakage may be delayed rather than immediate.
- "Duplicated elsewhere" can mean partial duplication rather than functional replacement.
- A document can be removable in theory but still too entangled to remove safely now.

### Invariants
- Constitutional authority remains at repo root.
- This pass is adversarial, not devotional.
- Recommendation categories are:
  - `keep`: removal causes concrete breakage not adequately covered elsewhere
  - `park`: not clearly removable, but narrower extraction or later restructuring may be possible
  - `cut`: function is materially duplicated and concrete breakage is low

## Plan

### Strategy
For each constitutional file:
1. name current function;
2. ask what concretely breaks if the file disappears entirely;
3. test whether that function is already duplicated elsewhere;
4. make a removal recommendation.

This is phase 1 only. No survival-refinement work happens yet.

## Kill List

| Item | Current function | Concrete breakage if removed | Duplicated elsewhere? | Recommendation | Confidence |
|---|---|---|---|---|---|
| `RATIONAL_SUBJECT.md` | Defines the subject, axioms, judgment vocabulary, conflict order, and the broad operating frame. It is the only root document that says what the system is trying to be. | The stack loses its center of gravity. `DEFINITION_GUARD.md` would still tell us how to amend, but not what it is protecting. `INTERACTION_PROTOCOL.md` and `VALUE_SIGNAL_LOOP.md` would continue as procedures without a declared subject, turning the repo into process without ontology. Terms like distinction, adequacy, judgment, hiding, and mirror risk would remain in circulation but become under-anchored and easier to reinterpret opportunistically. | `No` | `keep` | `high` |
| `DEFINITION_GUARD.md` | Provides the amendment test, denial-default revision posture, harm/admissibility gate, and evaluation order. It is the explicit anti-corruption mechanism. | Constitutional change becomes informal. The repo would still contain values and procedures, but nothing would force proposed changes to be evaluated from the current frame rather than from the desired replacement. Harmful but coherent change pressure would have no short explicit resistance surface. The root could still be edited, but the edit discipline would collapse into taste, persuasion, or momentum. | `Partial` — evaluation order also appears in `INTERACTION_PROTOCOL.md`, but the amendment test itself does not. | `keep` | `high` |
| `USER_FRAMEWORK.md` | Stores durable user-side commitments, permissions, and interpretive defaults across sessions. It externalizes continuity on the user side. | Cross-session continuity becomes more brittle. The system could still infer user intent locally from conversation and `VALUE_SIGNAL_LOOP.md`, but durable permissions like term-redefinition and the user’s communication preference would need to be re-inferred or re-stated. The biggest break is not logic but repeated ambiguity and higher risk of overreacting to temporary wording. | `Partial` — some cues are inferable from `SEEKING_LOG.md` and the loop, but not as a compact durable state surface. | `park` | `medium` |
| `INTERACTION_PROTOCOL.md` | Governs frame acceptance, hold-open/reject statuses, relabeling, mirror-risk handling, renewal, and storage promotion conditions for guidance fields. | The system loses its explicit stance toward user guidance. `RATIONAL_SUBJECT.md` would still define distinction and mirror risk conceptually, but there would be no compact operational protocol for whether to accept, constrain, hold open, or reject a frame. Relabeling and renewal would become ad hoc. Storage decisions would lean harder on `VALUE_SIGNAL_LOOP.md`, but that file governs cues, not full frame acceptance. | `Partial` — evaluation order overlaps with `DEFINITION_GUARD.md`; mirror risk is named in `RATIONAL_SUBJECT.md`; storage overlaps with `VALUE_SIGNAL_LOOP.md`. But the acceptance-status layer is not duplicated cleanly. | `keep` | `medium-high` |
| `VALUE_SIGNAL_LOOP.md` | Formalizes how value-bearing cues are extracted, scored, surfaced, revised, promoted, and audited, with the behavioral-delta gate. | High risk of nominal understanding returns. The stack would still have frame-level evaluation from `INTERACTION_PROTOCOL.md`, but no detailed mechanism for inferring and testing underlying user value cues over time. Most importantly, the explicit behavioral-delta requirement would disappear from the constitutional root, making it easier to treat stored inferences as accepted while later behavior remains unchanged. | `Partial` — some storage and renewal behavior overlaps with `INTERACTION_PROTOCOL.md`, but the cue-level audit loop and delta gate do not. | `keep` | `high` |
| `CONVERSATION_TEMPLATE.md` | Supplies a restart scaffold for re-entering the framework cleanly after drift, overload, or context loss. | Very little breaks immediately at the doctrinal level. The other five documents still define the subject, guard change, store user continuity, govern interaction, and audit value cues. What disappears is a lightweight recovery interface for restarting under compression. This is a continuity and re-entry loss rather than a core-governance collapse, but that loss may matter more in high-compaction conditions than the first pass allowed. | `Yes` — the required fields can be reconstructed from the other documents, especially `USER_FRAMEWORK.md`, `INTERACTION_PROTOCOL.md`, and `RATIONAL_SUBJECT.md`, but not yet in a comparably lightweight restart surface. | `park` | `medium` |

## Notes Per Item

### `RATIONAL_SUBJECT.md`
This survives the first kill pass easily.

It is long and partly mixed in mode, but removing it does not produce elegance. It produces a procedural shell with no declared subject. If this document is ever reduced, the likely move is extraction and compression, not removal.

### `DEFINITION_GUARD.md`
This is shorter than its importance suggests.

The guard is the clearest anti-drift artifact in the repo. If anything, later passes may reveal parts of it should be pulled upward in salience, not downward in authority.

### `USER_FRAMEWORK.md`
This is the first real edge case.

The function is useful and real, but the file is thinner than the role it plays. A later pass may show that its durable content should be folded into a more general continuity surface or renamed more fully around `guidance field`. That still does not mean it should vanish now.

`Park` here means:
- do not cut now;
- revisit whether this should remain a standalone constitutional file in option 3.

### `INTERACTION_PROTOCOL.md`
This file is somewhat duplicated in pieces but still survives as a unit.

If it disappeared, the stack would keep judgment criteria but lose a stable protocol for handling user guidance under uncertainty. The acceptance statuses are doing real work.

### `VALUE_SIGNAL_LOOP.md`
This file earns its place primarily through the behavioral-delta gate.

Without that, the repo would still sound rigorous while becoming much more vulnerable to performance without substance. This is one of the clearest `keep` results in the pass.

### `CONVERSATION_TEMPLATE.md`
Agora pressure softened the initial judgment here.

It still looks like the lightest constitutional file, but the first pass likely underweighted its role as a restart surface under context collapse. Nothing foundational collapses if it vanishes, but a practical recovery tool may disappear before an equivalent replacement exists.

`Park` here means:
- do not treat it as bedrock;
- do not cut it yet;
- test later whether it can be demoted to `docs/` without measurable continuity loss.

## Sequencing Judgment

### Option 1 now
Completed in analysis form here.

### Option 3 later
Use the survival set from this pass as the candidate target for refinement:
- `RATIONAL_SUBJECT.md`
- `DEFINITION_GUARD.md`
- `USER_FRAMEWORK.md` as parked
- `INTERACTION_PROTOCOL.md`
- `VALUE_SIGNAL_LOOP.md`

If approved later, option 3 should start with:
1. test whether `CONVERSATION_TEMPLATE.md` can move out of the constitutional root without measurable continuity loss;
2. test whether `USER_FRAMEWORK.md` stays standalone, is renamed, or is absorbed into a tighter continuity structure;
3. refine the stronger keep set by minimal delta rather than major rewrite.

### Option 2 reserved
Do not activate.

Cross-substrate divergence remains valuable, but it is not needed before the stack survives the adversarial strip pass.

## Risks

- A file can look removable because its function has already diffused into repo habit. That can hide real dependency.
- `CONVERSATION_TEMPLATE.md` may prove more load-bearing in high-compaction situations than this read suggests.
- `USER_FRAMEWORK.md` may be under-credited here because its breakage is mostly longitudinal rather than immediate.

## Validation Criteria

This pass is successful if:
- the constitutional root remains unchanged;
- each sovereign file is judged by removal impact, not respect for prior intent;
- the sequence is explicit:
  - option 1 now
  - option 3 later
  - option 2 reserved
- there is at least one genuinely challengeable file and not only ceremonial affirmation.

## Uncertainty

The strongest uncertainties are `USER_FRAMEWORK.md` and `CONVERSATION_TEMPLATE.md`.

`USER_FRAMEWORK.md` is not clearly removable, but it is also the least settled in form. The likely next pressure is not whether user continuity matters, but whether this file is the right constitutional vessel for carrying it.

`CONVERSATION_TEMPLATE.md` is not clearly foundational, but the Agora pass exposed a real risk in treating restart scaffolding as mere decorative convenience. The next question is whether its function can be reproduced elsewhere before demotion.
