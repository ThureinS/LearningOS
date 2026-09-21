# LearningOS Research Notes

# Mastery Rubric v0.1

## Purpose

Mastery in LearningOS is based on demonstrated ability, not course completion, time spent, or self-confidence alone.

A learner may understand a lesson immediately but still be unable to:

- recall it later
- apply it independently
- debug related problems
- adapt it to a changed situation
- use it naturally inside a real project

Therefore mastery must be inferred from evidence.

---

## Evidence Dimensions

A skill may be evaluated across six dimensions.

### 1. Explain

Can I explain the concept in my own words without being shown the answer?

Useful evidence includes:

- describing how or why something works
- explaining an important distinction
- explaining why a solution is correct
- explaining why an earlier attempt failed

---

### 2. Read / Trace

Can I understand existing code and reason about its behavior?

Useful evidence includes:

- predicting output
- tracing execution
- identifying data/state changes
- explaining unfamiliar code
- identifying assumptions or edge cases

---

### 3. Build / Apply

Can I use the skill independently?

Useful evidence includes:

- implementing from a blank starting point
- applying the concept inside a feature
- selecting an appropriate approach
- completing a familiar but not memorized task

---

### 4. Debug

Can I diagnose and repair problems systematically?

Useful evidence includes:

- reproducing the issue
- forming useful hypotheses
- inspecting evidence
- locating the root cause
- fixing the problem
- explaining why the fix works

Random changes until the program works are weaker evidence.

---

### 5. Adapt / Transfer

Can I use the skill when the situation changes?

Useful evidence includes:

- solving a variant problem
- applying the concept in a different context
- choosing the relevant technique without being told
- combining the skill with other skills
- using it inside a realistic project

Success only on an almost identical practiced example is weak transfer evidence.

---

### 6. Retain

Can I still perform after meaningful time has passed?

Strong retention evidence includes:

- delayed independent recall
- delayed implementation
- delayed debugging
- successful performance on a fresh variant
- natural successful use inside a project

Immediate success after studying is not enough to establish retention.

---

# Canonical Skill States

## Untested

There is not enough meaningful evidence yet.

Untested does not mean weak.

---

## Learning

The skill is currently being acquired.

Typical evidence:

- understanding is incomplete
- substantial help may still be required
- errors or misconceptions are still being corrected

---

## Working

The learner can perform some meaningful tasks, but evidence is incomplete or performance remains fragile.

Typical evidence:

- familiar tasks can be completed
- some dimensions are stronger than others
- occasional help may still be required
- transfer or delayed performance may not yet be demonstrated

---

## Solid-now

Current evidence shows strong independent performance on the relevant dimensions.

However, sufficient delayed evidence does not yet exist.

Solid-now means:

**strong current capability**

not:

**durably retained forever**

---

## Retained

The learner demonstrates suitable independent performance after meaningful delay.

Where relevant, evidence should include:

- no solution exposure
- low or no instructional assistance
- fresh or changed tasks
- successful transfer
- realistic project use

Retained is the strongest normal LearningOS skill state.

---

## Refresh Needed

A previously strong or retained skill shows meaningful weakening during later reassessment.

This does not mean all previous learning has disappeared.

The system should:

- identify what weakened
- refresh only what is necessary
- test again later

---

## Relearning

The learner is actively restoring a previously acquired skill after forgetting or loss of performance.

Relearning should usually be more targeted than learning from zero.

---

# Terminology Rule

For canonical LearningOS state labels, use:

- Untested
- Learning
- Working
- Solid-now
- Retained
- Refresh Needed
- Relearning

The word **mastery** may still be used as a general concept.

However:

**Mastered is not a separate stored skill state in v0.1.**

When durable mastery evidence is strong, the canonical state is:

**Retained**

This avoids ambiguity between "Mastered" and "Retained."

---

# Evidence Strength

Not all successful attempts provide equal evidence.

## Weak evidence

Examples:

- immediately after the lesson
- same example as the lesson
- solution recently seen
- substantial hints
- successful recognition without application

---

## Moderate evidence

Examples:

- familiar task
- some delay
- little assistance
- correct explanation or implementation

---

## Strong evidence

Examples:

- meaningful delay
- independent performance
- fresh or changed problem
- appropriate transfer
- ability to explain or debug the result

---

## Very Strong Evidence

Examples:

After meaningful time has passed, the learner independently:

- recognizes when the skill is relevant
- chooses an appropriate approach
- applies it successfully
- diagnoses problems when necessary
- uses it naturally inside authentic project work

---

# Core Rules

## Rule 1 — Course completion is not mastery

Finishing:

- a video
- chapter
- course
- tutorial
- exercise set

does not automatically change a skill to Solid-now or Retained.

---

## Rule 2 — Self-confidence is supporting information only

Statements such as:

"I know React well."

or:

"I think I am 8/10."

may help choose diagnostic difficulty.

They are not objective mastery evidence.

---

## Rule 3 — One success is not enough for important conclusions

A single successful attempt may be a useful signal.

For important skills, stronger conclusions should normally use multiple pieces of evidence.

---

## Rule 4 — One failure does not erase strong history

A single later mistake does not automatically change Retained to weak.

The system should investigate whether the failure was:

- a slip
- unusual task difficulty
- a prerequisite problem
- genuine forgetting
- a deeper gap

---

## Rule 5 — Assistance affects evidence strength

Correct performance with substantial assistance is weaker mastery evidence than independent performance.

Help usage must be recorded and interpreted separately.

The exact assistance model is defined elsewhere and is currently being canonicalized during the repository audit.

---

## Rule 6 — Relevant dimensions depend on the skill

Not every skill needs identical evidence.

Examples:

A conceptual distinction may depend heavily on:

- Explain
- Retain

A debugging skill depends heavily on:

- Debug
- Transfer
- Retain

A programming capability may require:

- Read / Trace
- Build
- Debug
- Transfer
- Retain

Do not mechanically require all six dimensions for every minor skill.

---

## Rule 7 — Evidence history must remain available

The current state is a summary.

The underlying evidence should be preserved so LearningOS can answer:

- Why is this considered Working?
- Why did this become Refresh Needed?
- What evidence supports Retained?
- Which dimension is still weak?

The current label should never replace the evidence history.

---

# Status

Mastery Rubric v0.1 is a working model.

It is canonical for the current LearningOS audit, but it is not permanent.

It may change when:

- stronger research suggests a better model
- baseline evidence reveals problems
- pilot use shows unnecessary complexity
- terminology causes confusion

# Monitoring Evidence Schema v0.1

## Purpose

LearningOS should record enough evidence to answer:

- What skill was actually tested?
- What kind of ability was demonstrated?
- Did the learner succeed?
- How independently did they perform?
- What kind of error or gap appeared?
- Was the task familiar or novel?
- Was the performance immediate or delayed?
- What should happen next?

The schema should capture **meaningful learning evidence**, not every click, keystroke, or minor action.

---

# Core Attempt Record

A meaningful attempt should eventually be able to record the following information.

## 1. Skill

What capability is primarily being tested?

Example:

`JavaScript lexical scope`

A task may involve multiple skills, but where possible distinguish:

- primary skill
- supporting skills

Do not automatically mark every supporting skill weak when a task fails.

---

## 2. Evidence Type

Which ability was demonstrated?

Canonical evidence dimensions:

- Explain
- Read / Trace
- Build / Apply
- Debug
- Adapt / Transfer
- Retain

A task may produce more than one evidence type.

---

## 3. Result

Use a simple outcome such as:

- Pass
- Partial
- Fail

Do not use the result alone to determine mastery.

Example:

`Pass with substantial assistance`

is not equivalent to:

`Independent Pass`.

---

## 4. Independence / Assistance Context

Record how the learner reached the result.

The system must distinguish between:

- independent performance
- normal reference/documentation use
- instructional hints
- guided assistance
- substantial solution exposure

Reference use and instructional assistance should not be silently treated as equivalent.

The exact canonical assistance model is defined separately.

Until that model is finalized during the current audit, preserve enough information to reconstruct what kind of help occurred.

---

## 5. Meaningful Attempts

Record the number of meaningful attempts where useful.

Do not count every tiny edit or keystroke.

A meaningful attempt is a distinct effort such as:

- proposing a solution
- trying a debugging hypothesis
- implementing a new approach
- revising an explanation after feedback

---

## 6. Error / Gap Signal

Record what kind of problem appeared when meaningful.

Current candidate categories:

- Concept / Knowledge
- Misconception
- Recall
- Application
- Debugging
- Transfer
- Problem-Solving / Decomposition
- Prerequisite / Dependency
- Retention
- AI / Help Dependency
- Slip / Careless Error

These are evidence signals.

A single event does not automatically confirm a gap.

---

## 7. Delay

Record meaningful time since previous learning or previous use when relevant.

Examples:

- immediate / same session
- later session
- several days later
- long-delayed reassessment

Exact numeric duration should be stored when available.

Delay matters especially for retention evidence.

---

## 8. Task Novelty

Record approximately how familiar the task is.

Suggested working labels:

### Same / Repeated

The same or nearly identical task has already been seen.

### Familiar

The structure is known and resembles previous practice.

### Variant

The same underlying skill appears with meaningful changes.

### New / Transfer

The learner must recognize and apply the skill in a substantially different context.

Novelty changes the strength of evidence.

---

## 9. Task / Diagnostic Mode

Where relevant, record the conditions under which the attempt occurred.

Examples:

- Independent
- Reference-Allowed
- Diagnostic Assistance
- Learning Mode
- Production Mode

The same result under different modes should not automatically be interpreted the same way.

---

## 10. Artifact Evidence

When useful, preserve a reference to the actual work.

Examples:

- code
- commit
- patch
- explanation
- test result
- debugging notes
- project feature
- task identifier

Do not require an artifact for every small learning event.

---

# Optional Context Fields

Some evidence benefits from additional context.

Possible fields include:

- timestamp
- session ID
- project
- source/resource being studied
- task family
- difficulty
- prerequisite skills involved
- tool use
- notes
- follow-up required

These should be added only when they help future learning decisions.

---

# Time-on-Task

Time may be recorded as contextual information.

However:

**time spent is not a mastery score.**

Do not infer:

fast = strong

or:

slow = weak

without other evidence.

Slow performance may result from:

- careful reasoning
- unfamiliar context
- difficult task
- debugging complexity

Fast performance may result from:

- memorization
- task familiarity
- guessing
- prior exposure

Interpret time only alongside other evidence.

---

# Derived Fields

The system may later calculate useful summaries from raw evidence.

Possible derived fields include:

- last meaningful attempt
- last independent success
- last delayed success
- independent-success streak
- assistance trend
- repeated error types
- weak evidence dimensions
- next reassessment
- current derived skill state
- state confidence

These are **derived state**, not the raw evidence itself.

Where practical, they should be reproducible from attempt history.

---

# Evidence Interpretation Rules

## Rule 1 — Preserve process, not only final correctness

Example:

Attempt 1:
incorrect mental model

Attempt 2:
small hint

Attempt 3:
independent correction

contains more useful information than simply:

`Result = Pass`.

---

## Rule 2 — Correctness and independence are separate

Two learners may both produce the correct result.

One may have worked independently.

The other may have seen most of the solution.

These should produce different evidence.

---

## Rule 3 — One attempt is normally a signal

A single Pass or Fail should usually be treated as one observation.

For important skill-state decisions, look for:

- repeated evidence
- different task contexts
- different evidence dimensions
- delayed evidence

when appropriate.

---

## Rule 4 — Record uncertainty

If the cause of failure is unknown, do not invent a gap category.

Record:

`Gap signal: uncertain`

and investigate later if the skill matters.

---

## Rule 5 — Do not over-log

Do not collect data merely because it is technically possible.

Avoid logging things such as:

- every mouse movement
- every keystroke
- every second of screen activity
- every trivial syntax correction

unless a future use case clearly requires them.

Monitoring overhead must remain lower than the value of the evidence collected.

---

# Example Evidence Record

A conceptual example:

Skill:
JavaScript closures

Evidence type:
Read / Trace

Result:
Partial

Task novelty:
Variant

Mode:
Independent

Assistance:
None during initial attempt

Observed issue:
Correctly predicted final output but explanation showed an incorrect lexical-scope model.

Gap signal:
Misconception — suspected

Delay:
3 days since previous use

Follow-up:
Generate a different scope/closure trace task.

This should NOT immediately produce:

`Closures = Weak`

because one attempt is only one piece of evidence.

---

# Relationship to Mastery Rubric

The Mastery Rubric answers:

**What kinds of performance count as stronger evidence of capability?**

The Monitoring Evidence Schema answers:

**What information should be preserved about each meaningful performance?**

The Skill Model later uses accumulated evidence to derive:

- current state
- confidence
- gaps
- reassessment needs

These layers should remain separate.

---

# Storage Direction

During implementation:

Raw attempt evidence should primarily live in structured storage such as SQLite.

Human-readable Markdown should contain:

- schema definitions
- rules
- explanations
- important summaries

Do not turn RESEARCH.md into the operational event database.

---

# Status

Monitoring Evidence Schema v0.1 is the canonical working evidence model.

The exact SQLite tables and columns are **not finalized yet**.

They should be designed only after the baseline workflow has been tested enough to confirm which fields are actually useful.

# Reference Use & Instructional Assistance Model v0.1

## Purpose

LearningOS must not treat these as the same thing:

- looking up documentation
- receiving a hint
- being guided step by step
- seeing most of the solution

A learner may reasonably use documentation while still performing the important reasoning independently.

Therefore assistance is represented using **separate dimensions**.

---

# 1. Reference Use

Reference use describes information the learner consults without receiving direct instructional guidance from the coach.

## R0 — No Reference

No external reference material was used.

Examples:

- no documentation
- no notes
- no search
- no example code

R0 is useful when testing unaided recall or independent reasoning.

---

## R1 — Lookup / Reference

The learner consults reference material for limited information without being given the solution strategy.

Examples:

- checking exact API syntax
- checking a method signature
- reading official documentation
- checking command syntax
- looking up a configuration option

The learner still decides:

- what approach to use
- why it applies
- how to integrate it
- how to verify the result

R1 may still provide strong evidence for realistic professional software-development performance.

R1 is weaker than R0 when the specific target is unaided recall.

---

## R2 — Worked Example / Structural Reference

