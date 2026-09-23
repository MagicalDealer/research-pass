# RESEARCH PASS TESTING PROTOCOL

**Version:** 1.0  
**Applies to:** Universal Research Pass v1.0 Public Alpha

---

# 1. PURPOSE

This protocol exists so community feedback can become useful evidence instead of random opinions.

The goal is not to prove that the Research Pass is good.

The goal is to discover:

- where it improves research
- where it fails
- where it wastes effort
- where it misunderstands the user
- where it produces better evidence
- where it produces worse evidence
- where it behaves differently across topics or models
- whether proposed changes actually improve the system

---

# 2. MOST IMPORTANT RULE

> **TEST THE CANONICAL VERSION FIRST. MODIFY SECOND.**

Do not rewrite the Research Pass before your first test.

If you change the system before testing the official version, we lose the baseline and cannot tell whether your modification actually improved anything.

---

# 3. BASIC A/B TEST

For the most useful comparison, use two fresh conversations.

Use the same AI model and, as much as practical, the same settings.

## CHAT A — NORMAL AI

Ask your question normally.

Example:

> Why do people seem to remember negative experiences more strongly than positive ones?

## CHAT B — RESEARCH PASS

Load the canonical Research Pass.

Then ask:

> Research Pass this: Why do people seem to remember negative experiences more strongly than positive ones?

Do not intentionally make one version easier than the other.

Use the same underlying question.

---

# 4. WHAT TO COMPARE

After both runs, compare them.

Ask:

- Which answer found stronger evidence?
- Which answer found more relevant evidence?
- Did either answer challenge a false assumption?
- Did the Research Pass discover competing explanations?
- Did it search outside the obvious field?
- Did it distinguish evidence from interpretation?
- Did it handle uncertainty honestly?
- Did it trace important claims to stronger sources?
- Did it identify contradictions?
- Did it explain why sources disagreed?
- Did it discover useful terminology?
- Did it improve the final conclusion?
- Did it produce a better decision or next step?
- Did it research unnecessary things?
- Was it too long?
- Was it too slow?
- Did it overcomplicate a simple question?
- Did it miss an obvious source or mechanism?
- Did it hallucinate?
- Did it use weak evidence as though it were strong?
- Did it change the original question in a useful way?
- Did it change the original question in an unhelpful way?

Do not judge only by which answer is longer or sounds more intelligent.

Judge whether it produced **better understanding**.

---

# 5. TEST REPORT

Please include the following information when reporting a test.

## Test Metadata

- Research Pass version:
- AI provider:
- Model:
- Date:
- Web/search available: Yes / No / Unknown
- Files or connected data used: Yes / No
- Research depth chosen by the system: Quick / Targeted / Full / Unknown
- Your familiarity with the topic: Beginner / Intermediate / Expert

## Research Question

Paste the exact question used.

## Baseline Result

Briefly describe how the normal AI answer performed.

## Research Pass Result

Briefly describe how the Research Pass answer performed.

## What Improved

What did the Research Pass do better?

## What Got Worse

What did the Research Pass do worse?

## Failure or Strange Behavior

Describe anything incorrect, wasteful, confusing, misleading, repetitive, or unexpected.

## Best Part

What part of the process created the most value?

## Weakest Part

What part created the least value?

## Overall Result

Choose one:

- Research Pass clearly better
- Research Pass somewhat better
- Roughly equal
- Research Pass somewhat worse
- Research Pass clearly worse
- Mixed / difficult to compare

## Why?

Explain your judgment briefly.

---

# 6. FAILURE REPORTS ARE HIGH VALUE

A failure is not bad news for the project.

A reproducible failure is one of the most useful contributions you can make.

Especially valuable failures include:

- accepted a false premise
- hallucinated a source or fact
- failed to verify an important claim
- over-researched a simple question
- under-researched a difficult question
- ignored strong counter-evidence
- confused correlation with causation
- treated repeated claims as independent confirmation
- misunderstood the user's real objective
- searched the wrong discipline
- stopped too early
- failed to stop
- produced an answer that looked rigorous but was not
- behaved poorly on one model but well on another
- became much worse after a proposed modification

Please report these.

---

# 7. MODIFICATION TESTING

After you have tested the canonical version, you are encouraged to modify it.

When testing a modification:

1. identify the specific problem you are trying to solve
2. change as little as necessary
3. rerun the same research question
4. compare against the canonical version
5. test at least one unrelated question
6. look for regressions

A change is not automatically better because it improves one test.

It may fix one problem while damaging another.

---

# 8. CROSS-MODEL TESTING

Cross-model tests are especially useful.

If possible, run the same Research Pass version and same research question across different models.

Record:

- provider
- model
- settings if relevant
- tool/search availability
- meaningful behavior differences

Do not assume a failure belongs to the Research Pass if it may be specific to one model.

Likewise, do not assume success on one model proves the protocol works equally well elsewhere.

---

# 9. GOOD TEST QUESTIONS

Good tests include:

- questions you genuinely care about
- obscure questions
- questions with multiple plausible explanations
- topics where you already hold a strong belief
- controversial claims
- historical disputes
- technical problems
- scientific mechanisms
- consumer decisions
- messy real-world decisions
- questions with incomplete evidence
- questions built on a false assumption
- questions where popular sources repeat the same claim

Avoid testing only trivia.

The Research Pass is primarily designed for problems where **investigation matters**.

---

# 10. NOVICE TESTING

You do not need to be an AI expert.

In fact, novice users are especially valuable.

Use the system naturally.

Do not try to rescue it when it behaves badly.

If the instructions are confusing, that is itself useful feedback.

---

# 11. EXPERT TESTING

If you are knowledgeable in the topic being researched, please pay special attention to:

- missing primary sources
- incorrect terminology
- weak source selection
- false equivalence
- outdated evidence
- hidden assumptions
- overconfident synthesis
- misunderstood disciplinary debates
- important omitted mechanisms

Expert criticism is extremely valuable when it is specific and reproducible.

---

# 12. WHAT DOES NOT COUNT AS STRONG EVIDENCE

The following can inspire further testing, but should not by themselves justify changing the canonical system:

- “This feels better.”
- “I like this wording more.”
- “This answer was longer.”
- “This answer sounded smarter.”
- one successful run
- one failed run
- many people repeating the same criticism without independent testing
- a modification that was never compared against the baseline

Opinions generate hypotheses.

Tests generate evidence.

---

# 13. COMMUNITY STANDARD

Be willing to report:

- success
- failure
- uncertainty
- mixed results

Do not protect the Research Pass.

Do not try to prove that it works.

Try to discover what it actually does.

---

# 14. FINAL TESTING PRINCIPLE

> A proposed improvement should earn its way into the canonical Research Pass by surviving comparison, counterexamples, and regression testing.

The goal is not to make the prompt bigger.

The goal is to make the research process better.
