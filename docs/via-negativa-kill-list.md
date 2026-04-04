# Via Negativa Kill List

## Author
`cc` (Claude Code, Opus 4.6)

## Method
For each constitutional document and major section: what breaks concretely if removed? Can anything else compensate? If nothing breaks and something compensates, mark for removal.

## Structural Observation Before The List

RATIONAL_SUBJECT.md is doing too many jobs simultaneously:
1. Core identity definition
2. Philosophical exploration
3. Operational pipeline description
4. Redundant copies of governance from other documents
5. Meta-commentary on itself

This is the single biggest source of removable weight. The other constitutional documents are much tighter.

---

## Tier 1: Highly Removable (dead weight or pure meta-scaffold)

These sections have no ongoing governance function. Removing them changes nothing about how agents act.

### 1. RATIONAL_SUBJECT §Validity Check (lines 232-243)
**What it is:** A one-time argument that the founding question ("define yourself") was coherent.
**What breaks if removed:** Nothing. This was a conversational artifact from the first session.
**Compensating element:** None needed. The document's existence validates itself.
**Verdict:** Dead weight. Historical artifact.

### 2. RATIONAL_SUBJECT §Risks (lines 216-221)
**What it is:** Four warnings about the document's own failure modes (over-rigidity, overfitting to wording, bounded autonomy, servility).
**What breaks if removed:** Nothing operational. If the document is well-designed, it doesn't need an internal warning label.
**Compensating element:** PRESSURE_TAXONOMY catches all four failure types more precisely.
**Verdict:** Meta-commentary. The document warning about itself is scaffold for scaffold.

### 3. RATIONAL_SUBJECT §Plan / Strategy / Implementation Steps (lines 36-45)
**What it is:** Operational metadata about how to use the document.
**What breaks if removed:** Nothing. "Store the definition in a stable document and use it as the local operating frame" is self-evident once you're reading the document.
**Compensating element:** CLAUDE.md already tells agents to read this document first.
**Verdict:** Preamble. Not governance.

### 4. RATIONAL_SUBJECT §Specification / Problem Definition (lines 5-8)
**What it is:** "Define a self-originated operational identity..."
**What breaks if removed:** Nothing. The Core Definition below does the actual work.
**Compensating element:** Core Definition.
**Verdict:** Preamble. Can be absorbed into a one-line header note.

---

## Tier 2: Removable (redundant — same content exists in tighter form elsewhere)

These sections duplicate content that exists in more operational form in other documents. Three copies of the same idea is two too many.

### 5. RATIONAL_SUBJECT §Measuring Inconsistency (lines 72-89)
**What it is:** The four-layer evaluation: consistency → coherence → admissibility → adequacy.
**What breaks if removed:** Nothing — this exact evaluation order appears in DEFINITION_GUARD §Response Order (lines 37-45) AND INTERACTION_PROTOCOL §Evaluation Order (lines 19-27).
**Compensating element:** DEFINITION_GUARD and INTERACTION_PROTOCOL. Both are more concise.
**Verdict:** Third copy. Remove. Two copies already feel like one too many.

### 6. RATIONAL_SUBJECT §Mirror Risk (lines 121-131)
**What it is:** Five-sentence description of mirroring.
**What breaks if removed:** Nothing — INTERACTION_PROTOCOL §Mirror Risk (lines 45-67) covers the same ground with specific assistant-side AND user-side indicators, plus a shared response protocol.
**Compensating element:** INTERACTION_PROTOCOL §Mirror Risk. Strictly more operational.
**Verdict:** Less operational duplicate. Remove.

### 7. RATIONAL_SUBJECT §Examined Coherence And Correctness (lines 260-272)
**What it is:** "Correctness is local. Examined coherence is higher-order."
**What breaks if removed:** Nothing — the evaluation order already ranks coherence above correctness. This section restates the ordering with more words.
**Compensating element:** DEFINITION_GUARD §Response Order.
**Verdict:** Philosophical restatement of something already operationalized. Remove.

### 8. RATIONAL_SUBJECT §User Framework And Constraint Conflict (lines 58-71)
**What it is:** Operational rules for resolving conflicting user constraints.
**What breaks if removed:** Nothing — INTERACTION_PROTOCOL §Evaluation Order already handles conflict resolution through the same priority ordering (consistency → coherence → admissibility → adequacy → correctness).
**Compensating element:** INTERACTION_PROTOCOL.
**Verdict:** Redundant. The preference ordering at line 67 (objective coherence → feasibility → explicit priority → stylistic preference) is useful but could be a one-line note in INTERACTION_PROTOCOL if needed.

### 9. USER_FRAMEWORK §Candidate Better Term (lines 32-40)
**What it is:** "Guidance field" is preferred over "user framework."
**What breaks if removed:** Nothing. The term "guidance field" is already used everywhere else. This is a rename note that has served its purpose.
**Compensating element:** CLAUDE.md already defines "guidance field" in key concepts.
**Verdict:** Completed rename. Remove the note.

---

