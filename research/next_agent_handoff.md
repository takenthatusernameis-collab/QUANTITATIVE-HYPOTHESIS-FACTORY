# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-20, **Cycle 11** · Targeted gap investigation round (G-01, G-02/G-07, G-03, G-05 literature) plus one frontier screening round. No new qualifying candidate found. G-01, G-02/G-07, G-03, G-05 (literature leg) remain open; G-14, G-15 remain open; G-04, G-16, G-13 closed as bounded negatives/conditions. Next: Cycle 12 — continue targeted gap closure and frontier screening; new IDs start at IDEA-015, S-146, V-010, G-18, R-011, P-011.

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | **14 dossiers (IDEA-001 … IDEA-014)** — 7 active candidates, 4 parked (P-008,P-009,P-010 plus related), 3 rejected |
| Ranked shortlist | **7 ranked** (76 / 74 / 72 / 71 / 65 / 63 / 60) + 4 parked + 3 withdrawn |
| Source ledger | **145+ verified sources (S-001 … S-145)** plus bounded-negative entries; gaps G-01,G-02/G-07,G-03,G-05,G-14,G-15 remain open; G-04,G-16 closed as bounded negatives |
| Validation hand-offs | **9 specifications (V-001 … V-009)**, of which V-004, V-005, V-006, V-007 withdrawn; 5 executable (V-001,V-002,V-003,V-008,V-009). V-001/V-002 amended per screens. |
| Rejected / parked | 10 rejected (R-001 … R-010), 10 parked (P-001 … P-010) |
| Canonical mission prompt | unchanged |

## 2. Highest-priority unresolved theoretical questions

1. **G-01** — public funding-state proxy (IDEA-002 parked). Cycle-11 finding: SCOOS is qualitative and quarterly; SOFR percentile spreads are published but do not directly measure dealer funding value adjustments; no continuous public series of dealer funding value adjustments located.
2. **G-02/G-07** — benchmark-specific passive-asset series (IDEA-001 scaling). Cycle-11 finding: ICI publishes category-level aggregates (indexed mutual funds + ETFs) but no benchmark-specific (e.g. S&P 500) tracked-asset series; gap remains open.
3. **G-03** — closing-auction convention/attribution (IDEA-001). Cycle-11 finding: no newly located documentation of index funds' effective-close trading convention; gap remains open.
4. **G-05** — single-name 0DTE literature leg (IDEA-003). Cycle-11 finding: no newly located peer-reviewed work establishing whether the single-name variance-gate channel is documented; gap remains open.
5. **G-14** — public borrow-cost series, not before 29 March 2029 (IDEA-008 parked).
6. **IDEA-013** — dated unblocking condition (post-2023 data).
7. **IDEA-014** — sign unasserted, first test is G-15 (data/literature side).
8. **New mechanisms** — continue screening for unclaimed mechanisms with published state before decision and sign decidable by published state.

## 3. Best next research task (Cycle 12)

1. **Address feasible gaps:** continue G-01 (composite proxy feasibility — test whether SOFR-percentile-spread × SCOOS composite predicts any disclosed dealer funding value adjustment), G-02/G-07 (benchmark-specific assembly from 13F/ICI category data), G-03 (auction convention/attribution), G-05 literature (single-name 0DTE).
2. **Screen frontier families:** run one search round per unexamined frontier family for mechanisms matching template. Write full dossier only if unclaimed, state published before decision, sign decidable by published state.
3. **Apply G-13/G-12 to any new candidate before ranking.** New IDs start at IDEA-015, S-146, V-010, G-18, R-011, P-011; call this Cycle 12.
4. **Maintain artifacts:** update idea register, ranked shortlist, source ledger, validation handoffs, rejected/parked, cycle notes.
5. **Theory only.** Cite every external claim with verifiable URL/DOI; distinguish index-rendered from directly fetched; scores are research-priority weights.
6. **Finish by rewriting this handoff and summarising into cycle_notes.**

## 4. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. Theory only: no backtests, no data
acquisition, no strategy code, no trading.

1. Read research/next_agent_handoff.md, then research/idea_register.md,
   research/ranked_shortlist.md, research/source_ledger.md and
   research/rejected_and_parked.md. Preserve prior work; do not renumber or delete IDs.

2. Execute the Cycle 12 task in section 3 of the handoff.

3. Run G-13 and G-12 as screens on every candidate before ranking; record both verdicts in the
   dossier, shortlist and source ledger. A failure re-scores or parks the candidate.

4. Apply the three-pass task-framing loop; record in research/cycle_notes.md. Do not modify the
   canonical prompt.

5. Rank with the fixed rubric; write V-010+ for any new top-three candidate; log rejections and
   parkings. New IDs start at IDEA-015, S-146, V-010, G-18, R-011, P-011; call this Cycle 12.

6. Absolute scope boundary: theory and discovery only.

7. Cite every external claim with a verifiable URL/DOI; never invent a citation; distinguish
   index-rendered from directly fetched verification. Scores are research-priority weights.

8. Finish by rewriting research/next_agent_handoff.md and summarising the superseded handoff into
   research/cycle_notes.md.
```

## 5. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 8 | 2026-10-20 | G-04 closed as bounded negative (equity crowd proxy); screened families 2–5 as published baselines, family 1 gave no new candidate; T5–T8 revisited, no closures. | Yes. |
| 9 | 2026-10-20 | Applied G-12/G-13 screens across all candidates; one-round frontier screening found no unclaimed qualifying mechanism. No new dossiers. Gaps carried forward; handoff updated. | Yes. |
| 10 | 2026-10-20 | Applied G-12/G-13 screens across all candidates (Cycle 9 result confirmed); one-round frontier screening found no unclaimed qualifying mechanism meeting template; IDEA-014 sign untested (G-15). Gaps confirmed; handoff rewritten for Cycle 11. | Yes. |
| 11 | 2026-10-20 | Targeted gap investigation round: G-01 (SCOOS/SOFR composite still not a published dealer funding value adjustment series), G-02/G-07 (ICI category-level only, no benchmark-specific series), G-03 (no newly located auction convention), G-05 literature (no newly located single-name 0DTE gate work). No new candidate; gaps carried forward; handoff rewritten for Cycle 12. | Yes. |
