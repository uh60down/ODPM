# ODPM with Jira and Confluence

This is a tooling guide for teams using Jira and Confluence alongside ODPM and Scrum.

The principles of how ODPM integrates with Scrum do not depend on any specific tool.

This guide shows one implementation. Jira can be replaced with Linear, GitHub Issues, or any backlog tool. Confluence can be replaced with Notion, Coda, or any wiki.

---

## Confluence: Ontology Home

The living ontology belongs in Confluence, not in Jira.

| Confluence Page | ODPM Role |
|---|---|
| Glossary | Concept definitions — the shared vocabulary |
| Relationship Map | Diagram showing how concepts connect |
| PRD | Intent, Requirements, Assumptions, Constraints |
| Decision Log | Snapshots of understanding at key decisions |
| Meeting Notes | Chase Understanding conversations preserved as evidence |

### Starting Template

A minimal ontology space needs three pages:

1. **Glossary** — one entry per concept: name, definition, example
2. **Relationship Map** — a Mermaid or draw.io diagram showing the most important connections
3. **Rules and States** — what must be true; what conditions concepts can be in

Update these pages at the end of each sprint. The page history becomes the evolution of understanding.

---

## Jira: Work That Executes the Ontology

| Jira Artifact | ODPM Role |
|---|---|
| Epic | Ontology domain or concept cluster |
| Story | Work that references ontology concepts |
| Bug | Reality diverging from the ontology |
| Task | Implementation step within the shared model |
| Sprint | A snapshot cycle — understanding and increment evolve together |
| Label | Status of understanding |
| Comment thread | Chase Understanding conversation on a specific item |

### Labels for Understanding Status

| Label | Meaning |
|---|---|
| `open-question` | Concept not yet agreed on; needs Chase Understanding |
| `chase` | Active conversation in progress |
| `ontology-update` | Story requires an ontology change before development starts |
| `decision-ready` | Concept agreed, story references shared ontology, ready to build |

### Epics as Ontology Domains

Each Epic covers a cluster of related concepts.

For an OTA feature: one Epic for Campaign, one for Vehicle Eligibility, one for Update State.

Stories within an Epic reference the concepts defined for that domain.

A story that crosses Epic boundaries often signals an ontology relationship that has not been named yet.

---

## Workflow

### During Product Discovery

1. Create a Confluence space for the ontology.
2. Draft the glossary and relationship map with the team.
3. Reach agreement on Concepts, Relationships, Rules, and States before opening Jira.

### During Backlog Refinement

1. Review each story for ontology references.
2. If a story introduces an undefined concept, label it `open-question` and schedule a Chase Understanding session.
3. Only label a story `decision-ready` when it references the shared ontology without introducing undefined concepts.

### During Sprint Review

1. Demo the increment against the Confluence ontology, not only against acceptance criteria.
2. If the implementation diverged from the model, decide: update the implementation or update the ontology.
3. Record the decision in the Decision Log.

### During Sprint Retrospective

1. Ask: "What did we learn about the world this sprint?"
2. If the answer changes the model, update the Confluence ontology before the next sprint.
3. The page edit history records the snapshot.

---

## The One-Line Version

> Confluence holds the ontology. Jira executes it. The sprint cadences the snapshots.

---

See also: [ODPM and Scrum](../principles/odpm-and-scrum.md) · [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md)
