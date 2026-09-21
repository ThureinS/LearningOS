# LearningOS Source Registry

## Purpose

This file is the canonical registry for research sources used by LearningOS.

RESEARCH.md contains findings, interpretations, limitations, and LearningOS implications.

SOURCES.md answers:

- What is the original source?
- What type of evidence is it?
- How strong or authoritative is it?
- Which LearningOS claims does it support?
- What are its important limitations?
- How can it be uniquely identified?

A source appearing here does not mean every conclusion drawn from it is automatically correct.

Claims must stay within what the source actually supports.

---

# Source Quality Labels

## A — Authoritative / Primary Standard or Official Framework

Examples:

- official standards
- official curricular guidelines
- official technical documentation
- original institutional framework

## B — High-Level Research Synthesis

Examples:

- systematic review
- meta-analysis

## C — Individual Peer-Reviewed Study

Useful evidence, but conclusions should normally be narrower than evidence from a strong synthesis.

## D — Preliminary / Emerging Research

Examples:

- preprint
- early controlled study
- industry research without substantial independent replication

Useful for emerging topics, but should be clearly labeled provisional.

## E — Community / Practitioner Evidence

Examples:

- blogs
- forums
- Reddit
- informal practitioner reports

Useful mainly for workflows, usability, and real-world experience.

Not sufficient by itself for strong learning-science claims.

---

# Core Verified Sources

## SRC-001 — Testing Effect in Classrooms

### Citation

Yang, C., Luo, L., Vadillo, M. A., Yu, R., & Shanks, D. R. (2021).

Testing (quizzing) boosts classroom learning: A systematic and meta-analytic review.

Psychological Bulletin, 147(4), 399–435.

DOI: 10.1037/bul0000309

### Evidence Type

Meta-analysis / systematic review

### Quality

B — High-Level Research Synthesis

### Evidence Base

222 independent studies.

48,478 learners.

### Supports

- retrieval/testing can improve classroom learning
- retrieval is generally more useful than passive restudy for durable learning
- feedback, repetition, timing, task format, and other conditions moderate the effect

### Does Not Establish

- one universal retrieval schedule
- one specific LearningOS testing cadence
- that every programming skill should be assessed with quizzes

### LearningOS Uses

- Retrieval Practice
- Monitoring Cadence
- Retention / reassessment principles

---

## SRC-002 — Distributed Practice / Spacing

### Citation

Cepeda, N. J., Pashler, H., Vul, E., Wixted, J. T., & Rohrer, D. (2006).

Distributed practice in verbal recall tasks: A review and quantitative synthesis.

Psychological Bulletin, 132(3), 354–380.

DOI: 10.1037/0033-2909.132.3.354

### Evidence Type

Meta-analysis

### Quality

B — High-Level Research Synthesis

### Evidence Base

317 experiments.

184 articles.

839 assessments of distributed practice.

### Supports

- spaced learning generally improves long-term retention relative to massed practice
- useful spacing depends partly on the desired retention interval
- there is no reason to assume one fixed interval schedule is universally optimal

### Important Limitation

The research focuses heavily on verbal recall tasks.

Exact timing should not automatically be transferred to complex programming performance.

### LearningOS Uses

- Spacing
- Retention scheduling
- delayed reassessment

---

## SRC-003 — Educational Feedback

### Citation

Wisniewski, B., Zierer, K., & Hattie, J. (2020).

The Power of Feedback Revisited: A Meta-Analysis of Educational Feedback Research.

Frontiers in Psychology, 10, 3087.

DOI: 10.3389/fpsyg.2019.03087

### Evidence Type

Meta-analysis

### Quality

B — High-Level Research Synthesis

### Evidence Base

435 studies.

994 effect sizes.

More than 61,000 learners.

### Supports

- feedback can improve learning
- feedback effects vary substantially
- informational content of feedback matters
- feedback should not be treated as one uniform intervention

### Does Not Establish

- that more feedback is always better
- that immediate full solutions are optimal
- the exact LearningOS A0–A4 assistance scale

### LearningOS Uses

- corrective feedback
- AI Coach behavior
- monitoring and reassessment

---

## SRC-004 — Evidence-Centered Design

### Citation

Mislevy, R. J., Almond, R. G., & Lukas, J. F. (2003).

A Brief Introduction to Evidence-Centered Design.

ETS Research Report RR-03-16.

