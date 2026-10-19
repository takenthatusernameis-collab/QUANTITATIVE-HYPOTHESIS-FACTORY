# QUANTITATIVE HYPOTHESIS FACTORY — THEORY-ONLY RESEARCH AREA

This directory holds the durable, theory-only research pipeline for this repository. Nothing in it
is a backtest, a strategy implementation, a performance claim, or a validation result. The scope is
defined by the canonical mission prompt, which is **not** to be modified:

- Mission prompt (canonical, maintainer-owned): `research_prompts/systematic_edge_discovery_agent_prompt.txt`

## Files

| File | Purpose |
| --- | --- |
| `next_agent_handoff.md` | **The durable handoff.** Start every session here. Holds the current task, the open questions, source gaps, and the ready-to-run initial task message for the next agent. |
| `idea_register.md` | Full dossiers for every retained candidate (mechanism, observables, rule sketch, falsifiers, evidence status). |
| `ranked_shortlist.md` | Rubric-scored ranking with hard-stop flags, weights, and per-score justification. |
| `source_ledger.md` | Verified citations (ID, full reference, URL/DOI, what each source supports, verification method, caveats). |
| `validation_handoffs.md` | Theory-to-validation specifications for shortlisted candidates. Specification only — never executed here. |
| `rejected_and_parked.md` | Rejected/parked candidates with reasons, plus the known-baseline list, to prevent rediscovery. |
| `cycle_notes.md` | Cycle log, the mandatory three-pass task-framing loop, and the change history of the artifacts. |

## Working agreements for future sessions

1. **Read `next_agent_handoff.md` first**, then the register and shortlist, before generating anything new.
2. **Preserve prior work.** Add to the register; do not silently delete, relabel, or renumber existing IDs.
3. **ID discipline.** Ideas are `IDEA-0NN` (next free: `IDEA-005`), sources are `S-0NN` (next free:
   `S-029`), validation specs are `V-0NN` (next free: `V-004`), cycles are `Cycle N` (next: `Cycle 3`).
   Reuse an existing source ID rather than duplicating a citation; extend the "supports" note instead.
4. **Never invent a citation.** Every external claim in a dossier points to an `S-0NN` entry in the
   source ledger, and every ledger entry records how it was verified. If a claim cannot be sourced,
   mark it as an unresolved conjecture in the dossier.
5. **Scores are research-priority weights, not success probabilities.** No numerical probability of
   profit is attached to any candidate; the rubric score is a transparent weighted total out of 100.
6. **Theory only.** No backtests, no data acquisition or processing, no executable strategy code, no
   performance metrics, no workflow/test/infra edits, no cross-repository work. Unresolvable questions
   are documented and handed off, not silently relaxed.
7. **Every session ends with an updated handoff** naming the best next research task, the highest-value
   unresolved theoretical questions, and the next mechanism families to investigate.