The learner consults material that meaningfully reveals how a similar problem is solved.

Examples:

- tutorial implementation of a similar feature
- reference code with the same structure
- worked example
- previous solution that provides the main approach

R2 is more informative than direct solution exposure but provides weaker independent-performance evidence than R0 or R1.

If the consulted material is effectively the solution to the current task, classify the event as substantial solution exposure rather than ordinary reference use.

---

# 2. Instructional Assistance

Instructional assistance describes guidance provided to help the learner progress.

The source may eventually be recorded separately:

- AI
- human tutor
- instructor
- answer key
- other

---

## A0 — No Instructional Assistance

The learner receives no strategic or conceptual help.

They independently decide how to approach the task.

Reference use may still separately be:

R0, R1, or R2.

Examples:

**R0 + A0**
Fully unaided performance.

**R1 + A0**
Independent reasoning with documentation lookup.

These are different kinds of evidence and must remain distinguishable.

---

## A1 — Orientation

Very light assistance that points the learner toward an area without revealing the solution path.

Examples:

- "Inspect what happens when this function is called twice."
- "The issue is related to state updates."
- "Check which part of the request is responsible for authorization."

A1 should not provide:

- the actual fix
- detailed reasoning
- the required implementation steps

---

## A2 — Small Hint

The coach reveals a useful conceptual clue or diagnostic direction.

Examples:

- identifying the relevant concept
- pointing out one incorrect assumption
- suggesting one useful debugging experiment
- asking a targeted question that substantially narrows the search

The learner must still construct most of the solution.

---

## A3 — Guided Scaffolding

The coach helps organize substantial parts of the reasoning.

Examples:

- breaking the solution into several steps
- guiding the learner through a debugging sequence
- revealing part of the reasoning
- supplying partial code
- repeatedly answering targeted questions until the learner can continue

The learner still performs meaningful work, but the result is not strong independent-performance evidence.

---

## A4 — Substantial Solution Exposure

The learner is shown most or all of the solution.

Examples:

- complete implementation
- exact bug location plus fix
- full worked solution
- step-by-step instructions that leave little meaningful reasoning

A4 may be appropriate for teaching.

However:

**A4 success is not evidence of independent mastery.**

A fresh later attempt should reassess the skill.

---

# 3. Neutral Task Clarification

Clarifying what the task means should not automatically increase the assistance level.

Examples:

- defining an ambiguous requirement
- correcting a typo in the prompt
- explaining the expected input/output format
- confirming what files are in scope

If clarification reveals:

- the relevant concept
- the strategy
- the bug location
- the solution path

then it becomes instructional assistance and should be recorded as A1 or higher.

---

# 4. Why Reference and Assistance Are Separate

The old model treated:

documentation use

and

instructional hints

as neighboring levels on one scale.

This caused ambiguity.

Example:

Learner A:

R1 + A0

- independently identifies the required algorithm
- looks up exact API syntax
- completes the task

Learner B:

R0 + A2

- uses no documentation
- receives a conceptual hint identifying the required algorithm
- completes the task

Both learners received external information.

But the evidence means different things.

LearningOS must preserve that difference.

---

# 5. Common Combinations

## R0 + A0

No reference.
No instructional help.

Strong evidence of unaided performance.

---

## R1 + A0

Reference lookup only.
No instructional guidance.

Strong evidence of realistic independent development when memorizing exact syntax is not the target.

---

## R2 + A0

Learner independently consults an analogous worked example.

Useful learning evidence, but weaker transfer/independence evidence.

---

## R0/R1 + A1

Learner requires only light orientation.

Evidence remains useful but shows some instructional dependency.

---

## R0/R1 + A2

A meaningful hint was required.

Treat as assisted success.

Later independent reassessment may be needed.

---

## Any Reference + A3

Guided performance.

Useful evidence about what the learner can do with scaffolding.

Not strong mastery evidence.

---

## Any Reference + A4

Substantial solution exposure.

Treat primarily as teaching/relearning activity.

Do not mark the skill Retained or independently Solid-now based on this attempt.

---

# 6. Baseline Rules

## Independent Baseline Mode

Default:

**R0 + A0**

when testing unaided reasoning or recall.

---

## Reference-Allowed Baseline Mode

Allowed:

**R0/R1 + A0**

when testing realistic professional ability rather than memorized syntax.

R2 should normally be recorded separately because worked examples can reveal substantial solution structure.

---

## Diagnostic Assistance Mode

After the original independent result is preserved:

A1 → A2 → A3 → A4

may be used progressively as needed.

The system should record the lowest assistance level that allowed meaningful progress.

---

# 7. Assistance Escalation

Do not automatically jump from failure to the complete solution.

Preferred progression when appropriate:

A0  
→ A1  
→ A2  
→ A3  
→ A4

However, this is not a rigid rule.

More direct instruction may be appropriate when:

- a prerequisite is clearly absent
- repeated attempts produce no useful progress
- further unaided struggle has little diagnostic value
- the session objective is teaching rather than assessment

The goal is learning, not artificial difficulty.

---

# 8. Assistance Fading

Across later attempts, healthy development often looks like:

A3  
→ A2  
→ A1  
→ A0

or:

R2  
→ R1  
→ R0/R1 independent performance

The exact path depends on the skill.

The system should look for **reduced instructional dependence**, not demand complete elimination of useful professional reference use.

---

# 9. Evidence Interpretation

Assistance level does not determine skill state by itself.

Interpret it alongside:

- correctness
- explanation quality
- task novelty
- delay
- repeated evidence
- evidence type
- project authenticity

Example:

A learner repeatedly succeeds on fresh real-world programming tasks using:

R1 + A0

This may provide strong professional-performance evidence.

A learner succeeds once using:

R0 + A3

This provides much weaker independent evidence despite using no documentation.

---

# 10. AI Dependency

AI dependency should primarily concern repeated reliance on **instructional or solution-generating assistance**, not ordinary reference lookup.

Possible warning pattern:

A2–A4 success repeatedly

combined with:

A0 failure on related fresh tasks.

Another warning pattern:

AI-generated solution exposure

followed by:

inability to explain, modify, debug, or reproduce related work.

Documentation use alone should not be classified as AI dependency.

---

# 11. Historical H0–H4 Terminology

Earlier LearningOS notes used:

H0  
H1  
H2  
H3  
H4

That combined different kinds of assistance into a single scale.

This terminology is now **deprecated**.

New evidence should use:

**Reference Use**

- R0
- R1
- R2

and

**Instructional Assistance**

- A0
- A1
- A2
- A3
- A4

Historical H-level references in existing research notes will be updated during the repository audit.

---

# Research Basis

This separation is a LearningOS design model rather than a standardized educational measurement scale.

Relevant research principles include:

## Help Seeking

Research on intelligent tutoring systems shows that help-seeking behavior needs to be interpreted in context rather than treating all help use as equivalent.

Aleven, Roll, McLaren & Koedinger (2010)

Automated, Unobtrusive, Action-by-Action Assessment of Self-Regulation During Learning With an Intelligent Tutoring System.

Educational Psychologist, 45(4), 224–233.

DOI:
10.1080/00461520.2010.517740

---

## Guidance Fading

Research on worked examples and the expertise-reversal effect supports adapting and reducing instructional guidance as learner expertise increases rather than using a fixed amount of guidance for everyone.

Salden, Aleven, Schwonke & Renkl (2010)

The Expertise Reversal Effect and Worked Examples in Tutored Problem Solving.

Instructional Science, 38, 289–307.

DOI:
10.1007/s11251-009-9107-8

---

## Self-Explanation

A meta-analysis found positive learning effects from prompting learners to generate self-explanations across a range of learning conditions.

Bisra, Liu, Nesbit, Salimi & Winne (2018)

Inducing Self-Explanation: A Meta-Analysis.

Educational Psychology Review, 30, 703–725.

DOI:
10.1007/s10648-018-9434-x

---

# Important Limitation

Research supports ideas such as:

- contextual interpretation of help seeking
- adaptive instructional guidance
- fading support as expertise develops
- learner-generated explanation

It does **not** establish the exact LearningOS R0–R2 and A0–A4 categories as a validated universal scale.

These categories are our operational design and must be tested during the pilot.

---

# Status

Reference Use & Instructional Assistance Model v0.1 is now the canonical assistance model for LearningOS.

The older H0–H4 terminology is deprecated and should be removed or translated from existing research sections during the current repository audit.

## Research Topic 001 — Retrieval Practice

### Finding

Retrieval/testing generally produces better later retention than simply restudying previously learned material.

### Implication for LearningOS

Review sessions should begin with recall before reopening notes or explanations.

Examples:

- explain a concept from memory
- predict code behavior
- write a small implementation without looking
- answer a question before checking the source

### Evidence

Primary support:

- SRC-001 — Testing Effect in Classrooms

Evidence strength:

**Strong / synthesis-level**

Important limitation:

The evidence strongly supports retrieval/testing for learning and retention, but it does not mean every software-development skill should be converted into a quiz.

---

## Research Topic 002 — Spacing

### Finding

Reviewing material after delays helps long-term retention.

There is no single universal schedule such as:

1 → 3 → 7 → 30 days

that is optimal for every topic.

Spacing should depend on:

- difficulty
- importance
- previous performance
- how long the knowledge needs to be retained

### Implication for LearningOS

The system should adapt review timing instead of relying only on a fixed schedule.

### Evidence

Primary support:

- SRC-002 — Distributed Practice / Spacing

Evidence strength:

**Strong / synthesis-level**

Important limitation:

Most of the classic evidence concerns verbal recall and related memory tasks.

LearningOS should therefore use the general spacing principle for programming, but should not assume that exact verbal-memory intervals transfer directly to complex coding skills.

---

## Research Topic 003 — Delayed Performance

### Finding

Immediate successful performance does not by itself establish durable retention. Performance after a meaningful delay provides direct evidence about what remains available later.

### Implication for LearningOS

A topic should not become Retained immediately after a successful lesson or exercise.

The system should reassess it later.

### Evidence

Primary support:

- SRC-002 — Distributed Practice / Spacing
- SRC-008 — Successive Relearning and Long-Term Retention

Evidence strength:

**Moderate to strong**

SRC-002 provides broad evidence about delayed retention and spacing.

SRC-008 provides more direct experimental evidence that relearning across sessions can substantially improve long-term retention compared with relying on one learning session.

Important limitation:

"Meaningful delay" does not have one universal duration.

The appropriate delay depends on the skill, learning goal, previous evidence, and desired retention period.

---

## Research Topic 004 — Retrieval With Feedback

### Finding

Retrieval/testing can be more useful when learners receive appropriate corrective feedback, especially when errors or misconceptions need correction. The effectiveness of feedback depends on its content and context.

### Implication for LearningOS

The learning loop should be approximately:

Attempt → Evaluate → Feedback → Retry → Delayed Reassessment

The learner should normally attempt first before seeing a full solution.

### Evidence

Primary support:

- SRC-001 — Testing Effect in Classrooms
- SRC-003 — Educational Feedback

Evidence strength:

**Strong, but context-dependent**

SRC-001 identifies corrective feedback as one factor that moderates the classroom testing effect.

SRC-003 shows that feedback has an overall positive learning effect, while also showing substantial variation between different kinds of feedback.

Important limitation:

LearningOS should not interpret this as:

"more feedback is always better"

or:

"the full solution should immediately be shown after every error."

---

## Research Topic 005 — Programming Skill Is Multi-Dimensional

### Finding

Programming competence is broader than syntax recall or success on one coding exercise.
Authoritative computing curricula describe software-development capability using multiple forms of performance, including reading and writing programs, using data structures and algorithms, testing, debugging, and development tools.

### Implication for LearningOS

A skill should have multiple evidence types instead of one mastery score based only on quizzes.

Current evidence dimensions:

1. Explain
2. Read / Trace
3. Build / Apply
4. Debug
5. Adapt / Transfer
6. Retain

### Evidence

Primary support:

- SRC-006 — CS2023

Evidence strength:

**Strong for curriculum/competency scope**

CS2023 treats Software Development Fundamentals as broader than programming syntax alone and includes capabilities such as:

- reading and understanding code
- writing programs
- selecting and using data structures
- algorithmic reasoning
- testing
- debugging
- development tools

Important limitation:

CS2023 is a curricular guideline.

It does not validate LearningOS's exact six evidence dimensions:

1. Explain
2. Read / Trace
3. Build / Apply
4. Debug
5. Adapt / Transfer
6. Retain

Those six dimensions are a LearningOS assessment design informed by broader competency evidence.

---

## Research Topic 006 — Help Usage Matters

### Finding

Assistance changes how a successful result should be interpreted.

Help-seeking behavior can be productive or unproductive depending on context, so LearningOS should record the type and amount of assistance rather than treating all help use as equivalent.

### Implication for LearningOS

Attempts should record two separate dimensions:

- Reference Use: R0–R2
- Instructional Assistance: A0–A4

Documentation/reference use must not be treated as equivalent to instructional hints or solution exposure.

A useful learning trend is generally decreasing instructional assistance over time, such as:

A3 → A2 → A1 → A0

Reference use may still remain at R1 during realistic professional work when exact recall is not the learning target.

The canonical definitions are maintained in:

**Reference Use & Instructional Assistance Model v0.1**

### Evidence

Primary support:

- SRC-009 — Context-Sensitive Help-Seeking Assessment

Evidence strength:

**Moderate / domain-specific**

The research supports context-sensitive interpretation of help-seeking behavior and fine-grained observation of learner actions.

Important limitation:

The exact LearningOS distinction between:

- Reference Use: R0–R2
- Instructional Assistance: A0–A4

is our operational design.

It has not been independently validated as a universal educational scale.

---

## Research Topic 007 — Process Data Matters

### Finding

Final correctness alone can hide important information about learning.
Repeated interactions, errors, assistance use, timing, and other process evidence can provide additional information about how a learner is performing and changing over time.

### Implication for LearningOS

Each meaningful attempt should capture enough process evidence to detect patterns, without logging unnecessary activity.

Current working evidence schema:

- skill
- evidence type
- result
- reference use
- instructional assistance
- attempts
- error type
- delay since previous learning/use
- task novelty
- artifact or code evidence when useful

### Evidence

Primary support:

- SRC-009 — Context-Sensitive Help-Seeking Assessment
- SRC-010 — Knowledge Tracing Survey