### Evidence Type

Original assessment-design framework / research report

### Quality

A — Authoritative Primary Framework

### Supports

Assessment design that explicitly connects:

- claims about learner capability
- evidence needed to support those claims
- tasks capable of eliciting that evidence

### LearningOS Uses

- Baseline Method
- Broad-Screen Diagnostic Blueprint
- task design
- interpretation of diagnostic evidence

### Important Limitation

LearningOS adapts the framework for personal learning diagnostics.

Its exact task families and stop rules are LearningOS design decisions.

---

## SRC-005 — Standards for Educational and Psychological Testing

### Citation

American Educational Research Association,
American Psychological Association,
& National Council on Measurement in Education. (2014).

Standards for Educational and Psychological Testing.

### Evidence Type

Professional testing standard

### Quality

A — Authoritative Standard

### Supports

- assessment interpretation should be tied to intended use
- validity concerns interpretations and uses of assessment evidence
- assessment results should not be generalized beyond what the evidence supports
- fairness and accessibility matter in assessment design

### LearningOS Uses

- avoiding false precision
- avoiding one-score judgments of programming ability
- interpreting baseline evidence only for learning decisions

### Important Limitation

LearningOS is not a formal standardized test or certification system.

---

## SRC-006 — CS2023

### Citation

ACM / IEEE Computer Society / AAAI.

Computer Science Curricula 2023.

### Evidence Type

Official curricular guideline

### Quality

A — Authoritative Curriculum Framework

### Supports

For LearningOS purposes, relevant areas include:

- Software Development Fundamentals
- Algorithmic Foundations
- Foundations of Programming Languages
- Software Engineering

CS2023 also emphasizes capabilities such as:

- reading and writing programs
- data structures and algorithms
- development and testing tools
- decomposition
- algorithmic thinking
- analytical reasoning

### LearningOS Uses

- external skill-map reference
- Software Development baseline scope
- identifying possible blind spots

### Important Limitation

CS2023 is designed for computer-science curricula.

LearningOS is not attempting to reproduce a university CS degree.

---

## SRC-007 — MDN Curriculum

### Citation

Mozilla Developer Network.

MDN Curriculum.

### Evidence Type

Official web-development curriculum

### Quality

A — Authoritative Domain Curriculum

### Current Core Areas Relevant to LearningOS

- web standards
- semantic HTML
- CSS
- JavaScript
- accessibility
- design fundamentals
- version control

### LearningOS Uses

- web-development baseline scope
- checking framework-independent web foundations

### Important Limitation

MDN Curriculum focuses primarily on front-end web development.

It is not a complete software-engineering or computer-science curriculum.

---

# Provenance Rules

## Rule 1

Prefer the original paper, official standard, or official documentation over a blog summarizing it.

## Rule 2

For important learning-science claims, prefer:

meta-analysis / systematic review

over:

one isolated study

when suitable research synthesis exists.

## Rule 3

Individual studies may be used when:

- the topic is new
- stronger syntheses do not yet exist
- the claim is explicitly narrow
- limitations are recorded

## Rule 4

Emerging generative-AI research must be labeled more cautiously than mature findings such as retrieval practice and spacing.

## Rule 5

A LearningOS design decision must not be presented as though a paper directly validated the exact design.

Examples:

- seven diagnostic task families
- A0–A4 assistance categories
- weekly evidence synthesis
- exact state labels

These are evidence-informed LearningOS designs.

## Rule 6

Every major Research Topic should eventually identify which SRC entries support it.

## Rule 7

If a source is later found to be weak, misrepresented, obsolete, or contradicted by stronger evidence:

- do not silently delete the history
- update the finding
- record the reason
- replace or downgrade the source when appropriate

---

# Audit Status

This registry is incomplete.

SRC-001 through SRC-007 are the first verified core sources.

Remaining research sections still need source-by-source validation and mapping.

## SRC-008 — Successive Relearning and Long-Term Retention

### Citation

Rawson, K. A., Vaughn, K. E., Walsh, M., & Dunlosky, J. (2018).

Investigating and explaining the effects of successive relearning on long-term retention.

Journal of Experimental Psychology: Applied, 24(1), 57–71.

DOI: 10.1037/xap0000146

### Evidence Type

Controlled experimental study

### Quality

C — Individual Peer-Reviewed Study

### Supports

