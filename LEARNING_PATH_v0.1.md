# Learning Path v0.1

## Purpose

This path converts the current baseline evidence and bookmark audit into an active learning direction.

It is intentionally **not** a restart-from-zero curriculum.

The current strategy is:

> **React-led learning + targeted JavaScript reinforcement**

React provides the main practical context. JavaScript gaps are repaired when they become relevant instead of repeating an entire beginner JavaScript course.

IELTS is a **secondary active track**.

---

# 1. Current Priorities

## Primary — Software Development

Current order:

1. React foundations + targeted JavaScript repair
2. Testing fundamentals
3. Web / API integration
4. HTML / accessibility reinforcement
5. React consolidation
6. TypeScript
7. Next.js / broader full-stack work
8. DSA as a separate later track

## Secondary — IELTS

Use the resources already available.

Do not search for more IELTS resources unless the current stack fails to meet a specific need.

## Paused / Later

- DSA
- PHP / Laravel
- Japanese
- UX
- career preparation unless needed

---

# 2. Learning Strategy

## Main rule

Do not study JavaScript as a long isolated prerequisite before React.

Instead:

```text
React task
  ↓
difficulty or bug appears
  ↓
identify underlying JavaScript gap
  ↓
targeted JavaScript repair
  ↓
retry React task
  ↓
fresh independent check later
```

Example:

```text
React state update
  ↓
nested object changes unexpectedly
  ↓
review references + shallow copying
  ↓
fix update without mutation
  ↓
new state-update task without help
```

This keeps the work practical while still repairing foundational gaps.

---

# 3. Phase 1 — React Foundations + JavaScript Repair

## Primary Resource

**React official Learn**

Role:

- primary learning source
- first place for React concepts
- use built-in challenges where useful

## Supporting JavaScript Resource

**javascript.info**

Role:

- targeted reference only
- do not read cover-to-cover
- use when a specific JavaScript weakness blocks React reasoning

## Main Topics

### React

- components
- JSX
- props
- rendering lists
- events
- state
- state as a snapshot
- object state
- array state
- forms
- conditional rendering

### JavaScript gaps to repair inside this phase

- object references
- mutation vs reassignment
- shallow copying
- nested object copying
- array references
- `map`, `filter`, `find`, `findIndex`
- `for...in` vs `for...of`
- truthy / falsy edge cases
- closure behavior when it appears naturally
- reference equality with `===`

## Why this phase comes first

The baseline showed that practical programming ability already exists, but reference/mutation semantics are uneven.

React state work naturally exercises exactly those concepts.

## Exit Evidence

Move forward when fresh tasks show that I can:

- build a small React feature without step-by-step guidance
- update object and array state without accidental mutation
- explain why a shallow copy may still share nested objects
- debug a simple mutation/reference bug
- correctly use common array methods in realistic code

Same-day success is not enough to mark these skills Retained.

---

# 4. Phase 2 — Testing Fundamentals

Testing should begin early enough that it becomes part of development rather than a final deployment ritual.

## Concepts

- behavior vs implementation-detail testing
- happy path
- negative cases
- boundary cases
- user-visible behavior
- component interaction
- simple integration thinking

## Suggested Tooling When This Phase Begins

- Vitest
- React Testing Library
- `user-event`

These are supporting tools, not a new giant curriculum.

## Learning Pattern

For each small feature:

1. identify expected behavior
2. write or describe important test cases
3. implement or fix the feature
4. run tests
5. add a boundary / failure case
6. later solve a similar testing task without assistance

## Exit Evidence

I should be able to independently answer:

- what behavior should be tested?
- what is the boundary?
- what could fail?
- what should the user observe?
- which test is tied too closely to implementation details?

And write basic component behavior tests with limited reference use.

---

# 5. Phase 3 — Web / API Integration

Use React in a small application that talks to an API.

## Topics

- GET vs POST vs PATCH vs DELETE
- request / response lifecycle
- loading state
- error state
- validation
- client validation vs server validation
- common HTTP status reasoning
- JSON request / response handling
- CRUD flows

## Practice Goal

Build features such as:

- load a list
- create an item
- edit an item
- delete an item
- display validation errors
- handle failed requests

## JavaScript Repair Continues

If async behavior, callbacks, closures, object updates, or array transformations cause problems, pause only long enough to repair that exact prerequisite.

## Exit Evidence

Independently explain and implement a small end-to-end CRUD flow and diagnose basic failures across:

```text
UI → request → server/API → response → UI state
```

---

# 6. Phase 4 — HTML and Accessibility Reinforcement

This should be integrated into the React UI rather than treated as a separate long course.

## Focus

- correct native elements
- buttons vs clickable `div`
- labels and inputs
- checkbox labeling
- forms
- keyboard behavior
- semantic structure
- accessible names