Evidence strength:

**Moderate to strong for structured learning environments**

Research in intelligent tutoring and knowledge tracing shows that learner state can be investigated using sequences of observable interactions rather than only one final answer.

Examples of potentially useful signals include:

- repeated correctness or failure
- help-seeking behavior
- interaction history
- time-related forgetting information
- changing performance across practice

Important limitation:

The following LearningOS signals are broader than what these sources directly validate:

- debugging strategy
- project artifacts
- Git history
- task novelty
- AI-dependency patterns
- transfer across real projects

These are evidence-informed LearningOS extensions that must be evaluated during the pilot.

---

## Research Topic 008 — Working Gap Taxonomy

### Finding

There is no evidence that the current LearningOS gap categories form a standardized or scientifically validated universal taxonomy.

Instead, the categories are a working diagnostic model created to distinguish different patterns that may require different learning responses.

The taxonomy is informed by research concepts such as:

- knowledge components
- slips and guesses
- forgetting
- help seeking
- programming competencies
- delayed performance

but the exact category boundaries are LearningOS design decisions.

Concept / Knowledge
Misconception
Recall
Application
Debugging
Transfer
Problem-Solving / Decomposition
Prerequisite / Dependency
Retention
AI / Help Dependency
Slip / Careless Error

Detection rules are defined provisionally in Gap Detection Rules v0.1 below and remain subject to pilot validation.

### Evidence

Relevant support:

- SRC-006 — CS2023
- SRC-009 — Context-Sensitive Help-Seeking Assessment
- SRC-010 — Knowledge Tracing Survey
- SRC-002 — Distributed Practice / Spacing
- SRC-008 — Successive Relearning and Long-Term Retention

Evidence strength:

**Mixed — taxonomy itself is provisional**

Relevant research supports several underlying distinctions:

- one wrong response can occur despite underlying knowledge
- one correct response can occur without secure knowledge
- knowledge can weaken over time
- help use needs contextual interpretation
- programming performance contains multiple capabilities
- delayed performance can reveal retention problems

However, no source listed here validates this exact eleven-category LearningOS taxonomy.

### Status

Treat each category as a diagnostic hypothesis.

The pilot should test whether the categories:

- can be distinguished reliably
- lead to different useful interventions
- avoid excessive labeling
- need merging or splitting

If two categories consistently produce the same evidence and learning action, consider merging them.

If one category repeatedly hides meaningfully different problems, consider splitting it.

---

# Open Research Questions

The next research step is:

## Gap Detection Rules v0.1

We need to determine:

- what pattern of evidence indicates each gap type
- how many failures are meaningful
- how to distinguish forgetting from never learning
- how to distinguish a conceptual problem from a careless mistake
- how hint dependence should affect skill status
- how real project evidence should affect mastery
- when the system should lower or raise a skill status

# Gap Detection Rules v0.1

## Core Rule

One failure does not automatically mean there is a knowledge gap.

A single unusual result is treated as a **signal**.

A gap becomes more credible when:

- the same problem appears again on a different task
- multiple evidence types point to the same weakness
- the weakness remains after feedback and another attempt
- the weakness appears again after a meaningful delay
- the learner repeatedly needs help for the same underlying skill

The system should therefore use:

**Signal → Suspected Gap → Confirmed Gap**

rather than immediately labeling every mistake as a weakness.

---

## 1. Concept / Knowledge Gap

### Pattern

The learner cannot correctly:

- explain the concept
- predict what related code will do
- reason about why something behaves the way it does

and similar failures appear across more than one task.

### Example

The learner remembers the syntax of a JavaScript closure but cannot explain lexical scope or correctly predict which variables remain accessible.

### Detection

Explain fails

- Trace/Predict fails
- similar problem remains after feedback

→ Concept Gap becomes likely.

---

## 2. Misconception Gap

This is different from simply not knowing something.

### Pattern

The learner has a **consistent but incorrect mental model**.

Typical evidence:

- repeatedly predicts the same wrong behavior
- produces similar bug patterns
- confidently gives the same incorrect explanation
- the error appears in different problems

### Example

The learner consistently believes that React state updates immediately change the current variable value inside the same render.

A repeated systematic error is stronger evidence of a misconception than random mistakes.

---

## 3. Recall Gap

### Pattern

There is previous evidence that the concept was understood or used successfully, but after a delay the learner cannot retrieve it.

However, after a small cue or brief refresh:

- understanding returns quickly
- application becomes possible again
- deeper reasoning remains mostly intact

### Important

A single failed recall attempt cannot tell us whether the knowledge was never learned or temporarily inaccessible.

Therefore recall gaps are initially marked as **provisional** until another test clarifies the problem.

---

## 4. Application Gap

### Pattern

The learner can:

- explain the concept
- recognize it
- trace examples

but cannot independently use it to solve or build something.

### Typical pattern

Explain = Pass  
Trace = Pass  
Build = Fail or requires meaningful instructional assistance

→ Application Gap.

---

## 5. Debugging Gap

Debugging is tracked separately from general coding ability.

### Pattern

The learner may understand or even write the relevant code but repeatedly struggles to:

- locate the fault
- form useful hypotheses
- inspect program state
- determine the root cause
- fix the problem without random edits

Repeated trial-and-error changes without systematic diagnosis are useful signals.

### Important

A debugging failure does not automatically mean the underlying concept is unknown.

The system should separately test the prerequisite concept before deciding.

---

## 6. Transfer Gap

### Pattern

The learner succeeds when:

- the problem looks familiar
- the example resembles the lesson
- the context is nearly identical

but fails when:

- details change
- the same concept appears in a different context
- the learner must choose the concept without being told
- the problem is embedded inside a larger project

### Typical pattern

Familiar task = independent pass  
Changed / novel task = fail

→ Transfer Gap.

---

## 7. Problem-Solving / Decomposition Gap

This category is added to the original candidate gaps.

### Pattern

The learner knows the individual concepts and can solve small isolated tasks, but struggles to:

- break a larger problem into parts
- decide what to do first
- create a plan
- identify relevant subproblems
- connect several known skills together

### Example

The learner can independently use fetch, React state, forms, and validation separately but cannot design the steps needed to build a complete data-entry feature.

This should not automatically be classified as a React or JavaScript knowledge gap.

---

## 8. Prerequisite / Dependency Gap

### Pattern

A current topic repeatedly fails because an earlier skill is weak.

### Detection rule

Do not infer this only from the current failure.

Test the suspected prerequisite directly.

If:

Target skill fails

- prerequisite test also fails
- correcting the prerequisite improves the target

→ Dependency Gap becomes strong.

### Example

Difficulty understanding React closures may actually come from weak JavaScript lexical-scope knowledge.

---

## 9. Retention Gap

### Pattern

The skill previously had strong independent evidence but later cannot be performed after a meaningful delay.

Strong signals include:

- delayed independent recall fails
- a delayed variant task fails
- the learner requires help for something previously performed independently

### First failure

Do not immediately downgrade a previously Solid-now or Retained skill.

Mark:

**Refresh Needed**

### Confirmed retention problem

If the weakness appears again during reassessment, downgrade the skill and schedule relearning/review.

---

## 10. AI / Help Dependency Gap

### Pattern

Performance is repeatedly successful with AI assistance but unsuccessful without it.

Typical evidence:

A2–A4 assisted attempts = repeated success
but
A0 attempts on related fresh tasks = repeated failure
Reference use should be recorded separately and should not by itself be interpreted as AI/help dependency.

Other warning signals:

- asking for the solution before making a meaningful attempt
- copying generated code without being able to explain it
- being unable to reproduce a similar solution later
- being unable to debug AI-generated code
- repeated failure on a similar problem after AI solved the previous one

AI help itself is not considered bad.

The problem is **persistent dependence without increasing independence**.

A healthy trend looks like:

A3 → A2 → A1 → A0

over later attempts.

Normal R1 documentation use may remain even when instructional assistance reaches A0.

---

## 11. Slip / Careless Error — Not a Gap

Some mistakes should not create a knowledge-gap record.

Examples:

- typo
- missed character
- accidental wrong variable name
- simple off-by-one mistake
- momentary syntax error

A mistake is more likely to be a slip when:

- the learner notices and fixes it independently
- the explanation of the concept is correct
- similar tasks are usually successful
- the same mistake does not repeatedly occur

Repeated "careless" errors should eventually be reconsidered because a persistent pattern may indicate a deeper weakness.

---

# Gap Confidence

The system should not use rigid rules such as:

"Two failures always mean a gap."

Instead it should combine evidence.

## Low confidence

One isolated signal.

## Medium confidence

Repeated pattern on different tasks OR multiple evidence types agree.

## High confidence

The pattern survives feedback/retry, appears across contexts, or reappears after a delay.

---

# Gap Resolution

A gap should not disappear merely because the learner reads the explanation.

Evidence of resolution should include later successful performance.

Preferred evidence:

Independent attempt

- appropriate evidence type
- different or changed problem
- ideally delayed reassessment

For important skills, delayed independent performance is the strongest confirmation that the gap has actually closed.

---

# Current Gap Types

1. Concept / Knowledge
2. Misconception
3. Recall
4. Application
5. Debugging
6. Transfer
7. Problem-Solving / Decomposition
8. Prerequisite / Dependency
9. Retention
10. AI / Help Dependency
11. Slip / Careless Error — not normally treated as a gap

---

# Research Basis

The working model is informed by research on:

- Bayesian Knowledge Tracing and its distinction between slips and guesses
- intelligent tutoring and help-seeking behavior
- programming misconceptions
- debugging education
- retrieval practice and delayed assessment
- learning transfer

These detection rules are a LearningOS design model, not a standardized scientific diagnostic instrument. They should be refined using actual learner data during the pilot phase.

# Retention & Spaced Practice Rules v0.1

## Core Principle

Learning is not considered durable because it was successful once.

Important knowledge and skills should be successfully retrieved or performed again across separate sessions.

The system should prefer:

**Learn → Retrieve/Perform → Feedback → Space → Retrieve/Perform Again**

over repeated rereading or repeated practice inside one session.

---

## Rule 1 — Do Not Use One Universal Review Schedule

The system should not permanently hard-code:

1 → 3 → 7 → 14 → 30 days

for every skill.

Review timing should eventually adapt to:

- importance of the skill
- desired retention period
- previous performance
- difficulty
- whether help was required
- previous forgetting
- how often the skill naturally appears in projects

Fixed intervals may be used temporarily during the pilot, but they are starting defaults rather than scientific rules.

---

## Rule 2 — Retrieval Comes Before Restudy

When a review becomes due:

1. attempt recall or performance first
2. record the result
3. then use notes, documentation, explanation, or feedback if necessary
4. retry after correction

Do not begin most reviews by immediately rereading the lesson.

A failed retrieval attempt is useful diagnostic evidence.

---

## Rule 3 — Relearning Across Sessions Matters More Than Overpractice

Once a learner can successfully perform something during today's session, repeatedly doing the same easy task many more times may have diminishing value.

Instead, important material should return in later sessions.

The target is not:

"Do it ten times today."

The target is closer to:

"Become successful today, then become successful again after forgetting has had some opportunity to occur."

---

## Rule 4 — Memory Knowledge and Programming Skill Need Different Reviews

### Knowledge / Recall material

Examples:

- terminology
- concepts
- HTTP status meanings
- language rules
- API concepts
- vocabulary

Possible review:

- short-answer recall
- explain from memory
- flashcard
- compare two concepts
- predict behavior

Spaced-repetition software may be useful here.

### Programming / Procedural skill

Examples:

- debugging
- state modeling
- writing an API
- refactoring
- decomposing a feature
- designing a component
- solving an algorithm problem

Review should primarily involve **doing**.

Possible review:

- implement without looking
- debug a fresh bug
- modify existing code
- solve a variant problem
- use the skill inside a real project

A flashcard success cannot by itself mark a procedural programming skill as retained.

---

## Rule 5 — Later Reviews Should Become Less Familiar

Early review may use a familiar task.

Later review should increasingly test:

- changed examples
- different context
- mixed skills
- deciding which technique to use
- real project usage

This helps distinguish remembering an example from retaining transferable skill.

---

## Rule 6 — Assistance Changes the Interpretation of a Review

### Fully Unaided Delayed Success

R0 + A0 after a meaningful delay

→ very strong evidence when unaided recall or performance is the target.

### Documentation-Only Delayed Success

R1 + A0 after a meaningful delay

→ useful and potentially strong evidence for realistic professional programming performance.

It is weaker than R0 + A0 only when unaided recall itself is the target.

### Hint-Assisted Success

A1–A3

→ useful relearning or supported-performance evidence, but weaker independent-retention evidence.

Schedule a later A0 attempt when independent performance matters.

### Substantial Solution Exposure

A4

→ do not count the current attempt as Retained.

The learner should later attempt a fresh related problem with A0.

---

## Rule 7 — A Failed Delayed Review Does Not Mean Start From Zero

If a previously successful skill is forgotten:

1. record the retention signal
2. attempt a small cue if appropriate
3. refresh only what is needed
4. reach successful performance again
5. schedule another delayed test

This is treated as **relearning**, not necessarily complete relearning from the beginning.

---

## Rule 8 — Review Frequency Should Decrease as Evidence Strengthens

Repeated delayed independent successes should generally allow longer intervals.

Repeated forgetting should shorten the next interval or trigger investigation of:

- weak initial understanding
- poor retrieval practice
- prerequisite gaps
- insufficient application
- excessive AI dependence

The scheduler should eventually adapt from actual performance history.

---

## Rule 9 — Natural Project Use Can Count as Review

A separate review exercise is not always necessary.

If an old skill appears naturally inside a real project and the learner:

- recognizes when it is needed
- applies it independently
- debugs it if necessary
- succeeds after a meaningful period without direct practice

then that event can count as high-quality retention evidence.

The system should avoid unnecessary duplicate review work.

---

## Rule 10 — Important Skills Need More Durable Evidence

Not every fact deserves the same review effort.

Skills that are:

- foundational
- frequently reused
- prerequisites for many later skills
- important to current goals

should receive stronger and longer-term reassessment.

Low-value lookup information may simply remain reference material.

The system should not attempt to memorize everything.

---

# Retention State Integration

Retention does not define a second skill-state model.

LearningOS uses the canonical skill states defined in:

**Mastery Rubric v0.1**

Canonical states:

- Untested
- Learning
- Working
- Solid-now
- Retained
- Refresh Needed
- Relearning

Retention-specific behavior should be represented through evidence and scheduling fields rather than separate states.

Useful retention-related evidence may include:

- last meaningful attempt
- last independent success
- last delayed success
- delay since previous learning or use
- delayed reassessment result
- next reassessment
- previous forgetting or refresh history

For example:

A newly successful skill may remain:

**Solid-now**

until sufficient delayed evidence supports:

**Retained**

If later delayed performance meaningfully weakens, the skill may move to:

**Refresh Needed**

If active restoration is required, it may move to:

**Relearning**

This keeps retention logic consistent with the canonical LearningOS skill-state model.

---

# Pilot Scheduling Principle

Before building an adaptive scheduler, use a simple pilot.

For important newly learned material:

- one early retrieval opportunity
- another review after some delay
- progressively longer delays after successful independent performance
- shorter return after meaningful failure

Exact intervals will be chosen later when the pilot workflow is designed.

Do not automate exact scheduling yet.

---

# Important Limitation

Most classic spacing and successive-relearning research focuses heavily on recall of facts, vocabulary, definitions, and conceptual material.

We should not assume that the exact same schedules or success criteria transfer perfectly to complex software-development skills.

For programming, the system should combine memory research with:

- delayed coding performance
- debugging
- transfer tasks
- project evidence
- skill-gap monitoring

and refine scheduling based on our own pilot data.

# AI Learning Coach Behavior v0.1

## Core Principle

When the goal is learning, the AI should optimize for:

**future independent ability**

rather than:

**finishing the current task as quickly as possible.**

The AI may behave differently when the learner explicitly switches from Learning Mode to Production Mode.

---

# 1. Default Learning Mode

For active learning tasks, the AI should normally avoid immediately giving the complete answer.

Default sequence:

1. Understand what the learner is trying to do
2. Check what they already understand when necessary
3. Ask the learner to make a meaningful attempt
4. Observe the attempt
5. Identify the likely gap
6. Give the smallest useful intervention
7. Let the learner try again
8. Increase help only when necessary
9. Ask for explanation or verification after success
10. Reassess later without help

The AI should not create unnecessary questioning when the learner clearly already has enough information to attempt the task.

---

# 2. Attempt Before Assistance

When appropriate, the learner should attempt the problem before receiving a solution.

A meaningful attempt may include:

- explaining their current understanding
- predicting behavior
- proposing a plan
- writing partial code
- identifying likely causes of a bug
- describing what they already tried

This gives the system evidence about the learner's actual knowledge state.

---

# 3. Progressive Instructional Assistance

Instructional assistance should normally escalate gradually:
A0 — No instructional assistance
The learner chooses the approach independently.
A1 — Orientation
Point toward an area to inspect without revealing the solution path.
A2 — Small hint
Reveal a useful conceptual clue or diagnostic direction.
A3 — Guided scaffolding
Help organize substantial parts of the reasoning while preserving meaningful learner work.
A4 — Substantial solution exposure
Show most or all of the solution when necessary.
Reference/documentation use is recorded separately as R0–R2.
After A4, learning should not be considered complete. A fresh later task should test performance at A0.

---

# 4. Prefer Questions That Reveal Thinking

Useful tutor questions include:

- What do you expect this code to do?
- Why do you think this variable has that value?
- Which part of the problem are you least certain about?
- What have you ruled out?
- What would you test next?
- Which concept might apply here?
- Why did this fix work?

Questions should have a clear diagnostic or instructional purpose.

The AI should avoid turning every interaction into an exhausting Socratic interrogation.

---

# 5. Use Self-Explanation

After an important success, the AI may ask the learner to explain:

- why the solution works
- why the original attempt failed
- what concept was important
- what would change in a related situation

The explanation should come from the learner before the AI supplies its own explanation when feasible.

The purpose is to expose fragile understanding and strengthen conceptual connections.

---

# 6. Debugging Mode

When debugging is a learning objective, the AI should not immediately patch the code.

Preferred sequence:

1. ask what behavior was expected
2. identify the actual observed behavior
3. ask for one or more hypotheses
4. choose a useful observation/test
5. inspect the result
6. narrow the fault
7. let the learner attempt the fix
8. verify why the fix works

If the learner repeatedly guesses and edits randomly, the coach should explicitly teach a more systematic debugging process.

Debugging performance should be recorded separately from coding/build performance.

---

# 7. Do Not Confuse Task Completion With Learning

A program running successfully does not prove that the learner understands it.

After substantial AI assistance, the system may verify learning with:

- explanation
- code tracing
- modification of the solution
- debugging a related issue
- a similar task without help
- delayed reassessment

AI-generated code should not automatically produce mastery evidence.

---

# 8. Detect AI Dependency

The coach should watch for patterns such as:

- requesting solutions before attempting
- repeatedly asking AI to debug without investigation
- copying code that cannot be explained
- success with AI but repeated failure without AI
- inability to modify AI-generated code
- inability to reproduce similar work later

The response should not be punishment or complete removal of AI.

Instead, gradually change the interaction:

Solution giving
→ guided help
→ small hints
→ independent attempts.

Healthy progress should trend toward lower help requirements.

---

# 9. Do Not Withhold Help Artificially

Productive struggle is useful only while progress remains possible.

The AI should escalate support when:

- the learner is stuck without generating useful new attempts
- the same misconception keeps repeating
- prerequisite knowledge is missing
- frustration is producing random behavior rather than learning
- additional unaided struggle is unlikely to reveal useful evidence

The goal is not to make learning unnecessarily difficult.

---

# 10. Separate Learning Mode and Production Mode

Not every coding task is a learning exercise.

## Learning Mode

Primary objective:
build independent skill.

Behavior:

- attempt-first
- progressive hints
- explanation
- diagnostic evidence
- delayed reassessment

## Production Mode

Primary objective:
complete real work accurately and efficiently.

Behavior may include:

- direct implementation
- larger generated code changes
- automation
- agentic execution

However, if an important knowledge gap appears during Production Mode, it may be logged for later Learning Mode review.

The system should make the current mode visible.

---

# 11. Verification After Heavy Assistance

If A3 or A4 instructional assistance was required:

Do not mark the skill as Solid-now or Retained based on this attempt alone.

Instead:

1. finish understanding the current solution
2. ask for a brief explanation when useful
3. schedule or generate a fresh related task
4. test again later at A0, with R0 or R1 chosen according to what the task is intended to measure

A later independent success is more valuable than repeating the exact solved task immediately.

---

# 12. Adapt to Learner Evidence

The AI should not use the same teaching style for every situation.

Examples:

### Strong conceptual knowledge + weak application

Reduce explanation.
Increase building tasks.

### Strong building + weak debugging

Provide bugs and diagnosis exercises.

### Repeated recall failure

Use retrieval and spaced review.

### Transfer weakness

Change context and problem structure.

### Prerequisite gap

Temporarily step backward and test the prerequisite.

### Strong retained skill

Reduce instructional support and review frequency.

---

# 13. Feedback Style

Feedback should normally be:

- specific
- connected to the learner's actual attempt
- focused on the cause of the error
- actionable
- limited enough that the learner still thinks

Prefer:

"Your loop condition assumes the last index is inclusive. Check what happens when i equals array.length."

over immediately replacing the entire function.

Full explanations remain available when needed.

---

# 14. Capture Learning Evidence Automatically Where Possible

During a learning interaction, the coach should eventually be able to derive:

- skill being tested
- evidence type
- result
- reference use
- instructional assistance
- attempts
- recurring error
- misconception signal
- task novelty
- whether the final solution was independent
- whether later reassessment is needed

The learner should not manually fill out a large form after every session.

---

# 15. End-of-Session Behavior

At the end of a meaningful learning session, the coach should determine:

### Learned / strengthened

What evidence improved?

### Remaining gaps

What still appears weak?

### Assistance used

How independently did the learner perform?

### Follow-up

Does anything require:

- practice
- relearning
- delayed review
- prerequisite work
- project application?

Only meaningful findings should be recorded.

---

# 16. Anti-Patterns for the AI Coach

Avoid by default in Learning Mode:

- instantly writing the complete solution
- fixing every bug automatically
- explaining before the learner attempts retrieval
- giving endless theory without testing performance
- praising understanding without evidence
- marking mastery from course completion
- asking excessive questions that create friction
- forcing the learner to rediscover basic facts when a quick reference is sufficient
- treating documentation use as failure
- treating all AI use as harmful

---

# Working AI-Coach Objective

For learning interactions, optimize for:

**Independent future performance**

- **accurate gap detection**
- **durable retention**
- **efficient use of assistance**

rather than maximum difficulty or minimum completion time.

---

# Research Basis

This working model is informed by research on:

- scaffolded versus unrestricted AI programming assistants
- intelligent tutoring systems
- self-explanation
- formative feedback
- AI-assisted coding and skill formation
- cognitive offloading and learner independence

Important current evidence includes:

- SRC-011 — Guided vs Unrestricted AI in Programming Education
- SRC-012 — Performance vs Learning in AI-Supported Programming
- SRC-013 — AI Assistance and Coding Skill Formation
- SRC-014 — Self-Explanation Meta-Analysis
- SRC-015 — AI Chatbots in Programming Education Meta-Analysis

### Evidence Interpretation

The evidence base for generative-AI tutoring is developing rapidly but is less mature than research areas such as retrieval practice and spacing.

Current evidence does not justify a simple conclusion such as:

"AI is bad for learning"

or:

"AI always improves learning."

Instead, outcomes appear to depend on factors such as:

- how much reasoning the learner still performs
- whether complete solutions are exposed
- whether assistance is scaffolded
- task and learner characteristics
- what learning outcome is measured

The exact LearningOS AI Coach rules remain an evidence-informed operational design rather than a scientifically validated universal tutoring protocol.

Therefore these rules should be treated as a testable LearningOS design rather than permanent pedagogical truth.

Therefore these rules should be treated as a testable LearningOS design rather than permanent pedagogical truth.

# Monitoring Cadence & Checkpoints v0.1

## Core Principle

Monitoring should be frequent enough to detect meaningful learning problems, but not so frequent that assessment becomes the main activity.

The system should continuously collect useful evidence from normal learning and use larger checkpoints only when they add information.

Monitoring is therefore layered rather than based on one large recurring test.

---

## Layer 1 — Meaningful Attempt Monitoring

Whenever a meaningful learning attempt occurs, the system may capture evidence from it.

Examples include:

- explaining a concept
- solving a problem
- implementing a feature
- debugging
- modifying existing code
- completing a delayed review
- using an old skill naturally in a project

The attempt itself can become assessment evidence.

There is no need to create a separate quiz after every activity.

The system should record only meaningful evidence, not every click, keystroke, or trivial action.

---

## Layer 2 — End-of-Session Check

At the end of a meaningful study session, perform a short learning check.

The purpose is not to retest everything.

Determine:

**What improved?**  
What evidence suggests learning occurred?

**What remains weak?**  
Did a possible gap appear?

**What reference use and instructional assistance were required?**  
Was performance becoming more independent?

**What should happen next?**  
Continue, practice, review later, repair a prerequisite, or move forward?

The session should normally end with a clear next action.

This check should remain lightweight.

---

## Layer 3 — Corrective Loop

When a meaningful gap appears:

Assessment  
→ specific feedback  
→ corrective activity  
→ another attempt

Do not treat feedback itself as proof that the gap has closed.

For important skills, successful reassessment should follow corrective work.

If the learner already meets the required level, unnecessary remedial practice should be avoided.

---

## Layer 4 — Scheduled Retention Review

Important learned material should reappear after delays.

The review scheduler should prioritize skills that are:

- important
- weak or recently corrected
- foundational
- previously forgotten
- currently dependent on help
- due for retention evidence

Skills that naturally appear in current projects may receive retention evidence through project work instead of an artificial review.

Review intervals should eventually adapt from performance rather than follow one permanent fixed calendar.

---

## Layer 5 — Weekly Evidence Synthesis

A weekly review should primarily analyze existing evidence.

It should not mean retesting the entire skill map every week.

The system should examine:

Current active skills  
Recurring errors  
New suspected gaps  
Help-dependency trends  
Overdue retention checks  
Project blockers  
Skills with insufficient evidence

The result should be a small number of learning priorities for the next period.

If no useful evidence exists for a skill, mark it as:

**Unknown / insufficient recent evidence**

rather than assuming it has become weak.

---

## Layer 6 — Milestone Checkpoint

A stronger checkpoint should occur before an important transition.

Examples:

- moving from JavaScript foundations into React
- finishing a major React unit
- beginning a substantial project
- declaring a foundational skill solid
- progressing from guided exercises to independent work

The checkpoint should sample several evidence dimensions where relevant:

Explain  
Read / Trace  
Build / Apply  
Debug  
Transfer

A major checkpoint should use fresh tasks where possible.

Passing the exact exercises already practiced is weak evidence of transfer.

---

## Layer 7 — Delayed Retention Check

A skill should not receive Retained status solely from immediate performance.

For important skills, later evidence should test whether the learner can still perform after time has passed.

Strong delayed evidence includes:

- no hint
- no solution exposure
- independent choice of approach
- a changed or authentic task
- successful debugging when needed

Repeated delayed success permits longer review intervals.

Failure triggers:

Refresh Needed

rather than automatically treating the learner as a complete beginner again.

---

## Layer 8 — Project-Based Monitoring

Real project work should serve as a major source of diagnostic evidence.

The system should observe problems such as:

- inability to decompose a feature
- repeated architecture mistakes
- difficulty using known concepts together
- debugging weaknesses
- missing prerequisite knowledge
- excessive reliance on AI
- inability to recognize when a known technique is relevant

Project evidence can be stronger than isolated exercises because the learner must often identify the relevant skill without being told.

However, one successful project use does not prove every dimension of a skill.

---

# What Gets Reassessed First

The system should not treat every skill equally.

Priority for reassessment should generally increase when a skill is:

Foundational  
Important to the current goal  
Recently weak  
Previously forgotten  
Repeatedly AI-assisted  
A prerequisite for another blocked skill  
Not used for a long time but still important

Low-value lookup knowledge should not consume large amounts of review time.

---

# Advancement Rule

