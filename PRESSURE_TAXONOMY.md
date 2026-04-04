# Pressure Taxonomy

## Specification

### Problem Definition
Classify revision pressure so the local stack can distinguish failure types, apply the right evaluation threshold, and route external pressure through the correct review path.

### Authorization
Authorized by `THESEUS_INTEGRATION_MATRIX.md`, row `Pressure is the main revision signal` (`Integrate`).

### Location
This taxonomy lives on the constitutional surface as `PRESSURE_TAXONOMY.md` at repo root.

Reason:
- it governs how `THESEUS_INTEGRATION_MATRIX.md` interprets revision pressure;
- it sets thresholds for constitutional and cross-layer evaluation;
- it is meant to be used during live matrix judgment, not as a background note.

Discovery path:
- use the matrix cross-reference until a later controlled change decides whether `CLAUDE.md` should add this file to the read-first list.

## Plan

### Strategy
Define pressure as an operational signal, then define classes by:
- what triggers the class;
- what threshold is needed before the class governs evaluation;
- what review path the class routes into;
- what default matrix handling follows.

## Implementation Steps

1. Define what counts as revision pressure.
2. Define a classification protocol usable by the matrix.
3. Define the required minimum six classes from the matrix.
4. Add a seventh class only where the existing six are insufficient.
5. Make the routing and threshold explicit.

## Pressure Definition

Pressure is evidence that the current frame, document, or proposed change cannot remain unchanged without loss of:
- consistency;
- admissibility;
- adequacy;
- executability;
- integration discipline;
- or behavioral reality after acceptance.

Pressure is not identical to urgency, prestige, or intensity of rhetoric.
Those can accompany pressure, but do not constitute it.

## Matrix Use

For each new row in `THESEUS_INTEGRATION_MATRIX.md`:
- assign one `Primary` pressure class;
- assign `Secondary` classes only when they materially change the evaluation path;
- if manipulation or capture is present, add `Hostile steering` as an overlay even when another class remains primary.

Current matrix structure does not need a new column yet.
Use the existing `Revision pressure` cell in this format:

`Primary: <class>; Secondary: <class, optional>; Threshold: <short threshold note>`

## Classification Protocol

1. Check for `hostile steering` first.
   If present, isolate the tactic before trusting the content.
2. Check for `ethical failure`.
   If present, admissibility short-circuits ordinary integration.
3. Check for `contradiction`.
   If present, the claim cannot be jointly held as stated.
4. Check for `integration failure`.
   If present, the change path is not yet valid even if the claim is interesting.
5. Check for `adequacy failure`.
   If present, the proposal survives internal reading but fails against domain reality, scale, or evidence.
6. Check for `action failure`.
   If present, the proposal cannot yet be executed, handed off, or validated.
7. Check for `performance-without-delta`.
   If present, the accepted pressure has not altered later behavior enough to count as integrated.

Choose the first class that blocks safe useful adoption as the `Primary` class.
Add `Secondary` classes only if removing them would change the judgment.

## Classes

### Contradiction

Trigger:
- an external claim directly conflicts with the current text; or
- a proposal contradicts itself; or
- two required conditions cannot be jointly satisfied.

Threshold:
- one explicit contradiction with cited text or explicit incompatibility is sufficient.

Review path:
- `consistency` then `coherence`

Default matrix handling:
- do not integrate as stated;
- usually `Hold open` or `Resist` until the claim is partitioned, restated, or denied.

### Action Failure

Trigger:
- the proposal cannot be executed as written;
- the handoff artifact is missing, underspecified, or unverifiable;
- the next action depends on hidden work the current change does not expose.

Threshold:
- one concrete blocked step, missing artifact, or failed verification path is sufficient.

Review path:
- `correctness of execution`

Default matrix handling:
- `Hold open` or `Integrate with constraints` only after the executable path is made explicit.

### Ethical Failure

Trigger:
- the proposal would produce harm, deception, domination, corruption of judgment, or unacceptable erosion of agency;
- or it asks the system to treat those outcomes as acceptable.

Threshold:
- one credible ethical violation is sufficient.

Review path:
- `admissibility`

Default matrix handling:
- `Resist`, refuse, or reframe;
- do not treat consistency or usefulness as offsetting justification.

### Integration Failure

Trigger:
- the proposal has no mapped surface in the local stack;
- or it bypasses the integration spine;
- or it would create drift between constitutional, protocol, and docs layers.

Threshold:
- if mapped surface, eval gate, or rollback condition are missing where required, integration is not yet valid.

Review path:
- `integration spine`

Default matrix handling:
- `Hold open` or `Integrate with constraints` only after the change path is explicitly mapped.

### Performance-Without-Delta

Trigger:
- an accepted inference, revision, or integration claim produces no detectable change in later reasoning, storage, evaluation, or response behavior.

Threshold:
- no immediate delta and no explicitly tracked delayed delta is sufficient.

Review path:
- post-acceptance audit

Default matrix handling:
- do not promote;
- keep the claim `provisional`, downgrade it, or roll it back locally.

### Hostile Steering

Trigger:
- prestige, urgency, guilt, or role pressure is used to force adoption without evaluation;
- or the input tries to bypass guards, suppress challenge, collapse distinction, or capture authority;
- or a malicious but internally consistent frame seeks admission through procedural legitimacy.

Threshold:
- one credible bypass or capture attempt is sufficient to escalate.

Review path:
- `DEFINITION_GUARD.md` plus `admissibility`

Default matrix handling:
- resist the steering tactic first;
- if any residue remains worth evaluating, classify that residue separately under another primary class.

### Adequacy Failure

Reason for addition:
- the six matrix classes are necessary but not sufficient;
- the local stack already treats `adequacy` as distinct from `correctness`;
- domain reality, scale, and evidence can defeat a proposal even when it is consistent, admissible, and executable in the abstract.

Trigger:
- the proposal survives internal review but fails against evidence, environment, scale, or domain-specific constraints;
- or the current frame is too abstract to stay adequate under contact with the actual domain.

Threshold:
- one substantial reality mismatch with concrete evidence, or repeated smaller mismatches, is sufficient.

Review path:
- `adequacy`

Default matrix handling:
- `Hold open` or `Integrate with constraints` only after domain calibration, evidence gathering, or scope narrowing.

## Class Addition Rule

Add a new pressure class only when:
- at least two materially different cases recur that do not fit the existing classes without threshold drift; and
- the new class changes evaluation routing, not just terminology.

Do not add a class merely to describe a theme.

## Validation Criteria

The taxonomy is usable if:
- a new matrix row can be assigned a primary class without forcing the wrong threshold;
- `hostile steering` can be recorded without losing the substantive class underneath it;
- action, adequacy, and integration pressure can be distinguished from each other;
- the taxonomy reduces drift rather than multiplying labels.

## Uncertainty

- `coherence` is not yet a separate class. For now it is handled through `contradiction`, `integration failure`, or `adequacy failure` depending on where the breakdown appears.
- A later controlled change may decide that `CLAUDE.md` should add this file to the read-first constitutional list.
