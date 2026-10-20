# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-20, **Cycle 13** · Evidence-currency pass on the register's own rank-1 candidate, plus four gap verdicts and six frontier screens. **The register's top-ranked candidate was rejected on published evidence (IDEA-001 RECON-FLOW → R-011; V-001 withdrawn)**: the S&P 500 index effect has collapsed to ≈0 in the modern sample (additions below 1% over the past decade, −3 bps in 2020) and the flow-scaling differentiator has a published null (S-146, *Journal of Finance* 2025); the front-running is published as competitive anticipatory liquidity provision that shifts price pressure away from the effective date (S-147); the passive-flow counterparty is the issuing firm (S-151). Three gaps closed (G-02/G-07 — a published construction method for benchmark-specific tracked assets now exists, S-148; G-03 — the effective-close convention is documented, S-149/S-150; G-05's literature half — against IDEA-003's *single-name* extension, S-153/S-154), one gap reopened in part (G-04) and one opened (**G-18**). Two re-scores: IDEA-004 74.0 → 69.0 (published decay of the base effect, S-156), IDEA-009 63.0 → 60.0 (mechanism and mean reversion now published, S-158/S-159). **No new candidate**; six frontier families screened, six bounded negatives. Next: Cycle 14 — new IDs start at IDEA-015, S-175, V-010, G-19, R-012, P-011.
---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | **14 dossiers (IDEA-001 … IDEA-014)** — **6 active candidates** (IDEA-003, IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), 4 parked (P-004, P-008, P-009, P-010), **4 rejected** (R-008, R-009, R-010, and now **R-011 = IDEA-001**) |
| Ranked shortlist | **6 ranked** (72 / 71 / 69 / 65 / 60 / 60) + 4 parked + 4 withdrawn (IDEA-001, IDEA-006, IDEA-007, IDEA-012) |
| Source ledger | **174 verified sources (S-001 … S-174)** plus bounded-negative entries; Cycle 13 added S-146 … S-174 and a gap-verdicts block; **closed**: G-02/G-07, G-03, G-05 (literature leg); **open**: G-01, G-04 (reopened in part), G-14, G-15, G-16, **G-18 (new)** |
| Validation hand-offs | **9 specifications (V-001 … V-009)**, of which **V-001, V-004, V-005, V-006, V-007 are withdrawn**; **4 executable: V-002, V-003, V-008, V-009** — with **V-002 on hold until G-18 closes** |
| Rejected / parked | **11 rejected (R-001 … R-011)**, 10 parked (P-001 … P-010) |
| Canonical mission prompt | unchanged |

## 2. Highest-priority unresolved theoretical questions

