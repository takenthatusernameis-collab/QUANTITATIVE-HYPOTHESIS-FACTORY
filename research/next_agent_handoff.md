# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-19, end of Cycle 3 · Cycle 3 closed · Next cycle: Cycle 4

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | 9 dossiers (IDEA-001 … IDEA-009) — 4 listed US equities, 5 outside them; IDEA-006 and IDEA-007 narrowed to v1.1 |
| Ranked shortlist | 9 ranked, scored out of 100 (76 / 74 / 72 / 71 / 65 / 64 / 63 / 63 / 59) |
| Source ledger | **89 verified sources (S-001 … S-089)**, source gaps G-01 … G-11 (G-06 narrowed, G-09/G-10 mostly closed, G-11 partially closed) |
| Validation hand-offs | 8 specifications (V-001 … V-008) |
| Rejected / parked | **7 rejected (R-001 … R-007)**, 7 parked (P-001 … P-007), 15-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged** |
| Validation performed | **None.** No candidate has been tested. |

Cycle 3 closed the three blocking originality gaps (G-06 narrowed, G-11 partially closed, G-10 residual still open), added two dossiers (IDEA-008 SECURITY-LEND, IDEA-009 PERP-FUND) in families where the state is published by an institution, wrote the state-proxy methodological note, and re-ranked. The state-proxy/venue-selection lesson stands; the methodological note is now recorded as a closing section of `research/idea_register.md`.

## 2. Highest-priority unresolved theoretical questions

1. **G-10 residual — is the cross-sectional funding-state claim already published?** Still open. No located paper tests which currencies respond most to a dollar funding expansion conditional on the interest differential. If found, IDEA-007 is rejected.
2. **G-11 — has anyone tested the settlement-side deadline cluster as a price determinant?** Partially closed: settlement-side mechanics are a priced friction (S-082, S-071) but the specific CLS deadline cluster / post-US-close T+1 window is untested. IDEA-006 v1.1 blocked.
3. **G-06 residual — does any commodity basis-convergence paper condition on passive share × depth?** Narrowed but not closed exhaustively.
4. **Bounded tasks T5–T8** (G-03/G-08 closing-auction concentration; G-01 composite funding spec; G-05 single-name side; G-07 benchmark-specific passive-asset series) remain open.

## 3. Next mechanism families to investigate (not yet in the register)

1. Corporate credit: index and ETF flow against dealer balance-sheet capacity.
2. Slow information diffusion with an identifiable event clock (accounting standards adoption dates).
3. Settlement and payment infrastructure as a structural dated flow (continuation of IDEA-006).

## 4. Best next research task (Cycle 4)

Close the remaining gaps (G-10 residual, G-11 fully, G-06 exhaustively, T5–T8) and produce 2–3 new dossiers in the untouched families above, where the decision-time state variable is published by an institution. Re-rank, add validation specs for new top-three candidates, update handoff.

## 5. Operating rules for the next session

1. Read this file first, then register, shortlist, source ledger, rejected/parked.
2. Theory only, absolutely. No backtests, data acquisition, code, metrics, workflow/test/infra edits, trading.
3. Do not modify the canonical prompt.
4. Preserve prior work; add, do not delete or renumber. New IDs: IDEA-010+, S-090+, V-009+, G-12+, R-008+, P-008+; call next cycle Cycle 4.
5. Never invent a citation; re-derive every identifier; treat agent-supplied bibliographies as unverified.
6. Locate contradicting evidence deliberately.
7. Scores are research priority, not success probability.
8. Update this handoff last; keep the initial task message current and self-contained.

## 6. Environment observations

Carried forward unchanged: `.github/workflows/main.yml` references missing `scripts/controller_progress.py` and test modules; run diagnostics report failure despite durable commits. Maintainer item; not acted on.

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
   2-3 new dossiers in mechanism families not yet in the register (corporate
   credit index/ETF flow vs dealer balance sheet; slow information diffusion
   with an event clock; settlement/payment infrastructure as a structural
   dated flow), choosing families where the decision-time state variable is
   published by a venue, regulator, benchmark administrator or settlement
   utility. Each dossier must name the participant, the binding constraint, a
   decision-time-observable state variable (with who publishes it and on what
   calendar), a dated or state-dependent flow, the expected return source, an
   honest originality comparison, falsifiable predictions with explicit
   rejection conditions, confounders, data requirements, a theory/evidence
   status, and verified sources. Also attempt T5-T8 and record any gap you
   cannot close as a new source gap.

3. Apply the three-pass task-framing loop and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file.

4. Rank the new candidates with the fixed rubric in
   research/ranked_shortlist.md (re-checking existing ranks), write
   validation hand-off specifications for any new top-three candidate
   (V-009 onward), and log anything rejected or parked.

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
| 3 | 2026-10-19 | G-06 narrowed, G-11 partially closed, G-10 residual open; IDEA-008 and IDEA-009 added; state-proxy methodological note written; V-007/V-008; re-ranked (9 candidates). | Yes — this file. |
