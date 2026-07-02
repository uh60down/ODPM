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

## Reframing 1: Development Progress Is Ontology Coverage

This is about tracking development *during execution* — after Decision Readiness, while the team is building.

By the time execution starts, the ontology is already **agreed**. It is not a moving target; it is the baseline — the definition of what "done" means for this build. The agreed ontology is the target-state model from [The Change Ontology](../principles/change-ontology.md): the full set of Concepts, Relationships, Rules, States, and Actions the team committed to realize.

Development progress, then, is each agreed element moving from *not built* to *built and verified*:

```text
not started → in progress → built → verified
```

- **not started** — agreed, but no work yet.
- **in progress** — a developer is building it.
- **built** — it exists in the running system.
- **verified** — reality has been checked against it; it behaves as the ontology says.

The unit of progress is the ontology element, not the task. Development work — tasks, commits, PRs — is tied to the element it realizes, so progress is read as *"which parts of the agreed model are real yet,"* weighted by the model itself.

"80% of tasks done" can hide that a core Rule was never verified. "Every Rule and Action for the payment Concept is verified; the refund Concept is only built, not verified; two Actions are still not started" is a truer development status — and it is expressed in the shared vocabulary, not in story points.

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

- **Step 6 (Execute)** — development progress is watched as agreed ontology elements moving `not started → in progress → built → verified`.
- **Step 7 (Update from feedback)** — a divergence bug that turns out to be "Missing Concept" or "Impossible State" feeds straight back into the ontology, which is exactly what step 7 is for.

---

## Open Questions

- What is the honest unit of "verified"? A test? A demo? A production observation? Or just a human saying "I checked reality against the model"?
- Does "coverage" invite the same false precision as story points, if teams start scoring it?
- Which of these earns promotion into a real principle or template, and which stays an idea? Candidates: a *Progress Is Ontology Coverage* principle, a *Bugs Are Ontology Divergence* principle, an ontology-coverage tracker template, a bug-triage-by-building-block template.

> The test, as always: not whether the lens is elegant, but whether naming coverage and divergence would make the next status call or the next bug triage better.

---

See also: [The Change Ontology](../principles/change-ontology.md) · [ODPM and Scrum](../principles/odpm-and-scrum.md) · [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) · [The ODPM Method](../ODPM-method.md)