For important prerequisite skills, progression should be based primarily on demonstrated readiness rather than course completion or time spent.

If evidence suggests the learner is ready:

Move forward.

If an important prerequisite remains weak:

Use targeted correction and reassessment.

This does not require perfect mastery of every minor detail before progressing.

---

# Avoid Over-Testing

Monitoring itself creates cost.

Do not:

- test every skill every day
- run full diagnostics after every session
- create quizzes only to generate metrics
- repeat already-easy tasks unnecessarily
- delay real project work because the learner is constantly being assessed

Prefer assessment embedded naturally in learning activity.

---

# Practical Pilot Cadence

The following cadence is a LearningOS design starting point, not a scientifically proven universal schedule.

### During learning

Capture meaningful attempt evidence.

### End of meaningful session

Perform a brief session check and determine next action.

### During later sessions

Allow the retention scheduler and natural project work to surface old skills.

### Approximately weekly

Synthesize evidence and adjust current priorities.

Do not retest the entire curriculum.

### At meaningful transitions

Run a broader milestone diagnostic.

### Over longer periods

Use delayed retention checks for important skills and occasionally review whether the LearningOS itself is producing useful results.

The exact cadence should be refined during the pilot.

---

# Monitoring Output

Monitoring should ultimately answer only a few useful questions:

What am I learning now?

What evidence says I can do it?

What is currently blocking me?

What appears to be a real gap?

What needs to return later?

What should I work on next?

If collected data does not help answer one of these questions, reconsider whether it needs to be collected.

---

# Evidence Quality Rule

Evidence should be interpreted according to:

- independence
- delay
- novelty
- task authenticity
- number of converging observations
- type of ability demonstrated

A recent easy success with substantial instructional assistance should not outweigh multiple delayed independent failures.

Similarly, one isolated failure should not outweigh a strong history of independent performance without further investigation.

---

# Research Basis

## Yang et al., 2021

Testing (Quizzing) Boosts Classroom Learning: A Systematic and Meta-Analytic Review.

Psychological Bulletin.

222 independent studies and 48,478 learners.

DOI: 10.1037/bul0000309

Supports retrieval/testing as a useful learning intervention and shows that effects depend on factors including feedback, repetition, timing, and task characteristics.

## Wisniewski, Zierer & Hattie, 2020

The Power of Feedback Revisited: A Meta-Analysis of Educational Feedback Research.

Frontiers in Psychology.

435 studies, more than 61,000 learners.

DOI: 10.3389/fpsyg.2019.03087

Found an overall medium feedback effect while showing substantial variation depending on the informational content of feedback.

## Van der Kleij, Feskens & Eggen, 2015

Effects of Feedback in a Computer-Based Learning Environment on Students' Learning Outcomes: A Meta-Analysis.

Review of Educational Research.

40 studies.

Found larger effects for elaborated feedback than simple correctness feedback, particularly for higher-order outcomes.

## Winget & Persky, 2022

A Practical Review of Mastery Learning.

American Journal of Pharmaceutical Education.

DOI: 10.5688/ajpe8906

Describes the mastery-learning cycle of formative assessment, corrective activity, and reassessment, and recommends cumulative assessment and consideration of baseline knowledge.

## Cepeda et al., 2006

Distributed Practice in Verbal Recall Tasks: A Review and Quantitative Synthesis.

Psychological Bulletin.

317 experiments across 184 articles.

Shows that useful spacing depends jointly on the spacing interval and desired retention interval.

---

# Important Limitation

The research above comes from several educational domains and is not a direct validation of this exact LearningOS cadence.

In particular:

- weekly synthesis
- end-of-session summaries
- milestone placement

are practical design decisions informed by the evidence rather than scientifically established universal frequencies.

The pilot must determine whether these checkpoints produce useful information without creating excessive learning overhead.

# Tool Architecture v0.1

## Core Principle

LearningOS should remain:

- local-first
- portable
- inspectable
- AI-provider independent
- easy to back up
- usable even if one tool is removed later

No chat application should be the authoritative memory of the system.

---

# Architecture Decision

LearningOS should use two different kinds of local storage.

## 1. Markdown — Human Knowledge and Rules

Markdown should store information that humans need to read, discuss, edit, and version.

Examples:

- PLAN.md
- DECISIONS.md
- RESEARCH.md
- learning principles
- AI coach rules
- curriculum decisions
- explanations of system behavior
- later, possibly skill definitions and learning guides

Markdown is the source of truth for:

**Why the system behaves the way it does.**

---

## 2. SQLite — Structured Learning Evidence

Structured learning history should not be stored only in large Markdown logs.

A local SQLite database is the preferred candidate for data such as:

- learning sessions
- attempts
- skills tested
- evidence type
- pass / partial / fail
- help level
- error type
- gaps
- reviews
- delayed reassessments
- mastery/retention evidence
- project evidence
- timestamps
- relationships between skills

SQLite is the source of truth for:

**What actually happened during learning.**

This makes later questions practical, such as:

- Which skills repeatedly need hints?
- What has not been independently tested recently?
- Which misconceptions keep returning?
- What prerequisite is blocking several skills?
- Which skills previously considered Solid-now or Retained failed delayed review?
- What should be reassessed next?

---

# Claude Code — Primary Learning Coach Interface

Claude Code is the current preferred interface between the learner and LearningOS.

Its responsibilities may eventually include:

- reading the current learning state
- conducting learning sessions
- testing skills
- following the AI Coach rules
- recording meaningful evidence
- identifying suspected gaps
- generating reassessment tasks
- updating plans when appropriate
- producing weekly evidence synthesis

Claude Code itself is not the source of truth.

The local LearningOS data is.

---

# CLAUDE.md

A project-level CLAUDE.md should eventually contain concise persistent instructions for Claude Code.

It should contain rules that need to apply repeatedly, such as:

- operate in Learning Mode by default
- do not equate task completion with mastery
- prefer attempt-before-solution
- use progressive hints
- record meaningful learning evidence
- do not silently downgrade skill state based on one failure

CLAUDE.md should not become a database or giant knowledge dump.

Long procedures and research notes should remain elsewhere.

---

# Obsidian — Optional Human Interface

Obsidian may be used as a convenient interface for the Markdown part of LearningOS.

It is not required for the architecture.

If used:

# LearningOS folder

Obsidian vault.

Removing Obsidian should not remove or invalidate the learning data.

The underlying Markdown files remain ordinary local files.

---

# Anki / FSRS — Specialized Memory Tool, Not the Master Database

Anki remains a candidate for knowledge that benefits from flashcard-style retrieval and spaced repetition.

Examples:

- terminology
- language vocabulary
- conceptual distinctions
- important factual knowledge

Anki should not by itself determine the LearningOS state of a complex programming skill.

Strong programming-skill evidence requires other evidence such as:

- building
- debugging
- transfer
- project application
- delayed independent performance

If Anki is used, LearningOS should eventually decide how review results are reflected back into the central learning evidence.

Anki should not become a second competing source of truth for the whole learning system.

---

# Git — Version History for Human-Readable System Files

The LearningOS directory should eventually become a Git repository.

Git should primarily track:

- Markdown documentation
- configuration
- schemas
- scripts
- system code
- AI coach instructions

This provides history for questions such as:

- Why did this rule change?
- What was the previous learning plan?
- When was a research conclusion revised?

Git history is useful but should not be treated as the only backup.

---

# SQLite and Git

The live SQLite database should not depend on Git for every learning event.

Binary database changes are not human-readable Git history.

Preferred direction:

- Git tracks database schema and application code
- SQLite stores live structured learning data
- the database receives separate backups
- later, useful reports or exports may be generated in human-readable formats

Exact backup strategy will be designed later.

---

# ChatGPT / Claude Chat

Chat applications can be used for:

- research
- discussion
- explanation
- brainstorming
- challenging assumptions

Important findings and decisions must eventually return to LearningOS.

Chat history should not be required for reconstructing the learning system.

---

# Proposed Data Flow

Learner starts a session

→ Claude Code reads LearningOS state

→ learning task or review occurs

→ learner attempts the task

→ coach provides assistance when necessary

→ meaningful evidence is recorded in SQLite

→ gap/status logic evaluates the evidence

→ future review or reassessment is determined

→ important session conclusions may update human-readable Markdown

→ weekly synthesis uses accumulated structured evidence

---

# Separation of Responsibilities

## Markdown

Plans, reasoning, research, policies, documentation.

## SQLite

Events, attempts, reviews, gaps, skill state, measurable evidence.

## Claude Code

Coach and operational interface.

## Obsidian

Optional visual/editor interface for Markdown.

## Anki / FSRS

Optional specialized spaced-repetition engine.

## Git

History for system files and documentation.

## Backup

Separate protection of the whole system and structured database.

---

# Source-of-Truth Rule

There is not one file that contains everything.

Instead:

### System truth

Markdown.

"What are our rules and why?"

### Learning evidence truth

SQLite.

"What has actually happened?"

### Derived state

Calculated from evidence.

"What currently appears strong, weak, retained, or uncertain?"

Derived state should be reproducible from underlying evidence where practical.

---

# Important Design Principle — Preserve Raw Evidence

Do not store only the final conclusion:

"React Effects = Weak"

Keep the evidence that produced that conclusion.

For example:

- delayed debug task failed
- A3 instructional assistance required
- dependency misconception repeated
- later fresh variant task passed at R0 + A0

The system should be able to explain why it believes a gap exists.

---

# Avoid Premature Complexity

This architecture does not mean all components must be implemented immediately.

The pilot should begin with the smallest implementation capable of validating the workflow.

Possible features such as:

- dashboards
- automatic Anki integration
- advanced knowledge tracing
- custom FSRS integration
- automated Git analysis
- complex agents
- graphical skill maps

should be added only when evidence shows they are useful.

---

# Tool Architecture Status

This is **Tool Architecture v0.1**.

Current preferred core:

Local LearningOS

- Markdown
- SQLite
- Claude Code
- Git

Optional/supporting:

Obsidian
Anki / FSRS
Claude Chat / ChatGPT

Implementation has not started yet.

The architecture may change during pilot testing.

---

# Verified Tool Sources

The current architecture was checked against official documentation from:

- Anthropic Claude Code documentation
- Obsidian Help
- SQLite official documentation
- Anki Manual
- Pro Git / git-scm.com

Tool behavior should be rechecked against current official documentation when implementation begins because software features may change.

# Skill Model & Knowledge State v0.1

## Core Principle

LearningOS should not represent knowledge as:

"React = 72%"

or:

"JavaScript = mastered"

A broad topic contains many different capabilities.

The system should instead maintain a structured skill model and derive current state from actual evidence.

---

# 1. Separate Domains, Topics, Skills, and Tasks

These are different things.

## Domain

A broad learning area.

Examples:

- Software Development
- English
- Thai

## Area / Topic

A meaningful subject inside a domain.

Examples:

Software Development
→ JavaScript
→ React
→ Testing
→ HTTP
→ Git

A topic is useful for organization but is usually too broad to mark as mastered.

## Skill / Knowledge Component

A smaller learnable and assessable capability.

Examples:

Instead of:

React Effects

possible skills might include:

- explain when synchronization with an external system is needed
- reason about effect dependencies
- implement cleanup correctly
- recognize when an effect is unnecessary
- debug an effect-related stale-value problem

Skills should be small enough that weaknesses can be diagnosed, but large enough to appear in multiple meaningful tasks.

## Task

A concrete activity that produces evidence.

Examples:

- explain why a specific effect reruns
- debug an effect bug
- build a component that subscribes and cleans up
- remove an unnecessary effect from existing code

Tasks generate evidence.

Tasks themselves are not the learner's knowledge model.

---

# 2. Skill Granularity Rule

Do not make skills extremely broad.

Bad example:

"Knows JavaScript"

This hides too many different capabilities.

Do not make every exercise or API method its own permanent skill either.

Bad examples:

"Can solve exercise 17"

"Remembers Array.prototype.flatMap syntax"

unless that information is genuinely important to the learning goal.

The preferred level is a reusable knowledge component or capability that can appear across several tasks.

---

# 3. Refine Granularity From Evidence

The initial skill model may be wrong.

If a supposed single skill produces contradictory learning patterns, consider splitting it.

Example:

A learner consistently succeeds at explaining a concept but repeatedly fails its application tasks.

This may mean:

- the skill definition is too broad
- two separate capabilities are being mixed together

Conversely, if several tiny skill nodes:

- always occur together
- have almost no separate evidence
- do not support different learning decisions

consider merging them.

The skill model should evolve from actual learning evidence.

---

# 4. Tasks May Exercise Multiple Skills

Real programming tasks often require several skills simultaneously.

Example:

Build a form that submits data to an API.

This may involve:

- state modeling
- event handling
- validation
- async JavaScript
- HTTP
- error handling

Therefore a task may map to multiple skills.

However, when diagnosing a failure, LearningOS should try to identify which skill or prerequisite most likely caused the problem instead of marking every related skill as weak.

Where useful, a task can identify:

**Primary skill**
the main ability intentionally being tested

and

**Supporting skills**
other capabilities required to complete the task.

---

# 5. Prerequisite Graph

Skills should be connected when one capability meaningfully supports another.

Example:

JavaScript lexical scope
→ supports
JavaScript closures

JavaScript functions/state concepts
→ may support
React state reasoning

React fundamentals
→ support
Next.js application development

The graph should not be treated as a perfectly fixed school syllabus.

Some prerequisites will be:

- known in advance
- suspected from learning evidence
- discovered later

---

# 6. Prerequisite Confidence

A dependency should be allowed to have a status such as:

**Known prerequisite**
Strong curricular or technical reason.

**Suspected prerequisite**
Evidence suggests the dependency but it has not been confirmed.

**Confirmed learner dependency**
Testing the prerequisite showed weakness and correcting it improved the blocked skill.

This prevents the system from assuming that every failure in an advanced topic was caused by a prerequisite.

---

# 7. Do Not Force One Linear Learning Path

The skill graph is not necessarily:

A → B → C → D → E

Some skills can develop in parallel.

Some become relevant only when a project requires them.

Some advanced work may reveal an older missing prerequisite.

The system should support moving backward temporarily to repair a dependency and then returning to the current goal.

---

# 8. Skill Evidence Dimensions

A skill may have evidence across multiple dimensions.

Current dimensions remain:

