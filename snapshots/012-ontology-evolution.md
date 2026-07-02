# Snapshot 012: Ontology Evolution

## Status

**Epistemic status:** Open Research Question
**Snapshot date:** July 2026
**Origin:** Discussion on separating Product Ontology and Delivery Ontology

> A snapshot records our current best understanding.
> It is dated, revisable, and expected to be superseded.

---

## Summary

While exploring whether Product Ontology and Delivery Ontology should be separated, a deeper question emerged: **how does ontology evolve?**

The original question — *"Should we split the ontology?"* — was replaced by a better one:

> **What evidence justifies an ontology boundary?**

This snapshot records the findings of that exploration.

---

## Findings

### 1. Ontology boundaries are discovered, not designed

We do not decide upfront to split an ontology.
We let **Chase Understanding** reveal where boundaries naturally emerge.
A boundary is a *finding*, with the same evidentiary status as any other ontology output.

### 2. A boundary requires two conditions

A split is justified only when **both** conditions hold:

1. **Semantic divergence** — shared terms mean different things on each side.
2. **Independent evolution** — the domains change at independent rates.

Neither condition alone is sufficient:

| Condition present | Correct response |
|---|---|
| Semantic divergence only | Disambiguation, not a split |
| Independent evolution only | Versioning discipline, not a split |
| Both | A context boundary with an explicit mapping |

### 3. Boundaries are evidence

An ontology boundary is not a design preference.
It is an **empirical finding** produced by understanding.

### 4. Boundaries are revisable

Like all snapshots, boundary decisions can be overturned as understanding evolves.

The primitive operations of ontology evolution (candidate list):

| Operation | Operand |
|---|---|
| Split | Ontology |
| Merge | Ontology |
| Term Migration | Term |
| Deprecation | Concept / Term |

A split made too early is a falsifiable claim.
Ontologies can merge as well as split — this bidirectionality keeps
*"discovered, not designed"* honest rather than a one-way ratchet toward fragmentation.

### 5. ODPM inverts traditional DDD

Traditional Domain-Driven Design:

```
Bounded Context
      ↓
   Ontology
```

Contexts are drawn early — often along team or system lines — and language is
cultivated within them. Conway's Law does the real drawing.

ODPM proposes the inversion:

```
   Ontology
      ↓
Bounded Context
```

Build a shared ontology first. Let boundaries emerge from evidence.

> **The boundary becomes a property of the problem, not the org chart.**

### 6. One artifact, two state machines

A GitHub Issue carries two independent lifecycles:

**Delivery state** (GitHub tracks work):

```
Open → Closed
```

**Understanding state** (ODPM tracks understanding):

```
Open Research Question
      ↓
Emerging Principle
      ↓
ODPM Principle
      ↓
Superseded / Refuted
```

The terminal state **Superseded / Refuted** matters: without it, the lifecycle
is a one-way escalator toward Principle. With it, the state machine itself
encodes falsifiability. *A principle can die.*

Notably, the word **"Status"** already fractures across these two contexts —
delivery status vs. epistemic status — inside the very document that predicts
such fractures. The finding demonstrates itself.

### 7. The issue itself became an ODPM artifact

Adding an epistemic status header and snapshot date turned a GitHub issue
into a **snapshot of understanding**, not merely a work item.
The framework applies its own discipline to itself.

---

## Hypothesis and Falsification Criterion

Every snapshot should state what it believes and what would change its mind.

**Hypothesis:**

> Ontology boundaries are discovered, not designed.

**Test question:**

> What evidence justifies an ontology boundary?

**Falsification:** Evidence from multiple domains consistently showing that
boundaries imposed by design outperform or contradict boundaries revealed by
Chase Understanding.

---

## Candidate First Experiment

Pick a **shared term that appears in two otherwise-separate features of the same
product** — for example, a word like **Update** used by two different
capabilities that each mean something slightly their own by it.

Apply Chase Understanding to that term across both features. Investigate whether they represent:

1. one concept,
2. two bounded contexts, or
3. a shared concept with different states and rules.

Compare the discovered boundary with the existing organizational structure.

**A result that diverges from Conway's Law** — the org predicts a boundary the
ontology refutes, or the ontology reveals a boundary no team structure
predicted — would be the existence proof that boundaries are discovered.

---

## Open Questions

- Can bounded contexts reliably emerge from ontology rather than being imposed?
- What evidence is sufficient to justify splitting an ontology?
- Under what circumstances should previously separated ontologies merge?
- How should ontology evolution be represented?
- Do ontology changes themselves have a lifecycle?

---

## Success Criteria

Evidence from multiple domains consistently supports (or refutes) the
hypothesis that ontology boundaries emerge through Chase Understanding.

Until then, this remains an **Open Research Question**, not an ODPM principle.

---

## Provenance

This snapshot is itself an instance of what it describes: it began as a
question about Product vs. Delivery ontology and evolved, through Chase
Understanding, into a research direction about how ontology evolves.

*Snapshot recorded: July 2026. Expected to be revised.*

---

See also: [Tracking Against the Ontology](011-tracking-against-the-ontology.md) · [Ontology Design Principles](010-ontology-design-principles.md) · [Chase Understanding](../principles/chase-understanding.md) · [One Concept, Not Two](../principles/one-concept-not-two.md) · [Open Research Questions](../questions.md)
