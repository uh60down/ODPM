# ODPM and Scrum

Scrum answers how the team works.

ODPM answers what the team needs to agree on before work begins.

They do not conflict. ODPM sits around Scrum's ceremonies, not inside them.

---

## The Relationship

Scrum is sprint-cadenced.

ODPM is understanding-cadenced.

Scrum structures delivery. ODPM structures the shared model that delivery executes.

---

## Before Meaningful Backlog Refinement Begins

During product discovery, before stories are written, build the initial ontology.

A glossary and a lightweight relationship diagram are enough.

The goal is for the team to agree on what exists — the Concepts, Relationships, Rules, and States — before agreeing on what to build.

Stories written before this agreement each encode a private model.

Stories written after share a common one.

---

## Backlog Refinement

Add one question to every story review:

> Does this story reference established ontology concepts, or does it introduce an undefined one?

An undefined concept is not a blocker. It is a Chase Understanding signal.

Resolve the concept first. Then write the story.

---

## Definition of Ready

A story is Decision Ready when it references the shared ontology.

---

## Sprint Planning

The question is not only "do we have capacity?"

The question is also "do we have enough shared understanding to act responsibly on this scope?"

Decision Readiness applies at the sprint level, not just the story level.

---

## Sprint Review

The increment should be reviewed against the ontology, not only against acceptance criteria.

If the implementation diverged from the shared model, that is worth naming.

Either the implementation needs to change, or the ontology needs a snapshot update.

---

## Sprint Retrospective

Add one question:

> What did we learn about the world this sprint?

If the answer changes the shared model, update the ontology before the next sprint begins.

The retrospective becomes a natural snapshot moment.

---

## Daily Scrum

ODPM does not change the Daily Scrum.

If a Daily Scrum uncovers a change in understanding, update the ontology outside the ceremony.

Keep Scrum clean.

---

## Bugs as Ontology Signals

When a bug appears, ask two questions:

1. Was this a coding error? Fix the code.
2. Was the world model wrong? Fix the ontology, then the code.

Bugs that keep recurring are usually category 2.

The team keeps fixing symptoms because the shared model was never corrected.

---

## What ODPM Does Not Change

Scrum's ceremonies, cadence, and roles stay intact.

ODPM changes the quality of what enters those ceremonies — stories that reference a shared model instead of each encoding a private one, and retrospectives that update understanding rather than only process.

---

See also: [Decision Readiness](decision-readiness.md) · [Chase Understanding](chase-understanding.md) · [Snapshot Thinking in BOOK.md](../BOOK.md)
