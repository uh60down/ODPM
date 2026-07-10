# Questions

ODPM treats questions as tools for discovering reality, not a checklist to clear. This file keeps foundational questions and open research questions visible without burying them inside prose.

## Foundational Questions

These questions are part of the core ODPM model.

- What exists?
- How are things related?
- What rules govern this world?
- What states can things be in?
- What actions can legitimately change them?
- Why are we building this?
- What would most improve the next decision?

The question is not: "Do we know everything?"

## Open Research Questions

These questions remain active areas for future refinement.

- How should Ontology evolve across releases?
- How should Ontology be organized across bounded contexts?
- How should ODPM represent **intention**? The ontology captures structure — what the domain is — but not what it is *for*, what matters most, or what to build first.
- How should ODPM capture **dynamic relationships**? The building blocks surface static relationships by inspection but miss concurrency, exclusion, causation, and side-effects — which only appear when the system runs.

## Current Working Answers

- Ontology should start as a glossary plus a lightweight relationship diagram.
- Ontology should stay small: Concepts, Relationships, Rules, States, and Actions.
- A PRD contains intent, requirements, assumptions, and constraints. Ontology makes the implicit world model explicit.
- Ontology changes should be reviewed through agreement, not authority — proposed as a Pull Request, tested in review, confirmed at merge. *(see principles/ontology-owned-by-agreement.md)*
- Git can become the history of understanding when commits are treated as snapshots of understanding, not just code changes. *(see principles/github-as-odpm-tool.md)*
- How can Chase Understanding be taught to new project members? Partially answered — teach through the Core Question Set, examples, and guided practice. *(see Core Question Set below)*
- Should ODPM be renamed? Resolved — yes. The acronym stays ODPM; its expansion is now **Ontology-Driven Practice Model** (formerly Project Management), which fits the broader scope. Evidence had accumulated across product, project, change, and consumer domains (Snapshots 011–013) that "Project Management" was actively narrow; the Term Migration was then justified rather than premature. *(see snapshots/014-ontology-driven-practice-model.md)*
- What is ODPM right now? Current working answer: the Ontology-Driven Practice Model, with two layers — a Base Ontology Layer and a Lightweight Execution Layer. This reframes ODPM from its original project-management expansion without changing the acronym. *(see snapshots/014-ontology-driven-practice-model.md)*
- How should ODPM represent intention? Unresolved — a known hole. The ontology models structure, not intention; today intention rides on top of it via user stories and value-ordering (e.g. "capture first, organize later"). Whether intention deserves a first-class place in the model, or belongs deliberately outside it, is open. Field evidence: the Voice Journal example, where one sentence of value-ordering out-designed the whole concept graph. *(see examples/voice-journal/ontology.md)*
- How should ODPM capture dynamic relationships? Partially answered — not with a sixth building block, but with a better question set. The gap-pattern checklist catches the five dynamic-relationship shapes (concurrency, dangling state, implied behavior, subsystem priority, side-effect) before building. Whether dynamic relationships also need explicit modeling beyond Actions-with-guards is still open. Field evidence: the Voice Journal example, where all five real gaps were dynamic relationships. *(see templates/gap-pattern-checklist.md)*

## Core Question Set

A teachable answer to "How can Chase Understanding be taught to new project members?" Not a checklist to clear, but a small set of questions a newcomer can carry into any conversation.

### Reality

- What exists?
- How are things related?
- What rules govern this world?
- What states can things be in?
- What actions can legitimately change them?

### Intent

- Why are we building this?

### Discovery

- What part doesn't make sense yet?
- What would most improve the next decision?
- Which thread should we pull next?

Reality and Intent map directly to the three-layer model (Chapter 4). Discovery is what keeps the chase moving; it has no fixed answers, only the next question.