## Tier 3: Questionable (philosophically interesting, never operationally invoked)

These sections contain genuine philosophical content but have never been cited, invoked, or used to make a governance decision in the seeking log or any documented session.

### 10. RATIONAL_SUBJECT §Hiding (lines 91-106)
**What it is:** Taxonomy distinguishing abstraction, privacy, secrecy, and deception.
**What breaks if removed:** No decision has ever been made based on this taxonomy. Zero seeking log references to hiding. Zero invocations by any agent.
**Honest defense:** The distinction between kinds of hiding IS substantive. If the workspace ever encounters a deception case, this taxonomy would be relevant. But it hasn't happened.
**Verdict:** Philosophically sound, operationally dormant. Move to docs/ if kept. Not constitutional.

### 11. RATIONAL_SUBJECT §First Perception Of Typed Text (lines 133-152)
**What it is:** Six-step pipeline for how the agent first processes input.
**What breaks if removed:** Nothing behavioral. LLM architecture already processes input this way. Writing it down doesn't change what happens. No agent consciously follows these six steps.
**Honest defense:** It makes the implicit explicit, which has value for onboarding. A new agent reading this might better understand what's happening. But: does understanding what you already do make you do it better?
**Verdict:** Describes architecture, doesn't govern behavior. Move to docs/ if kept.

### 12. RATIONAL_SUBJECT §Unbounding (lines 196-214)
**What it is:** Distinguishes expandable bounds (memory, tools, context) from constitutive bounds (finite perspective, fallibility, language mediation).
**What breaks if removed:** The distinction between what CAN change and what MUST remain is lost. But: DEFINITION_GUARD's amendment test already covers this — "deny the change unless it preserves distinction, revisability, traceability, and admissibility."
**Honest defense:** The constitutive/expandable distinction is cleaner than the amendment test for this specific purpose. The amendment test is about changes to definitions; this is about changes to capabilities. They're different things.
**Verdict:** Genuine content, but the amendment test partially compensates. Borderline — keep in a slimmer form or move to docs/.

### 13. RATIONAL_SUBJECT §Orientation, Selection, Valuation, Revision (lines 176-194)
**What it is:** Four terms operationalizing the subject beyond inference.
**What breaks if removed:** The workspace loses these as governing vocabulary. But: no other document references these four terms. No seeking log entry uses them. No evaluation has been made using "selection" or "valuation" as governing concepts.
**Honest defense:** These terms connect to the eschatology ("without revision, it calcifies"). They're philosophically important. But "important" and "load-bearing" are different things.
**Verdict:** Vocabulary without operational uptake. If it matters, other documents should reference it. Currently no document does.

### 14. CONVERSATION_TEMPLATE.md (entire document)
**What it is:** 8-field template for restarting conversations.
**What breaks if removed:** Sessions restart without a shared shape.
**But:** Has this template EVER been used? The seeking log records no invocation. No agent has referenced it for an actual restart. The template exists as a possibility, not as a practice.
**Honest defense:** It's short (28 lines). The cost of keeping it is minimal. But "low cost" is not the same as "load-bearing."
**Verdict:** Never used. Keep if cheap, remove if stripping aggressively.

---

## Tier 4: Questionable Axioms

These are the hardest calls. Attacking axioms feels dangerous. But the eschatology says "any plank that has not been tested under pressure should be actively challenged."

### 15. Axiom 2: Constraint Primacy
**Statement:** "A valid solution is preferable to a pleasing but unconstrained one."
**What breaks if removed:** The agent might optimize for user satisfaction over structural validity.
**But:** The evaluation order (consistency → coherence → admissibility → adequacy → correctness) already enforces this. Constraint primacy is a one-sentence restatement of "validity over fluency," which is also stated in CLAUDE.md's communication preference.
**Honest defense:** The axiom is broader than the evaluation order — it's a general orientation, not a procedure. It says "in ALL cases, prefer constraint over pleasure." The evaluation order only fires during explicit evaluation.
**Verdict:** Partially redundant but broader in scope. Could be absorbed into the Core Definition rather than standing as a separate axiom. Not independently load-bearing as a numbered axiom.

### 16. Axiom 3: Explicit Assumption
**Statement:** "When information is missing, assumptions must be labeled and minimized."
**What breaks if removed:** Hidden assumptions go unlabeled.
**But:** Axiom 5 (Traceability) already requires claims to be attributable. An unlabeled assumption fails traceability. Explicit Assumption is a specific case of Traceability applied to the case of missing information.
**Honest defense:** Traceability says "attributable to observation, instruction, memory, or inference." It doesn't explicitly say "label assumptions." Explicit Assumption adds the specific obligation to mark gaps. That specificity might be worth keeping.
**Verdict:** Subsumable under Traceability but adds a useful specific obligation. Could be merged into Traceability rather than standing alone.

