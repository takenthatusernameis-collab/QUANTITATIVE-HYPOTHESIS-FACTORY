# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-20, **Cycle 14 (continued)** · Evidence-currency pass on IDEA-011 (post-2010 IFRS/adoption effects) and IDEA-003 (VRP decline). Added S-175/S-176/S-177. G-18 remains open (comomentum vs holdings-based crowding); V-002 on hold until G-18 closes. No new candidates. IDs available: IDEA-015, S-178+, V-010, G-19, R-012, P-011.

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | **14 dossiers (IDEA-001 … IDEA-014)** — **6 active candidates** (IDEA-003, IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), 4 parked (P-004, P-008, P-009, P-010), **4 rejected** (R-008, R-009, R-010, **R-011 = IDEA-001**) |
| Ranked shortlist | **6 ranked** (72 / 71 / 69 / 65 / 60 / 60) + 4 parked + 4 withdrawn (IDEA-001, IDEA-006, IDEA-007, IDEA-012) |
| Source ledger | **177+ verified sources (S-001 … S-177)**; **closed**: G-02/G-07, G-03, G-05 (literature leg); **open**: G-01, G-04 (reopened in part), G-14, G-15, G-16, **G-18 (new)** |
| Validation hand-offs | **9 specifications (V-001 … V-009)**, of which **V-001, V-004, V-005, V-006, V-007 are withdrawn**; **4 executable: V-002, V-003, V-008, V-009** — with **V-002 on hold until G-18 closes** |
| Rejected / parked | **11 rejected (R-001 … R-011)**, 10 parked (P-001 … P-010) |
| Canonical mission prompt | unchanged |

---

## 2. Highest-priority unresolved theoretical questions

1. **G-18 (highest-value for register execution)** — *is a return-correlation crowding measure (comomentum, S-157) a valid substitute for a holdings-based crowding measure (S-026)?* Never validated against each other. Until closed, **V-002 must not be executed** and IDEA-004 must not be re-specified around it. Find literature directly comparing comomentum/correlation-based crowding to 13F holdings-based measures.
2. **IDEA-011 post-2010 evidence (in progress)** — Post-2010 studies (Hung et al 2015, Song & Woo 2015 K-IFRS/PEAD, Rosmianingrum et al 2023 etc.) show IFRS adoption improves information environment and reduces PEAD in some settings, suggesting slow-diffusion drift may have decayed. Need targeted review: is there tradable announcement-to-first-report drift for low-info firms in post-2010 settings? If decayed like momentum (S-156), re-score down/park.
3. **IDEA-003 post-2010 magnitude** — Dew-Becker & Giglio (2025 Chicago Fed WP 2025-17, S-177) show VRP premium/alphas have declined to near zero; gate on harvestability is critical. Reassess state-gate strength.
4. **IDEA-010/014** thin evidence bases; G-16, G-15 open.
5. **G-01/G-04/G-16** — funding/dealer crowding proxies as before.

---

## 3. Best next research task (Cycle 15)

1. **Close or bound G-18**: Search for validation/comparison of return-correlation crowding proxies vs holdings-based crowding (comomentum S-157 vs Brown-Howard-Lundblad S-026). Look for papers testing substitutability/predictive overlap. If none exists, record bounded negative and keep V-002 frozen.
2. **Deeper evidence-currency for IDEA-011**: Focus on post-2010 PEAD magnitude around IFRS/adoption; check studies comparing pre/post adoption drift magnitude. Also consider enforcement regimes.
3. **IDEA-003 follow-up**: Review Dew-Becker & Giglio implications for state-gate; confirm gate design still viable.
4. **Maintain artifacts** as needed.
5. **Theory only.** No backtests, simulations, data acquisition, etc. Cite every claim.
6. **Finish by rewriting this handoff** and summarizing into cycle_notes.md. New IDs start at IDEA-015, S-178, V-010, G-19, R-012, P-011; call this **Cycle 15**.

---

## 4. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. Theory only: no backtests, no data
acquisition, no strategy or signal code, no trading, no job or workflow changes.

1. Read research/next_agent_handoff.md, then research/idea_register.md,
   research/ranked_shortlist.md, research/source_ledger.md and
   research/rejected_and_parked.md. Preserve prior work; do not renumber or delete IDs.

2. Execute the Cycle 15 task in section 3 of the handoff. Priority order:
   (a) close or bound G-18 (comomentum S-157 vs holdings-based crowding S-026) -
       find direct comparisons/validation; if none, record bounded negative and keep V-002 frozen;
   (b) deeper post-2010 evidence-currency check on IDEA-011 (PEAD magnitude around IFRS/adoptions,
       enforcement effects);
   (c) review implications of Dew-Becker & Giglio (2025 WP 2025-17, S-177) for IDEA-003 state-gate.

3. Run G-13 and G-12 as screens on every candidate whose evidence base changed, and
   record both verdicts. Re-read nearest published test in post-2010 sample before scoring.

4. Apply three-pass task-framing loop; record in research/cycle_notes.md. Do not modify
   canonical prompt.

5. Rank with fixed rubric; write V-010+ for any new top-three candidate; log
   rejections/parkings with reasons/sources. New IDs start at IDEA-015, S-178, V-010,
   G-19, R-012, P-011; call this Cycle 15.

6. Absolute scope boundary: theory and discovery only.
7. Cite every external claim with verifiable URL/DOI; distinguish index-rendered from
   directly fetched; quote pre-publication numbers with version. Scores are research-priority
   weights, never probabilities of profit.
8. Finish by rewriting research/next_agent_handoff.md and summarising superseded handoff
   into research/cycle_notes.md.
```

## 5. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 13 | 2026-10-20 | IDEA-001 rejected (R-011), G-02/G-07/G-03/G-05 closed, G-18 opened, re-scores IDEA-004/009, six frontier screens no new candidate. | Yes. |
| 14 | 2026-10-20 | Evidence-currency pass on IDEA-011 post-2010 (info environment improved -> drift opportunity likely weakened), added S-175/S-176, reviewed IDEA-003 (Dew-Becker & Giglio 2025-17 S-177) showing VRP harvestability declined; G-18 still open, V-002 on hold, frontier screens done. | Yes. |
| 14 (continued) | 2026-10-20 | Completed evidence-currency checks; added S-177; documented findings; handoff updated for Cycle 15. | Yes. |
