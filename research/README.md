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
3. **ID discipline.** Ideas are `IDEA-0NN` (next free: `IDEA-017`; `IDEA-016` is **reserved and
   unused**),    sources are `S-0NN` (next free: `S-383`; `S-210 … S-219` are **reserved and unused**),
   validation specs are `V-0NN` (next free: `V-012`; `V-011` is **reserved and unused**, and `V-010`
   is written and now marked **never-to-execute**), rejections are `R-0NN` (next free: `R-056`), parkings are `P-0NN` (next
   free: `P-015`; `P-013` is **reserved and unused**), source gaps are `G-NN` (next free: `G-37`;
   `G-17` and `G-26` were skipped by the sequence and have never been used), and cycles are `Cycle N`
   (next: `Cycle 103`; **Cycle 102 completed the Cycle-101 provenance-upgrade operation over its
   thirteen named targets (nine fully upgraded, six partial with the unverified parts named, one
   honest negative), closed four of the six Priority-3 open questions, consumed two new source
   identifiers (S-381, S-382), struck one quotation in place, made three material bibliographic
   corrections, recorded a state-integrity finding — the Cycle-101 operation had never reached the
   ledger — and rewrote the handoff body**; **Cycle 97 was
   executed but never written up in the cycle log — its boundary record
   was added retrospectively in Cycle 98, and its work is visible only as annotations in the source
   ledger**).
   A reserved identifier is one that a prior cycle claimed in writing but never wrote into an
   artifact; it is left unused on purpose so that a later reconstruction of that work cannot collide
   with a new one.
   Reuse an existing source ID rather than duplicating a citation; extend the "supports" note instead.
   **The ID ranges quoted in the repository's `AGENTS.md` are historical** (they stop at IDEA-012 and
   S-094); the authoritative next-free IDs are the ones in item 3 above and in `next_agent_handoff.md`.
   **Re-derive every identifier yourself** (publisher, Crossref, arXiv, NBER or the institution's
   own site) before it enters the ledger: identifiers supplied by a search or research agent have
   been found wrong, and one registered working paper carries a fabricated bibliography. Record
   whether a document was **fetched directly** or read only through a **search index**, and never
   present an index-rendered quotation as a directly parsed document. **A quotation that cannot be
   re-checked by extracting the document's text layer is not yet a quotation** — extract it, or
   record the entry as index-rendered and unattributed. **A failed retrieval must be recorded as a
   failed retrieval**: mark the entry NOT VERIFIED, list the routes tried and their failure modes, label
   the wording as index-rendered, and restate the corpus's verification status (how many items are
   line-verified versus index-confirmed). Never let a "fetched directly" verification line stand on a
   document that was in fact unreachable.
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
