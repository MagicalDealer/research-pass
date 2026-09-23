Brian Modular-Control Research Pass

Contributor: Brian_from_accounts
Status: EXPERIMENTAL COMMUNITY CANDIDATE
Canonical status: NOT CANONICAL
Based on: Universal Research Pass v1.0

Origin

Submitted through community testing as a substantial redesign of the Universal Research Pass.

The contributor explicitly gave permission for the proposal to be preserved as an experimental fork.

Core Architectural Changes

This candidate introduces:

a control layer

selective research modules

smallest-sufficient-depth routing

capability honesty

Ready / Partial / Insufficient Evidence completion states

question-type routing

stronger separation between working research machinery and visible output

evidence confidence separated from decision readiness

record-retrieval / absence protocol

explicit execution checks

self-testing rules

Why We Are Preserving It

This proposal overlaps with several independently emerging community hypotheses that the Research Pass may benefit from:

modular execution

reduced over-research

doctrine / execution separation

model-aware capability handling

reduced performative complexity

The purpose of preserving this candidate is not to endorse it as the next canonical version.

It is to create a stable experimental artifact that can be tested directly against frozen canonical v1.0.

Related Hypotheses

H001 — Over-research on simple questions

H004 — Modular skill architecture may reduce Research Pass overhead

H009 — Research Pass value may come primarily from doctrine rather than prose volume

H012 — Research doctrine and execution architecture should be separated

H013 — Modern model capabilities may make parts of explicit Research Pass scaffolding redundant

H014 — Research Pass value may depend on model generation and capability level

Main Questions to Test

Does its routing reduce over-research?

Does “smallest sufficient” ever cause premature stopping?

Does it correctly handle questions spanning multiple types?

Does it preserve unknown-unknown discovery?

Does it improve capability honesty?

Does it reduce visible complexity?

Does it reduce token or tool cost?

Does anything important from canonical v1.0 disappear?

Does performance hold across model families?

Does conditional execution create routing failures that canonical v1.0 avoids?

Testing Standard

This candidate should be compared against frozen canonical v1.0 using:

the existing Alpha benchmark

real community research questions

cross-model testing

token / latency measurement where possible

regression testing

failure analysis

source-quality checks

user-usefulness comparison

No result from this candidate becomes canonical merely because the redesign appears cleaner, shorter, more sophisticated, or more efficient.

A future canonical change should be supported by reproducible evidence and should survive regression testing.

Preservation Rule

The contributor's original proposal should remain preserved unchanged inside this experiment folder.

Project interpretation, test notes, results, and eventual conclusions should be added around the artifact rather than silently rewriting the submitted version.

Current Result

Pending testing.
