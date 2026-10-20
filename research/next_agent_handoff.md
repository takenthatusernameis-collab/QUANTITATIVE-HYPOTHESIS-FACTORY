# DURABLE HANDOFF — NEXT AGENT

Last updated: 2026-10-20, **Cycle 38**. Cycle 38 executed priorities: (1) G-29 (IDEA-010) — inspected corporate-bond ETF prospectuses/SAIs (AGG, ISTB) via filings; prospectuses disclose AP concentration risk generically but **do not name authorised participants**. EDGAR searches found no bond ETF filing naming AP sets for the inspected funds. **Coverage count**: 0 of inspected corporate-bond ETFs have a publicly reconstructable AP set from their statutory filings; consequently (ETF, AP) cells with both a published AP set and a public capital ratio are 0 from this route. **Verdict:** not specifiable from public bond ETF filings — untested, not dead. Do not substitute a published crowding proxy (S-026, S-157, S-222 measure different crowds). G-27/G-29 bounded by this finding; V-010 executable only if a specifiable route emerges. (2) G-27/G-29 counts noted: X-17A-5 is public (S-231) so capital state availability is closed in favour (Cycle 37); coverage count remains bounded by (1). (3) G-28 (IDEA-004) remains frozen (13F holdings-matching route with four objections). (4) G-21 (IDEA-011) confirmed null and comparison written down. (5) IDEA-014 state-free limb remains inconclusive. Screened (A) Rule 10b-18 daily buyback cap as rate-limited template → **bounded negative R-019** (issuer cap, not third-party deadline-driven flow; remaining capacity published monthly/lagged). **No score changed; no candidate created; no validation specification added.**

## 1. State of the pipeline

Counts re-derived from artifact files (Cycle 38):

| Item | Status |
| --- | --- |
| Idea register | 15 dossiers (IDEA-001 … IDEA-015); **5 active** (IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), **6 parked** (IDEA-002 P-004, IDEA-003 P-012, IDEA-005 P-009, IDEA-008 P-010, IDEA-013 P-008, IDEA-015 P-011), **4 rejected** (IDEA-001 R-011, IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010) |
| Ranked shortlist | 5 ranked — **IDEA-011 69.0 (rank 1), IDEA-004 69.0 (rank 2), IDEA-010 68.0 (rank 3), IDEA-009 60.0, IDEA-014 52.0**; tie at 69.0 broken in IDEA-011's favour on falsifiability (4 vs 3) |
| Source ledger | **228 verified sources** (S-001 … S-209, S-220 … S-238); S-210 … S-219 reserved and unused |
| Validation hand-offs | 10 specs (V-001 … V-010). **Executable: V-008, V-009, V-010.** V-002 **frozen** (G-28). V-003 **never-to-execute**. Withdrawn: V-001, V-004, V-005, V-006, V-007. V-010 amended in Cycle 37 |
| Rejected / parked | **19 rejections** (R-001 … R-019) and **12 parkings** (P-001 … P-012); P-013 reserved and unused |
| Known-baseline table | **59 rows** (ex-dividend R-017, Rule 201 R-018, Rule 10b-18 R-019 added) |
| Gaps | G-01 … G-29 defined (G-17 skipped, G-26 reserved and unused). **Open: G-04, G-21, G-28, G-29, G-01.** G-27 closed in IDEA-010's favour in Cycle 37 |
| Next free identifiers | **IDEA-017, S-239, V-012, G-30, R-019 is consumed, next R-020, P-014** |

## 2. Highest-priority unresolved theoretical questions

1. **G-29 (IDEA-010)** — mapping ETF → authorised participants and coverage count. Bond ETF statutory filings inspected do not name APs; verify via prospectus/SAI of other major corporate-bond ETFs (additional issuers) using EDGAR full-text API where direct fetches block. If no bond ETF names APs, record "not specifiable — untested, not dead" and do not substitute proxy.

2. **G-27/G-29** — compute effective-sample counts (firms with public capital ratio, per-firm cadence, regime composition, resulting (ETF,AP,episode) cells). Note entity_filter truncation to 30 buckets; page properly.

3. **G-28 (IDEA-004)** — frozen; test whether published short leg (FINRA twice-monthly short interest, S-127) can separate convergence capital from directional bear, record as lead with objections.

4. **G-21 (IDEA-011)** — null confirmed; comparison documented.

5. **IDEA-014** state-free existence limb — inconclusive.

## 3. Best next research task (Cycle 39)

Execute in order as specified by priorities below.

## 4. Initial task message for the next agent (copy verbatim)

