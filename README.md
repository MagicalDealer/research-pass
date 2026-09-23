Universal Research Pass

An open, community-tested protocol for rigorous AI-assisted research.

The Research Pass is a structured way to make an AI investigate a question instead of simply answering it.

You can give it a question, theory, decision, claim, observation, or even a messy thought. The system then helps the AI:

identify what actually needs to be researched

search beyond the user's original wording

generate competing explanations

distinguish discovery from proof

verify important claims

trace where popular claims came from

look for contradictions and failure cases

compare independent evidence

calibrate confidence

explain what is still unknown

translate the research into a useful conclusion, decision, or next test

The goal is not to collect the most information.

The goal is:

maximum useful understanding

Quick Start

Open RESEARCH_PASS.md.

Give the Research Pass to your AI assistant.

Then say:

Research Pass this: [whatever you want to understand]

Examples:

Research Pass this: Why do people seem to remember negative experiences more strongly than positive ones?

Research Pass this: Is buying an EV actually cheaper for me over five years?

Research Pass this: How strong is the historical evidence for this claim?

Research Pass this: I think this strategy is failing because of X. Find out whether I'm right.

You do not need to write a sophisticated research prompt.

You bring the question.

The Research Pass builds the investigation.

Why This Exists

Most AI research workflows are still variations of:

search → summarize → answer

The Research Pass is designed to do more.

It treats research as an evolving investigation. It can challenge the starting belief, discover better terminology, compare rival explanations, investigate contradictions, search across disciplines, and stop only when the remaining uncertainty is understood well enough to act.

It is closer to a research protocol implemented through an AI than a normal prompt.

Current Status

Version: 1.0
Status: Public Alpha — Canonical Baseline

Version 1.0 is intentionally frozen as the first public baseline.

The purpose of this repository is to find out:

where the system works

where it fails

where it wastes effort

where it produces better research than a normal AI conversation

which parts are unnecessary

which parts need stronger instructions

how well it transfers across topics and AI models

whether community modifications genuinely improve it

whether the current monolithic prompt should eventually become a modular skill, agent system, or other architecture

The Research Pass should not be protected from criticism.

We want people to break it.

How to Test It

For the most useful test:

A — Normal AI

Ask your research question normally in a fresh conversation.

B — Research Pass

Open another fresh conversation using the same model and ask:

Research Pass this: [the exact same question]

Then compare the results.

Useful questions include:

Did the Research Pass uncover explanations the normal answer missed?

Did it find stronger or more relevant evidence?

Did it challenge assumptions?

Did it handle uncertainty better?

Did it research things that did not matter?

Was it unnecessarily long?

Did it misunderstand the question?

Did it hallucinate or misuse sources?

Did it change the question in a productive way?

Did it materially improve the conclusion?

Did it add enough value to justify its token, time, and tool cost?

Please test the canonical version first before modifying it.

That gives the community a real baseline.

For the full testing method, see TESTING_PROTOCOL.md.

For a quick tester walkthrough, see TESTER_GUIDE.md.

Community Research Lab

This repository is meant to evolve through real-world testing.

Good contributions include:

failure cases

unexpected successes

edge cases

cross-model comparisons

domain-specific tests

proposed improvements

simplified versions

specialized forks

evidence that a current rule is unnecessary

evidence that a proposed change causes regressions

architectural alternatives such as modular, skill-based, or multi-agent implementations

Ideas are welcome.

Evidence is better.

Experimental Hypotheses

Community feedback is already generating testable ideas about how the Research Pass may need to evolve.

These are tracked in:

EXPERIMENTAL_HYPOTHESES.md

Examples currently being tested include:

whether Research Pass over-researches simple questions

whether its strongest value appears on messy or poorly framed questions

whether research scaffolding can amplify hallucination when real research tools are unavailable

whether modular or skill-based implementations can preserve quality at lower token cost

whether performance changes materially across model families

whether a shared glossary improves consistency

whether redundant instructions can be safely removed

whether multi-agent or cross-vendor systems outperform single-context execution

whether modern frontier models make some explicit scaffolding unnecessary

whether Research Pass doctrine should be separated from its execution architecture

Nothing in the hypothesis ledger is canonical merely because it is listed.

The intended lifecycle is:

Observation → Hypothesis → Test → Counter-test → Supported / Weakened / Rejected / Inconclusive → Possible canonical change

Canonical vs. Forks

You are encouraged to modify, remix, specialize, shorten, or rebuild the Research Pass.

Examples might eventually include:

Academic Research Pass

Journalism Research Pass

Technical Research Pass

Lightweight Research Pass

Model-specific versions

Modular skill implementations

Multi-agent implementations

Cross-vendor implementations

But there will remain one clearly identified:

Universal Research Pass — Canonical

A change should enter the canonical version because testing shows that it improves the system — not merely because the wording sounds better.

Benchmark

The project includes an early experimental benchmark in benchmark/.

The current alpha benchmark is designed to stress-test behaviors such as:

research-depth selection

false-premise detection

source lineage

competing scientific explanations

historical multicausality

vocabulary discovery

user-context gathering

confirmation-bias resistance

technical diagnosis

current-state research

The benchmark is not a scientific leaderboard.

It is an evolving regression set that should increasingly be built from real community failures.

Core Principle

Research does not finish when we have collected information.

It finishes when outside knowledge has collided with the question hard enough to teach us something we did not know before.

Contributing

The project now includes:

CONTRIBUTING.md — contribution rules

TESTING_PROTOCOL.md — structured testing method

TESTER_GUIDE.md — quick-start testing guide

EXPERIMENTAL_HYPOTHESES.md — testable community hypotheses

CHANGELOG.md — canonical version history

benchmark/ — experimental regression tests

structured GitHub Failure Report and Improvement Proposal issue forms

GitHub Discussions for test results, failure cases, ideas, questions, and forks

The most valuable feedback is specific enough that someone else could reproduce the problem.

A typical contribution should move through:

Observation → Discussion → Reproducible Problem → Hypothesis or Issue → Test → Regression Check → Review → Merge / Reject / Keep Experimental

Project Roadmap

The early project will focus on:

collecting real-world A/B tests

expanding cross-model testing

reproducing community-reported failures

testing token and latency costs

comparing canonical v1.0 against compressed, modular, and agentic alternatives

growing the benchmark from real failure cases

testing which instructions are genuinely necessary

separating model-specific behavior from Research Pass behavior

evidence-based version releases

The goal is not to make the longest or most complicated research prompt.

The goal is to make the most reliable, efficient, and transferable research process we can collectively build.
