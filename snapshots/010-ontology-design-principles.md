# Snapshot 010: Ontology Design Principles

Date: 2026-07-02

A talk on advanced ontology design at a Palantir developer conference surfaced four design principles — each borrowed from software engineering — for building an ontology well.

This snapshot records what those principles suggest for ODPM: which transfer, which do not, and one thing they quietly confirm.

These are observations from an external comparison, not decided changes. The same posture as Snapshot 006.

---

## What They Confirm

The talk framed the ontology as evolving through three stages:

1. **Golden Tables** — integrating disparate sources into one unified, trusted structure. The foundation.
2. **Operational** — capturing organizational *kinetics* through actions, logic, and functions.
3. **AI-First** — layering automation over the captured workflows.

The middle stage is the interesting one. A mature platform treats *actions* — the legitimate operations that change things — as a distinct evolutionary stage, not a detail.

ODPM reached the same place independently this session. The four static building blocks could not express who legitimately changes a State; [Snapshot 008](008-actions-as-a-missing-building-block.md) named the gap and Action became the fifth building block.

Two frameworks, arriving at the kinetic layer from different directions, is weak evidence that the layer is real.

The three stages also map onto ODPM's [maturity model](../maturity-model.md): Golden Tables near Documented, Operational at Operational, AI-First beyond Platformed.

---

## The Four Principles

Assessed honestly against ODPM, which is a framework for human agreement — not a software platform.

### Domain-Driven Design — transfers

Objects should be virtual twins of real-world entities, so the model is intuitive to the people and agents using it.

This is already ODPM's core. Concepts are the things that exist in the world; "the world before the work." ODPM never named the lineage, but this is the same instinct.

### Don't Repeat Yourself / Rule of Three — transfers

Refactor repeated workflows into one canonical representation.

ODPM already holds the principle: [One Concept, Not Two](../principles/one-concept-not-two.md). What ODPM lacks is the *heuristic* — the Rule of Three: wait until an idea repeats a third time, then canonicalize it. That is a concrete tool for deciding *when* to promote something into the shared ontology, rather than modeling everything up front.

### Open for Extension, Closed for Modification — transfers, with care

Lock the core; let people build on top of it without changing it underneath.

ODPM has no analog, and the fit is not clean — ODPM insists the ontology *evolves*, which sounds like the opposite of "closed." But there is a real idea underneath: stabilize the agreed core Concepts, and extend at the edges rather than silently redefining the center. That connects directly to [Ontology Is Owned by Agreement](../principles/ontology-owned-by-agreement.md) — the center changes only by agreement, not by quiet edit. Worth exploring as a principle.

### Producer Extends / Consumer Super — does not transfer

This borrows covariance and contravariance from a platform's type system.

It is real and useful inside a software platform. It does not map onto a human-agreement framework without cargo-culting the vocabulary. ODPM should leave it alone rather than force a parallel.

---

## One Feature Worth Noting: Interfaces

The talk described *interfaces* — one workflow that works across multiple object types without duplicating code.

ODPM has [One Ontology, Multiple Views](../principles/one-ontology-multiple-views.md), but that is about different audiences seeing the same ontology differently. Interfaces are a different idea: different Concepts sharing a common *shape*. Anything with a lifecycle has States and Actions; a review workflow could apply to any Concept that implements "reviewable."

ODPM does not need this yet. It is a Level 4–5 concern. But it names a real pattern: shared behavior across Concepts, not just shared viewing of one.

---

## The Open Question

> Do "Rule of Three" and a tempered "Open-Closed" earn their way into ODPM's principles, or are they platform-scale concerns that would weigh down a framework meant to stay small?

The test is the usual one: not whether the idea is elegant, but whether naming it would improve the next real decision.

---

See also: [Ontology as a Platform Layer](006-ontology-as-platform-layer.md) · [Actions as a Missing Building Block](008-actions-as-a-missing-building-block.md) · [One Concept, Not Two](../principles/one-concept-not-two.md)
