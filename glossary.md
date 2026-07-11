# Glossary

## Ontology

The team's shared model of the world: what exists, how things are related, what rules govern that world, what states matter, and what actions can legitimately change them.

Every good PRD already contains an implicit model of the world. ODPM makes that model explicit.

## Ontology-Driven Practice Model

The current expansion of ODPM: the base ontology-driven framework for turning intent into shared ontology, using that ontology to reach Decision Readiness, executing lightly against it, and updating it as reality pushes back.

## Base Ontology Layer

The ODPM layer that explains what ontology is and how teams model the world using Things, Relationships, Rules, States, and Actions.

## Lightweight Execution Layer

The ODPM layer that explains how teams use ontology in practice: source artifact → ontology → open questions → Decision Readiness → execution → feedback.

## Methodology

An execution strategy such as PMBOK, Agile, Scrum, Kanban, or SAFe.

ODPM does not replace methodologies. It clarifies the shared ontology those methodologies execute against.

## Methodologies as Strategies Over Ontology

The principle that methodologies do not define the world; they move work through a model of the world.

PMBOK, Scrum, Kanban, SAFe, and similar methods are strategies over an ontology. ODPM makes that ontology explicit.

## Delivery Ontology

An ontology for the work of delivery: Work Items, Changes, Verifications, Bugs, dependencies, capacity, and the relationships between them.

Distinct from a product ontology, which models the world being built.

## Understanding-unit

The atom of delivery in the project ontology: a unit of understanding being transformed into verified reality.

In software delivery, a Story or Bug can be a delivery-shaped instance of an understanding-unit.

## Verification Invariant

The rule that done means verified, never merely claimed.

A unit is not realized until reality has been checked against the understanding it was meant to express.

## Done Means Verified

The practical expression of the verification invariant.

An item is done only when it has been confirmed to match the ontology, acceptance criteria, or model it was meant to realize.

## Realizes

The relationship between a delivery unit and the thing or understanding it brings into verified reality.

Example: a Story realizes a Product Concept.

## Realizes-beyond

A relationship where a delivery grouping realizes more than its agreed things or child work items define.

It is a signal of unrecorded scope or an ontology gap.

## Ontology Boundary

A boundary between ontologies or bounded contexts.

In ODPM, boundaries are discovered through evidence, not imposed by preference. A boundary is justified when semantic divergence and independent evolution both appear.

## Term Migration

An ontology evolution operation where a term changes meaning, name, or scope.

Term migrations should be evidence-driven because a premature rename can hide confusion rather than resolve it.

## Thing

Something that exists in the world the team is modeling — concrete or abstract. The answer to "what exists?"

Formerly called *Concept* (still a valid synonym; see [One Concept, Not Two](principles/one-concept-not-two.md)).

Examples: User, Vehicle, Software Update, Campaign, Eligibility.

## Relationship

How things connect to each other.

Examples: a User owns a Vehicle, a Vehicle receives a Software Update, a Campaign targets a Vehicle Group.

## Rule

Something that must be true in the world.

Examples: an update cannot install while a vehicle is moving, a campaign cannot target unsupported hardware.

## State

A meaningful condition a thing can be in.

Examples: update available, download in progress, install scheduled, install failed, rollback required.

## Action

A named, legitimate way to move a thing from one state to another.

Distinct from a Rule, which constrains whether the action is allowed to happen, and from a State, which describes the condition before or after.

Examples: Install (download in progress → install scheduled), Rollback (install failed → rollback required), Offer Update (not eligible → update available).

## PRD

A product requirements document that contains intent, requirements, assumptions, and constraints.

In ODPM, a PRD is evidence for ontology. It is not replaced by ontology.

## Decision Readiness

The judgment that the team's current ontology is sufficient to take the next responsible action.

## Chase Understanding

The practice of using questions to discover reality and improve the next responsible decision.

## Snapshot

A numbered capture of the manuscript's thinking at a point in time.
