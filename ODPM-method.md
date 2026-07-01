# The ODPM Method

ODPM is a way of thinking. This is the repeatable cycle that puts it to work.

The method is deliberately small. It is meant to be picked up on a real piece of work — a feature, a change, a plan, an existing system — and run, not studied first.

---

## The Cycle

```text
1. Start from a source artifact
2. Extract the ontology
3. Mark open questions
4. Chase Understanding
5. Decide readiness
6. Execute
7. Update the ontology from feedback
        ↑___________________________|
```

### 1. Start from a source artifact

Every run begins with something that already exists.

A PRD, a charter, a mandate, a brief, an existing system, a complaint, a change request.

ODPM does not ask for a new artifact first. It reads the one you already have.

### 2. Extract the ontology

Read the artifact for the five building blocks:

- **Concepts** — the things that exist.
- **Relationships** — how they connect.
- **Rules** — what must be true.
- **States** — the conditions things can be in.
- **Actions** — the named, legitimate ways things move between states.

The output is a lightweight model, not a finished document: a glossary, a relationship sketch, and a list of rules, states, and actions.

### 3. Mark open questions

While extracting, mark everything that is unclear, disputed, missing, or assumed.

An open question is not a failure of the artifact. It is the most valuable thing the run produces.

### 4. Chase Understanding

Take the open questions to the people who can answer them.

The goal is not to answer everything. It is to answer what would most improve the next decision.

### 5. Decide readiness

Ask: is the ontology aligned enough to take the next responsible action?

Not "do we know everything?" — "do the remaining unknowns still block the next responsible move?"

If yes, keep chasing. If no, proceed.

### 6. Execute

Do the work, from a model everyone can point to.

### 7. Update the ontology from feedback

Execution tests the ontology. Feedback refines it.

What you learned goes back into the model, and the next run starts from a better one.

---

## The Maturity Jump

The cycle above produces insight. On its own, insight leaks between runs.

The step that turns insight into operational force is wiring each open question through to a resolution:

```text
open question → tracked item → owner → decision → ontology update
```

- **open question** — surfaced in step 3.
- **tracked item** — it becomes an Issue, not a bullet in a doc that no one reopens.
- **owner** — one person is accountable for moving it.
- **decision** — it is resolved, deferred, or explicitly accepted as a risk.
- **ontology update** — the resolution changes the model, so the answer is not lost.

Without this chain, ODPM is a tool you pick up per run. With it, ODPM is a process that holds between runs.

The mechanism already exists in this repository: see [GitHub as an ODPM Tool](principles/github-as-odpm-tool.md) — an Issue is an Open Question, a Label is its status, a Merge is agreement.

---

## What "Decision Ready" Looks Like

Decision Readiness is observable, not a feeling. A team is Decision Ready for a given decision when it can do four things out loud:

1. **Point to the model** it is executing from — the concepts, relationships, rules, states, and actions in scope.
2. **Show what is still uncertain** — the open questions that remain.
3. **Show who owns each uncertainty** — every remaining open question has a name against it.
4. **Explain why the remaining unknowns no longer block** the next responsible decision.

If a team cannot do all four, it is not yet Decision Ready — it is executing on private understanding and calling it alignment.

This is the line the whole method exists to reach.

---

## Scope of a Run

A run can be as small as a single feature or as large as a whole change initiative.

The cycle is the same at every scale. Only the size of the ontology changes.

Run it once and you get findings. Run it as a habit — with the maturity jump wired in — and the ontology becomes the team's durable memory of the world it is building.

For a full run of the cycle on one feature, see the worked example: [Send Money (P2P Transfer)](examples/banking/send-money-p2p.md).

---

See also: [ODPM at a Glance](ODPM-at-a-glance.md) · [Decision Readiness](principles/decision-readiness.md) · [Chase Understanding](principles/chase-understanding.md) · [GitHub as an ODPM Tool](principles/github-as-odpm-tool.md)
