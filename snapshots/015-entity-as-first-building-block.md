# Snapshot 015: Entity as the First Building Block

## Status

**Epistemic status:** Current terminology, term migration
**Snapshot date:** July 2026
**Origin:** Teaching and facilitation review of the five ODPM building-block questions.

> A snapshot records our current best understanding.
> It is dated, revisable, and expected to be superseded.

---

## Summary

ODPM's first building block is now **Entity**, not **Concept**.

This is not only a rename.

It changes the teaching posture of ODPM.

Concept emphasized abstraction.

Entity points directly at the domain:

> What exists?

That question is easier to ask, easier to answer, and easier to remember.

---

## The Five Building Blocks

### Entity

What exists?

Discover the things that make up the domain.

Examples:

- User
- VoiceRecord
- Vehicle
- Requirement
- Sprint

### Relationship

How are they related?

Describe how entities are connected and what those connections mean.

Examples:

- User creates VoiceRecord
- Vehicle belongs to Fleet
- Sprint contains Story

### Action

What can happen?

Identify the meaningful behaviors that occur within the domain.

Examples:

- Record Voice
- Play VoiceRecord
- Assign Requirement
- Complete Story

### State

What condition can they be in?

Describe the lifecycle or condition of an entity over time.

Examples:

- Recording
- Saved
- Playing
- Completed
- Archived

### Rule

What must always hold?

Capture the business rules, constraints, and invariants that preserve the integrity of the domain.

Examples:

- A VoiceRecord must contain exactly one AudioFile.
- Only one recording session may be active.
- A completed Story cannot return to Draft.

---

## Why These Five

Together they answer the five fundamental questions needed to build shared understanding:

| Building Block | Fundamental Question |
|---|---|
| Entity | What exists? |
| Relationship | How are they related? |
| Action | What can happen? |
| State | What condition can they be in? |
| Rule | What must always hold? |

The sequence also guides discovery:

1. Identify the entities.
2. Understand their relationships.
3. Discover the actions.
4. Describe their states.
5. Capture the rules.

This mirrors how people naturally explore a domain.

---

## What This Migrates

Older snapshots and examples may use **Concept** because that was the term at the time.

Current ODPM uses **Entity** as the canonical first building block.

Formal or technical language can still map to it:

| ODPM term | Nearby formal term |
|---|---|
| Entity | Entity / Class / Object |

But ODPM keeps one building-block name.

This follows the same discipline as [One Entity, Not Two](../principles/one-entity-not-two.md): one canonical term for one ODPM building block.

---

## Open Questions

- Does Entity remain approachable for non-technical teams?
- Should older historical snapshots keep Concept as written, or receive notes pointing to this migration?
- Does Action belong before State in teaching order, even though state diagrams often show states first?

---

See also: [Glossary](../glossary.md) · [One Entity, Not Two](../principles/one-entity-not-two.md) · [ODPM at a Glance](../ODPM-at-a-glance.md)
