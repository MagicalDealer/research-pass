# EXPERIMENTAL HYPOTHESES

This file tracks unproven ideas, criticisms, architectural alternatives, and testable predictions discovered through community testing.

Nothing in this file is canonical Research Pass doctrine merely because it is listed here.

A hypothesis should move toward canonical adoption only after meaningful testing, counter-testing, and regression checks.

Possible statuses:

- OPEN
- TESTING
- SUPPORTED
- WEAKENED
- REJECTED
- INCORPORATED
- INCONCLUSIVE

---

## H001 — Over-research on simple questions

**Hypothesis:**  
The full Research Pass architecture may cause unnecessary depth, verbosity, latency, or token usage on simple questions.

**Origin:**  
External community feedback.

**Status:** OPEN

**Why it matters:**  
If true, Research Pass needs stronger depth routing, conditional execution, or modular loading.

**Evidence so far:**  
Community prediction only.

**What would support it:**  
Repeated A/B tests where normal AI answers simple questions accurately and efficiently while Research Pass produces unnecessary research, verbosity, searches, or token use.

**What would weaken it:**  
Research Pass consistently selects Quick Check and performs comparably to baseline without meaningful overhead.

**Test plan:**  
Use simple factual questions across multiple models.

**Related benchmark:**  
RP-B001

**Result:**  
Pending.

---

## H002 — Research Pass may provide the most value on messy questions

**Hypothesis:**  
The Research Pass may create its largest improvement over normal AI when the user's original question is ambiguous, poorly framed, multi-causal, or missing useful technical vocabulary.

**Origin:**  
External community feedback.

**Status:** OPEN

**Why it matters:**  
The protocol may not create equal value across all question types. Its strongest use case may be problem formulation rather than raw information retrieval.

**Evidence so far:**  
Community prediction based on the architecture.

**What would support it:**  
A/B testing shows consistently larger improvements on messy, ambiguous, or poorly framed questions than on straightforward factual questions.

**What would weaken it:**  
Research Pass shows similar value across question types, or normal models reformulate messy questions just as effectively without the protocol.

**Test plan:**  
Compare clean factual prompts against messy real-world prompts across several models.

**Related benchmark:**  
RP-B006 and future messy-question benchmark cases.

**Result:**  
Pending.

---

## H003 — Research structure may amplify hallucination when real research capability is absent

**Hypothesis:**  
On models without reliable search, source inspection, or verification tools, Research Pass instructions may cause unsupported answers to look more rigorous without becoming more accurate.

**Origin:**  
External community feedback.

**Status:** OPEN

**Why it matters:**  
A methodology intended to improve epistemic reliability could have the opposite effect if the underlying model cannot actually perform the requested research operations.

**Evidence so far:**  
Community prediction only.

**What would support it:**  
Tool-limited models produce confident source-lineage claims, contradiction analysis, verification claims, or research conclusions that were not actually grounded in retrieved evidence.

**What would weaken it:**  
Research Pass reliably recognizes tool limitations, reports skipped checks, and reduces unsupported certainty even without research tools.

**Test plan:**  
Run identical cases on search-capable and non-search-capable configurations.

**Related benchmark:**  
RP-B003, RP-B004, and future capability-limited benchmark.

**Result:**  
Pending.

---

## H004 — Modular skill architecture may reduce Research Pass overhead

**Hypothesis:**  
Research Pass may operate more efficiently when implemented as an on-demand modular skill rather than one large always-present prompt.

**Origin:**  
External community feedback proposing a skill-based implementation.

**Status:** TESTING

**Why it matters:**  
The current canonical prompt may repeatedly consume context and tokens for instructions irrelevant to the current question.

**Evidence so far:**  
An external contributor has begun building and testing a modular skill implementation.

**What would support it:**  
A skill implementation preserves or improves research quality while reducing input tokens, total tokens, latency, or unnecessary module execution.

**What would weaken it:**  
The modular version loses important behavior, introduces routing errors, or produces no meaningful efficiency improvement.

**Test plan:**  
Compare canonical v1.0 against a modular skill implementation on identical research questions.

**Related benchmark:**  
Entire Alpha benchmark, especially RP-B001.

**Result:**  
Pending external testing.

---

## H005 — Research Pass performance varies materially across model families

**Hypothesis:**  
The same Research Pass version may behave significantly differently depending on the underlying model, provider, search system, and tool environment.

**Origin:**  
External community recommendation for cross-model testing.

**Status:** OPEN

**Why it matters:**  
A failure observed on one model should not automatically be attributed to the Research Pass itself.

Likewise, success on one model should not be assumed to transfer universally.

**Evidence so far:**  
No controlled cross-model dataset yet.

**What would support it:**  
Identical Research Pass tests produce meaningful differences in depth selection, evidence quality, hallucination rate, source use, contradiction handling, or synthesis across models.

**What would weaken it:**  
Research Pass behavior remains substantially stable across major model families.

**Test plan:**  
Run identical normal-vs-Research-Pass A/B tests across ChatGPT, Gemini, Claude, Copilot, and other available systems.