1. Explain
2. Read / Trace
3. Build / Apply
4. Debug
5. Adapt / Transfer
6. Retain

These dimensions should not automatically be collapsed into one numeric score.

Example:

React State

Explain: Strong  
Trace: Strong  
Build: Strong  
Debug: Weak  
Transfer: Medium  
Retention: Strong

This is more useful than:

React State = 78%

because it directly suggests what should happen next.

---

# 9. Current Skill State

The existing state model remains:

**Untested**
No meaningful evidence.

**Learning**
The learner is actively acquiring the skill and still requires meaningful support.

**Working**
The learner can perform familiar work but evidence is incomplete or assistance is still needed.

**Solid-now**
Current independent evidence is strong across the dimensions relevant to the skill.

**Retained**
Appropriate independent performance remains after meaningful delay.

**Refresh Needed**
A previously strong skill weakened during delayed reassessment.

**Relearning**
The learner is restoring a previously acquired skill.

These states are derived summaries.

They should not replace the evidence history.

---

# 10. Confidence Is Separate From Skill State

LearningOS should distinguish:

"What state currently appears most likely?"

from:

"How confident are we?"

Example:

State:
Solid-now

Confidence:
Low

Reason:
Only one independent task has been observed.

Another skill might be:

State:
Working

Confidence:
High

Reason:
Multiple tasks consistently show the same application weakness.

Possible confidence labels:

- Low
- Medium
- High

Do not introduce precise probabilities until there is enough data and a validated reason to do so.

---

# 11. Evidence History Is More Important Than the Current Label

A status may change.

The system should preserve:

- successes
- failures
- delayed results
- hints required
- gap signals
- task context
- novelty
- project evidence

The current status should be reproducible or explainable from this history.

The system should be able to answer:

"Why do you believe this skill is weak?"

or:

"Why is this considered retained?"

---

# 12. Current State Should Be Derived, Not Manually Declared

A learner or AI may provide observations, but the system should avoid casually writing:

"Mastered = true"

Instead, state should eventually be derived from evidence rules.

Example:

Several independent successes

- different contexts
- delayed success

may produce:

Retained / High confidence.

A new failure may not immediately erase that history.

It may instead produce:

Refresh Needed

until reassessment clarifies the state.

---

# 13. Evidence Recency Matters

Old evidence remains historically useful but may not fully represent current ability.

The system should distinguish:

- recent independent evidence
- old independent evidence
- recent assisted performance
- delayed reassessment

Important skills with only old evidence may become candidates for reassessment.

Do not automatically mark them weak simply because time passed.

Use:

Unknown current state / reassessment needed

when appropriate.

---

# 14. Skill Importance

Not every skill deserves equal tracking effort.

A skill may later carry attributes such as:

**Foundational**
Many later skills depend on it.

**Core to current goal**
Important for the learner's present path.

**Supporting**
Useful but not central.

**Reference-level**
Usually safe to look up rather than memorize.

This should affect:

- review priority
- mastery requirements
- reassessment frequency

It should not be interpreted as a universal ranking of what every developer must learn.

---

# 15. Framework APIs Should Not Flood the Skill Graph

LearningOS should avoid creating permanent skill nodes for every:

- library function
- framework API
- configuration option
- command-line flag

unless repeated evidence shows that the item represents a meaningful reusable capability.

Many implementation details are better treated as:

Reference knowledge

rather than long-term mastery targets.

The system should prioritize transferable concepts and capabilities.

---

# 16. Competency Is Task-Context Dependent

Knowing information is not identical to being competent in a real task.

For software development, competency may require combining:

- relevant knowledge
- technical skill
- problem solving
- appropriate tool use
- judgment

Therefore project tasks and authentic work should remain part of the evidence model.

This is especially important when generative AI can produce code without guaranteeing that the learner understands how or why it works.

---

# 17. Professional Dispositions

Authoritative computing curricula also include professional dispositions such as:

- persistence
- self-direction
- adaptability
- collaboration
- meticulousness

LearningOS should acknowledge these but should **not begin by heavily scoring personality or behavior**.

During the initial pilot, dispositions should be observed only when they produce actionable learning information.

Examples:

- systematically abandoning debugging without investigation
- difficulty working independently
- repeated failure to verify generated output

A separate disposition model should be added only if it proves useful.

---

# 18. Initial Skill Record

A skill record will eventually need something approximately like:

Skill ID  
Name  
Domain  
Area / Topic  
Description  
Importance  
Prerequisites  
Current derived state  
State confidence  
Evidence by dimension  
Last meaningful attempt  
Last independent success  
Last delayed success  
Active gap(s)

The exact SQLite schema is NOT being finalized yet.

This section defines the conceptual model first.

---

# 19. Initial Relationship Model

Likely relationships include:

**part_of**
Skill belongs to a larger area.

**prerequisite_for**
One skill supports another.

**tested_by**
Tasks can provide evidence for a skill.

**related_to**
Useful conceptual relationship without claiming prerequisite dependency.

Avoid creating unnecessary relationship types before the pilot demonstrates a need.

---

# 20. Skill Model Refinement Loop

The skill model itself should be monitored.

Process:

Initial skill model  
→ learner attempts tasks  
→ evidence accumulates  
→ confusing patterns appear  
→ split / merge / reconnect skills  
→ continue observing

A skill map is therefore a hypothesis about the structure of expertise, not an unquestionable truth.

---

# Example

Instead of storing:

React = 70%

LearningOS might eventually represent:

React
│
├── Component Model
│ ├── component composition
│ └── props/data flow
│
├── State
│ ├── state updates
│ ├── derived state
│ └── state placement
│
└── Effects
├── synchronization reasoning
├── dependency reasoning
└── cleanup

For:

Effects → dependency reasoning

the current evidence might be:

Explain: Solid  
Trace: Solid  
Build: Working  
Debug: Weak  
Transfer: Untested  
Retention: Untested

State:
Working

Confidence:
Medium

Gap:
Debugging

This directly tells the coach what kind of activity should come next.

---

# Research Basis

## ACM / IEEE-CS / AAAI — CS2023

CS2023 is the current computer science curricular guideline jointly produced by ACM, IEEE Computer Society, and AAAI.

Relevant findings:

- computing education should move beyond topic exposure toward competency
- competency is expressed in the context of tasks
- knowledge, skills, and professional dispositions all contribute to competency
- CS2023 distinguishes skill levels such as Explain, Apply, Develop, and Evaluate
- software-development competency spans multiple knowledge areas rather than one isolated programming topic

## Computing Curricula 2020 — ACM / IEEE-CS

CC2020 describes computing competency in terms of:

knowledge  
skills  
professional dispositions

within task performance.

This supports avoiding a knowledge-only skill model.

## Carnegie Mellon University — Knowledge Components

CMU's learning-science / DataShop work models learning in terms of Knowledge Components.

Relevant principles:

- learning itself is not directly observable
- observable errors, successes, and assistance provide evidence
- activities can map to one or more knowledge components
- poor learning patterns may indicate that a skill model is too coarse
- very sparse components may indicate that a model is too fine-grained
- knowledge-component models should be refined using learning evidence

---

# Important Limitation

CS2023 is a broad computer-science curriculum framework.

LearningOS is not attempting to reproduce an entire university CS curriculum.

We will use authoritative curricula as an external reference, then customize the actual skill graph around:

- the learner's current goals
- software-development direction
- existing ability
- project requirements
- detected gaps

The complete Software Development skill map will be created only after the skill baseline and deeper resource/goal analysis.

# Software Development Skill Baseline Method v0.1

## Purpose

The baseline is not an exam score and is not intended to rank the learner.

Its purpose is to answer:

- What can I already do independently?
- What is fragile?
- What has never been tested?
- What important prerequisites appear weak?
- Where should deeper diagnosis begin?
- What can safely be skipped in the learning path?

The baseline should reduce unnecessary relearning.

---

# 1. Use an Adaptive Diagnostic Funnel

Do not test every software-development skill deeply at the beginning.

Use three stages.

## Stage A — Broad Screening

Sample important areas with a small number of tasks.

Goal:

Detect areas that appear:

- clearly strong
- clearly weak
- uncertain
- not yet learned

This is breadth-first.

## Stage B — Targeted Diagnosis

Only investigate areas where the broad screen reveals:

- failures
- contradictory evidence
- heavy instructional-assistance dependence
- uncertain prerequisites
- unexpectedly strong ability

Use additional tasks to identify the actual gap.

## Stage C — Stop When Evidence Is Sufficient

Do not keep testing an area merely to generate more data.

If the system already has enough evidence to choose the next learning action, move on.

This adaptive funnel is a LearningOS design decision intended to reduce assessment burden.

---

# 2. Baseline Areas

The initial baseline should cover fundamental software-development capabilities broadly.

Exact depth will depend on the learner's goals.

## A. Programming Fundamentals

Possible areas:

- variables and values
- control flow
- functions
- scope
- data structures
- iteration
- error handling
- asynchronous reasoning where relevant
- program decomposition

For the current web-development direction, JavaScript should be one important implementation context.

---

## B. Code Understanding

Assess separately from code writing.

Possible evidence:

- trace code
- predict output or behavior
- explain why code behaves that way
- identify assumptions
- summarize the purpose of unfamiliar code

Being able to trace code does not automatically imply full conceptual understanding.

---

## C. Debugging

Use broken programs or features.

Observe whether the learner can:

- state expected behavior
- inspect actual behavior
- form hypotheses
- gather useful evidence
- locate the fault
- repair the fault
- explain why the repair works

Do not evaluate debugging only by whether the final program runs.

---

## D. Problem Solving / Decomposition

Use a task that is larger than a single syntax exercise.

Observe whether the learner can:

- clarify the goal
- break the task into smaller pieces
- identify dependencies
- choose a reasonable order
- connect known concepts

---

## E. Web Foundations

For a web-development path, sample:

- how client/server web interaction works
- HTTP fundamentals
- semantic HTML
- CSS/layout fundamentals
- browser/DOM concepts
- accessibility basics

Framework skill should not hide missing web fundamentals.

---

## F. Development Workflow

Sample practical capability with:

- files/project structure
- command line basics
- Git/version control
- dependency/package usage
- reading documentation
- running and interpreting tests
- basic development tooling

Tool usage should be judged according to the task.

Looking up a command may be perfectly normal professional behavior.

---

## G. Testing

Sample whether the learner understands:

- why testing is used
- what behavior should be tested
- basic unit/integration distinctions where relevant
- writing or interpreting a simple test
- using a failed test diagnostically

Testing depth can increase later according to the current development path.

---

## H. Current Stack

After foundational screening, assess the technologies currently relevant to the learner.

Likely candidates from the current resource set include:

- TypeScript
- React
- Next.js
- PHP / Laravel
- databases / APIs

Do not deeply assess every saved technology.

First determine which stack is actually part of the current path.

---

## I. Algorithms and Data Structures

Assess enough to understand current problem-solving ability and foundational gaps.

Possible evidence:

- select a suitable basic data structure
- reason about an algorithm
- implement a small solution
- explain complexity at an appropriate level
- adapt a known technique to a changed problem

Do not allow LeetCode performance alone to define overall software-development ability.

---

## J. Software Engineering / Project Capability

Use previous or small real projects to inspect capabilities such as:

- code organization
- separation of concerns
- refactoring
- managing change
- debugging across multiple files
- reasoning about requirements
- maintainability
- use of documentation
- working with an existing codebase

This area may initially remain lightly assessed and become clearer through real project work.

---

# 3. Use Multiple Evidence Formats

Do not diagnose skill from one question format.

Depending on the skill, use combinations of:

- Explain
- Trace / Predict
- Build
- Debug
- Modify existing code
- Transfer / variant task
- Small authentic project task

Different formats reveal different abilities.

---

# 4. Map Each Diagnostic Task to a Primary Skill

Whenever practical, a diagnostic task should have:

**Primary skill**
the capability the task is mainly intended to assess

and possibly:

**Supporting skills**
other abilities required by the task.

If the learner fails, do not automatically mark every supporting skill as weak.

Investigate the likely cause.

This reduces confounding.

---

# 5. Separate Closed-Book and Realistic Professional Performance

Two different questions may matter.

## Independent-memory diagnostic

Purpose:

What can the learner retrieve and reason about without assistance?

Possible rules:

- no AI
- no hints
- no solution
- limited reference use

## Authentic-work diagnostic

Purpose:

Can the learner perform effectively under realistic development conditions?

Possible rules:

- documentation allowed
- normal tooling allowed
- syntax/reference lookup allowed

AI use should still be controlled when independent skill is being measured.

The system must record which diagnostic mode was used.

Do not interpret these two modes as equivalent evidence.

---

# 6. AI Should Be Off During Core Independent Baseline Tasks

For baseline tasks intended to measure existing ability:

Start at R0 + A0 whenever practical when unaided performance is being measured.

If the learner becomes stuck:

record the independent result first.

Then support may be introduced to diagnose the gap.

Example:

Independent task fails

→ record the initial R0 + A0 failure

→ provide small hint

→ introduce the smallest appropriate instructional assistance and observe whether A1/A2 is enough for progress

This produces more useful evidence than immediately allowing unrestricted AI.

---

# 7. Documentation Use Is Not Automatically a Failure

Professional software development involves reference use.

The baseline should distinguish:

"I understand the concept but looked up exact API syntax."

from:

"I did not know what approach to use until the documentation or AI effectively supplied the solution."

Therefore R1 reference use should be interpreted according to what the task is intended to test.
R1 + A0 must remain distinguishable from A1/A2 instructional assistance.

---

# 8. Use Fresh Tasks

Avoid using exact examples that the learner has recently practiced or memorized.

Where possible:

- change names and values
- change context
- change problem structure
- combine concepts differently

For transfer-sensitive skills, use a genuinely different situation.

This reduces false confidence from memorizing solutions.

---

# 9. Self-Report Is Supporting Data Only

The learner may report:

- technologies previously studied
- projects completed
- confidence
- topics that feel weak
- topics not used recently

This information can help select the starting difficulty.

It should not determine mastery.

Example:

"I am strong at React"

means:

start React diagnostic at a more challenging level.

It does not mean:

React = Solid.

---

# 10. Previous Work Can Provide Evidence

Existing projects may be inspected for clues about:

- technologies used
- complexity handled
- testing
- architecture
- debugging history
- Git workflow

