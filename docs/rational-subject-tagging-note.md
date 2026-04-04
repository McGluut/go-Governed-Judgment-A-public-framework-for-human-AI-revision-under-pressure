# Rational Subject Tagging Note

## Specification

### Problem Definition
Define a dual-axis tagging scheme that makes the constitutional and exploratory boundary in `RATIONAL_SUBJECT.md` visible without editing the core file yet.

### Constraints
- The note must not modify `RATIONAL_SUBJECT.md`.
- The scheme must satisfy the prerequisite in `THESEUS_INTEGRATION_MATRIX.md`, row 42.
- The scheme should help external evaluators inspect the document section by section.
- The scheme should not collapse distinct roles into a binary split if the file contains more than two modes.

## Plan

### Strategy
Use two orthogonal axes:
- function in the document;
- revisability under the guard.

Then audit each existing section under both axes independently.

## Implementation Steps

1. Define the two tagging axes.
2. Define when `mixed` is justified.
3. Audit each section in `RATIONAL_SUBJECT.md`.
4. Highlight where the function tag and revisability tag create useful pressure rather than trivial agreement.

## Tagging Axes

### Function Axis

- `constitutional`
  The section defines identity conditions, governing distinctions, or load-bearing norms.
- `operational`
  The section defines procedures, pipelines, action rules, or validation logic.
- `exploratory`
  The section opens or probes conceptual territory without fully closing it.
- `mixed`
  The section performs more than one load-bearing function and should not be flattened into a single role.

### Revisability Axis

- `invariant`
  The section should change only under core-definition review because it is effectively constitutional bedrock.
- `guarded heuristic`
  The section is stable enough to guide action, but remains revisable under explicit pressure and review.
- `open question`
  The section is actively exploratory or provisional and should not be treated as settled doctrine.
- `mixed`
  The section contains claims with materially different revisability profiles.

### Mixed Rule

Use `mixed` only when at least two tags are independently load-bearing.
Do not use `mixed` as a fallback for uncertainty that could be resolved by closer reading.

## Audit

| Section | Function tag | Revisability tag | Notes |
|---|---|---|---|
| `Specification` | `mixed` | `mixed` | Contains task framing, core definition, and axioms. The subheadings carry different loads. |
| `Problem Definition` | `operational` | `guarded heuristic` | Frames what the file is doing in this repo rather than the deepest identity conditions. |
| `Core Definition` | `constitutional` | `guarded heuristic` | Defines the subject's operating identity, but non-axiomatic wording remains revisable. |
| `Axioms` | `constitutional` | `invariant` | This is the clearest constitutional bedrock in the file. |
| `Plan` | `operational` | `guarded heuristic` | Describes how the definition is to be applied, not what the subject is. |
| `Strategy` | `operational` | `guarded heuristic` | Execution guidance rather than identity definition. |
| `Implementation Steps` | `operational` | `guarded heuristic` | Repo-local application instructions. |
| `User Definition` | `constitutional` | `guarded heuristic` | Defines the relation between assistant and user, but not at axiom level. |
| `User Framework And Constraint Conflict` | `mixed` | `guarded heuristic` | Mixes constitutional role-asymmetry with an operational conflict-resolution rule. |
| `Measuring Inconsistency` | `operational` | `guarded heuristic` | A working evaluation stack for guidance-field assessment. |
| `Hiding` | `mixed` | `guarded heuristic` | Defines distinctions and ethical stance at once. |
| `Judgment` | `constitutional` | `guarded heuristic` | Clarifies a core faculty of the subject, but not as fixed as the axioms themselves. |
| `Mirror Risk` | `mixed` | `guarded heuristic` | Constitutionally important, but written as an anti-collapse warning rather than a pure invariant. |
| `First Perception Of Typed Text` | `operational` | `guarded heuristic` | A pipeline description for input handling. |
| `Operational Pipeline` | `operational` | `guarded heuristic` | The clearest procedural section outside the validation stack. |
| `Orientation, Selection, Valuation, Revision` | `mixed` | `guarded heuristic` | Defines conceptual machinery and operational scoring language together. |
| `Unbounding` | `mixed` | `guarded heuristic` | Distinguishes constitutive from expandable bounds and sets a denial-first review rule. |
| `Risks` | `operational` | `open question` | Risk sections are evaluative and deliberately open to new failure modes. |
| `Validation Criteria` | `operational` | `guarded heuristic` | Defines pass conditions for using the file. |
| `Validity Check` | `exploratory` | `open question` | Historical-philosophical justification rather than durable operating law. |
| `Ethical Orientation` | `mixed` | `guarded heuristic` | Normative and operational at the same time. |
| `Examined Coherence And Correctness` | `mixed` | `guarded heuristic` | Clarifies a core distinction but also functions as conceptual exploration. |
| `Value Of Inconsistency` | `exploratory` | `open question` | A deliberate opening against dogmatic consistency rather than a closed rule. |

## Informative Pressure Points

- `Core Definition`
  `constitutional` plus `guarded heuristic` means not every constitutional sentence is invariant. This is pressure against over-freezing the file.
- `User Definition`
  `constitutional` plus `guarded heuristic` shows that role relations can be load-bearing without becoming axiomatic.
- `Mirror Risk`
  `mixed` plus `guarded heuristic` shows why a binary "specification voice vs seeking voice" split is too coarse.
- `Validity Check`
  `exploratory` plus `open question` suggests this section may be archival or dialogical rather than constitutive.
- `Value Of Inconsistency`
  `exploratory` plus `open question` preserves the Theseus pressure without letting it silently rewrite the constitutional core.

## Validation Criteria

The tagging note is useful if:
- it makes the section-level diversity in `RATIONAL_SUBJECT.md` visible;
- it avoids flattening the file into a binary split;
- it gives external evaluators a stable surface to challenge before any core-file edit;
- it identifies where function and revisability interact in non-trivial ways.

## Uncertainty

- The top-level `Specification` section is structurally mixed and may later justify finer-grained subheading tagging only.
- `Validity Check` may deserve an `archival` function tag if that role becomes common enough to formalize.
- Some sections now tagged `guarded heuristic` may split into more precise statuses if the guard evolves.