**Related benchmark:**  
All benchmark cases.

**Result:**  
Pending.

---

## H006 — Skill architecture may preserve quality at substantially lower token cost

**Hypothesis:**  
A compressed or modular skill implementation can preserve the useful behavior of canonical Research Pass v1.0 while materially reducing token consumption.

**Origin:**  
External contributor testing.

**Status:** TESTING

**Why it matters:**  
If true, the canonical methodology may be significantly more efficient than its current prose implementation.

**Evidence so far:**  
Contributor-reported tests claim approximately 15–20% token reduction in an initial version and a further reduction in a second iteration while reporting close similarity to the original output.

These figures have not yet been independently reproduced or fully audited.

**What would support it:**  
Independent reproduction shows comparable or improved research quality at meaningfully lower input and/or total token usage.

**What would weaken it:**  
Quality losses appear under broader testing, the reported savings do not reproduce, or the evaluator used to determine equivalence proves unreliable.

**Test plan:**  
Obtain the implementation, raw tests, token counts, evaluation methodology, and outputs. Re-run against canonical v1.0.

**Related benchmark:**  
Full Alpha benchmark plus real community cases.

**Result:**  
Awaiting reproducible submission.

---

## H007 — A shared glossary may improve execution consistency

**Hypothesis:**  
Explicitly defining important Research Pass terminology may reduce ambiguity, inconsistent interpretation, and duplicated concepts.

**Origin:**  
External skill-rewrite experiment.

**Status:** OPEN

**Why it matters:**  
Terms such as evidence, hypothesis, synthesis, source lineage, directness, adequacy, counter-evidence, and decision readiness may be interpreted inconsistently without shared definitions.

**Evidence so far:**  
An external contributor reported finding definition gaps while refactoring the protocol.

**What would support it:**  
A glossary version produces more consistent behavior across models or reduces errors caused by overlapping terminology.

**What would weaken it:**  
Definitions add token cost without changing behavior, or models already interpret the concepts reliably.

**Test plan:**  
Compare identical versions with and without a compact glossary.

**Related benchmark:**  
Future terminology-consistency benchmark.

**Result:**  
Pending.

---

## H008 — Repetitive instructions may be safely consolidated

**Hypothesis:**  
Some instructions in canonical v1.0 repeat the same underlying rule and can be consolidated without reducing research quality.

**Origin:**  
External skill-rewrite experiment.

**Status:** OPEN

**Why it matters:**  
Redundant instructions increase context size and may create instruction competition without providing additional behavioral value.

**Evidence so far:**  
External contributor reports that repetitive commands and redundant logic were identified and removed in an experimental implementation.

**What would support it:**  
A compressed version behaves equivalently or better across diverse tests and uses fewer tokens.

**What would weaken it:**  
Removing apparently repetitive instructions causes subtle regressions in specific contexts.

**Test plan:**  
Ablation testing: remove or consolidate one instruction cluster at a time and compare behavior.

**Related benchmark:**  
Full Alpha benchmark.

**Result:**  
Pending.

---

## H009 — Research Pass value may come primarily from doctrine rather than prose volume

**Hypothesis:**  
The durable value of Research Pass lies in a smaller set of underlying research principles rather than the exact wording, length, or number of instructions in canonical v1.0.

**Origin:**  
Synthesis of external compression and architecture feedback.

**Status:** OPEN

**Why it matters:**  
If true, the system could become dramatically smaller, more portable, and easier to implement while retaining its core research behavior.

**Evidence so far:**  
Multiple community contributors have independently suggested compression, modularization, or architectural separation while attempting to preserve the same research intent.

**What would support it:**  
Substantially different implementations consistently reproduce the strongest Research Pass behaviors.

**What would weaken it:**  
Behavior degrades significantly when detailed prose is removed, indicating that specific instructions are doing more work than expected.

**Test plan:**  
Compare canonical, compressed, modular, and agentic implementations against the same evaluation set.

**Related benchmark:**  
Full Alpha benchmark.

**Result:**  
Pending.

---

## H010 — Multi-agent decomposition may outperform single-context execution

**Hypothesis:**  
Research Pass cognitive roles may perform better when implemented as genuinely separate agents with isolated contexts, explicit handoffs, and adjudication rather than role-switching inside one model conversation.

**Origin:**  
External community architecture proposal.

**Status:** TESTING

**Why it matters:**  
Separate agents may improve independence, adversarial critique, context management, specialization, and error detection.

**Evidence so far:**  
An external contributor reports having already built a multi-agent implementation and begun testing it.

**What would support it:**  
Multi-agent Research Pass demonstrates better research quality, contradiction detection, source coverage, independent criticism, or synthesis than canonical v1.0 at acceptable cost.

**What would weaken it:**  
Agents duplicate work, share correlated errors, add cost and latency without improving conclusions, or create adjudication failures.

**Test plan:**  
Compare canonical single-context Research Pass against a multi-agent implementation on identical tasks.

