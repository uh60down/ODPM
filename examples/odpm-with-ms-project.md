# ODPM with MS Project and SharePoint

This is a tooling guide for teams using MS Project and SharePoint alongside ODPM and PMBOK.

The principles of how ODPM integrates with PMBOK do not depend on any specific tool.

## Three Tool Roles

Any ODPM + PMBOK implementation needs three roles filled:

| Role | Purpose | Example tools |
|---|---|---|
| Knowledge Base | Holds the living ontology: glossary, relationship map, decision log | SharePoint, Confluence, Notion |
| Schedule and Work Management | Tracks tasks, milestones, WBS, and resource assignments | MS Project, Smartsheet, Primavera P6 |
| Change Control | Records and evaluates change requests against the ontology | SharePoint list, Jira, or MS Project change log |

This guide uses SharePoint as the Knowledge Base and MS Project as Schedule and Work Management.

The patterns apply to any equivalent tool pair.

---

## SharePoint: Ontology Home

The living ontology belongs in SharePoint, not in MS Project.

| SharePoint Page or Document | ODPM Role |
|---|---|
| Glossary page | Concept definitions — the shared vocabulary |
| Relationship diagram | How concepts connect (Visio, draw.io, or embedded diagram) |
| Project Charter page | Intent, Requirements, Assumptions, Constraints |
| Assumptions Log | Unresolved ontology questions — Chase Understanding targets |
| Decision Log | Snapshots of understanding at key decisions |
| Lessons Learned | End-of-project ontology snapshot |
| Meeting notes | Chase Understanding conversations preserved as evidence |

### Starting Template

A minimal ontology space needs four pages:

1. **Glossary** — one entry per concept: name, definition, example
2. **Relationship Diagram** — the most important connections between concepts
3. **Rules and States** — what must be true; what conditions concepts can be in
4. **Assumptions Log** — open questions being chased, with status and owner

Update these at each phase gate. The version history becomes the evolution of understanding.

---

## MS Project: Executing the Ontology

MS Project tracks the work that delivers the ontology into reality.

| MS Project Element | ODPM Role |
|---|---|
| Project Summary Task | Maps to the top-level ontology scope |
| WBS phases | Map to ontology domains or concept clusters |
| Tasks | Implementation steps within the shared model |
| Milestones | Phase gates — Decision Readiness checkpoints |
| Resource assignments | Execution ownership mapped to roles and responsibilities |
| Custom fields | Status of understanding (optional — see labels below) |

### Custom Field Labels for Understanding Status

These are example labels. Adapt them to your organization's existing conventions.

| Label | Meaning |
|---|---|
| `open-question` | Concept or scope area not yet agreed on |
| `ontology-update` | Work item requires ontology change before execution starts |
| `decision-ready` | Shared model agreed, item is ready to execute |

---

## Workflow Across Process Groups

### During Initiating

1. Receive the approved Project Charter.
2. Create the ontology space in SharePoint.
3. Extract the implicit ontology from the Charter: What concepts exist? What relationships? What rules? What states?
4. Add unresolved assumptions to the Assumptions Log as open questions.

### During Planning

1. Build the Glossary and Relationship Diagram with the team.
2. Work through the Assumptions Log using Chase Understanding — schedule sessions for significant open questions.
3. Baseline the ontology alongside the Scope Statement before building the WBS.
4. Align the WBS phases to ontology domains.
5. Build the Communications Plan as a One Ontology, Multiple Views exercise — what does each audience need to see?

### During Executing

1. When a stakeholder raises a concern or resists a direction, treat it as an ontology gap before treating it as a stakeholder management problem.
2. If new understanding emerges, log it in the Decision Log before it becomes a change request.

### During Monitoring and Controlling

1. For every change request, ask first: does this redefine a concept, relationship, rule, or state?
2. If yes — that is an ontology-level change. Evaluate it at that level before approving scope, schedule, or cost changes.
3. Update the ontology in SharePoint when a change is approved. The version history records the snapshot.

### During Closing

1. Conduct a Lessons Learned session structured around the ontology: What concepts were wrong or missing? What rules turned out not to hold? What states were we missing?
2. Archive the final ontology alongside the project closure documents.
3. The ontology becomes a starting point for similar future projects — brownfield onboarding rather than starting from zero.

---

## The One-Line Version

> SharePoint holds the ontology. MS Project executes it. Phase gates version the snapshots.

---

See also: [ODPM and PMBOK](../principles/odpm-and-pmbok.md) · [One Ontology, Multiple Views](../principles/one-ontology-multiple-views.md) · [Change Ontology](../principles/change-ontology.md)