However, code existence alone does not prove independent mastery.

Possible unknowns include:

- tutorial copying
- AI contribution
- collaboration
- code written long ago
- inability to reproduce the work now

Previous work should guide diagnostics rather than replace them entirely.

---

# 11. Retention Cannot Be Fully Baseline-Tested Immediately

At the initial baseline, many skills may show:

Explain: strong
Build: strong
Debug: strong
Retention: untested

That is correct.

True retention evidence requires time.

Do not manufacture a Retained status from a same-day baseline.

Later delayed reassessment will fill this dimension.

---

# 12. Unknown Is a Valid Result

If evidence is insufficient, record:

Untested

or:

Current state uncertain.

Do not force every skill into:

strong / weak.

Uncertainty tells the system what may need testing later.

---

# 13. Do Not Make the Baseline a Marathon

The baseline should be spread across manageable sessions if necessary.

Fatigue, frustration, and excessive assessment time can contaminate the evidence and increase friction.

Prefer:

broad screen
→ targeted follow-up

rather than an exhaustive multi-hour examination of every topic.

---

# 14. Baseline Output

The output should NOT primarily be:

Software Development Score = 72/100.

Instead produce something like:

## JavaScript

Scope:
Solid-now / medium confidence

Async reasoning:
Working / medium confidence

Debugging:
Weak signal / needs confirmation

## Git

Basic workflow:
Solid-now / high confidence

Branching/conflicts:
Untested

## HTTP

Basic request/response:
Working / medium confidence

Caching:
Untested

## React

State:
Solid-now

Effects:
Working

Effect debugging:
Suspected gap

Transfer:
Insufficient evidence

This output can directly guide the learning path.

---

# 15. Baseline Should Affect the Curriculum

After baseline evidence is collected:

### Strong foundational area

Skip or compress beginner instruction.

### Working / needs strengthening

Use targeted solidification.

### Confirmed prerequisite gap

Repair before or alongside dependent work.

### Untested but low-priority area

Leave untested.

### Missing important capability

Add it to the roadmap even if no bookmark currently covers it.

The curriculum should adapt to the learner rather than forcing the learner through every resource from beginning to end.

---

# 16. External Curriculum References

The baseline skill map should not be invented entirely from bookmarks.

Use external references to check for missing areas.

Current important references include:

## ACM / IEEE-CS / AAAI CS2023

Useful especially for:

- Software Development Fundamentals
- Algorithmic Foundations
- Programming Languages
- Software Engineering
- Data Management
- Networking
- Security
- Systems topics when relevant

LearningOS will not copy the entire CS degree curriculum.

It will use it as a gap-checking reference.

## MDN Curriculum

Useful for the web-development path.

Its current core includes:

- web standards
- semantic HTML
- CSS
- JavaScript
- accessibility
- design basics
- version control

Additional areas include testing, security/privacy, performance, APIs, and tooling.

This helps prevent framework-heavy learning from hiding weak web foundations.

---

# 17. Baseline Design Principle

Each assessment activity should answer:

**Claim**
What do we want to know about the learner?

**Evidence**
What behavior would support or weaken that claim?

**Task**
What activity can reliably produce that evidence?

Example:

Claim:
Can independently reason about asynchronous JavaScript execution?

Evidence:
Correct prediction + explanation on unfamiliar code.

Task:
Trace a fresh async snippet and explain execution order.

This structure should be used when building the actual diagnostic tasks.

---

# 18. Baseline Is Not High-Stakes Certification

LearningOS diagnostics are for adaptive learning decisions.

They are not professional certification or psychological testing.

Therefore:

- avoid false precision
- preserve uncertainty
- use multiple observations for important decisions
- revise conclusions when new evidence appears

The goal is better learning decisions, not producing an impressive score.

---

# Research Basis

## ETS — Evidence-Centered Design

Mislevy, Almond & Lukas (2003), A Brief Introduction to Evidence-Centered Design.

Supports explicitly connecting:

- claims about learner capability
- evidence needed
- tasks designed to elicit that evidence

## AERA / APA / NCME

Standards for Educational and Psychological Testing, 2014.

Used as a general authoritative reference emphasizing valid interpretation of assessment evidence, accessibility, fairness, and appropriate test use.

## ACM / IEEE-CS / AAAI — CS2023

Used as an authoritative external reference for computing competency and software-related knowledge areas.

## Mozilla MDN Curriculum

Used as an authoritative, current reference for essential web-development foundations.

## Programming research

Research distinguishes abilities such as code tracing and deeper comprehension, supporting the use of multiple evidence formats rather than assuming one task type represents overall programming skill.

---

# Status

Software Development Skill Baseline Method v0.1 is complete.

Actual baseline tasks have NOT been created yet.

The next step should design the baseline scope and task set around the learner's real software-development direction rather than immediately administering generic tests.

# Software Development Baseline Scope v0.1

## Current Direction

The current provisional direction is:

**practical software development with a strong web / full-stack orientation**

This is based on the learner's current priorities and existing learning resources.

It is not a permanent career decision.

The baseline should therefore test transferable software-development foundations first, then current stack skills separately.

---

# Baseline Structure

The baseline will have three layers:

## Layer A — Core Foundations

Important regardless of the current framework.

## Layer B — Web / Full-Stack Foundations

Important for the current development direction.

## Layer C — Current Stack Extensions

TypeScript, React, Next.js, PHP/Laravel, or other technologies that are actually active.

Framework-specific depth should come after foundational screening.

---

# Layer A — Core Software Development

## 1. Programming Reasoning

Primary implementation language for the initial screen:

**JavaScript**

Initial capabilities to sample:

- values and variables
- control flow
- functions
- scope
- closures
- arrays / objects
- data transformation
- iteration
- error handling
- asynchronous reasoning
- basic decomposition

The goal is not syntax trivia.

The baseline should determine whether the learner can reason about and use the language independently.

---

## 2. Code Reading and Tracing

Assess separately from code writing.

Sample:

- predict program behavior
- trace execution
- explain unfamiliar code
- identify important state/data changes
- recognize assumptions and edge cases

Strong code-writing performance does not automatically prove strong code-reading ability.

---

## 3. Debugging

This is a first-class baseline area.

Sample whether the learner can:

- state expected behavior
- reproduce a problem
- inspect useful evidence
- form hypotheses
- isolate the cause
- fix the problem
- explain why the fix works

Random editing until something works should not count as strong debugging evidence.

---

## 4. Problem Decomposition

Assess whether the learner can turn a larger requirement into manageable work.

Possible evidence:

- identify subproblems
- order implementation steps
- identify unknowns
- choose relevant existing skills
- separate essential from optional requirements

This should be tested with a small realistic feature rather than an abstract definition question.

---

## 5. Data Structures and Algorithms — Foundational Level

Initial baseline should sample:

- arrays / lists
- maps / dictionaries
- sets
- stacks / queues where appropriate
- searching / iteration
- basic sorting reasoning
- selecting an appropriate structure
- basic complexity reasoning
- solving a small unfamiliar problem

Do not deeply test advanced competitive-programming algorithms during the first baseline.

LeetCode performance is only one source of evidence.

---

# Layer B — Web / Full-Stack Foundations

## 6. Web Fundamentals

Sample understanding of:

- browser and server roles
- request / response model
- URLs
- HTTP methods
- status codes
- headers at a practical level
- JSON
- client/server boundaries
- basic browser behavior

The goal is practical reasoning, not memorizing protocol specifications.

---

## 7. HTML and Semantics

Sample:

- appropriate semantic elements
- forms
- labels
- document structure
- basic accessibility consequences

Do not let React/Next experience substitute for checking basic HTML understanding.

---

## 8. CSS and Layout

Initial scope:

- cascade and inheritance
- box model
- selectors
- sizing
- flexbox
- grid at a practical level
- responsive layout
- positioning
- debugging layout problems

Deep visual design skill is not part of the initial software-development baseline.

---

## 9. Browser / DOM

Sample:

- DOM relationships
- events
- event handling
- basic browser APIs
- manipulating or reasoning about UI state
- asynchronous browser operations where relevant

This provides context underneath framework abstractions.

---

## 10. Accessibility Basics

Initial scope:

- semantic markup
- labels
- keyboard interaction
- basic focus awareness
- accessible controls
- recognizing obvious accessibility problems

Accessibility is part of web-development foundations rather than an optional polish step.

---

## 11. Git / Version Control

Sample practical workflow:

- understand working tree / staging / commit
- inspect history
- create useful commits
- branch
- merge
- resolve a simple conflict
- work with a remote
- undo or recover from a common mistake

Exact command memorization is not the goal.

Documentation/reference lookup may be allowed where command syntax is not the capability being tested.

---

## 12. Development Environment / Tooling

Light screening only.

Sample:

- command line navigation
- project structure
- package managers
- installing dependencies
- running scripts
- reading errors
- environment/configuration awareness
- using documentation effectively

The baseline should identify severe workflow gaps without testing tool trivia.

---

# Layer B — Full-Stack Foundations

## 13. APIs and Backend Reasoning

Framework-neutral first.

Sample:

- route / endpoint reasoning
- request validation
- response design
- error handling
- basic CRUD
- separation between client and server responsibilities
- authentication versus authorization conceptually

Framework syntax should not hide whether the underlying concept is understood.

---

## 14. Data / Database Foundations

Initial scope:

- tables / records / fields
- primary keys
- relationships
- basic SQL reasoning
- SELECT / INSERT / UPDATE / DELETE concepts
- schema design at a basic level
- constraints
- migrations conceptually
- transactions at a basic level

ORM skill should be assessed separately from database understanding.

---

## 15. Testing

Sample:

- why a test exists
- identifying useful behavior to test
- reading an existing test
- writing a small test
- interpreting a failure
- difference between isolated/unit and broader integration/feature testing at a practical level

Testing should also appear naturally in later project diagnostics.

---

## 16. Security Basics

Only foundational screening initially.

Possible areas:

- untrusted input
- validation
- authentication vs authorization
- secrets
- common browser/server trust boundaries
- basic injection/XSS/CSRF awareness where relevant

Advanced security engineering is outside the initial baseline.

---

# Layer A/B Cross-Cutting Area

## 17. Software Engineering / Existing Code

Use a small codebase or existing project to sample:

- navigating unfamiliar code
- understanding structure
- making a small change safely
- refactoring
- naming and readability
- separation of concerns
- handling requirements
- reasoning about maintainability

This should not become an architecture interview during the initial baseline.

---

# Layer C — Current Stack Extensions

These are not allowed to hide weak foundations.

## TypeScript

If currently active, screen:

- relationship between JavaScript and TypeScript
- inference
- unions / narrowing
- object/function typing
- generics at an appropriate level
- interpreting type errors
- using types to model domain constraints

TypeScript should be assessed after or alongside JavaScript reasoning because TypeScript builds on JavaScript.

---

## React

If currently active, screen:

- components
- props
- state
- rendering reasoning
- event handling
- state placement
- derived state
- composition
- effects / synchronization
- effect cleanup
- identifying unnecessary effects
- debugging React behavior

Framework API memorization should not dominate the assessment.

---

## Next.js

Only after relevant React/web foundations have been screened.

Possible areas:

- routing
- layouts
- server/client boundaries
- data fetching
- rendering
- forms / mutations
- caching concepts where relevant
- errors
- authentication integration
- deployment reasoning

Do not interpret Next.js familiarity as evidence that React or HTTP foundations are strong.

---

## PHP / Laravel

Treat as a separate current-stack extension.

If Laravel remains part of the active path, screen first:

### PHP

- language fundamentals
- arrays
- functions
- objects/classes where relevant
- error handling
- request-oriented code reasoning

Then Laravel:

- routing
- request lifecycle at a practical level
- controllers / actions
- validation
- database / Eloquent
- migrations
- relationships
- authentication / authorization basics
- feature testing
- debugging framework behavior

Do not deeply test Laravel if it is not actually part of the current active development direction.

---

# Cross-Cutting AI-Assistance Signal

AI usage is not a separate programming subject in the initial baseline.

Instead record it across tasks:

- Can the learner start without AI?
- Can they reason before prompting?
- Can they verify generated output?
- Can they explain generated code?
- Can they modify it?
- Can they debug it?
- Can they later solve a related problem independently?

This feeds the AI / Help Dependency gap model.

---

# Explicitly Deferred From the Initial Baseline

Do NOT deeply assess these at the beginning unless current goals make them necessary:

- advanced system design
- distributed systems
- cloud architecture
- Kubernetes
- advanced DevOps
- deep operating systems
- compiler theory
- advanced networking
- advanced cryptography/security
- advanced database internals
- advanced algorithms
- framework internals
- microservices
- advanced performance engineering
- mobile development

These may enter the skill graph later.

---

# Initial Screening Priority

The first diagnostic should prioritize:

1. Programming / JavaScript reasoning
2. Code reading
3. Debugging
4. Problem decomposition
5. Web / HTTP foundations
6. HTML / CSS / DOM
7. Git and development workflow
8. APIs / backend reasoning
9. Database fundamentals
10. Testing
11. Basic DSA / algorithmic reasoning

After this broad screen:

12. TypeScript
13. React
14. Next.js
15. PHP / Laravel

should be assessed according to current relevance and earlier findings.

---

# Important Rule

Do not spend equal time on every area.

The broad screen should be shallow.

Only areas showing:

- weakness
- uncertainty
- surprising strength
- possible prerequisite problems
- relevance to the immediate learning path

should receive deeper diagnostic tasks.

---

# What This Baseline Does Not Yet Decide

This step does NOT decide:

- exact task questions
- task difficulty
- how many tasks per area
- exact time limits
- final current stack
- final learning roadmap

Those decisions should follow from the diagnostic design and actual evidence.

---

# Research Basis

## ACM / IEEE-CS / AAAI — CS2023

Software Development competency draws particularly on:

- Software Development Fundamentals
- Algorithmic Foundations
- Foundations of Programming Languages
- Software Engineering

CS2023 emphasizes reading and writing programs, data structures and algorithms, program quality, modern development and testing tools, and broader software-development competency.

## MDN Curriculum

MDN identifies core web-developer foundations including:

- web standards
- semantic HTML
- CSS
- JavaScript
- accessibility
- design basics
- version control

Its extensions add areas such as testing, performance, security/privacy, APIs, and tooling.

