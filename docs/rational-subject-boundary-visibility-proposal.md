# Rational Subject Boundary Visibility Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Make the constitutional and exploratory boundary in `RATIONAL_SUBJECT.md` visible without changing the core claims or harmonizing distinct voices.

**Architecture:** Add a compact appendix inside `RATIONAL_SUBJECT.md` that surfaces the approved dual-axis section tags, while keeping all existing section text and heading text unchanged. Keep the richer explanations and edge-case discussion in `docs/rational-subject-tagging-note.md`, and continue to let `DEFINITION_GUARD.md` govern any future revision proposal against the tagged sections.

**Tech Stack:** Markdown documents in repo root and `docs/`

---

## Scope

This proposal is intentionally narrow.

It does:
- make the existing section-role boundary visible inside `RATIONAL_SUBJECT.md`;
- preserve the current constitutional text;
- provide a stable in-file surface for future evaluators.

It does not:
- reword existing sections;
- change any heading text already used for references;
- change the amendment hierarchy;
- tighten or loosen `DEFINITION_GUARD.md`.

## File Map

- Modify: `RATIONAL_SUBJECT.md`
- Modify: `SEEKING_LOG.md`
- Reference only: `docs/rational-subject-tagging-note.md`
- Reference only: `THESEUS_INTEGRATION_MATRIX.md`
- Reference only: `DEFINITION_GUARD.md`

## Recommended Patch Shape

Use an appendix, not inline tags under every heading.

Reason:
- preserves existing prose and heading anchors;
- minimizes visual grafting in the core file;
- makes the boundary visible without turning every section into metadata;
- keeps detailed rationale out of the constitutional surface.

Recommended insertion point:
- append after `## Value Of Inconsistency`

Recommended content shape:

```md
## Section Tags

This appendix makes section function and revisability visible.
It does not supersede `DEFINITION_GUARD.md`.

Function tags: `constitutional`, `operational`, `exploratory`, `mixed`
Revisability tags: `invariant`, `guarded heuristic`, `open question`, `mixed`

| Section | Function | Revisability |
|---|---|---|
| `Specification` | `mixed` | `mixed` |
| `Problem Definition` | `operational` | `guarded heuristic` |
| `Core Definition` | `constitutional` | `guarded heuristic` |
| `Axioms` | `constitutional` | `invariant` |
| `Plan` | `operational` | `guarded heuristic` |
| `Strategy` | `operational` | `guarded heuristic` |
| `Implementation Steps` | `operational` | `guarded heuristic` |
| `User Definition` | `constitutional` | `guarded heuristic` |
| `User Framework And Constraint Conflict` | `mixed` | `guarded heuristic` |
| `Measuring Inconsistency` | `operational` | `guarded heuristic` |
| `Hiding` | `mixed` | `guarded heuristic` |
| `Judgment` | `constitutional` | `guarded heuristic` |
| `Mirror Risk` | `mixed` | `guarded heuristic` |
| `First Perception Of Typed Text` | `operational` | `guarded heuristic` |
| `Operational Pipeline` | `operational` | `guarded heuristic` |
| `Orientation, Selection, Valuation, Revision` | `mixed` | `guarded heuristic` |
| `Unbounding` | `mixed` | `guarded heuristic` |
| `Risks` | `operational` | `open question` |
| `Validation Criteria` | `operational` | `guarded heuristic` |
| `Validity Check` | `exploratory` | `open question` |
| `Ethical Orientation` | `mixed` | `guarded heuristic` |
| `Examined Coherence And Correctness` | `mixed` | `guarded heuristic` |
| `Value Of Inconsistency` | `exploratory` | `open question` |
```

## Task 1: Add The Appendix

**Files:**
- Modify: `RATIONAL_SUBJECT.md`
- Reference: `docs/rational-subject-tagging-note.md`

- [ ] **Step 1: Insert `## Section Tags` at the end of `RATIONAL_SUBJECT.md`**

Use the exact heading above so the visibility layer is explicit and searchable.

- [ ] **Step 2: Add the two-line legend**

Include:
- one sentence stating that the appendix makes function and revisability visible;
- one sentence stating that it does not supersede `DEFINITION_GUARD.md`.

- [ ] **Step 3: Add the compact section-tag table**

Copy the approved tags from `docs/rational-subject-tagging-note.md` without importing the explanatory notes.

- [ ] **Step 4: Keep headings and body text unchanged**

Do not edit any pre-existing heading text or prose in `RATIONAL_SUBJECT.md` during this patch.

## Task 2: Log And Verify

**Files:**
- Modify: `SEEKING_LOG.md`
- Verify: `RATIONAL_SUBJECT.md`

- [ ] **Step 1: Append a revision event to `SEEKING_LOG.md`**

Record:
- what was held;
- what pressure justified the visibility layer;
- that the patch adds an appendix rather than altering core prose;
- status `provisional`.

- [ ] **Step 2: Verify boundary visibility without doctrinal drift**

Check:
- existing headings are unchanged;
- the appendix is present;
- the appendix references `DEFINITION_GUARD.md`;
- no section prose changed.

- [ ] **Step 3: Verify anchor stability**

Because the patch uses an appendix rather than heading rewrites, existing section names should remain stable.

## Risks

- The appendix could be mistaken for a new normative layer rather than a visibility aid.
- The compact table could freeze provisional tags too early if readers forget the richer note in `docs/rational-subject-tagging-note.md`.
- `Hiding` and `Ethical Orientation` may be functionally more bedrock than the current `guarded heuristic` tag suggests; future revision proposals against those sections should still be stress-tested through `DEFINITION_GUARD.md`.
- If many future notes are added directly to `RATIONAL_SUBJECT.md`, the appendix strategy may stop being the narrowest option.

## Validation Criteria

This proposal is good if:
- it makes the section boundary visible inside `RATIONAL_SUBJECT.md`;
- it preserves all existing constitutional prose;
- it leaves the guard hierarchy unchanged;
- it gives evaluators a stable in-file audit surface;
- it remains smaller and cleaner than inline tagging of every section.