You are continuing a **theory-only** hypothesis-generation and research-prioritisation repository. Read `research/next_agent_handoff.md` first, then `research/idea_register.md`, `research/ranked_shortlist.md`, `research/source_ledger.md`, `research/validation_handoffs.md`, `research/rejected_and_parked.md` and `research/cycle_notes.md`, before generating anything. Mission defined by canonical prompt `research_prompts/systematic_edge_discovery_agent_prompt.txt` (maintainer-owned, must not be edited).

**Absolute scope boundary.** Not allowed: backtests, simulations, parameter sweeps, optimisation, significance testing on strategy results, performance/risk metrics, market-data acquisition/processing, strategy/signal implementation, executable research infrastructure, job/workflow launches, changes to workflow files, tests, credentials/infrastructure, work outside this repository, trading. Allowed: reading/summarising literature, market-structure/venue/regulator docs, this repo's notes; specifying hypotheses, falsifiable predictions, observables, data requirements; maintaining theory-only artifacts. If only answerable by running something, write question precisely and hand off.

**Current state (re-derive yourself).** 15 dossiers: 5 active (IDEA-011 69.0 rank 1, IDEA-004 69.0 rank 2, IDEA-010 68.0 rank 3, IDEA-009 60.0, IDEA-014 52.0), 6 parked, 4 rejected. 228 verified sources (S-001 … S-209, S-220 … S-238; S-210 … S-219 reserved). 10 validation specs (V-001 … V-010): V-008,V-009,V-010 executable; V-002 frozen; V-003 never-to-execute; V-001,V-004–V-007 withdrawn. 19 rejections (R-001 … R-019), 12 parkings (P-001 … P-012; P-013 reserved), 59 baseline rows. Gaps G-01–G-29; open G-04,G-21,G-28,G-29,G-01. Cycle 37 found X-17A-5 public (G-27 closed favour IDEA-010), G-29 opened. Cycle 38: bond ETF filings don't name APs → coverage 0 from that route; R-019 added. Next free: **IDEA-017, S-239, V-012, G-30, R-020, P-014**. This cycle **Cycle 39**.

**Execute these priorities in order.**
1. **G-29 (IDEA-010)** — do corporate-bond ETF statutory prospectus/SAI name authorised participants? Inspect major corporate-bond ETFs (AGG, ISTB, and one each from two other issuers). If direct sec.gov/Archives fail (403), use EDGAR full-text API: `https://efts.sec.gov/LATEST/search-index?q="authorized participants"&forms=497` (add ciks/dateRange/from/size as needed). Compute coverage: how many bond ETFs have reconstructable AP set; how many (ETF,AP) cells where AP also has public capital ratio. If none name APs, record: "state cannot be attached to ETF from public filings; IDEA-010 not specifiable — untested, not dead". Do not substitute proxy. Update G-29, IDEA-010, V-010.
2. **G-27/G-29** — using Cycle-37 routes (X-17A-5 EDGAR; listed 10-Q/10-K XBRL; FR Y-9C for bank APs), count distinct firms with public capital ratio, per-firm cadence, regime composition, resulting (ETF,AP,episode) cells. Note entity_filter truncation (max 30 buckets) — page with from/size. Report "untested — not dead" if counts small; never upgrade small-sample null to kill.
3. **G-28 (IDEA-004)** — keep frozen, V-002 frozen. Test FINRA twice-monthly short-interest (S-127) mapped to pair structure (short interest in acquirer around announcement) to separate convergence capital from directional bear. Record as lead with objections (construction not published measure; bi-monthly; equities only).
4. **IDEA-014 state-free limb** — maintain inconclusive; no effort without new source.
5. **One new mechanism family screen** — (A) Rule 10b-18 daily 25% ADTV cap (daily, not monthly; no 10b-18 source in ledger — add one if needed); (B) eligibility-switch (who may hold, published compliance date, published distance-to-limit); (C) benchmark methodology change with published effective date. Apply strict bar, log bounded negatives as R-020+.
6. **Wrap up.** Update idea_register.md, ranked_shortlist.md, source_ledger.md (explicit verification tags, never invent citation), validation_handoffs.md (specifications only), rejected_and_parked.md, cycle_notes.md (three-pass task-framing loop). Score with fixed rubric as research priority, never probability of profit. Rewrite `research/next_agent_handoff.md` with re-derived counts, next priorities, fresh verbatim initial task message for Cycle 40.

**Standing rules.** Read handoff+register before generating; preserve prior work. Every external claim → source ledger entry with verification; never present index-rendered quote as directly parsed. Re-derive all counts/IDs from files. Leave session with updated handoff and fresh initial task message for next agent.
