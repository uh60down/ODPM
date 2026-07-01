# The ODPM Maturity Model

ODPM is not all-or-nothing. A team can get value from naming its ontology long before that ontology becomes operational or executable.

This model gives teams a path — and, just as important, permission not to demand too much too early. Most teams do not need Level 5. The right level is the one that makes the next decision better.

---

## The Ladder

| Level | Name | In one line |
|---|---|---|
| 0 | Implicit | Understanding is private and scattered. |
| 1 | Named | The team uses ODPM language. |
| 2 | Documented | A lightweight ontology exists as an artifact. |
| 3 | Reviewed | Ontology changes go through agreement. |
| 4 | Operational | Work references the ontology. |
| 5 | Platformed | The ontology is executable. |

Each level assumes the ones below it.

---

## Level 0 — Implicit

Teams rely on private understanding and scattered documents. Everyone has a model of the world in their head; no two are quite the same.

**You're here when:** the same disagreement keeps resurfacing, and no one can point to where the shared model is written down — because it isn't.

**To advance:** start naming things. Run the [method](ODPM-method.md) once on a real artifact.

## Level 1 — Named

The team uses ODPM language: ontology, concepts, relationships, rules, states, actions. The vocabulary is shared even if the model isn't written yet.

**You're here when:** people say "that's a new concept" or "which state is it in?" without being prompted.

**To advance:** write the vocabulary down. A [glossary](glossary.md) is enough to start.

## Level 2 — Documented

A lightweight ontology exists as an artifact: a glossary, a relationship map, and the rules, states, and actions. Not a heavy model — a page the team can point to.

**You're here when:** a newcomer can read the ontology instead of interviewing five people.

**To advance:** use the [templates](templates/) — the [Ontology Canvas](templates/ontology-canvas.md) is the fastest start. Then stop letting anyone change it silently.

## Level 3 — Reviewed

Ontology changes are proposed, reviewed, and agreed — like pull requests. No single person redefines a shared concept alone.

**You're here when:** changing the ontology feels like changing shared code: it needs a proposal and a second pair of eyes.

**To advance:** adopt [Ontology Is Owned by Agreement](principles/ontology-owned-by-agreement.md) and the [GitHub-as-ODPM-tool](principles/github-as-odpm-tool.md) mapping — Issue as Open Question, PR as Proposed Refinement, Merge as Ontology Aligned.

## Level 4 — Operational

Work items, decisions, bugs, and change requests reference the ontology. It is no longer a document you visit — it is the thing the work points back to.

**You're here when:** the maturity jump is wired in — every open question becomes a tracked item with an owner, and its resolution updates the ontology:

```text
open question → tracked item → owner → decision → ontology update
```

**To advance:** close the loop with the [Open Question Log](templates/open-question-log.md) and the [issue template](.github/ISSUE_TEMPLATE/open-question.md), and fold the framework-specific reviews ([Scrum](templates/sprint-ontology-review.md), [PMBOK](templates/pmbok-phase-gate-ontology-review.md)) into your cadence.

## Level 5 — Platformed

The ontology becomes executable or semi-executable through tools, workflows, agents, or systems. Applications query the same objects, follow the same relationships, respect the same rules — there is no per-application re-interpretation of what a concept means.

**You're here when:** the ontology is not just describing the world, it is running part of it. See [Snapshot 006: Ontology as a Platform Layer](snapshots/006-ontology-as-platform-layer.md). (That snapshot predates the Action building block, so it maps four blocks to a platform's objects, links, rules, and states; at this level, Actions become the platform's operations.)

**To advance:** there is no next level. The work here is keeping the platformed ontology honest — the higher the automation, the more governance, permissions, and auditability matter.

---

## How to Use This

- **Locate yourself honestly.** Most teams are at Level 0 or 1 and think they are higher.
- **Aim one level up, not five.** The jump from Implicit to Named is worth more than any leap toward Platformed.
- **Stop where value stops.** A small team may top out at Level 3 and be perfectly served. Level 5 is for teams whose scale or safety needs justify it.

The model is a ladder, not a scoreboard.

---

See also: [The ODPM Method](ODPM-method.md) · [ODPM at a Glance](ODPM-at-a-glance.md) · [Templates](templates/) · [GitHub as an ODPM Tool](principles/github-as-odpm-tool.md)
