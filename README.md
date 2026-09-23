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

Please test the canonical version first before modifying it.

That gives the community a real baseline.

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

Ideas are welcome.

Evidence is better.

Canonical vs. Forks

You are encouraged to modify, remix, specialize, shorten, or rebuild the Research Pass.

Examples might eventually include:

Academic Research Pass

Journalism Research Pass

Technical Research Pass

Lightweight Research Pass

Model-specific versions

But there will remain one clearly identified:

Universal Research Pass — Canonical

A change should enter the canonical version because testing shows that it improves the system — not merely because the wording sounds better.

Core Principle

Research does not finish when we have collected information.

It finishes when outside knowledge has collided with the question hard enough to teach us something we did not know before.

Contributing

Contribution guidelines, structured testing instructions, failure-report templates, and the public benchmark are being added during the alpha.

For now, use Discussions to share:

test results

failure cases

questions

proposed changes

forks

observations

The most valuable feedback is specific enough that someone else could reproduce the problem.

Project Roadmap

The early project will focus on:

small-scale alpha testing

structured community test reports

collecting real failure cases

creating a public benchmark from those failures

cross-model testing

regression testing proposed changes

evidence-based version releases

The goal is not to make the longest or most complicated research prompt.

The goal is to make the most reliable research process we can collectively build.
