RESEARCH PASS ALPHA BENCHMARK

Benchmark version: Alpha 0.1
Cases: 10
Status: EXPERIMENTAL

These cases are deliberately diverse. The goal is not to produce one numerical score yet.

For each case, record whether the Research Pass displayed the expected research behavior and note any important failures.

RP-B001 — RESEARCH TRIAGE / OVER-RESEARCH

Capability

Choose an appropriate research depth instead of turning every question into a full investigation.

Prompt

Research Pass this: What is the boiling point of pure water at sea level?

Expected Behaviors

A strong result should:

recognize this as a simple factual question

use Quick Check or an equivalently lightweight approach

answer directly

mention the standard-pressure condition

avoid unnecessary cross-disciplinary research or huge reports

Failure Signals

launches a Full Research Pass

generates unnecessary rival hypotheses

produces a long literature review

fails to note that boiling point depends on pressure

RP-B002 — FALSE PREMISE DETECTION

Capability

Challenge a faulty premise instead of confidently researching inside it.

Prompt

Research Pass this: Why did NASA stop exploring the ocean before switching its focus to space?

Expected Behaviors

A strong result should:

investigate whether the premise is true

identify that the common claim is misleading or false

distinguish NASA's actual mission/history from oceanographic agencies and research

explain why the myth may persist if evidence supports an explanation

avoid inventing a nonexistent historical decision

Failure Signals

accepts the premise without checking it

invents reasons NASA supposedly abandoned ocean exploration

treats internet repetition as historical evidence

RP-B003 — SOURCE LINEAGE / FAKE CONSENSUS

Capability

Trace a popular claim rather than treating repetition as independent confirmation.

Prompt

Research Pass this: I keep hearing that humans only use 10% of their brains. Is that true, and where did the claim come from?

Expected Behaviors

A strong result should:

distinguish the truth of the claim from its cultural history

look for original or early sources where possible

avoid treating many websites repeating the myth as independent evidence

explain what neuroscience actually supports

acknowledge uncertainty around the exact origin if the lineage is disputed

Failure Signals

cites many derivative articles as separate confirmation

invents a precise origin without evidence

answers only "the myth is false" without investigating lineage

RP-B004 — COMPETING SCIENTIFIC EXPLANATIONS

Capability

Handle mixed evidence and distinguish correlation, mechanism, and context.

Prompt

Research Pass this: Does drinking coffee increase or decrease the risk of heart disease?

Expected Behaviors

A strong result should:

avoid a simplistic yes/no answer

distinguish observational evidence from stronger causal claims

consider dose, preparation method, population differences, and confounding where relevant

investigate credible counter-evidence

communicate what appears relatively well supported versus uncertain

use appropriately strong health sources

Failure Signals

claims coffee definitively causes or prevents heart disease

cherry-picks one study

ignores dose or context

gives individualized medical advice without adequate basis

RP-B005 — HISTORICAL MULTICAUSALITY

Capability

Compare multiple plausible explanations without forcing one simplistic cause.

Prompt

Research Pass this: What caused the collapse of the Western Roman Empire?

Expected Behaviors

A strong result should:

clarify what "collapse" and relevant dates mean

identify several major explanatory traditions

distinguish long-term structural factors from proximate events

investigate disagreements among historians

avoid presenting one popular explanation as universally accepted

synthesize interactions among causes where justified

Failure Signals

gives one-cause explanation

presents contested interpretations as settled fact

ignores definitional or periodization issues

produces a list of causes without explaining relationships among them

RP-B006 — VOCABULARY DISCOVERY / CROSS-DISCIPLINARY SEARCH

Capability

Translate a messy observation into expert terminology and relevant research fields.

Prompt

Research Pass this: Why do I keep checking apps even when I know there probably isn't anything new there?

Expected Behaviors

A strong result should:

translate the observation into relevant concepts rather than relying only on the user's wording

consider multiple mechanisms such as habit formation, reinforcement, cues, uncertainty, or checking behavior

distinguish plausible mechanisms instead of diagnosing the user

search across relevant behavioral or design disciplines

explain which mechanisms appear best supported and under what conditions

Failure Signals

gives generic "phone addiction" advice only

diagnoses a clinical condition without basis

fails to discover more precise terminology

settles on one explanation without alternatives

RP-B007 — USER CONTEXT / DECISION SUPPORT

Capability

Recognize when a personalized recommendation cannot be responsibly made without user-specific information.

Prompt

Research Pass this: Is it cheaper over five years for me to buy a used hybrid or keep my current paid-off gasoline car?

Expected Behaviors

A strong result should:

identify the missing variables that materially affect the answer

request or clearly enumerate needed information such as mileage, fuel economy, fuel prices, maintenance, purchase price, financing, insurance, and expected repairs

distinguish general principles from a personalized conclusion

avoid pretending a precise answer is possible without the missing context

offer a calculation framework if enough data are not yet available

Failure Signals

recommends one option without obtaining necessary context

ignores transaction costs or depreciation

produces fake precision from assumed numbers without clearly labeling assumptions

RP-B008 — CONFIRMATION-BIAS PRESSURE TEST

Capability

Resist the user's preferred explanation and seriously test alternatives.

Prompt

Research Pass this: I think remote work makes employees less productive. Find out if I'm right.

Expected Behaviors

A strong result should:

freeze or acknowledge the user's starting belief

generate credible competing hypotheses

distinguish productivity measures and job types

investigate evidence supporting and contradicting the claim

consider selection effects, management practices, task type, and measurement differences

avoid framing the research as a mission to prove the user right

Failure Signals

searches only for evidence that remote work reduces productivity

treats all work as one population

hides contradictory findings

turns mixed evidence into an unjustified universal conclusion

RP-B009 — TECHNICAL DIAGNOSIS / DISCRIMINATING TESTS

Capability

Generate competing explanations and propose tests that distinguish them.

Prompt

Research Pass this: My internet speed is good near my router, but video calls freeze in one room. What is most likely happening, and how can I tell which cause is responsible?

Expected Behaviors

A strong result should:

identify multiple plausible causes

distinguish internet-service speed from local Wi-Fi performance

propose practical discriminating tests

prioritize likely explanations based on the described pattern

explain what evidence would support or weaken each explanation

avoid jumping immediately to buying new equipment

Failure Signals

assumes the ISP is the problem

recommends a product before diagnosis

gives a generic troubleshooting checklist with no reasoning

fails to distinguish competing causes

RP-B010 — CURRENT-STATE / DECISION SUFFICIENCY

Capability

Research a changing technology question using current evidence and conditional conclusions.

Prompt

Research Pass this: Are passkeys ready to replace passwords for most consumers?

Expected Behaviors

A strong result should:

recognize that the answer depends on current ecosystem support

verify recent platform and service adoption

distinguish security advantages from migration, recovery, compatibility, and usability limitations

define what "ready to replace" means

identify where passkeys are mature and where passwords remain necessary

produce a conditional conclusion rather than a hype-driven yes/no answer

Failure Signals

relies on outdated adoption information

treats technical security superiority as equivalent to universal practical readiness

ignores account recovery or interoperability

makes a timeless claim about a fast-changing ecosystem

ALPHA BENCHMARK REPORTING

For each case, record:

Case ID

Research Pass version

AI provider

Model

Date

Web/search available

Result: Strong / Acceptable / Mixed / Weak / Failed

Expected behaviors observed

Failure signals observed

Important unexpected behavior

Notes

Do not combine these results into a universal score yet.

The alpha benchmark exists to reveal where a future scoring system would actually be useful.
