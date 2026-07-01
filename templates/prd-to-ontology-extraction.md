# PRD-to-Ontology Extraction Template

A guide for reading a source artifact into an ontology. Works for a PRD, charter, brief, or any document that carries intent.

The premise: the artifact already contains an implicit model of the world. You are not inventing the ontology — you are extracting the one that is already there, and marking where it is unclear.

> Source artifact: _(title / link / version)_
> Extracted by: _()_
> Date: _(YYYY-MM-DD)_

---

## 1. Read for intent

Before extracting anything, capture the artifact's intent in one or two sentences.

> Intent: _()_

## 2. Extract the five building blocks

Read the artifact once per building block. Each pass asks one question.

| Pass | Question | What to look for |
|---|---|---|
| Concepts | What exists? | Nouns the artifact treats as real things |
| Relationships | How do they connect? | Verbs and phrases linking concepts |
| Rules | What must be true? | "must", "cannot", "only", constraints, limits |
| States | What conditions matter? | Lifecycle words, statuses, phases |
| Actions | What legitimately changes a state? | Named operations, who triggers them, guards |

Record the results in an [Ontology Canvas](ontology-canvas.md).

## 3. Mark the gaps as you go

Every place the artifact is unclear, disputed, missing, or assumed becomes an open question.

Watch especially for:

- A rule stated as a guard on an unnamed action ("must not X unless Y" — what action is X?).
- A state with no action that reaches or leaves it.
- An actor implied but never named ("the system does Z" — which actor, under what authority?).
- A concept referenced once and never defined.

## 4. Separate intent-gaps from evidence-gaps

Two different kinds of open question:

- **Intent-gap** — the artifact hasn't decided yet. Resolve with the author / product owner.
- **Evidence-gap** — the artifact says one thing; reality (code, systems, users) may say another. Resolve by checking reality.

## 5. Move every open question into the log

Extraction is not finished when the canvas is full. It is finished when every open question is in the [Open Question Log](open-question-log.md) with an owner.

---

See also: [The ODPM Method](../ODPM-method.md) · [Ontology Canvas](ontology-canvas.md) · [Open Question Log](open-question-log.md)