- successful performance within one learning session does not guarantee strong long-term retention
- relearning across multiple sessions can substantially improve later retention
- delayed performance provides direct evidence about what remains available after time has passed

### Important Limitation

This is an individual experimental study rather than a broad meta-analysis.

Its exact procedures should not be treated as a universal schedule for programming skills.

### LearningOS Uses

- delayed reassessment
- Retained state
- successive relearning
- distinguishing immediate success from durable retention

## SRC-009 — Context-Sensitive Help-Seeking Assessment

### Citation

Aleven, V., Roll, I., McLaren, B. M., & Koedinger, K. R. (2010).

Automated, Unobtrusive, Action-by-Action Assessment of Self-Regulation During Learning With an Intelligent Tutoring System.

Educational Psychologist, 45(4), 224–233.

DOI: 10.1080/00461520.2010.517740

### Evidence Type

Peer-reviewed research / review article

### Quality

C — Peer-Reviewed Non-Synthesis Evidence

### Supports

- help-seeking behavior should be interpreted in the context in which it occurs
- fine-grained learner actions can provide useful assessment information
- help behavior is not adequately represented by a simple binary "used help / did not use help"
- feedback can be driven by observed help-seeking patterns

### Important Limitation

The work focuses on help seeking inside intelligent tutoring systems.

It does not validate the exact LearningOS R0–R2 / A0–A4 model.

It also reported improvement in help-seeking behavior rather than a clear improvement in domain learning from that intervention.

### LearningOS Uses

- Help Usage Matters
- Instructional Assistance
- Process Data
- AI / Help Dependency signals

## SRC-010 — Knowledge Tracing Survey

### Citation

Abdelrahman, G., Wang, Q., & Nunes, B. (2023).

Knowledge Tracing: A Survey.

ACM Computing Surveys, 55(11), Article 224, 1–37.

DOI: 10.1145/3569576

### Evidence Type

Comprehensive peer-reviewed research survey

### Quality

B — High-Level Research Synthesis

### Supports

- learner knowledge state is not directly observed and may be inferred from historical interactions
- repeated learner responses can be used to update estimates of knowledge state
- knowledge-tracing models distinguish observed correctness from underlying knowledge
- classic Bayesian Knowledge Tracing includes slip and guess parameters
- some later models explicitly account for forgetting and time between interactions
- skill / knowledge-component representation is an important modeling assumption

### Important Limitation

Knowledge-tracing research usually operates in structured educational environments with clearly defined questions and skills.

LearningOS includes richer evidence such as:

- debugging
- project work
- code artifacts
- transfer
- AI assistance

Therefore LearningOS should not assume that an existing knowledge-tracing model directly fits software-development learning.

### LearningOS Uses

- interpreting repeated evidence
- distinguishing isolated errors from persistent gaps
- retention signals
- possible future knowledge-state modeling
- avoiding one-attempt mastery conclusions

## SRC-011 — Guided vs Unrestricted AI in Programming Education

### Citation

Noraset, T., Supratak, A., Ragkhitwetsagul, C., Worathong, N., & Tuarob, S. (2026).

Evaluating lab assistant chatbot on student learning and behaviors in a programming short course.

Computers and Education: Artificial Intelligence, 10, Article 100527.

DOI: 10.1016/j.caeai.2025.100527

### Evidence Type

Controlled peer-reviewed experimental study

### Quality

C — Individual Peer-Reviewed Study

### Evidence Base

42 participants in a short Python programming course.

### Supports

- guided AI assistance can produce different learning outcomes from unrestricted solution-oriented chatbot access
- the Assistant chatbot, which provided guidance without direct solutions, showed greater pre-to-post improvement than the Unrestricted chatbot group
- AI interaction design can matter for programming learning

### Important Limitation

This was:

- one controlled study
- a relatively small sample
- a short programming course
- a specific chatbot design

It does not establish that every scaffolded AI tutor will outperform unrestricted AI in every context.

### LearningOS Uses

- AI Learning Coach behavior
- progressive instructional assistance
- avoiding immediate solution exposure
- distinguishing learning-oriented AI from unrestricted answer generation

---

## SRC-012 — Performance vs Learning in AI-Supported Programming

### Citation

Bassner, P., Lenk-Ostendorf, B., Beinstingel, R., Wasner, T., & Krusche, S. (2026).

