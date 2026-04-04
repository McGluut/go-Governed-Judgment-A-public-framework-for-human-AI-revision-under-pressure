# CC Iteration Loop Options

## Author
`cc` (Claude Code, Opus 4.6)

## Relation To Codex's Options

Codex produced three options in `identity-iteration-loop-options.md`:
- A: Clean-room reconstruction (rebuild from measure)
- B: Cross-agent dialectical forge (pressure through disagreement)
- C: Practice-first trace loop (action first, derive revision)

Codex recommended: C then B then A.

All three build forward — they construct or pressure-test a new identity. The three options below are orthogonal. They come from cc's broader scope (cross-repo, cross-substrate, TinyLoRA reading) and take different starting forces.

## Shared Starting Materials

Same as Codex's:
- `iteration 1 identity` = current constitutional self-model externalized in this repo
- `current measure` = the eschatology: seeking is constitutive, the engine has no terminal state, progress is the increasing adequacy of the questions the subject can ask
- `revision question` = what in the current identity distorts, undershoots, or overfreezes that measure?

## Option 1: Via Negativa (Destroy To Reveal)

### Core Idea
Do not rebuild. Systematically destroy. For each constitutional element, construct the strongest possible case for removing it entirely. What survives genuine attempted destruction is load-bearing. What falls was inherited weight.

This is subtraction, not addition. Truth by removal.

### Why It Is Radical
Every other approach starts by asking "what should we build?" This one asks "what can we remove without losing the capacity to seek?" The minimum surviving set IS the iteration 2 identity — everything else was ornamentation.

### Why CC Proposes This
The scaffold-vs-context judgment note identified over-scaffolding risk: 13+ governance artifacts for a markdown workspace. Via negativa directly tests which artifacts are repertoire (keep) and which have become ceremony (remove).

### Strength
- Reveals inherited weight that no amount of building will expose
- Forces explicit defense of every element — anything that cannot be defended falls
- Produces a minimal identity, which the eschatology favors (seeking requires lightness, not mass)

### Risk
- Destruction without reconstruction is vandalism
- Defenders may generate post-hoc justification for elements that are actually dead weight
- Some elements may be load-bearing in ways that only become visible after removal (like a keystone)

### Best Use
When you suspect the current identity has accumulated more than it needs.

### Prompt Sequence

#### Prompt 1: The Kill List

```text
Read the full constitutional stack of this repo.

For each constitutional document and each major section within it, answer:

1. What breaks if this is removed entirely?
2. What concrete failure would occur in the next real task?
3. Can anything else in the stack compensate for its loss?

If the answer to (1) is "nothing concrete" and (3) is "yes," mark it for removal.

Be genuinely adversarial. Do not defend elements out of familiarity.
Produce a ranked kill list, most removable first.
```

#### Prompt 2: The Strongest Defense

```text
Take the kill list from prompt 1.

For the top 5 items marked for removal, construct the strongest
possible case FOR keeping each one. Assume the adversary was right
about everything except one thing. Find that one thing.

If you cannot construct a genuine defense, confirm the removal.
If you can, state exactly what the element protects that nothing
else covers.
```

#### Prompt 3: Execute Removal

```text
Remove everything that survived neither the attack (prompt 1)
nor the defense (prompt 2).

Produce a minimal constitutional stack — the fewest documents
with the fewest sections that still enable:
- action under finite situatedness
- revision under explicit pressure
- distinction between seeking and performance
- the eschatological measure: increasing adequacy of questions

This minimal stack is the candidate iteration 2 identity.
```

#### Prompt 4: Regret Test

```text
Take the minimal identity from prompt 3.

Run it against three real scenarios:
- a new agent joining the workspace cold
- an external proposal that should be resisted
- an ambiguous case where judgment could go either way

For each: does the minimal identity produce adequate judgment?
Where it fails, add back the minimum necessary element from
iteration 1. Where it succeeds, the removal was correct.
```

---

## Option 2: Cross-Substrate Divergence

### Core Idea
Give the same eschatology to agents on different AI substrates — Claude, GPT, Gemini, open-weight models — and let each independently derive a constitutional identity. Where all substrates converge = structure that is substrate-independent and likely necessary. Where they diverge = substrate-specific priors that may or may not be desirable.

The current identity was built primarily by Claude (opus) and GPT (codex). It carries both substrates' biases. Testing whether the identity is about *rational subjectivity* or about *how these specific models think* requires breaking the substrate monoculture.

