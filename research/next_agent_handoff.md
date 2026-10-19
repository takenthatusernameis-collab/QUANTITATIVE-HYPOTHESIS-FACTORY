# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-19, partial Cycle 5 pass · G-10 residual narrowed (likely closed by Fed 2024 / Avdjiev cross-sectional CIP work, pending verification); G-11, G-06 and T5–T8 remain open

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | 12 dossiers (IDEA-001 … IDEA-012) — 4 listed US equities, 8 outside them; IDEA-006 and IDEA-007 narrowed to v1.1 |
| Ranked shortlist | 12 ranked, scored out of 100 (76 / 74 / 72 / 72 / 71 / 68 / 65 / 64 / 63 / 63 / 59 / 56) |
| Source ledger | **94 verified sources (S-001 … S-094)**, source gaps G-01 … G-11 (G-06 narrowed, G-09/G-10 mostly closed, G-11 open) |
| Validation hand-offs | **9 specifications (V-001 … V-009)** |
| Rejected / parked | **7 rejected (R-001 … R-007)**, 7 parked (P-001 … P-007), 15-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged** |
| Validation performed | **None.** No candidate has been tested. |

Cycle 4 added three dossiers (IDEA-010 CREDIT-ETF, IDEA-011 ACCTCLOCK, IDEA-012 CLS-CLOSE),
re-ranked all twelve candidates under the fixed rubric (IDEA-011 enters at rank 3 tied at 72.0;
IDEA-010 at rank 6; IDEA-012 at rank 12), wrote V-009 for IDEA-011, extended the state-proxy
methodological note to cover the new candidates' data-access profile, and added S-090 … S-094 to
the source ledger. G-10 residual remains open (aggregate dollar-funding channel confirmed, not the
cross-section). G-11 remains open (settlement-side deadline cluster untested as a price
determinant). G-06 remains narrowed but not closed exhaustively. T5–T8 remain open with recorded
verdicts. The state-proxy/venue-selection lesson stands; the methodological note is recorded as a
closing section of `research/idea_register.md`.

## 2. Highest-priority unresolved theoretical questions

1. **G-10 residual — partially narrowed.** Fed 2024 "Quantities and Covered-Interest Parity" tests
   cross-sectional variation in CIP bases conditional on safe-asset ratios and intermediary capacity;
   Avdjiev et al. (2016) [S-009] already explains cross-sectional CIP variation via differential
   dollar sensitivity. Pending verification whether either tests the *interest-differential-conditional*
   currency response to a dollar funding expansion specifically; if confirmed, IDEA-007 v1.1 is
   rejected. Candidate new source S-095 (Fed 2024 working paper).
2. **G-11 — has anyone tested the settlement-side deadline cluster as a price determinant?** Open.
   Settlement-side mechanics are a priced friction (S-082, S-071) but the specific CLS deadline
   cluster / post-US-close T+1 window is untested. IDEA-006 v1.1 and IDEA-012 are both blocked.
3. **G-06 residual — does any commodity basis-convergence paper condition on passive share ×
   depth?** Narrowed but not closed exhaustively.
4. **Bounded tasks T5–T8** (G-03/G-08 closing-auction concentration; G-01 composite funding spec;
   G-05 single-name side; G-07 benchmark-specific passive-asset series) remain open.

## 3. Next mechanism families to investigate (not yet in the register)

1. Corporate credit: index and ETF flow against dealer balance-sheet capacity (IDEA-010 added but
   its AP-level data constraint is commercial).
2. Slow information diffusion with an identifiable event clock (accounting standards adoption dates
   — IDEA-011 added).
3. Settlement and payment infrastructure as a structural dated flow (continuation of IDEA-006's
   vein; IDEA-012 added but blocked on G-11).

## 4. Best next research task (Cycle 5)

Close the remaining gaps (G-10 residual, G-11 fully, G-06 exhaustively) and the bounded supporting
tasks T5–T8, then produce 2–3 new dossiers in mechanism families not yet in the register, where
the decision-time state variable is published by a venue, regulator, benchmark administrator or
settlement utility. Re-rank, add validation specs for new top-three candidates (V-010 onward),
update handoff.

## 5. Operating rules for the next session

1. Read this file first, then register, shortlist, source ledger, rejected/parked.
2. Theory only, absolutely. No backtests, data acquisition, code, metrics, workflow/test/infra
   edits, trading.
