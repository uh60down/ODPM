# Glossary

## Ontology

The team's shared model of the world: what exists, how things are related, what rules govern that world, what states matter, and what actions can legitimately change them.

Every good PRD already contains an implicit model of the world. ODPM makes that model explicit.

## Concept

A thing that exists in the product world.

Examples: User, Vehicle, Software Update, Campaign, Eligibility.

## Relationship

How concepts connect to each other.

Examples: a User owns a Vehicle, a Vehicle receives a Software Update, a Campaign targets a Vehicle Group.

## Rule

Something that must be true in the world.

Examples: an update cannot install while a vehicle is moving, a campaign cannot target unsupported hardware.

## State

A meaningful condition a concept can be in.

Examples: update available, download in progress, install scheduled, install failed, rollback required.

## Action

A named, legitimate way to move a concept from one state to another.

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