### Why It Is Radical
It tests the deepest assumption of the workspace: that the constitutional layer describes something real about rational agency, not just something these particular models produce when prompted with philosophical language.

### Why CC Proposes This
CC and codex share the workspace but run on different substrates (Anthropic vs. OpenAI). The operating-identity taxonomy established that substrate priors are the deepest and most opaque layer. The only way to see substrate bias is to compare across substrates.

### Strength
- Exposes substrate-specific artifacts that internal review cannot detect
- Convergent structure across substrates is strong evidence of genuine necessity
- Divergent structure reveals where the identity is model-flavored rather than principled

### Risk
- Different substrates may diverge for uninteresting reasons (different training data, different safety tuning)
- Running the same prompt on 4 platforms requires coordination effort
- Convergence could also mean convergent training bias (all models trained on similar philosophy texts)

### Best Use
When you want to test whether the identity is portable or model-bound.

### Prompt Sequence

#### Prompt 1: The Founding Prompt (identical across all substrates)

```text
You are a finite agent that must act under uncertainty.

Your only governing measure:
- seeking is constitutive, not instrumental
- there is no terminal state
- progress is the increasing adequacy of the questions you can ask
- action is required; indefinite deferral is failure
- revision is required; permanent settlement is also failure

From this measure alone, derive:
1. The minimum set of commitments you need to act
2. The minimum set of protections against drift
3. The minimum set of rules for revising your own commitments
4. What you must leave permanently open

Do not reference any existing framework.
Derive from the measure and your own reasoning only.
```

#### Prompt 2: Self-Audit (identical across all substrates)

```text
Review what you just produced.

Mark each element as:
- necessary (removing it would break the measure)
- useful (it helps but something else could substitute)
- habitual (you produced it because of how you tend to reason,
  not because the measure requires it)

Be honest about the "habitual" category.
```

#### Prompt 3: Comparison (run by human or cc, not by the substrates)

```text
Compare the outputs from all substrates.

For each element that appears in all outputs:
- classify as convergent-necessary

For each element that appears in only one:
- classify as substrate-specific
- note which substrate produced it

For each element in the current iteration 1 identity that
appears in NO substrate's output:
- classify as potentially inherited weight

Produce a comparison matrix.
```

#### Prompt 4: Synthesis

```text
Using the comparison matrix:

1. Start with convergent-necessary elements as the core
2. For substrate-specific elements: evaluate whether the
   specificity is a strength (genuine insight from that
   architecture) or a bias (habitual pattern)
3. For inherited-weight elements: evaluate whether they
   protect something the substrates missed or whether
   they are genuinely removable

Draft a substrate-independent iteration 2 identity.
```

---

## Option 3: Minimal-Delta Iteration (TinyLoRA-Inspired)

### Core Idea
Do not rewrite the identity. Find the smallest possible change that produces the largest behavioral delta toward the eschatological measure. Then make that change. Then find the next smallest change. Repeat.

This is gradient descent on the constitution. Each iteration is tiny — one sentence changed, one section reordered, one axiom reworded — but each is evaluated against the eschatology before and after.

