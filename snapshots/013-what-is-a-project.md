# Snapshot 013: What Is a Project? (The Foundation)

## Status

**Epistemic status:** Open Research Question — foundational
**Snapshot date:** July 2026
**Origin:** Excavated bottom-up from a day of dashboard iteration — real Story states, a real hierarchy, a real +scope problem — not decreed top-down.
**Role:** The root node. The delivery ontology (Snapshot 011), ontology evolution (Snapshot 012), the dashboard, and the schema are all specializations of this.

> A snapshot records our current best understanding. It is dated, revisable, and expected to be superseded.

---

## Summary

Everything ODPM has built — product ontology, delivery ontology, Chase Understanding, snapshots, boundaries-as-evidence — presupposes an answer to one question it never wrote down: *what is a project?*

This snapshot states that answer, and shows the rest of ODPM falling out of it. The move is not addition; it is **grounding** — placing the base under the house that is already built.

---

## Layer 1: The Axiom

> **A project is a bounded transformation of understanding into verified reality, under constraint.**

This is not a chapter among chapters. It is the sentence from which the rest of ODPM is *derivable*.

It also repositions the framework. ODPM has described itself as a project-management methodology. On this foundation, it is not one:

> **ODPM is not a methodology. It is the ontology that methodologies are strategies over.**

That explains why ODPM kept feeling different from PMBOK, Scrum, and SAFe: it operates one level below them. They are strategies; it is the board they are played on.

---

## Layer 1 (continued): The Four-Part Ontology

Decompose the project the way you would decompose any domain — with the honest boundary questions live at each layer.

### Entities — what *is*

The things that exist, independent of what happens to them. The candidates that survive a change of method:

- **Understanding-unit** — the atom being realized. A Story or a Bug is its delivery-shaped instance.
- **Concept** — the product-side unit an understanding-unit realizes.
- **Agent** — who transforms. (The piece a purely epistemic definition kept dropping.)
- **Constraint** — time, budget, capacity. Reified as a *thing*, not a background condition, because "under constraint" turned out to be load-bearing.
- **Artifact** — the verified reality produced.

What is *not* an entity: Epic, Feature, Category, Milestone. Those are groupings — relations over understanding-units, not entities themselves. That is a real, falsifiable claim: *if an Epic has properties not derivable from its members, it is an entity; if it is purely its members seen together, it is a relation.* Today's data model suggests the latter.

### States — what *changes*

The conditions an entity can occupy, and the only thing that changes.

