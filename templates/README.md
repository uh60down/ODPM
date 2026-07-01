# ODPM Templates

Practical, pick-up-and-use templates for running [the ODPM method](../ODPM-method.md).

The goal is not bureaucracy. The goal is to make ODPM usable without reading the whole theory first.

## Available now

| Template | Use it when | Method step |
|---|---|---|
| [Ontology Canvas](ontology-canvas.md) | Extracting the five building blocks from a source artifact | 2 |
| [PRD-to-Ontology Extraction](prd-to-ontology-extraction.md) | Reading a PRD or charter into an ontology | 1–2 |
| [Open Question Log](open-question-log.md) | Keeping findings from leaking between runs | 3–4, 7 |
| [Decision Readiness Checklist](decision-readiness-checklist.md) | Deciding whether to execute | 5 |
| [Change Ontology Canvas](change-ontology-canvas.md) | Modeling a change as the delta between two ontologies | 1–2 |
| [Sprint Ontology Review](sprint-ontology-review.md) | Running ODPM alongside Scrum ceremonies | 3–7 |
| [PMBOK Phase Gate Ontology Review](pmbok-phase-gate-ontology-review.md) | Gating a PMBOK phase on ontology alignment | 5, 7 |

## Wiring to GitHub

The maturity jump — `open question → tracked item → owner → decision → ontology update` — is wired through GitHub:

- [Open Question issue template](../.github/ISSUE_TEMPLATE/open-question.md) — every open question gets a home as an Issue.
- [Pull request template](../.github/pull_request_template.md) — every PR is a proposed ontology refinement.

See [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) for the full mapping.

**One-time setup:** GitHub only applies a label from an issue template if the label already exists. Create the ODPM label set once per repo so the issue template's `open-question` label takes effect:

```sh
gh label create open-question --description "An unresolved ontology question to chase"
gh label create chase        --description "Understanding is being pursued"
gh label create proposed     --description "A refinement has been suggested"
gh label create landed       --description "Understanding crystallized into an artifact"
gh label create archived     --description "Question closed without resolution"
```

---

See also: [The ODPM Method](../ODPM-method.md) · [ODPM at a Glance](../ODPM-at-a-glance.md)
