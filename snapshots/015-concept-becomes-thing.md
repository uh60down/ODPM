# Snapshot 015: Concept Becomes Thing

## Status

**Epistemic status:** Resolved — a Term Migration, applied
**Snapshot date:** July 2026
**Operation:** Term Migration (the first building block), per [Ontology Evolution](012-ontology-evolution.md)

> A snapshot records our current best understanding. It is dated, revisable, and expected to be superseded.

---

## The Decision

The first building block is renamed **Concept → Thing**. The five building blocks are now:

> **Thing · Relationship · Rule · State · Action**

"Concept" is kept as a synonym, alongside Entity and Class.

---

## Why

The block was named "Concept," but across every example its members are overwhelmingly concrete: *User, Vehicle, Story, Bug, Sprint, Release, VoiceRecord, AudioFile.* The genuinely abstract members (Eligibility, Capacity) are the minority. So "Concept" over-abstracted the common case — it read as *an idea* when the block means *a thing that exists.*

The deciding test was the block's own question. Each building block should be the answer to the question it answers:

| Building block | Question |
|---|---|
| **Thing** | what exists? |
| **Relationship** | how are they linked? |
| **Action** | what do they do? |
| **State** | how do they change? |
| **Rule** | what must hold? |

Ask *"what is there?"* and you get back a User, a Vehicle, a Story — **things**, not "concepts." A building block should be the answer to its own question, and ODPM's first question has always been *"What exists?"* The answer is **Thing**.

"Thing" also keeps ODPM's plain-English voice (*ontology is not philosophy*), and unlike "Entity" it covers both concrete and abstract without strain — *a Thing is something that exists, concrete or abstract.*

---

## Evidence It Was Justified, Not Premature

[Snapshot 012](012-ontology-evolution.md) says a Term Migration should be evidence-driven — "a migration made too early is a falsifiable claim." The evidence here was concrete: the actual membership of the block, across five worked domains, is mostly concrete things, and "Concept" was observed to read too abstract for what the block is. This was a migration on evidence, not on taste.

---

## Scope of the Migration

- **Renamed** everywhere the word named the building block or an instance of it: glossary, BOOK, the method, at-a-glance, questions, maturity model, templates, principles, and the GitHub templates.
- **Kept as-is:**
  - Generic English uses of "concept" ("GitHub's concepts," "concept graph") — not the building block.
  - The principle *One Concept, Not Two* — its title uses "concept" in the ordinary sense of *one idea, not two*, and its point is unchanged.
  - The embedded domain term **Product Concept** (in the delivery ontology) — a named term, not the bare block; left pending a separate decision.
- **Snapshots** are left as historical record (they still say Concept), per Snapshot Thinking.
- Examples migrate in a follow-up pass.

---

## The Open Edge

"Concept" as a synonym is retained deliberately. If it turns out that readers reach for "Concept" so often that "Thing" never takes, that is falsifying evidence — and the migration is, like every snapshot, revisable.

---

See also: [Ontology Evolution](012-ontology-evolution.md) · [One Concept, Not Two](../principles/one-concept-not-two.md) · [Glossary](../glossary.md)