1. **G-18 (new, and the highest-value item in the register)** — *is a return-correlation crowding measure a valid substitute for a holdings-based crowding measure?* The only decision-time, public, price-computable crowding proxy found in thirteen cycles is comomentum (S-157, Lou & Polk, *RFS* 2021), which infers arbitrage activity from return correlations. It has **never** been validated against the holdings-based position-concentration measure (S-026, Brown–Howard–Lundblad 2021) that IDEA-004's specification is frozen on. Until G-18 is closed, **V-002 must not be executed** and IDEA-004 must not be re-specified around the new proxy. The register's own rule forbids re-specifying around an unvalidated proxy.
2. **IDEA-011's post-2010 evidence base (never searched)** — IDEA-011 ACCTCLOCK is now the register's rank-1 item at 72.0 with an evidence score of 3/5, and its literature of record (Armstrong et al. 2010; Beuselinck et al. 2009) is largely pre-2015. The mirror image of the check that killed IDEA-001 has never been run for it: **does the announcement-to-first-report drift survive the post-2010 sample?** If it has decayed the way the momentum factor did (S-156), the candidate is a historical curiosity and must be re-scored down or parked; if it has not, that materially strengthens the evidence base. This is a bounded literature question and it is the single most valuable task available.
3. **G-01** — public funding-state proxy for a *dealer-level* funding value adjustment (IDEA-002 parked, P-004). Cycle-13 finding: the construct is peer-reviewed (S-155, Andersen–Duffie–Song, *JF* 2019) and the funding-state family is published — TGA flows drive repo-spread swings (S-160, IMF WP 2025) and the public TGCR − IORB spread is the decision-time stress measure (S-162) — but no public continuous dealer-level FVA series exists, and the published dealer-funding-terms measures remain the qualitative, quarterly SCOOS. The gap should now be stated as: *can any published, decision-time series proxy a dealer's marginal funding cost closely enough to condition a cross-sectional trade?* Do not spend more effort on "is the concept published" — it is.
4. **G-04 / G-16** — proxy validity. G-04 is reopened in part by S-157 (see item 1). G-16 (a validated public proxy for *credit*-dealer balance-sheet stress, IDEA-010's precondition) is narrowed but open: published Treasury-repo funding measures (S-161, S-162) are a *different construct* from credit-dealer balance-sheet stress, so they are not yet a valid substitute.
5. **G-15** — the RIN compliance-deadline price pattern (IDEA-014's first test). The candidate's sign is unasserted by design; the sign is the first empirical test. The California screen (below) is a boundary case worth reading first: it shows what the template needs (a state that makes the deadline demand *tight*) and what it does not need (a price collar).
6. **G-14** — a public borrow-cost series, not before 29 March 2029 (IDEA-008 parked, P-010). Dated; no effort needed before then.
7. **IDEA-013** — dated unblocking condition (post-2023 compliance years; next TNAC ~May/June 2027, deadline 30 September 2027). Do not spend effort before 2029.
8. **New mechanisms** — continue screening, but with the sharpened filter below (item 3 of section 3).

## 3. Best next research task (Cycle 14)

1. **Run the evidence-currency check on the remaining candidates — this is the priority, not new discovery.** Apply the standing condition added in Cycle 13 (see `rejected_and_parked.md`, rediscovery guard): *before a candidate is written or re-scored, its nearest published test must be re-read in the post-2010 sample.* Start with **IDEA-011** (the accounting-adoption drift in the post-2010 sample — the single highest-value question in the register), then **IDEA-003** (the aggregate variance risk premium's post-2010 magnitude: the Cycle-12 pass found the VRP's alpha contribution shrinking, Dew-Becker & Giglio, Chicago Fed WP 2025-17 — locate and register it properly), then **IDEA-010** and **IDEA-014** (both have thin, largely pre-2015 or non-refereed evidence bases).
2. **Close G-18 if it is closable by literature.** The question is narrow: does any published work validate a return-correlation crowding measure against a holdings-based crowding measure, or establish that the two proxies agree? If no such work exists, G-18 becomes a bounded negative and IDEA-004's specification is unexecutable in decision-time form — record that as such rather than leaving it ambiguous. Do **not** re-specify IDEA-004 around the new proxy either way.
3. **Screen frontier families with the sharpened filter.** The Cycle-13 screens showed that the template's binding practical question is not "is the state published?" but "**is the price-insensitive flow actually binding when it falls due, and who is on the other side of it?**" Apply it to every family screened: a supply valve that never opens (California's Allowance Price Containment Reserve, S-163/S-164) and an obligation met in advance (California's near-100% compliance surrender, S-165) both carry beautiful published state and no tradeable effect. Unexamined venues to consider: **fixed-income cash** (the register has no cash-bond candidate), **energy and power** (auction-settled, published settlement prices, published capacity calendars), **weather and catastrophe-linked instruments** (published event calendars), **shipping and aviation compliance dates** (IMO-style dated obligations with published schedules), and **US statutory deadlines outside the cap-and-trade family** (payment, tax-payment and reporting deadlines whose *size* is published, e.g. estimated-tax payment dates with published income aggregates). Write a full dossier only if the mechanism is unclaimed, the state is published *before* the decision, the sign (or existence) is decidable from that state, the flow is binding at the deadline, and the venue is feasible.
4. **Apply G-13/G-12 to any new candidate before ranking**, and re-state the two screens for every candidate whose evidence base changed.
5. **Maintain artifacts:** update `idea_register.md`, `ranked_shortlist.md`, `source_ledger.md`, `validation_handoffs.md`, `rejected_and_parked.md`, `cycle_notes.md`.
6. **Theory only.** No backtests, simulations, parameter sweeps, data acquisition, market-data processing, strategy or signal implementation, executable infrastructure, job launches, workflow changes, tests or trading. Cite every external claim with a verifiable URL/DOI; never invent a citation; distinguish index-rendered from directly fetched verification. Scores are research-priority weights, never probabilities of profit.
7. **Finish by rewriting this handoff** (section 4 is the verbatim message to paste into the next session) and by summarising the superseded handoff into `research/cycle_notes.md`. New IDs start at **IDEA-015, S-175, V-010, G-19, R-012, P-011**; call this **Cycle 14**.

## 4. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. Theory only: no backtests, no data
acquisition, no strategy or signal code, no trading, no job or workflow changes.

1. Read research/next_agent_handoff.md, then research/idea_register.md,
   research/ranked_shortlist.md, research/source_ledger.md and
   research/rejected_and_parked.md. Preserve prior work; do not renumber or delete IDs.

2. Execute the Cycle 14 task in section 3 of the handoff. Priority order:
   (a) run the evidence-currency check on the surviving candidates, starting with
       IDEA-011's post-2010 accounting-adoption drift; (b) attempt to close G-18
       (is a return-correlation crowding measure a valid substitute for a
       holdings-based crowding measure?); (c) screen frontier families in unexamined
       venues (fixed-income cash, energy/power, weather and catastrophe-linked,
       shipping and aviation compliance dates, US statutory deadlines outside the
       cap-and-trade family) using the filter "is the price-insensitive flow actually
       binding when it falls due, and who is on the other side of it?".

3. Run G-13 and G-12 as screens on every candidate whose evidence base changed, and
   record both verdicts in the dossier, the shortlist and the source ledger. A failure
   re-scores, parks or rejects the candidate. Re-read the nearest published test of any
   candidate in the post-2010 sample before you score it: that check is what rejected
   IDEA-001 in Cycle 13 (R-011).

4. Apply the three-pass task-framing loop; record it in research/cycle_notes.md. Do not
   modify the canonical prompt (research_prompts/systematic_edge_discovery_agent_prompt.txt).

5. Rank with the fixed rubric; write V-010+ for any new top-three candidate; log
   rejections and parkings with reasons and sources. New IDs start at IDEA-015, S-175,
   V-010, G-19, R-012, P-011; call this Cycle 14.

6. Absolute scope boundary: theory and discovery only.

7. Cite every external claim with a verifiable URL/DOI; never invent a citation;
   distinguish index-rendered from directly fetched verification; quote pre-publication
   numbers with their version. Scores are research-priority weights, never probabilities
   of profit.

8. Finish by rewriting research/next_agent_handoff.md and summarising the superseded
   handoff into research/cycle_notes.md.
```

## 5. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 8 | 2026-10-20 | G-04 closed as bounded negative (equity crowd proxy); screened families 2–5 as published baselines, family 1 gave no new candidate; T5–T8 revisited, no closures. | Yes. |
| 9 | 2026-10-20 | Applied G-12/G-13 screens across all candidates; one-round frontier screening found no unclaimed qualifying mechanism. No new dossiers. Gaps carried forward; handoff updated. | Yes. |
| 10 | 2026-10-20 | Applied G-12/G-13 screens across all candidates (Cycle 9 result confirmed); one-round frontier screening found no unclaimed qualifying mechanism meeting template; IDEA-014 sign untested (G-15). Gaps confirmed; handoff rewritten for Cycle 11. | Yes. |
| 12 | 2026-10-20 | Targeted gap investigation round: G-01 (no public dealer funding value adjustment series), G-02/G-07 (ICI category-level only), G-03 (no newly located auction convention), G-05 literature (index-level 0DTE VRP documented by Almeida/Freire/Hizmeri 2024/2025; single-name gate work not located). No new candidate; gaps carried forward; handoff rewritten for Cycle 13. | Yes. |
| 13 | 2026-10-20 | **Evidence-currency pass: IDEA-001 (rank 1, 76.0) rejected on published evidence (R-011; V-001 withdrawn)** — the index effect has collapsed to ≈0 and the flow-scaling differentiator has a published null (S-146), the mechanism is published as anticipatory liquidity provision (S-147) and the passive-flow counterparty is the issuer (S-151). Gaps closed: G-02/G-07 (published construction method, S-148), G-03 (convention documented, S-149/S-150), G-05's literature half (against IDEA-003's single-name extension, S-153/S-154). G-04 reopened in part; **G-18 opened**. Re-scores: IDEA-004 74.0 → 69.0 (S-156), IDEA-009 63.0 → 60.0 (S-158/S-159). Six frontier families screened (token unlocks; California surrender deadline; California reserve sale; TGA → repo; accelerated share repurchases; perpetual funding), six bounded negatives, **no new candidate**. Active ranking: 72 / 71 / 69 / 65 / 60 / 60. | Yes. |