3. Do not modify the canonical prompt.
4. Preserve prior work; add, do not delete or renumber. New IDs: IDEA-013+, S-095+, V-010+,
   G-12+, R-008+, P-008+; call next cycle Cycle 5.
5. Never invent a citation; re-derive every identifier; treat agent-supplied bibliographies as
   unverified.
6. Locate contradicting evidence deliberately.
7. Scores are research priority, not success probability.
8. Update this handoff last; keep the initial task message current and self-contained.

## 6. Environment observations

Carried forward unchanged: `.github/workflows/main.yml` references missing
`scripts/controller_progress.py` and test modules; run diagnostics report failure despite durable
commits. Maintainer item; not acted on.

## 7. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. This is a research-prioritisation
environment only.

1. Read the durable handoff at research/next_agent_handoff.md first, then
   research/idea_register.md, research/ranked_shortlist.md,
   research/source_ledger.md and research/rejected_and_parked.md. Do not
   regenerate what already exists and do not renumber or delete existing IDs.

2. Execute the best next research task stated in section 4 of the handoff:
   close the remaining blocking originality gaps (G-10 residual, G-11 fully,
   G-06 exhaustively) and the bounded supporting tasks T5-T8, then produce
   2-3 new dossiers in mechanism families not yet in the register, choosing
   families where the decision-time state variable is published by a venue,
   regulator, benchmark administrator or settlement utility. Each dossier must
   name the participant, the binding constraint, a decision-time-observable
   state variable (with who publishes it and on what calendar), a dated or
   state-dependent flow, the expected return source, an honest originality
   comparison, falsifiable predictions with explicit rejection conditions,
   confounders, data requirements, a theory/evidence status, and verified
   sources. Also attempt T5-T8 and record any gap you cannot close as a new
   source gap.

3. Apply the three-pass task-framing loop and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file.

4. Rank the new candidates with the fixed rubric in
   research/ranked_shortlist.md (re-checking existing ranks), write
   validation hand-off specifications for any new top-three candidate
   (V-010 onward), and log anything rejected or parked.

5. Absolute scope boundary: theory and discovery only. No backtests,
   simulations, parameter sweeps, significance tests, market data
   acquisition/processing, strategy code, executable research infrastructure,
   job/workflow/CI launches, workflow/test/credential/infrastructure changes,
   or trading. If a question can only be answered by running something,
   document it precisely and hand it off.

6. Cite every external claim with a verifiable URL or DOI and never invent
   a citation. Re-derive every identifier yourself; treat agent-supplied
   bibliographies as unverified. Record how each source was verified.
   Scores are research-priority weights, not probabilities of profit.

7. Finish by rewriting research/next_agent_handoff.md: current pipeline
   state, highest-priority unresolved questions, next families, open gaps,
   best next task, environment observations, and a fresh self-contained
   initial task message. Summarise the superseded handoff into
   research/cycle_notes.md.
```

## 8. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 1 | 2026-10-19 | First cycle: pipeline created, 4 dossiers, 28 sources, 3 validation specs, 3 rejections, 4 parkings, baseline table, durable handoff. | Yes. |
| 2 | 2026-10-19 | New venue families: 3 new dossiers, 26 sources, gap verdicts, re-ranked shortlist, V-004 + 2 optional specs, 2 new rejections, 3 new parkings, baseline table extended. | Yes. |
| 2 (closure 1) | 2026-10-19 | G-10 mostly closed; IDEA-007 narrowed to v1.1 (R-006); no published cross-currency basis series in BIS. | Yes. |
| 2 (closure 2) | 2026-10-19 | G-09 mostly closed; IDEA-006 narrowed to v1.1 (R-007, 66→59); G-11 opened; phantom citation and fabricated bibliography found. | Yes. |
| 3 | 2026-10-19 | G-06 narrowed, G-11 partially closed, G-10 residual open; IDEA-008 and IDEA-009 added; state-proxy methodological note written; V-007/V-008; re-ranked (9 candidates). | Yes. |
| 4 | 2026-10-19 | IDEA-010/011/012 added; V-009 written; all twelve re-ranked (IDEA-011 at rank 3 tie, IDEA-010 at 6, IDEA-012 at 12); S-090…S-094 added; state-proxy note extended; G-10 residual open, G-11 open, G-06 narrowed but not closed; T5–T8 verdicts recorded. | Yes — this file. |
