RESEARCH PASS BENCHMARK

This folder contains standardized research challenges used to test the Universal Research Pass across versions, models, and domains.

Status

Alpha benchmark — not yet validated.

These cases are intended to expose useful failures and regressions during early community testing.

They are not a scientific leaderboard and should not be treated as one.

Purpose

The benchmark exists to answer questions such as:

Does a new Research Pass version fix the problem it was meant to fix?

Does it accidentally make unrelated research worse?

Does behavior change across AI models?

Does the system choose an appropriate research depth?

Does it challenge false premises?

Does it distinguish uncertainty from confidence?

Does it gather needed user context before making personalized recommendations?

Does it investigate competing explanations instead of confirming the user's preferred theory?

How to Use

For each case:

use the exact benchmark prompt

record the Research Pass version

record the AI provider and model

record whether web/search was available

run the test in a fresh conversation when practical

compare behavior against the case's expected behaviors

record notable successes and failures

do not silently rewrite the benchmark prompt

For regression testing, compare the current canonical Research Pass against the proposed modified version using the same case.

Important

A benchmark case should test a capability, not merely factual recall.

Future cases should primarily come from:

real community failures

repeated weaknesses

important edge cases

cross-model disagreements

regressions caused by proposed changes

The benchmark should evolve because testing teaches us what actually needs to be measured.