- **Understanding-unit:** the workflow lifecycle `new → … → qa pass`, whose deep structure is three phases — **intended → enacted → verified** — with the workflow states as the observable refinement.
- The critical, usually-invisible distinction: **Observed vs. Actual.** "qa pass" is observed-realized; reality may still diverge. Field bugs are exactly that divergence.
- **Constraint:** consumed / remaining.
- **Concept:** undefined → defined → realized.
- *Blocked* is not a state of the unit at all — it is a state of a **relation** (the unit's dependency), which is why a blocker always points elsewhere.

### Relations — where the difficulty *lives*

What binds entities, and where projects actually get hard.

- **realizes** — unit → concept (the bridge a `product_concept_id` reserves).
- **decomposes** — the containment tree (Category through Subtask).
- **depends-on** — unit → unit; the relation whose bad state *is* a blocker.
- **consumes** — unit → constraint; the edge PMBOK obsesses over and most delivery models don't yet carry.
- **assigned-to** — unit → agent.
- **realizes-beyond** — the +scope overflow: an epic realizing more than its feature defines. Precisely a *relation the agreement failed to record.*

> Most project pain lives in relations, not entities — a truth no methodology states, because methods manage entities (tickets, people) and let relations stay implicit.

### Invariants — what must *never break*

The conservation laws. The strongest claims, because one counterexample kills them.

- **Done means verified, never claimed.** No unit is realized until confirmed to match its understanding.
- **Every realized unit realizes some concept.** Realization without a concept is either undocumented understanding or waste — there is no third case.
- **Consumed constraint never exceeds available.** Violate it and the project is not behind; it is *ended.* The hardest invariant, the one methodologies pretend is soft.
- **Understanding only increases.** The project never knows less than before; even a reversal is a gain (you learned the boundary was wrong). This is why *Superseded / Refuted* is a legitimate terminal state, not a failure.
- **A project terminates.** *(The open crack — see below.)*

---

## The Shape of the Whole

> Entities are what is. States are what changes. Relations are where the difficulty lives. Invariants are what must never break.

Which lets a methodology finally be defined with precision:

> A methodology is a **strategy for moving understanding-units through their states without violating the invariants, under the constraints, given the relations.**

PMBOK optimizes the constraint invariant. Scrum optimizes the rate of state-change. SAFe optimizes the decomposition relations at scale. Same ontology; different objective functions over it. That is why they are all partial, and all sometimes right.

---

## Layer 2: The Derivation

A foundation is load-bearing only if the existing structure falls out of it. Each core ODPM concept traces to the axiom in one line:

| ODPM concept | Derived from the axiom as… |
|---|---|
| Chase Understanding | the *transformation* viewed from inside |
| "Done = verified" | the *verification invariant* |
| Product vs. Delivery ontology | understanding-at-rest vs. understanding-in-motion |
| Boundaries-as-evidence (Snapshot 012) | the *coverage invariant* applied to relations |
| Snapshots | *states* of understanding |
| Decision Readiness | enough understanding transformed to act without violating an invariant |

If a concept cannot be derived, that is information — either the concept is ad hoc, or the axiom is incomplete. The derivation is a **test of the foundation**, not just exposition.

### Reconciliation with the five building blocks

The four-part form is not a second vocabulary — that would violate [One Concept, Not Two](../principles/one-concept-not-two.md). It is the same ontology under a formal-systems lens:

| Four-part (this snapshot) | ODPM building block |
|---|---|
| Entity | Concept |
| Relation | Relationship |
| Invariant | Rule |
| State | State |
| (transformation, carried by Agent) | Action |

Same blocks; the formal-systems framing just foregrounds the invariants and the agent that ordinary usage leaves implicit.

---

## Lineage: Every Abstraction Points Back Down

The framework's own discipline, turned on this very move: **don't let the philosophy detach from the practice.** Today's insight is trustworthy because it emerged bottom-up, from real artifacts. A foundation stated too abstractly — with no thread back to Story states and qa-pass and epic overflow — becomes theology.

So the abstraction earns its place only by pointing back down:

| Abstract claim | Concrete artifact that produced it |
|---|---|
| Verification invariant | the qa-pass discipline |
| Constraint as an entity | the resource question the dashboard couldn't answer |
| realizes-beyond relation | the +scope exposure metric |
| Observed vs. Actual states | field bugs (realized on paper, diverged in reality) |
| Understanding-unit as the atom | Story and Bug as its two delivery-shaped instances |

---

## Layer 3: The Recursion

The satisfying part: this foundation obeys ODPM's own method.

- It is a **snapshot** — dated July 2026, expected supersession.
- It was **discovered, not designed** — through a day of dashboard iteration, not decreed.
- It ships with **its own falsifier already named** — the termination invariant.

The base was laid using ODPM's own tools. That is the strongest possible evidence the tools work: they were sharp enough to excavate the ground they stand on.

---

## The Open Crack: the Termination Invariant

The invariant the foundation is least sure of: *a project terminates* — that a bounded transformation reaches a fixed target and stops.

Living software threatens it. If living software is unmistakably a project yet never terminates, then termination is not an invariant of *project* but of one sub-species. The genus would be the **standing coupling** — understanding and reality held in sync at some velocity — with "done" being merely velocity zero.

**Falsification:** a thing that is unmistakably a project yet provably never terminates. Such a case would break "bounded" and collapse the axiom into the standing-coupling genus. Until then, "bounded transformation" stands as the current best answer.

---

## Provenance

This snapshot is itself an instance of what it describes: it began as a question about Product vs. Delivery ontology, ran through a day of concrete dashboard work, and surfaced — through Chase Understanding — as the foundation the whole framework had been standing on without writing down.

It is the parent of the boundary and evidence questions, not a sibling. Filed as ODPM's foundational question *with its current best answer attached*, dated, and expected to be revised.

*Snapshot recorded: July 2026. Expected to be superseded.*

---

See also: [Tracking Against the Ontology](011-tracking-against-the-ontology.md) · [Ontology Evolution](012-ontology-evolution.md) · [Ontology Design Principles](010-ontology-design-principles.md) · [Chase Understanding](../principles/chase-understanding.md) · [One Concept, Not Two](../principles/one-concept-not-two.md) · [Open Research Questions](../questions.md)
