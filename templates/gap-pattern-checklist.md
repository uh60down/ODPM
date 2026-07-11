# Gap-Pattern Checklist

Run this **after drafting an ontology and before building.** It catches the *dynamic* relationships — concurrency, exclusion, causation, side-effects, state/action coherence — that the five building blocks surface less reliably than static structure.

> The nouns come out right by inspection. The verbs between the verbs go missing.

Earned from the [Voice Journal example](../examples/voice-journal/ontology.md), where all five of the real gaps turned out to be dynamic relationships — invisible on paper, and only visible once the system ran. Each check below caught one of them.

---

## The five checks

- [ ] **State exclusivity** — for every State: is it exclusive of the others, or concurrent with them? A "mode" that can run alongside another isn't one exclusive state — it's a separate axis. *(Voice Journal: Playback runs alongside browsing, so it's a `Stopped`/`Playing` axis, not an App state.)*

- [ ] **Dangling states** — for every State: does an Action both *produce* it and *consume* it? A state no Action reaches, or that no Action leaves, is a modeling gap. *(Voice Journal: `Paused` existed with no Pause action — removed from MVP.)*

- [ ] **Action implication** — for every pair of Actions: does one imply the other? Make the implied relationship explicit. *(Voice Journal: Stop Recording implies Save; with no Discard, stopping always saves.)*

- [ ] **Subsystem priority** — for every pair of subsystems / state machines: what is their priority or exclusion rule when both are active? *(Voice Journal: starting a recording stops active playback — recording wins.)*

- [ ] **Side-effects** — for every Action: what states does it disturb *besides* its target? *(Voice Journal: deleting the playing record must stop playback first.)*

---

## For each gap you find

Turn it into a **rule candidate** (make the decision explicit and write it as a Rule), or, if it can't be resolved yet, move it to the [Open Question Log](open-question-log.md) with an owner.

The five questions ODPM starts with collect static relationships cleanly but systematically miss dynamic ones. This checklist is the earned hardening — a better question set, derived from evidence, not theory.

---

See also: [Voice Journal Example](../examples/voice-journal/ontology.md) · [Ontology Canvas](ontology-canvas.md) · [Open Question Log](open-question-log.md) · [Decision Readiness Checklist](decision-readiness-checklist.md)
