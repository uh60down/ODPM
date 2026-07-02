# Snapshot 011: Tracking Against the Ontology

Date: 2026-07-02

ODPM's center of gravity is upstream: intent → ontology → Decision Readiness. The method's steps 6 (Execute) and 7 (Update from feedback) are one-liners.

But most of a project's life is spent *after* Decision Readiness — building, tracking progress, and handling bugs. This snapshot explores what ODPM has to say about that downstream half, without abandoning what makes it ODPM.

These are observations to react to, not decided changes.

---

## The Question ODPM Should Be Able to Answer

Traditional project management answers "are we on schedule?" by counting tasks.

ODPM should be able to answer a different question:

> How much of the agreed model of the world is real yet — and is what we built still faithful to it?

That reframes both progress and bugs around the ontology instead of around a task board.

---

## Reframing 1: Progress Is Ontology Coverage

A task board tells you how many tasks are closed. It does not tell you how much of the *world you agreed to build* actually exists.

ODPM already describes change as the delta between two ontologies — a current state and a target state ([The Change Ontology](../principles/change-ontology.md)). Build progress is the same delta, watched over time:

- The **target-state ontology** is what the team agreed to build (Concepts, Relationships, Rules, States, Actions).
- The **realized ontology** is what actually exists and behaves in the running system.
- Progress is that gap closing.

Each element of the ontology moves through a small lifecycle:

```text
agreed → built → verified
```

- **agreed** — the team has aligned on it (Decision Ready).
- **built** — it exists in the system.
- **verified** — reality has been checked against it; it behaves as the ontology says.

"80% of tasks done" can hide that a core Rule was never verified. "Every Rule and Action for the payment Concept is verified; the refund Concept is only built, not verified" is a truer status — and it is expressed in the shared vocabulary, not in story points.

---

## Reframing 2: A Bug Is Ontology Divergence

A bug is a place where reality no longer matches the agreed model.

ODPM already carries the seed of this: [ODPM and Scrum](../principles/odpm-and-scrum.md) asks, for a bug, whether it was a coding error (fix the code) or a wrong world-model (fix the ontology, then the code).

The extension is a taxonomy. Every bug can be classified by *which building block it violates*:

| Divergence | What happened | Usually means |
|---|---|---|
| Broken Rule | A constraint that should always hold didn't | Coding error — fix the code |
| Impossible State | The system reached a state the ontology says can't exist | The State model is wrong or incomplete |
| Unguarded Action | A transition fired without its guard being satisfied | Missing enforcement, or a wrong guard |
| Missing Concept / Relationship | Reality has a thing or link the ontology never named | The ontology is incomplete — update it, then the code |

The value is in triage. "Broken Rule" bugs are usually code fixes. "Impossible State" and "Missing Concept" bugs are usually signals the *ontology* was wrong — the recurring, expensive kind. Naming the divergence points at whether you're fixing a symptom or the model.

---

## This Is a Lens, Not a New Tracker

ODPM does not replace Jira, GitHub Issues, or a burndown chart — the same way [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) reads GitHub's native concepts as ontology concepts rather than proposing a new tool.

Coverage status and divergence type are a *lens* laid over whatever tracker a team already uses. A bug is still a GitHub issue; ODPM just adds "which building block did this violate?" A sprint board still exists; ODPM just asks "which ontology elements moved from built to verified this week?"

---

## What This Would Deepen

If these reframings hold, the thin steps of the method gain substance:

- **Step 6 (Execute)** — execution is watched as ontology elements moving `agreed → built → verified`.
- **Step 7 (Update from feedback)** — a divergence bug that turns out to be "Missing Concept" or "Impossible State" feeds straight back into the ontology, which is exactly what step 7 is for.

---

## Open Questions

- What is the honest unit of "verified"? A test? A demo? A production observation? Or just a human saying "I checked reality against the model"?
- Does "coverage" invite the same false precision as story points, if teams start scoring it?
- Which of these earns promotion into a real principle or template, and which stays an idea? Candidates: a *Progress Is Ontology Coverage* principle, a *Bugs Are Ontology Divergence* principle, an ontology-coverage tracker template, a bug-triage-by-building-block template.

> The test, as always: not whether the lens is elegant, but whether naming coverage and divergence would make the next status call or the next bug triage better.

---

See also: [The Change Ontology](../principles/change-ontology.md) · [ODPM and Scrum](../principles/odpm-and-scrum.md) · [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) · [The ODPM Method](../ODPM-method.md)
