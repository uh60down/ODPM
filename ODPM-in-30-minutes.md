# How to Run ODPM in 30 Minutes

A single, time-boxed run of [the ODPM method](ODPM-method.md) on one real thing. No theory required — just follow the clock.

## Before you start (2 min)

- **Pick one small artifact** you already have: a PRD, a ticket, a feature brief, an email describing a change. One feature, not a whole product.
- **Get the right two or three people** in the room, or plan to message them for the questions you'll surface.
- **Open the [Ontology Canvas](templates/ontology-canvas.md)** and the [Open Question Log](templates/open-question-log.md). That's all the tooling you need.

## The 30 minutes

### 0–5 min — Read for intent

Read the artifact once. Write one sentence: *what is this actually trying to do?* Don't model yet.

### 5–17 min — Extract the ontology

Fill the [Ontology Canvas](templates/ontology-canvas.md). One pass per building block:

- **Concepts** — the nouns that are real things.
- **Relationships** — how they connect.
- **Rules** — what must always be true.
- **States** — the conditions things can be in.
- **Actions** — the named ways something moves between states (with *who* triggers it and *what must be true first*).

Keep it rough. Bullet points beat diagrams. If you get stuck naming an action's actor or guard — good, that's a finding.

### 17–24 min — Mark the open questions

Every time the artifact was unclear, disputed, missing, or assumed, write it in the [Open Question Log](templates/open-question-log.md). Give each one an **owner** — a name, not a team.

The best signals: an Action with no clear actor, a State nothing reaches, a Rule that's really a guard on an unnamed action, a concept used but never defined.

### 24–29 min — Decide readiness

Run the [Decision Readiness Checklist](templates/decision-readiness-checklist.md) for the next decision on the table. Can you, out loud:

1. Point to the model?
2. Show what's still uncertain?
3. Show who owns each uncertainty?
4. Explain why the unknowns no longer block the next step?

Four yeses → you're Decision Ready. Any no → you've found exactly where to chase next.

### 29–30 min — Name the next move

One line: either *"we're ready to proceed because…"* or *"we're blocked on Q_ , owned by _ , resolving by _ ."*

## What you'll walk out with

- A one-page ontology you didn't have before.
- A short list of owned open questions — findings, not vibes.
- A clear yes/no on whether to proceed, with the reason.

That's a full ODPM run. Do it again next week on the next thing, and wire the open questions into tracked issues — see [The ODPM Method](ODPM-method.md) and the [Maturity Model](maturity-model.md) for where it goes from here.

---

See also: [ODPM at a Glance](ODPM-at-a-glance.md) · [Templates](templates/) · [Worked Example](examples/banking/send-money-p2p.md)
