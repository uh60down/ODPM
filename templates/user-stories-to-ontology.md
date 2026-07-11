# User Stories → Ontology

A guide for the most common ODPM step-2 crossing. Most teams already have user stories; turning them into an ontology is where the framework earns its keep.

> **A user story tells you the intention and the thing. The ontology tells you the world.**

A worked demonstration lives in the Voice Journal example (`examples/voice-journal/`).

---

## 1. Read the grammar of the stated part

A story has a precise shape, and each clause maps to a building block:

> **As a** [role] · **I want** [capability] · **so that** [intention].

| Clause | Becomes |
|---|---|
| **role** — "As a user" | a **Thing** (an actor) |
| **capability** — the verbs and their nouns | **Actions** + the **Things** they touch |
| **so that** — the intention | a **Rule** or a priority — *or nothing* (watch this one) |

Three quick passes over your stack of stories:

- **Nouns → Things.** Every real thing a story mentions.
- **Verbs → Actions.** Record, browse, edit, delete…
- **Qualifiers → Rules and States.** "immediately", "only when", "must not" → Rules; lifecycle words → States.

## 2. Recover what the stories left implicit

A story is told from one vantage and states one capability. Most of the ontology is what the story *didn't* say. Recover it:

- **Missing actors.** Who else acts? Every rule that begins "the app must…" is an actor the stories never named — the System, a Clock, an external service. Assign each one.
- **Missing links.** How do the nouns connect? `contains` / `has` / `displays` are structural links no story states. Draw them.
- **Missing interactions.** What happens when two stories' actions run at once — concurrency, priority, side-effects? These *dynamic* relationships are the ones that only surface here (and then when you build).
- **Missing negative space.** What is out of scope or forbidden? Name it as clearly as what's in.

## 3. Run three checks before building

- **Watch the "so that."** Is each story's intention promoted into a rule, or has it silently dropped? Intention lost here is the [intention gap](../snapshots/011-tracking-against-the-ontology.md).
- **Name the missing actors.** Does every "the app must…" rule have an actor against it?
- **Draw the missing links.** Is every pair of things that interacts actually connected?

## 4. Mark the gaps

Everything the stories left implicit that you *couldn't* resolve becomes an open question. Move each into the [Open Question Log](open-question-log.md) with an owner.

---

See also: [Ontology Canvas](ontology-canvas.md) · [PRD-to-Ontology Extraction](prd-to-ontology-extraction.md) · [Open Question Log](open-question-log.md) · [The ODPM Method](../ODPM-method.md)