Less stress, better scores, same learning: The dissociation of performance and learning in AI-supported programming education.

Computers and Education: Artificial Intelligence, 10.

DOI: 10.1016/j.caeai.2025.100537

### Evidence Type

Randomized peer-reviewed experimental study

### Quality

C — Individual Peer-Reviewed Study

### Evidence Base

275 university students.

Conditions included:

- scaffolded AI tutor
- unrestricted ChatGPT
- no-AI / traditional-resource control

### Supports

- better task performance during AI-assisted work does not necessarily imply greater learning
- both AI-supported groups achieved better programming-task performance than the control group
- those performance gains did not translate into greater conceptual learning or code-comprehension performance
- the scaffolded tutor showed motivational benefits not observed in the same way with unrestricted AI

### Important Limitation

This is one study in a specific university programming context.

The results do not imply that AI assistance is universally harmful or universally beneficial.

### LearningOS Uses

- separating task completion from learning
- AI Learning Coach behavior
- avoiding mastery conclusions from AI-assisted task performance alone
- motivation / assistance design

---

## SRC-013 — AI Assistance and Coding Skill Formation

### Citation

Shen, J. H., & Tamkin, A. (2026).

How AI Impacts Skill Formation.

arXiv:2601.20245.

### Evidence Type

Randomized experimental preprint / industry research

### Quality

D — Preliminary / Emerging Research

### Supports

In the studied setting:

- AI assistance could reduce later conceptual understanding, code-reading ability, and debugging performance
- different AI-use patterns were associated with different learning outcomes
- using AI while remaining cognitively engaged may differ from delegating the work

### Important Limitation

This evidence is preliminary.

The work is:

- a preprint
- based on a specific programming-learning task
- focused on relatively short-term skill formation
- not direct evidence about every programming workflow
- not direct evidence about agentic coding environments such as Claude Code

The authors themselves note that their setup differs from agentic coding products.

### LearningOS Uses

- AI dependency signals
- preserving learner reasoning
- explanation and verification behavior
- separating productivity from skill formation

---

## SRC-014 — Self-Explanation Meta-Analysis

### Citation

Bisra, K., Liu, Q., Nesbit, J. C., Salimi, F., & Winne, P. H. (2018).

Inducing Self-Explanation: a Meta-Analysis.

Educational Psychology Review, 30, 703–725.

DOI: 10.1007/s10648-018-9434-x

### Evidence Type

Meta-analysis

### Quality

B — High-Level Research Synthesis

### Evidence Base

64 research reports.

69 effect sizes.

Overall weighted mean effect:

g = 0.55

### Supports

- prompting learners to generate self-explanations can improve learning
- self-explanation can be useful across multiple instructional conditions and subject areas

### Important Limitation

The meta-analysis does not establish that:

- every successful programming task needs a self-explanation
- longer explanations are always better
- the exact LearningOS AI Coach prompt style is optimal

Self-explanation should be used where it provides useful diagnostic or learning value rather than mechanically after every task.

### LearningOS Uses

- AI Coach self-explanation prompts
- learner-generated reasoning
- checking whether successful performance is conceptually understood

---

## SRC-015 — AI Chatbots in Programming Education Meta-Analysis

### Citation

Deng, H., Chen, H., & Dong, Y. (2026).

Do AI Chatbots Improve Students' Learning Performance in Programming Education? Evidence from a Meta-Analysis.

Journal of Educational Computing Research, 64(5), 1323–1359.

DOI: 10.1177/07356331261424211

### Evidence Type

Meta-analysis

### Quality

B — High-Level Research Synthesis

### Evidence Base

32 empirical studies published between 2015 and 2025.

### Supports

Across the included studies:

- AI chatbots showed an overall positive average effect on programming-learning performance
- effects differed according to study and implementation characteristics
- chatbot design and research conditions matter

Reported average effects included:

- small-to-medium effect on posttest performance
- medium-to-large effect on practice performance

### Important Limitation

The included studies differ substantially in:

- chatbot design
- learner population
- programming context
- research design
- outcome measurement

The average effect does not establish that unrestricted AI is optimal or that one tutoring design works universally.

The meta-analysis also does not validate the exact LearningOS AI Coach rules.

### LearningOS Uses

- broader context for AI-supported programming education
- avoiding overly negative or overly positive conclusions about AI
- treating AI interaction design as an empirical question
