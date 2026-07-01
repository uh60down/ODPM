# Snapshot 008: Actions as a Missing Building Block

Date: 2026-07-01

ODPM's ontology has four building blocks: Concept, Relationship, Rule, State.

Palantir's Foundry Ontology has a similar structure, but splits it differently — into a Semantic layer (Object Types, Link Types), a Kinetic layer (Action Types, Functions), and a Dynamic layer (business rules, policies, permissions).

That split exposes a seam in ODPM's four building blocks that is worth naming.

---

## Rule Currently Does Two Jobs

ODPM's glossary defines Rule as "something that must be true in the world" — a constraint.

> An update cannot install while a vehicle is moving.

That is a constraint: a condition that must always hold.

Palantir's Action Type is a different kind of thing: a named, controlled operation that legitimately moves an object from one state to another, with defined side effects.

> Approve this order. Escalate this alert. Schedule this install.

That is not a constraint. It is a sanctioned transition — the mechanism, not the boundary.

ODPM currently has no building block for this. It has States (before and after), and it has Rules (what must always be true), but it has nothing that names who is allowed to move a Concept from one State to another, and how.

---

## Why This Gap Matters

Teams routinely reach agreement on what exists (Concepts), how things relate (Relationships), and what states are possible (States).

They rarely reach explicit agreement on who is authorized to cause a state transition, and by what named action.

That is usually where disagreements about ownership, authority, and process actually live — not in the states themselves, but in the transitions between them.

A vehicle can be in state `available` or `deployed`. Everyone agrees on that. The disagreement is over who can move it from one to the other, and whether that move requires approval, a side effect (notify someone), or a guard condition (only if maintenance is current).

Naming that as its own building block — Action — would give teams a place to Chase Understanding about authority and process, instead of folding it silently into Rule or leaving it undocumented entirely.

---

## A Possible Fifth Building Block

**Action**: a named, legitimate way to move a Concept from one State to another.

Distinct from:
- **Rule** — a constraint that must always hold, regardless of any specific transition.
- **State** — a condition that exists, independent of how it was reached.

An Action would answer three questions a Rule and a State cannot:
1. What is this transition called?
2. Who or what is allowed to trigger it?
3. What else happens when it occurs (side effects)?

---

## What This Is Not (Yet)

This snapshot is not a proposal to change BOOK.md, the glossary, or ODPM-at-a-glance.md.

The four-building-block model is foundational and referenced throughout the manuscript. A change to it should not be made lightly or immediately after a single external comparison.

This snapshot exists to record the observation and let it sit — consistent with Snapshot Thinking. If the distinction still seems necessary after further use, it becomes a candidate for the manuscript. If it turns out that Rule already carries enough of this meaning in practice, it can be discarded.

---

## The Open Question

> Does ODPM need a fifth building block for sanctioned transitions, or is the transition itself just a special case of Rule that doesn't need its own name?

---

See also: [Ontology as Platform Layer](006-ontology-as-platform-layer.md) · [Glossary](../glossary.md)
