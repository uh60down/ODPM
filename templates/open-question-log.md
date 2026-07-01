# Open Question / Chase Understanding Log

The log that keeps findings from leaking between runs.

Every open question surfaced while extracting the ontology goes here, and every row is driven along the maturity chain:

```text
open question → tracked item → owner → decision → ontology update
```

A question is not done when it is asked. It is done when the ontology has been updated with the answer — or when the risk of leaving it open has been explicitly accepted.

---

| ID | Question | Raised by | Owner | Tracked item | Status | Resolution → ontology update |
|----|----------|-----------|-------|--------------|--------|------------------------------|
| Q1 | | | | _(Issue link)_ | open / chasing / decided / accepted-risk | |
| Q2 | | | | | | |

---

## Status meanings

- **open** — surfaced, not yet being pursued.
- **chasing** — Chase Understanding is in progress with the right people.
- **decided** — answered; the resolution has been written back into the ontology.
- **accepted-risk** — deliberately left open, with the risk named and owned.

## How this connects to GitHub

Each row's tracked item should be a real Issue, so the question has a home outside this file. See the [Open Question issue template](../.github/ISSUE_TEMPLATE/open-question.md) and [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md).

The log is the index. The Issues are where the chasing happens. The ontology update is where the answer is kept.

Note: this **Status** column tracks a question's resolution lifecycle. It is a different axis from the GitHub *labels* in [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) (`open-question`, `chase`, `proposed`, `landed`, `archived`), which mark an item's epistemic status. A question can be `chasing` here while its Issue carries the `chase` label — the two travel together but are not the same field.

Setup: the Open Question issue template applies the `open-question` label, and GitHub only applies a label that already exists. Create the label set from [GitHub as an ODPM Tool](../principles/github-as-odpm-tool.md) once per repo, or the auto-label silently does nothing.

---

See also: [The ODPM Method](../ODPM-method.md) · [Chase Understanding](../principles/chase-understanding.md)
