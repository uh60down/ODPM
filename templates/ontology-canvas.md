# Ontology Canvas

A one-page canvas for extracting the ontology from a source artifact.

Copy this file, fill each section, and keep it short. The goal is a shared model the team can point to — not a complete specification.

> Source artifact: _(PRD / charter / mandate / brief / existing system / complaint / change request)_
> Date: _(YYYY-MM-DD)_
> Owner: _(who maintains this canvas)_

---

## Concepts

The things that exist in this world.

| Concept | Meaning |
|---|---|
| | |
| | |

## Relationships

How the concepts connect.

- _(A owns B)_
- _(B receives C)_

## Rules

What must always be true. Constraints, independent of any single action.

- _()_
- _()_

## States

The meaningful conditions a concept can be in.

- _(Concept: state → state → state)_

## Actions

The named, legitimate ways a concept moves from one state to another.

| Action | Actor | From → To | Guard (what must be true first) |
|---|---|---|---|
| | | | |

---

## Open Questions

Anything unclear, disputed, missing, or assumed. Move each of these into the [Open Question Log](open-question-log.md).

- [ ] _()_
- [ ] _()_

---

## Example (filled)

A small slice, using the software-update domain from the [glossary](../glossary.md), to show the shape:

- **Concepts:** Vehicle, Software Update, Campaign.
- **Relationships:** a Campaign targets Vehicles; a Vehicle receives a Software Update.
- **Rules:** an update cannot install while a vehicle is moving.
- **States:** Software Update — available → downloading → install scheduled → installed → install failed.
- **Actions:**

| Action | Actor | From → To | Guard |
|---|---|---|---|
| Install | Vehicle owner | install scheduled → installed | vehicle stationary; battery sufficient |
| Roll back | System | install failed → available | update left the vehicle unsafe |

- **Open question:** who is authorized to trigger *Roll back* — the owner, or the system automatically? _(→ Open Question Log)_

---

See also: [The ODPM Method](../ODPM-method.md) · [Glossary](../glossary.md)