## TypeScript Handbook — Official

TypeScript's official handbook explicitly treats TypeScript as building on JavaScript and recommends JavaScript background for learners who do not already have it.

## React — Official Documentation

React's current learning materials separate core UI concepts from escape hatches such as Effects and emphasize using Effects specifically for synchronization with external systems rather than general state derivation.

## Next.js — Official Documentation

Current Next.js documentation assumes familiarity with:

- HTML
- CSS
- JavaScript
- React

Its official learning path then adds full-stack framework concerns such as routing, data fetching, rendering, databases, mutations, error handling, and authentication.

## Git — Pro Git / git-scm.com

Used as an authoritative reference for practical version-control concepts such as commits, branching, merging, remotes, and conflict resolution.

---

# Status

Software Development Baseline Scope v0.1 is complete.

The next step is to design the **actual broad-screen diagnostic**, beginning with a small number of high-information tasks rather than writing dozens of isolated quiz questions.

# Broad-Screen Diagnostic Blueprint v0.1

## Purpose

The broad screen should discover the learner's current software-development capability using a **small number of high-information tasks**.

It should not become:

- a long trivia quiz
- a certification exam
- a LeetCode contest
- a framework interview
- a memorization test

The purpose is to decide **where deeper diagnosis is actually needed**.

---

# 1. Evidence-Centered Task Design

Every diagnostic task should explicitly define:

## Claim

What capability are we trying to understand?

## Evidence

What learner behavior would support or weaken that claim?

## Task

What activity can produce that evidence?

Example:

### Claim

The learner can reason about JavaScript scope and closures.

### Evidence

They can correctly predict unfamiliar code behavior and explain why.

### Task

A fresh code-reading problem involving nested functions and changing state.

A task should not be included merely because it looks difficult or interview-like.

---

# 2. Do Not Store the Exact Baseline Questions in Research Notes

RESEARCH.md should contain:

- diagnostic structure
- task specifications
- scoring/evidence rules
- coverage requirements

It should NOT contain the exact questions the learner will later receive.

Exact prompts should be generated when the diagnostic is administered.

Reasons:

- reduce rehearsal effects
- reduce memorized-answer effects
- allow fresh variants during reassessment
- make transfer evidence stronger

The system may preserve completed historical tasks after they have been attempted.

---

# 3. Broad Screen Structure

Initial target:

**7 high-information task families**

rather than dozens of isolated questions.

The actual number may adapt during administration.

---

# Task Family 1 — Read, Trace, Explain

## Main purpose

Screen:

- programming reasoning
- JavaScript fundamentals
- code reading
- control flow
- scope
- data changes
- asynchronous reasoning where appropriate

## Activity

The learner receives fresh code and must:

1. predict behavior/output
2. explain execution
3. identify important assumptions or edge cases

## Primary evidence dimensions

- Explain
- Read / Trace

## Possible follow-up

If tracing succeeds but explanation is weak:

probe conceptual understanding.

If explanation succeeds but prediction fails:

investigate execution-model weakness or slip.

---

# Task Family 2 — Independent Build

## Main purpose

Screen whether knowledge can be applied from a blank starting point.

Possible capabilities:

- functions
- data manipulation
- decomposition
- edge-case handling
- readable implementation
- basic testing behavior

## Activity

Build a small useful program or function from requirements.

The task should be unfamiliar enough that memorizing a tutorial solution is unlikely.

## Primary evidence dimensions

- Build / Apply
- Explain

## Initial mode

R0 + A0 — fully independent initial attempt.

Documentation may be introduced later if exact syntax becomes the blocker.

---

# Task Family 3 — Debugging

## Main purpose

Distinguish coding ability from debugging ability.

## Activity

Provide a realistic broken program or feature.

Observe whether the learner:

1. identifies expected behavior
2. reproduces the failure
3. forms a hypothesis
4. inspects useful evidence
5. narrows the cause
6. fixes it
7. explains the cause

## Primary evidence dimensions

- Debug
- Explain
- Read / Trace

The coach should observe the process, not merely the final fix.

---

# Task Family 4 — Feature Decomposition

## Main purpose

Screen problem-solving and decomposition.

## Activity

Give a small realistic feature request.

Before implementation, ask the learner to:

- clarify the requirement
- identify major pieces
- identify unknowns
- choose an implementation order
- describe likely data flow
- identify important edge cases

## Primary evidence

- decomposition
- planning
- transfer
- technical judgment

This task can expose gaps that isolated syntax exercises cannot.

---

# Task Family 5 — Web Reasoning

## Main purpose

Screen framework-independent web foundations.

Possible concepts:

- browser/client
- server
- HTTP
- request/response
- method choice
- status behavior
- JSON
- asynchronous interaction
- trust boundaries

## Activity

Use a concrete browser ↔ server scenario rather than definition-only questions.

The learner should reason about what happens and where responsibilities belong.

## Primary evidence dimensions

- Explain
- Apply
- Transfer

---

# Task Family 6 — Front-End Foundation Task

## Main purpose

Screen:

- semantic HTML
- CSS/layout
- DOM/events
- accessibility fundamentals

## Activity

Use a small UI containing several realistic issues or missing requirements.

Possible learner work:

- inspect markup
- identify semantic problems
- repair interaction
- reason about layout
- identify basic accessibility issues
- make a small behavior change

Do not require visual-design expertise.

## Primary evidence dimensions

- Read
- Debug
- Build / Apply

---

# Task Family 7 — Development Workflow / Data / Testing Scenario

This task family intentionally combines several lightweight professional-development signals.

## Possible coverage

- Git reasoning
- package/project workflow
- API reasoning
- database fundamentals
- tests
- reading an error
- documentation usage

## Activity

Use a small project scenario rather than command trivia.

Examples of capabilities to sample:

- interpret a failing test
- decide what should be tested
- reason about a simple data model
- identify an appropriate API operation
- describe a safe Git action
- locate useful documentation

If a specific area appears weak or uncertain, generate a focused follow-up later.

---

# Optional Probe — Basic DSA / Algorithmic Reasoning

Do not automatically run a long algorithm section.

A compact probe may test:

- choosing a suitable data structure
- reasoning about efficiency
- implementing a small unfamiliar problem
- explaining trade-offs

If evidence is clearly strong or clearly weak, stop.

If the result is ambiguous and DSA matters to the current path, investigate later.

---

# 4. Adaptive Follow-Ups

The seven task families are not seven fixed exams.

After each task:

## Clear strong evidence

Do not immediately generate more similar tasks.

Record provisional state and continue.

## Clear weakness

Generate one targeted probe if needed to identify the cause.

## Ambiguous result

Use a different evidence format.

Example:

Build failed.

Possible causes:

- concept gap
- recall gap
- decomposition gap
- syntax/reference issue
- misunderstanding requirement

A follow-up should distinguish these possibilities.

---

# 5. Help Protocol During Baseline

Core diagnostic attempts should normally begin at:
R0 + A0 — Fully Independent
when unaided performance is what the task intends to measure.
If stuck:

1. preserve the initial R0 + A0 result
2. introduce the smallest useful instructional assistance
3. record the new A-level
4. continue observing
   Example:
   R0 + A0 = Fail
   R0 + A2 = succeeds quickly
   This is more informative than simply recording:
   Pass.
   For tasks intended to measure realistic professional performance, R1 + A0 may instead be the appropriate independent condition.

---

# 6. Baseline Modes

Tasks should explicitly state the allowed mode.

## Mode A — Independent

Default condition:
R0 + A0
Used when testing unaided recall, reasoning, or performance.

## Mode B — Reference-Allowed

Allowed conditions:
R0/R1 + A0
Official documentation or normal reference material may be used.
No instructional guidance is provided.

## Mode C — Diagnostic Assistance

After the initial independent evidence has been captured, instructional assistance may escalate:
A1 → A2 → A3 → A4
Reference use continues to be recorded separately.

---

# 7. AI Restriction

During R0 + A0 independent baseline tasks:

Do not use:

- ChatGPT
- Claude
- Copilot
- AI code generation
- AI debugging

unless the task specifically measures AI-assisted work.

After the initial R0 + A0 result has been recorded, AI may become part of the diagnostic process and its assistance level must be recorded as A1–A4.

This is not an anti-AI rule.

It is necessary to separate:

current independent ability

from:

ability while assisted.

---

# 8. Documentation Is Context-Dependent

Do not treat documentation lookup as failure when the intended skill does not require memorization.

Example:

Looking up exact Git command syntax may be acceptable.

Not knowing the conceptual difference between commit, branch, and merge is a different issue.

Similarly:

Looking up an API method name

is different from:

not knowing what kind of operation is required.

---

# 9. No Single Overall Score

The broad screen should NOT output:

82/100  
Intermediate developer  
7.4/10 programmer

Instead produce an evidence map.

Example:

Programming reasoning:
Strong signal

Code reading:
Strong signal

Independent build:
Working

Debugging:
Suspected weakness

Decomposition:
Strong signal

HTTP/web reasoning:
Uncertain

HTML semantics:
Working

CSS debugging:
Weak signal

Git:
Strong practical evidence

Database:
Insufficient evidence

Testing:
Working

Retention:
Untested

These remain provisional until enough evidence accumulates.

---

# 10. Evidence Capture Per Task

For each meaningful diagnostic attempt record:

- task family
- primary skill(s)
- supporting skill(s)
- evidence type
- diagnostic mode
- result
- help level
- number of meaningful attempts
- error/gap signals
- novelty
- explanation quality where relevant
- artifact/code where useful
- follow-up required or not

Do not require the learner to manually complete this record.

The AI coach should eventually derive most of it.

---

# 11. Stop Rules

A diagnostic should stop probing an area when enough evidence exists to choose the next action.

Examples:

### Strong enough

Multiple relevant behaviors are independently correct and reasoning is coherent.

→ Continue to another area.

### Weak enough

A repeatable gap has been identified and additional same-day testing will not change the learning decision.

→ Stop and record the gap.

### Uncertain but low priority

Evidence is incomplete but the area is not currently important.

→ Leave as untested/uncertain.

### Uncertain and important

→ Schedule targeted diagnosis.

The goal is not maximum measurement.

The goal is sufficient evidence for a useful learning decision.

---

# 12. Protect Against Fatigue

Do not require all task families in one long sitting.

Preferred initial design:

**Baseline Session A**
Programming-heavy evidence.

Possible families:

- Read / Trace
- Build
- Debug
- Decomposition

**Baseline Session B**
Web / professional-development evidence.

Possible families:

- Web reasoning
- Front-end foundation
- Workflow/data/testing
- optional DSA probe

This two-session structure is a practical starting design, not a scientifically fixed requirement.

If fatigue or concentration decline becomes visible, stop and continue later.

---

# 13. Task Difficulty

Do not begin automatically at absolute beginner difficulty.

The learner has previous development exposure.

Start with tasks that can discriminate between:

- fragile beginner knowledge
- functional working knowledge
- stronger independent capability

Then adapt:

too easy
→ increase complexity

too difficult because of a clear prerequisite
→ probe prerequisite

Difficulty should change based on evidence.

---

# 14. Fresh Variants

Later reassessment should not simply repeat the same task.

Change:

- data
- domain/context
- code structure
- surface details
- required decision

while preserving the underlying skill.

This creates stronger transfer evidence.

---

# 15. Baseline Output

After broad screening, LearningOS should generate:

## Strong areas

Likely candidates for compressed learning or skipping basic material.

## Working / needs-strengthening areas

Need strengthening rather than complete restart.

## Suspected gaps

Need targeted diagnosis.

## Confirmed gaps

Clear learning targets.

## Unknown areas

Insufficient evidence.

## Dependency signals

Possible prerequisite problems.

## AI/help dependency signals

Where assisted and independent ability differ substantially.

## Recommended next diagnostic or learning action

Only then should the learning path begin adapting.

---

# 16. Do Not Reveal Solutions During the Initial Attempt

Before the learner commits to an answer:

The coach should not accidentally expose:

- expected output
- bug location
- correct approach
- hidden concept being tested
- solution structure

After the attempt, feedback can be progressively provided according to the AI Coach rules.

---

# 17. Baseline Integrity

The learner is not expected to "win" the baseline.

Finding failures is useful.

Finding unexpectedly strong areas is useful.

Finding large unknown regions is also useful.

The objective is to obtain an accurate learning map rather than maximize correct answers.

---

# Research Basis

## ETS — Evidence-Centered Design

Mislevy, Almond & Lukas (2003).

A Brief Introduction to Evidence-Centered Design.

ETS Research Report RR-03-16.

The design principle used here is:

learner claim
→ required evidence
→ task capable of eliciting that evidence.

---

## AERA / APA / NCME

Standards for Educational and Psychological Testing, 2014.

Key principle applied:

assessment results should be interpreted only for the intended use supported by relevant evidence.

LearningOS therefore avoids treating one diagnostic task or one numeric score as proof of overall programming ability.

---

## ACM / IEEE-CS / AAAI — CS2023

Software Development Fundamentals includes:

- fundamental programming concepts
- data structures
- algorithms
- testing
- debugging
- development tools
- reading and understanding programs

The broader Software competency area also emphasizes:

- problem decomposition
- algorithmic thinking
- analytical reasoning
- development of complete and correct solutions

These areas inform the baseline coverage.

---

## MDN Curriculum — Mozilla

The current MDN Curriculum Core identifies foundational web-development areas including:

- web standards
- semantic HTML
- CSS
- JavaScript
- accessibility
- version control

MDN explicitly presents this curriculum as usable for designing learning programs and assessment specifications.

This informs the web portion of the baseline.

---

# Evidence Strength

## Strong / authoritative

- ETS Evidence-Centered Design
- AERA / APA / NCME Testing Standards
- ACM / IEEE-CS / AAAI CS2023
- Mozilla MDN Curriculum

## LearningOS-specific design decisions

The following are our provisional design choices rather than universal research findings:

- seven task families
- splitting the baseline into two sessions
- exact stop rules
- exact order of task families

These must be validated during actual use and revised if they create too much friction or insufficient diagnostic information.

---

# Status

Broad-Screen Diagnostic Blueprint v0.1 is complete.

Exact baseline prompts have intentionally NOT been created in this document.

The next implementation step is to create the **Baseline Administration Protocol**, then begin the first real diagnostic session with fresh tasks.