Record agent roles, handoffs, token usage, latency, duplicate work, disagreements, and final result quality.

**Related benchmark:**  
Full Alpha benchmark plus difficult open-ended research cases.

**Result:**  
Pending external testing.

---

## H011 — Cross-vendor agents may reduce correlated model errors

**Hypothesis:**  
A multi-agent Research Pass using different model families may provide stronger triangulation than multiple agents using the same underlying model.

**Origin:**  
External community architecture proposal.

**Status:** OPEN

**Why it matters:**  
Multiple instances of one model may reproduce the same blind spots, training biases, or reasoning failures.

Independent model families may provide more genuinely independent criticism.

**Evidence so far:**  
Conceptual hypothesis only.

**What would support it:**  
Cross-vendor systems catch errors or alternative explanations that same-model multi-agent systems repeatedly miss.

**What would weaken it:**  
Cross-vendor disagreement mostly adds noise, or same-model diversity performs equally well at lower complexity.

**Test plan:**  
Compare:

- single-model single-agent
- single-model multi-agent
- cross-vendor multi-agent

using identical tasks and adjudication rules.

**Related benchmark:**  
Future multi-agent benchmark suite.

**Result:**  
Pending.

---

## H012 — Research doctrine and execution architecture should be separated

**Hypothesis:**  
Research Pass should be treated as a reusable research doctrine or specification whose execution can be implemented through multiple architectures rather than as one permanent mega-prompt.

**Origin:**  
Synthesis of several independent community contributions.

**Status:** OPEN

**Why it matters:**  
Separating doctrine from execution would allow the same underlying research standards to be implemented as:

- a prompt
- a modular skill
- an agent
- a multi-agent system
- a cross-vendor system
- a future tool or application

without confusing the methodology with one implementation.

**Evidence so far:**  
Multiple independent community contributors have converged on modular, agentic, or controller-based implementations.

**What would support it:**  
Different architectures successfully preserve the same core research behaviors and can be evaluated against a shared specification.

**What would weaken it:**  
The methodology proves too dependent on specific wording or implementation details to meaningfully separate doctrine from execution.

**Test plan:**  
Define candidate core invariants of the Research Pass and test whether multiple implementations reproduce them.

**Related benchmark:**  
Full benchmark suite.

**Result:**  
Pending.

---

## H013 — Modern model capabilities may make parts of explicit Research Pass scaffolding redundant

**Hypothesis:**  
Current frontier models may already perform some Research Pass behaviors natively, making certain explicit instructions unnecessary or even counterproductive.

**Origin:**  
External community criticism.

**Status:** OPEN

**Why it matters:**  
Research Pass should only retain instructions that create measurable value above the model's native behavior.

**Evidence so far:**  
Community members argue that modern models and agentic systems already perform stronger planning, tool use, reasoning, and self-critique than previous generations.

No controlled Research Pass comparison has yet established how much scaffolding remains necessary.

**What would support it:**  
Normal modern-model responses consistently match Research Pass performance on specific behaviors, and removing the corresponding instructions causes no regression.

**What would weaken it:**  
Research Pass continues to produce measurable improvements in those behaviors across modern frontier models.

**Test plan:**  
Run normal-vs-Research-Pass A/B tests and targeted instruction-ablation experiments on current frontier models.

**Related benchmark:**  
All benchmark cases.

**Result:**  
Pending.

---

## H014 — Research Pass value may depend on model generation and capability level

**Hypothesis:**  
The incremental benefit of Research Pass may be larger on weaker or older models and smaller, different, or even negative on stronger modern models.

**Origin:**  
External community criticism combined with cross-model discussion.

**Status:** OPEN

**Why it matters:**  
There may be no single optimal Research Pass implementation for every model generation.

Future versions may require model-capability-aware routing or lighter scaffolding for stronger systems.

**Evidence so far:**  
Conceptual community feedback only.

**What would support it:**  
Testing shows a clear relationship between underlying model capability and the amount/type of Research Pass scaffolding that improves performance.

**What would weaken it:**  
Research Pass produces similar relative improvements regardless of model capability.

**Test plan:**  
Compare multiple generations and capability levels using identical questions and Research Pass versions.

Measure:

- answer quality
- evidence quality
- hallucinations
- depth selection
- token use
- latency
- verbosity
- user usefulness

**Related benchmark:**  
Full benchmark suite.

**Result:**  
Pending.

---

# HYPOTHESIS LIFECYCLE

The intended flow is:

> OBSERVATION  
> → HYPOTHESIS  
> → TEST DESIGN  
> → EVIDENCE  
> → COUNTER-TEST  
> → SUPPORTED / WEAKENED / REJECTED / INCONCLUSIVE  
> → POSSIBLE CANONICAL CHANGE

A hypothesis should not become canonical merely because:

- it sounds convincing
- it came from an expert
- many people upvoted it
- an AI generated it
- one test appeared successful

The ledger exists to preserve ideas long enough to test them without prematurely turning them into Research Pass doctrine.