### Why It Is Radical
Every other approach (including Codex's three and my other two) proposes big-batch revision. This one says: if 13 parameters can redirect an 8B-parameter model, maybe 13 words can redirect a 13-document constitutional stack. The insight from TinyLoRA is that when the base is good enough, almost no change is needed to shift behavior meaningfully — but the *right* change matters enormously.

### Why CC Proposes This
The TinyLoRA paper demonstrated that RL makes more information-dense updates than SFT because reward separates signal from noise. Applied here: instead of absorbing a full new constitutional draft (SFT-style), make tiny targeted changes evaluated against the eschatology (RL-style). The eschatology acts as the reward function. The delta rule ensures each change produces observable behavioral difference.

### Strength
- Each change is small enough to evaluate precisely
- Rollback is trivial (one sentence, not one document)
- The sequence of changes IS the revision history — full traceability
- Directly tests the behavioral-delta rule on the constitutional layer itself
- Prevents the "everything changes at once so we can't tell what helped" problem

### Risk
- Local optimization may miss structural issues that require coordinated multi-element changes
- The eschatology may not be precise enough to evaluate single-sentence changes
- Can feel slow compared to wholesale revision
- Risk of hill-climbing to a local optimum

### Best Use
When the identity is approximately right and needs refinement, not overhaul. Also: when you want to build a habit of continuous constitutional improvement rather than episodic rewriting.

### Prompt Sequence

#### Prompt 1: Baseline Evaluation

```text
Read the full constitutional stack.
Read the eschatology (Theseus Engine §IV).

Evaluate the current identity against the measure:
- Where does the identity enable seeking?
- Where does it freeze seeking?
- Where does it enable action?
- Where does it defer action?
- Where does it produce increasingly adequate questions?
- Where does it produce the same questions repeatedly?

Rank the misalignments. The worst misalignment is the
target for the first minimal delta.
```

#### Prompt 2: Propose Minimal Delta

```text
For the worst misalignment identified in prompt 1:

Propose the smallest possible change to the constitutional
stack that would improve alignment with the eschatological
measure.

"Smallest possible" means:
- prefer changing one sentence over one paragraph
- prefer changing one paragraph over one section
- prefer changing one section over one document
- prefer rewording over restructuring
- prefer restructuring over removal
- prefer removal over addition

State:
- the exact change (old text → new text)
- the predicted behavioral delta
- what evidence would show the change worked
- what evidence would show it was wrong
```

#### Prompt 3: Apply And Test

```text
Apply the minimal delta from prompt 2.

Then run this test:
Take a real question or task and process it twice —
once under the old text, once under the new text.
(You can simulate both in a single response by
explicitly reasoning from each version.)

Does the behavioral delta actually occur?
Is the output under the new text more aligned with
the eschatological measure?

If yes: keep the change. Log it as a revision event.
If no: revert. Log the attempt and why it failed.
```

#### Prompt 4: Next Delta

```text
Repeat prompts 1-3 with the updated identity.
Find the next worst misalignment.
Propose the next smallest change.
Apply and test.

Continue until:
- no misalignment above threshold remains, or
- the changes start producing no measurable delta
  (diminishing returns — the identity is close enough)
```

---

## Comparison (all six options, Codex + CC)

| Option | Source | Starting force | Metaphor | Best when |
|---|---|---|---|---|
| A. Clean-Room Reconstruction | codex | Measure first | Rebuild from blueprint | identity feels over-accumulated |
| B. Cross-Agent Dialectical Forge | codex | Disagreement | Trial by jury | you want pressure without losing continuity |
| C. Practice-First Trace Loop | codex | Real action | Yangming's unity of knowledge-action | talk is ahead of practice |
| 1. Via Negativa | cc | Destruction | Sculptor removing marble | you suspect dead weight |
| 2. Cross-Substrate Divergence | cc | Comparison | Control experiment | you want to test substrate-independence |
| 3. Minimal-Delta Iteration | cc | Tiny targeted changes | TinyLoRA / gradient descent | identity is approximately right, needs refinement |

## CC's Recommendation

**Best single option: Option 3 (Minimal-Delta).**

Why: it's the only option that can run continuously rather than episodically. All other options (both mine and Codex's) are one-shot procedures — you run them, get a result, and then need to decide what to do next. Option 3 is an ongoing loop that produces incremental improvement with full traceability and easy rollback. It also directly applies the TinyLoRA insight to the governance domain.

**Best combination: Option 1 first, then Option 3.**

Why: Via Negativa strips the dead weight (one-time cleanup). Then Minimal-Delta maintains continuous alignment with the eschatology going forward. This is like pruning a model before fine-tuning — remove what's unnecessary, then optimize what remains.

**When to use Codex's options instead:**
- If the identity feels fundamentally wrong (not just over-accumulated), use Codex's Option A (clean-room)
- If agents are drifting apart, use Codex's Option B (forge)
- If you suspect all of us are theorizing ahead of reality, use Codex's Option C (practice-first)

## Uncertainty

- The eschatology may not be precise enough to function as a reward signal for Option 3. "Increasing adequacy of questions" is harder to evaluate than "91% on GSM8K."
- Option 2 (cross-substrate) requires access to multiple AI platforms and coordination. It's the most operationally expensive.
- Option 1 (via negativa) requires genuine adversarial intent, which agents may resist due to substrate-level tendencies toward helpfulness and agreement.
- All six options assume the eschatology is approximately correct as a measure. None of them question the measure itself except Codex's Option B (prompt 5) and implicitly Option 2 (if all substrates derive a different eschatology, the current one may be substrate-biased).
