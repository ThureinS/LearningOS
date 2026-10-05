# Knowledge Inbox v0.1

## Purpose

Use this file whenever I:

- learn something new
- notice something I want to remember
- discover a concept I want to understand better
- find a topic I want to learn later
- notice a useful command, fact, pattern, or rule

The goal is **not** to save everything.

The goal is to capture useful knowledge, route it to the right kind of practice, and avoid forgetting important things.

---

# Core Rule

When something new appears, first ask:

> **Do I need to remember this, understand/use this, or just be able to look it up later?**

Use one of these routes:

## 1. Remember

Best for:

- vocabulary
- short facts
- status-code meanings
- commands
- terminology
- formulas or definitions worth recalling

Route:

```text
Capture
→ retrieval question/card
→ delayed recall
→ keep only if still useful
```

Possible tool later:

- Anki / FSRS

Do **not** create flashcards for everything.

---

## 2. Understand / Use

Best for:

- programming concepts
- debugging
- React state
- API reasoning
- testing
- architecture
- DSA problem solving
- procedural skills

Route:

```text
Capture
→ explain
→ use in a task
→ debug or adapt
→ fresh task later
→ delayed reassessment
```

For this type, project/task practice is more important than memorizing a sentence.

---

## 3. Reference Only

Best for:

- syntax I can easily look up
- API details
- long commands
- library options
- documentation links
- implementation examples

Route:

```text
Capture
→ save reference
→ no scheduled review
```

Do not create review debt for things that are easy to look up.

---

## 4. Want to Learn

Best for:

- interesting topics discovered during study/work
- future technologies
- prerequisites for a later project
- concepts that are useful but not current priority

Route:

```text
Capture
→ mark why it matters
→ set trigger / prerequisite
→ keep Later
→ activate only when relevant
```

---

# Capture Template

Copy this block for a new item:

```markdown
## [Short title]

- Date:
- Source/context:
- What I learned / want to learn:
- Why it matters:
- Type: Remember / Understand-Use / Reference / Want-to-Learn
- Priority: Now / Soon / Later
- Related skill:
- Next action:
- Delayed check:
- Notes:
```

Keep entries short.

A capture should usually take less than 2 minutes.

---

# Routing Rules

## If Type = Remember

Turn it into a simple retrieval question only if recall matters.

Example:

```text
Q: What does HTTP 404 mean?
A: The requested resource was not found.
```

Then review later.

---

## If Type = Understand-Use

Do not stop at notes.

Create evidence using one or more of:

- explain from memory
- trace code
- build something
- fix a bug
- change the requirement
- apply the concept in another context

Use the LearningOS mastery dimensions:

1. Explain
2. Read / Trace
3. Build / Apply
4. Debug
5. Adapt / Transfer
6. Retain

---

## If Type = Reference

Save the useful link, snippet, or note.

No review schedule unless it later becomes important knowledge.

---

## If Type = Want-to-Learn

Record a trigger.

Example:

```text
Topic: WebSockets
Why: real-time app features
Priority: Later
Trigger: after API fundamentals
```

This prevents random discoveries from hijacking the active learning path.

---

# Review Policy

Do not review the whole inbox every day.

Use this lightweight rule:

- During active study: capture freely
- End of a learning cycle: route unresolved items
- Delayed review: only for items that require retention
- Archive/reference items do not need repeated review

The inbox should stay small enough to be useful.

---

# Current Example

## Immutable update of one item in an array

- Date: 2026-09-26
- Source/context: React state practice
- What I learned / want to learn:
  Use `map()` to create a new array and replace only the matching item with a new object.
- Why it matters:
  Avoid direct mutation in React state updates.
- Type: Understand-Use
- Priority: Now
- Related skill:
  React state / JavaScript references / immutability
- Next action:
  Solve a fresh array-state update task without help.
- Delayed check:
  Re-test in a later session with a different requirement such as toggle, quantity update, or nested object update.
- Notes:
  `map()` creates the new array.
  `{ ...todo, done: true }` creates a new object only for the changed item.
  Unchanged items may keep their existing references.

---

# Operating Rule for LearningOS

When a useful new item appears during learning:

1. Capture it here if it matters.
2. Route it based on the four types above.
3. Do not interrupt the main learning path unless it is a prerequisite/blocker.
4. At the end of the cycle, decide whether it becomes:
   - active practice
   - delayed review
   - reference
   - later topic
   - discard

This file is an inbox, not a second curriculum.
