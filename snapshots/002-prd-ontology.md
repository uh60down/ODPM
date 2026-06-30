# Snapshot 002: Ontology Finds Its Place

Date: 2026-06-30

Today was a turning point.

We stopped asking "What is ontology?" and started using ontology as a practical artifact in project management.

The biggest realization was not a new framework, but finding the natural place where ontology belongs.

```text
PRD
(Intent + Requirements + Assumptions + Constraints)

    v

Ontology
(Shared Model of the World)

    v

Design
Architecture
Implementation
Testing
```

This simple model explains how existing project artifacts relate to each other without replacing them.

## Key Discoveries

### 1. Ontology found its place

Ontology is the shared model of the world.

It sits between the PRD and implementation.

It does not replace PRDs, Figma, Architecture, APIs, or Code.

Instead, every downstream artifact consumes the ontology.

### 2. PRD is not the problem

A PRD contains intent, requirements, assumptions, and constraints.

Example:

> "As a user, I want to switch between vehicles."

This statement expresses intent, but the complete PRD usually carries more.

The missing piece was never a replacement for the PRD.

The missing piece was the ontology describing the world already implicit in the PRD.

### 3. Chase Understanding

We replaced the idea of interviews and requirement elicitation with a simpler activity.

Chase Understanding.

Questions are not asked to complete a checklist.

Questions are asked to discover reality.

Every answer naturally leads to the next question.

### 4. Decision Readiness

Decision Readiness became clearer through practical discussion.

> The remaining unanswered questions no longer prevent the next responsible decision.

The goal is not complete understanding.

The goal is sufficient understanding to act responsibly.

### 5. Brownfield onboarding

Introducing ODPM into an existing project starts by reverse engineering the ontology from existing artifacts.

Artifacts become evidence of previous understanding.

Architecture diagrams, PRDs, Figma, APIs and code all reveal different parts of the same world.

### 6. User Stories and Ontology

User stories describe work.

Ontology describes the world.

Stories should reference ontology rather than duplicate domain knowledge.

Multiple stories can share the same ontology.

### 7. Ontology is a living artifact

Ontology evolves.

It is refined continuously through Chase Understanding.

Refinement is expected.

Changing the ontology is not correcting mistakes.

It is becoming more faithful to reality.

## Boss Compass

- Keep it simple and straightforward.
- Clarity over complexity.
- Principles over procedures.
- Questions over assumptions.
- Alignment over individual brilliance.
- Shared understanding before execution.

## Quotes Worth Keeping

> Understanding is not a destination we arrive at. It is a journey we share.

> We don't begin with shared understanding. We build it by chasing understanding together.

> Shared understanding is not transferred. It is co-created.

> Questions discover understanding.

> Artifacts preserve understanding.

> Every good PRD already contains an implicit model of the world. ODPM makes that model explicit.

> PRD gives everyone the mission and boundaries. Ontology ensures design, architecture, implementation, and testing aim at the same world.

## Current Core Model

```text
PRD
(Intent + Requirements + Assumptions + Constraints)

    v

Ontology
(Shared Model of the World)

    v

Design
Architecture
Implementation
Testing
```

This model satisfies KISS.

It explains the relationship between existing project artifacts without introducing unnecessary complexity.

## Open Threads

- How should ontology evolve across releases?
- How should ontology be visualized?
- How should ontology changes be reviewed?
- Can Git become the history of understanding?
- How should ontology be organized across bounded contexts?
- How can Chase Understanding be taught to new project members?

## Closing Thought

Today we stopped trying to improve existing artifacts.

Instead, we discovered the missing bridge that naturally connects them.

Ontology no longer feels like a philosophical concept.

It feels like something that can be used on Monday morning in a real project.
