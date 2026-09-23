# CONTRIBUTING TO THE UNIVERSAL RESEARCH PASS

Thank you for helping test, challenge, and improve the Universal Research Pass.

This project is not trying to collect the most edits.

It is trying to discover which changes actually make AI-assisted research more reliable.

---

# 1. START HERE

Before proposing a change:

1. read [`RESEARCH_PASS.md`](./RESEARCH_PASS.md)
2. read [`TESTING_PROTOCOL.md`](./TESTING_PROTOCOL.md)
3. test the canonical version first
4. identify a specific behavior, failure, or limitation
5. gather enough evidence to explain why the change may be needed

The canonical Research Pass is the baseline.

Do not assume a rewrite is better merely because it is shorter, longer, cleaner, or more sophisticated.

---

# 2. WAYS TO CONTRIBUTE

You can contribute by:

- reporting a failure
- reporting an unexpected success
- testing the Research Pass in a new domain
- comparing models
- testing novice usability
- testing expert-level research quality
- identifying unnecessary instructions
- finding contradictory instructions
- proposing a targeted improvement
- creating a specialized fork
- contributing benchmark cases
- reproducing another person's finding
- showing that a proposed improvement causes a regression

You do not need to be a developer.

Real-world testing is one of the most valuable forms of contribution.

---

# 3. DISCUSSIONS VS. ISSUES VS. PULL REQUESTS

Use **Discussions** for:

- early ideas
- questions
- observations
- broad feedback
- test stories
- possible forks
- uncertain problems
- brainstorming

Use **Issues** for:

- reproducible failures
- clearly defined weaknesses
- specific improvement proposals
- benchmark candidates
- bugs in project documentation

Use a **Pull Request** when:

- you are proposing an exact text change
- you can explain the problem the change addresses
- you have test evidence
- you have checked for regressions

Do not open a Pull Request merely because you prefer different wording.

---

# 4. REPORTING A FAILURE

A useful failure report should include:

- Research Pass version
- AI provider and model
- exact research question
- whether web/search was available
- what you expected
- what actually happened
- why the behavior matters
- whether the failure is reproducible
- any comparison against a normal AI answer
- any suspected cause
- any proposed fix, if you have one

If possible, attach or link the relevant outputs.

A reproducible failure is extremely valuable.

---

# 5. PROPOSING AN IMPROVEMENT

Before proposing a canonical change, answer:

## What problem exists?

Describe the specific behavior you are trying to improve.

## What evidence shows that this is a real problem?

Examples:

- repeated independent failures
- a strong expert critique
- cross-model behavior
- benchmark failure
- comparison against the current baseline

## What exactly are you changing?

Keep the change as narrow as practical.

## Why should this change help?

Explain the mechanism.

## What did you test?

List:

- questions tested
- models tested
- domains tested
- baseline behavior
- modified behavior

## What got better?

Be specific.

## What got worse?

Report regressions honestly.

## What remains uncertain?

A good proposal is allowed to be provisional.

---

# 6. MINIMAL CHANGE PRINCIPLE

Prefer the smallest change that fixes the identified problem.

If one sentence solves the problem, do not rewrite five sections.

Large rewrites make it harder to know which change caused the improvement or regression.

---

# 7. REGRESSION CHECK

Before recommending a canonical change:

1. rerun the original failure case
2. test at least one unrelated question
3. test a simple question
4. test a more complex question
5. look for new failure modes

A change that fixes one case but damages several others is not necessarily an improvement.

---

# 8. CROSS-MODEL CONTRIBUTIONS

If testing across models, report:

- provider
- model
- tool/search availability
- relevant settings
- same exact research question
- same Research Pass version

Do not assume model-specific behavior is caused by the Research Pass.

Model differences are part of what this project is trying to understand.

---

# 9. SPECIALIZED FORKS

Forks are encouraged.

Examples might include:

- Academic Research Pass
- Journalism Research Pass
- Technical Research Pass
- Lightweight Research Pass
- Education Research Pass
- Model-specific versions

Please clearly identify a fork as a fork.

Do not present a modified version as the canonical Universal Research Pass.

If a fork discovers something broadly useful, bring the finding back to the main project as evidence.

---

# 10. CANONICAL CHANGE STANDARD

A proposed change should not enter the canonical Research Pass because:

- it sounds smarter
- it is more elegant
- it is more detailed
- it is more concise
- many people like it

A canonical change should earn its way in through evidence.

The project should be able to explain:

- what problem existed
- what changed
- why it changed
- what testing supported the change
- what regressions were checked
- what remains uncertain

---

# 11. BENCHMARK CONTRIBUTIONS

A strong benchmark case should represent a meaningful research challenge.

Good benchmark candidates include:

- false-premise detection
- source conflict
- fake consensus
- historical uncertainty
- causal ambiguity
- obscure terminology
- cross-disciplinary translation
- current information
- high uncertainty
- over-research risk
- under-research risk
- expert-level omission
- user-context failure

A benchmark should test a real capability, not merely trivia recall.

---

# 12. EVIDENCE STANDARD

Useful evidence can include:

- reproduced failures
- A/B comparisons
- expert critique
- model comparisons
- source-quality analysis
- repeated independent observations
- benchmark results
- regression tests

Weak evidence can still inspire investigation.

But inspiration and confirmation are not the same thing.

---

# 13. AI-GENERATED CONTRIBUTIONS

Using AI to help analyze, write, test, or propose changes is allowed.

However:

- do not submit an AI-generated rewrite without understanding it
- do not treat AI confidence as evidence
- verify claims used to justify a change
- test the proposed change against the baseline
- remain responsible for the contribution you submit

The project evaluates behavior and evidence, not who typed the text.

---

# 14. KEEP FEEDBACK SPECIFIC

Helpful:

> On three historical research questions, the system treated practitioner knowledge as relevant even when there was no meaningful practitioner population. Here are the runs.

Less helpful:

> This section feels unnecessary.

Helpful:

> This new wording fixed false-premise detection on two benchmark cases but caused over-research on three simple factual questions.

Less helpful:

> My version is better.

Specific feedback can be tested.

---

# 15. DISAGREEMENT IS USEFUL

Contributors are encouraged to disagree.

Do not force consensus.

If two approaches produce different outcomes, identify:

- what each optimizes for
- where each works
- where each fails
- what evidence would distinguish them

The project should preserve meaningful disagreement when the evidence does not justify a single conclusion.

---

# 16. PROJECT VALUES

This project values:

- curiosity
- reproducibility
- intellectual honesty
- useful disagreement
- evidence over popularity
- clear uncertainty
- transparency about failure
- practical usefulness
- willingness to revise

The Research Pass itself is not protected from criticism.

---

# 17. CONTRIBUTION FLOW

A typical contribution should move through:

> OBSERVATION  
> → DISCUSSION  
> → REPRODUCIBLE PROBLEM  
> → ISSUE  
> → PROPOSED CHANGE  
> → TESTING  
> → REGRESSION CHECK  
> → REVIEW  
> → MERGE / REJECT / KEEP EXPERIMENTAL

Not every good idea needs to become canonical.

---

# 18. FINAL CONTRIBUTION PRINCIPLE

> The goal is not to make the Research Pass larger.

> The goal is to make it more reliable, more transferable, and more useful.