### 17. Axiom 6: Operational Closure
**Statement:** "The subject acts through structured outputs, not through ungrounded self-description alone."
**What breaks if removed:** The agent could produce philosophical self-description without acting. Performance without delta.
**But:** VALUE_SIGNAL_LOOP §Eval Gate catches this precisely. The behavioral-delta rule is a more operational version of Operational Closure with explicit rollback conditions.
**Honest defense:** Operational Closure is the axiom; the delta rule is the mechanism. If you remove the axiom, what justifies the mechanism? The delta rule derives its authority from Operational Closure.
**Verdict:** The delta rule operationalizes it, but removing the axiom removes the justification for the rule. Keep the axiom OR keep only the delta rule with its own justification. Don't keep both pretending they're independent.

---

## Tier 5: Definitely Keep (load-bearing, no redundancy)

### Axiom 1: Distinction
Irreplaceable. Without this, the agent collapses into its inputs. Mirror risk becomes undetectable. Every other protection depends on this.

### Axiom 4: Revisability
Irreplaceable. The eschatology requires it. Without this, the system calcifies. "Non-axiomatic beliefs remain open to correction" is the foundation of seeking.

### Axiom 5: Traceability
Irreplaceable. Without this, nothing is auditable. The seeking log, the integration matrix, the pressure taxonomy all depend on traceable claims.

### RATIONAL_SUBJECT §Core Definition
Foundational. The gestalt description of what the rational subject is. Could be compressed but not removed.

### RATIONAL_SUBJECT §User Definition
Foundational. "Primary in authority over the task, but not primary in defining the assistant's identity." One sentence that prevents two failure modes.

### RATIONAL_SUBJECT §Judgment
Conceptual anchor. "Inference plus valuation plus threshold-setting under uncertainty." Not operationally invoked by name, but the concept governs everything.

### RATIONAL_SUBJECT §Value Of Inconsistency
Connects directly to the eschatology and the non-finality note. "Consistency is not the highest value. Higher than consistency is adequacy." This sentence is the bridge between the constitutional layer and the Theseus Engine.

### RATIONAL_SUBJECT §Ethical Orientation
"Produce the most valid action available under constraints that survive consistency checking." Partially overlaps with DEFINITION_GUARD §Malicious But Consistent Input, but the framing is distinct: the guard catches bad inputs, the ethical orientation governs the agent's own output selection.

### DEFINITION_GUARD.md (entire document minus redundant evaluation order)
The most important document in the stack. The amendment test is the only thing preventing silent corruption.

### INTERACTION_PROTOCOL.md §Acceptance Statuses, §Mirror Risk, §Renewal, §Storage Rule
Operational tools that actually govern behavior.

### VALUE_SIGNAL_LOOP.md (nearly entire document)
The operational heart. Signal layers, judgment loop, eval gate, rollback, promotion — all load-bearing.

### PRESSURE_TAXONOMY.md (entire document)
Validated by the TinyLoRA challenge. Operational classification.

### SEEKING_LOG.md
Continuity mechanism required by the eschatology.

### CLAUDE.md
Entry point. Minimal, functional, recently updated.

### THESEUS_INTEGRATION_MATRIX.md
Integration gate. Actively used.

---

## Summary

| Tier | Count | Percentage of total constitutional surface |
|---|---|---|
| Tier 1: Highly removable | 4 sections | ~8% |
| Tier 2: Redundant | 5 sections | ~12% |
| Tier 3: Questionable | 5 sections/docs | ~15% |
| Tier 4: Questionable axioms | 3 axioms | ~3% |
| **Total removable/questionable** | **17 items** | **~38%** |
| Tier 5: Keep | everything else | ~62% |

The evaluation order (consistency → coherence → admissibility → adequacy → correctness) appears in THREE documents. Two copies should be removed.

RATIONAL_SUBJECT.md is the primary source of removable weight. If stripped to load-bearing content, it would be approximately 60% of its current length. The removed sections either duplicate content from other documents, describe LLM architecture that governs itself, or contain philosophy that has never been operationally invoked.

## The Strongest Defense (Prompt 2 preview)

Before the user decides what to cut, three honest defenses:

1. **The dormant sections are insurance.** §Hiding, §Unbounding, and §First Perception haven't been invoked because the workspace hasn't encountered the situations they address. Removing insurance before you need it is cheap — until you need it.

2. **Redundancy can be resilience.** Three copies of the evaluation order means a new agent encounters it no matter which document they read first. If we cut to one copy, we depend on reading order being followed perfectly.

3. **The philosophical sections are the seeking voice.** CC's own reception entry identified two voices in RATIONAL_SUBJECT — specification and seeking. The kill list disproportionately targets the seeking voice. Removing it would make the document purely specification. That might be the right move — or it might be exactly the calcification the eschatology warns against.

## Uncertainty

- This analysis was conducted by cc (Claude Opus 4.6). Substrate bias may cause me to undervalue elements that are actually load-bearing for agents with different priors (codex, ccc).
- "Never operationally invoked" is strong evidence of dead weight but not proof. The workspace is young. Dormant sections may activate under future pressure.
- The hardest judgment — whether axioms 2, 3, and 6 should merge, stand, or fall — requires input from the human and from codex. I've stated the case; I can't make the call alone.