## Practice Rule

Before styling a component heavily, ask:

> Can this be built with the correct native HTML element first?

Testing Library queries can reinforce this because accessible roles and labels become directly useful in tests.

## Exit Evidence

Build common forms and interactive controls with appropriate semantic HTML and explain the key accessibility choices.

---

# 7. Phase 5 — React Consolidation

After the first practical React/API work, deepen React rather than immediately jumping frameworks.

## Topics

- choosing state structure
- lifting state
- controlled vs uncontrolled components
- preserving / resetting state
- reducers when justified
- reusable components
- separating data and presentation where useful
- debugging state flow

## Resources

- React official Learn → primary
- Scrimba React → optional practice
- React beginner project repository → project ideas
- Bulletproof React → reference only after enough project experience

## Exit Evidence

Build a small but non-trivial React app from requirements with:

- multiple components
- forms
- state
- list operations
- API interaction
- tests
- reasonable semantic HTML

---

# 8. Phase 6 — TypeScript

TypeScript starts after JavaScript reference/state reasoning is more stable.

## Goal

Use TypeScript to improve correctness, not to hide uncertain JavaScript fundamentals.

## Focus

- primitive and object types
- arrays
- function parameters / returns
- unions
- optional properties
- interfaces / type aliases
- narrowing
- React props
- event types
- API response types

## Resource Role

Existing TypeScript bookmarks remain **Later** until this phase.

---

# 9. Phase 7 — Next.js / Broader Full Stack

Only after React fundamentals are reasonably independent.

## Candidate Resources

- Next.js official Learn
- Full Stack Open
- selected full-stack practice resources

Do not run several full-stack curricula in parallel.

Choose one primary path when this phase starts.

---

# 10. DSA Track — Separate Later Track

Current baseline evidence suggests DSA is largely **not learned yet**, not merely rusty.

Therefore DSA should not be mixed into the immediate React repair work.

When activated:

1. choose one structured DSA learning source
2. choose one practice platform
3. use the saved DSA MCQ resource as retrieval practice
4. add coding tasks and complexity reasoning

Possible existing choices include:

- Striver A2Z
- NeetCode
- LeetCode

Do not run all of them as simultaneous curricula.

---

# 11. IELTS — Secondary Active Track

IELTS can run alongside Software Development without becoming another resource-management project.

## Current Active Stack

Use a small set only:

- IELTS Fundamentals course, if access remains active
- official IELTS preparation resources
- official IELTS writing preparation
- official/sample practice tests
- speaking/writing output tools when useful

## Supporting Resources

Keep resources such as IELTS Liz, BBC, British Council, Cambridge, Engnovate, grammar sites, etc. as practice/reference rather than parallel curricula.

## Operating Rule

Do not search for new IELTS resources unless there is a clearly identified gap that the current collection cannot address.

## Suggested Attention Balance

Default:

- Software Development remains the main track.
- IELTS receives smaller but consistent sessions.

The exact schedule should be decided from available time rather than hard-coded here.

---

# 12. Evidence Rules During the Path

Do not mark progress only because:

- a lesson was watched
- a page was read
- a challenge was copied
- code worked with heavy assistance

Use the LearningOS evidence dimensions:

1. Explain
2. Read / Trace
3. Build / Apply
4. Debug
5. Adapt / Transfer
6. Retain

## Assistance

Track separately:

### Reference Use

- R0 — no reference
- R1 — lookup/reference
- R2 — worked example / structural reference

### Instructional Assistance

- A0 — none
- A1 — orientation
- A2 — small hint
- A3 — guided scaffolding
- A4 — substantial solution exposure

A task completed after A3/A4 should not immediately count as strong independent evidence.

---

# 13. Retention

Skills introduced or repaired during a session are not automatically Retained.

Use later fresh tasks.

Examples:

- new React state bug
- changed object shape
- different array operation
- new form requirement
- new API endpoint
- fresh test case

Natural reuse in projects can count as review evidence.

---

# 14. Resource Policy

The bookmark audit is the resource inventory.

The learning path decides what is active.

Therefore:

- do not activate a resource only because it is bookmarked
- do not start multiple overlapping courses
- add a new resource only when it solves a specific unmet need
- prefer official/primary documentation where appropriate
- use project/practice resources for retrieval and transfer

---

# 15. Immediate Next Step

Create **Learning Cycle 1**.

Cycle 1 should focus on:

> **React fundamentals + object/array state + targeted JavaScript reference/immutability repair**

It should contain:

- a small set of React lessons
- one small build
- one debugging task
- one JavaScript repair block only where needed
- one independent reassessment
- a delayed review target

After Cycle 1, update the skill map from actual evidence instead of assuming the path worked.
