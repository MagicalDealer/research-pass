Candidate A — Capability & Output Discipline

Status: EXPERIMENTAL CANDIDATE
Canonical status: NOT CANONICAL
Based on: Universal Research Pass v1.0 frozen public-alpha baseline

Purpose

Candidate A tests whether a small set of capability-honesty and output-discipline rules can improve reliability without changing the core Research Pass architecture.

This candidate intentionally preserves canonical v1.0 and adds only four experimental changes.

Experimental Changes

1. Capability Honesty

The model should only claim research steps it actually performed with the tools and access available.

It must not imply that it:

searched a source it did not search

inspected a source it could not access

followed a citation chain it did not follow

checked corrections, retractions, or superseding versions when it could not

performed multilingual research when it did not

reproduced a technical test when it did not

If a consequential check could not be completed, the model should state the limitation, explain whether it could affect the conclusion, and give the best next verification step.

2. Working Process ≠ Visible Answer

Internal research machinery should not automatically appear in the final response.

Hypothesis maps, evidence tables, source-role labels, search lanes, and other scaffolding should stay in the working process unless they materially improve understanding or auditability.

3. Completion State

A Research Pass may end as:

READY

PARTIAL

INSUFFICIENT EVIDENCE

This is intended to reduce pressure to manufacture a complete-sounding answer when research access or evidence is incomplete.

4. Evidence Confidence ≠ Decision Readiness

The candidate explicitly separates:

How strongly does the evidence support this conclusion?

from:

Is there enough information to reasonably act?

A reversible, low-cost action may be reasonable on incomplete evidence.

A high-cost, irreversible action may remain unready even when the leading explanation is strongly supported.

Related Hypotheses

This candidate primarily tests:

H003 — Research structure may amplify hallucination when real research capability is absent

H013 — Modern model capabilities may make parts of explicit Research Pass scaffolding redundant

H014 — Research Pass value may depend on model generation and capability level

It may also provide evidence relevant to:

H001 — Over-research on simple questions

H009 — Research Pass value may come primarily from doctrine rather than prose volume

H012 — Research doctrine and execution architecture should be separated

What We Want to Learn

Does capability honesty reduce unsupported research claims?

Does it make tool-limited results more trustworthy?

Does hiding unnecessary research machinery make answers clearer without reducing rigor?

Do READY / PARTIAL / INSUFFICIENT EVIDENCE states improve calibration?

Do those states become unnecessary ceremony on simple questions?

Does separating confidence from decision readiness improve practical recommendations?

Does Candidate A introduce any regressions compared with canonical v1.0?

Does the effect differ across models and tool environments?

How to Test

Use the same research question and the same model in separate fresh conversations.

A — Canonical Baseline

Run frozen Universal Research Pass v1.0.

B — Candidate A

Run:

experiments/candidate-a-capability-output/RESEARCH_PASS.md

Compare:

factual accuracy

source quality

unsupported claims about research steps

clarity

verbosity

uncertainty calibration

usefulness

decision readiness

token usage when available

any regressions

Whenever possible, preserve the raw outputs.

Promotion Rule

Candidate A should not enter the canonical Research Pass merely because the additions sound sensible.

A future canonical change should be supported by repeatable evidence showing that the change improves the motivating cases without creating meaningful regressions elsewhere.

Current Result

Pending testing.
