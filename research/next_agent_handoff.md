# DURABLE HANDOFF — NEXT AGENT

Last updated: 2026-10-20, **Cycle 39**. Cycle 39 executed priorities: (1) G-29 (IDEA-010) — inspected additional major corporate-bond ETF issuers beyond AGG/ISTB: Vanguard (Target Maturity 2027–2036 Corporate Bond, Core-Plus Bond Index), Xtrackers (USD High Yield Corporate Bond, HYLB), PGIM (Corporate Bond 0-5/5-10/10+ Year), Global X (Investment Grade Corporate Bond, GXIG), Northern Funds (tax-exempt bond series), Columbia (Corporate Bond, Core Plus Bond). All statutory prospectuses/SAIs disclose AP concentration risk generically and do not name authorised participants. Coverage count remains 0 of inspected corporate-bond ETFs with a publicly reconstructable AP set; (ETF, AP) cells with both a published AP set and a public capital ratio remain 0 from this route. Verdict stands: not specifiable from public bond ETF filings — untested, not dead. Do not substitute a published crowding proxy. (2) G-27/G-29 counts remain bounded by (1); X-17A-5 public route (S-231) still open in favour. (3) G-28 (IDEA-004) remains frozen. (4) G-21 (IDEA-011) null confirmed. (5) IDEA-014 state-free limb remains inconclusive. (6) One new mechanism family screen: Rule 201 short-sale price test (R-018) already logged Cycle 37; no new bounded negative added this cycle. No score changed; no candidate created; no validation specification added.

## 1. State of the pipeline

Counts re-derived from artifact files (Cycle 39):

| Item | Status |
| --- | --- |
| Idea register | 15 dossiers (IDEA-001 … IDEA-015); **5 active** (IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), **6 parked** (IDEA-002 P-004, IDEA-003 P-012, IDEA-005 P-009, IDEA-008 P-010, IDEA-013 P-008, IDEA-015 P-011), **4 rejected** (IDEA-001 R-011, IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010) |
| Ranked shortlist | 5 ranked — **IDEA-011 69.0 (rank 1), IDEA-004 69.0 (rank 2), IDEA-010 68.0 (rank 3), IDEA-009 60.0, IDEA-014 52.0** |
| Source ledger | **228 verified sources** (S-001 … S-209, S-220 … S-238); S-210 … S-219 reserved and unused |
| Validation hand-offs | 10 specs (V-001 … V-010). **Executable: V-008, V-009, V-010.** V-002 **frozen** (G-28). V-003 **never-to-execute**. Withdrawn: V-001, V-004, V-005, V-006, V-007. V-010 amended in Cycle 37 |
| Rejected / parked | **19 rejections** (R-001 … R-019) and **12 parkings** (P-001 … P-012); P-013 reserved and unused |
| Known-baseline table | **59 rows** |
| Gaps | G-01 … G-29 defined (G-17 skipped, G-26 reserved and unused). **Open: G-04, G-21, G-28, G-29, G-01.** G-27 closed in IDEA-010's favour in Cycle 37 |
| Next free identifiers | **IDEA-017, S-239, V-012, G-30, R-019 is consumed, next R-020, P-014** |

## 2. Highest-priority unresolved theoretical questions

1. **G-29 (IDEA-010)** — confirmed across additional issuers: no corporate-bond ETF prospectus/SAI names APs. Coverage 0. If no bond ETF ever names APs, record "not specifiable — untested, not dead". V-010 executable only if a specifiable route emerges.
2. **G-27/G-29** — effective-sample counts using X-17A-5 EDGAR, listed 10-Q/10-K XBRL, FR Y-9C routes. Page properly (entity_filter max 30 buckets).
3. **G-28 (IDEA-004)** — frozen; FINRA twice-monthly short-interest (S-127) mapped to pair structure as a lead with objections.
4. **G-21 (IDEA-011)** — null confirmed; comparison specified.
5. **IDEA-014** state-free existence limb — inconclusive.

## 3. Best next research task (Cycle 40)

Execute in order as specified by priorities below.

## 4. Initial task message for the next agent (copy verbatim)

You are continuing a **theory-only** hypothesis-generation and research-prioritisation repository. Read `research/next_agent_handoff.md` first, then `research/idea_register.md`, `research/ranked_shortlist.md`, `research/source_ledger.md`, `research/validation_handoffs.md`, `research/rejected_and_parked.md` and `research/cycle_notes.md`, before generating anything. Mission defined by canonical prompt `research_prompts/systematic_edge_discovery_agent_prompt.txt` (maintainer-owned, must not be edited).

**Absolute scope boundary.** Not allowed: backtests, simulations, parameter sweeps, optimisation, significance testing on strategy results, performance/risk metrics, market-data acquisition/processing, strategy/signal implementation, executable research infrastructure, job/workflow launches, changes to workflow files, tests, credentials/infrastructure, work outside this repository, trading. Allowed: reading/summarising literature, market-structure/venue/regulator docs, this repo's notes; specifying hypotheses, falsifiable predictions, observables, data requirements; maintaining theory-only artifacts. If only answerable by running something, write question precisely and hand off.

**Current state (re-derive yourself).** 15 dossiers: 5 active (IDEA-011 69.0 rank 1, IDEA-004 69.0 rank 2, IDEA-010 68.0 rank 3, IDEA-009 60.0, IDEA-014 52.0), 6 parked, 4 rejected. 228 verified sources (S-001 … S-209, S-220 … S-238; S-210 … S-219 reserved). 10 validation specs (V-001 … V-010): V-008,V-009,V-010 executable; V-002 frozen; V-003 never-to-execute; V-001,V-004–V-007 withdrawn. 19 rejections (R-001 … R-019), 12 parkings (P-001 … P-012; P-013 reserved), 59 baseline rows. Gaps G-01–G-29; open G-04,G-21,G-28,G-29,G-01. Cycle 39: additional bond ETF issuers inspected (Vanguard, Xtrackers, PGIM, Global X, Northern, Columbia) — all generic AP risk disclosure, none name APs; coverage remains 0. Next free: **IDEA-017, S-239, V-012, G-30, R-020, P-014**. This cycle **Cycle 40**.

**Execute these priorities in order.**
1. **G-29 (IDEA-010)** — final verification whether *any* corporate-bond ETF statutory filing names APs (EDGAR full-text: `https://efts.sec.gov/LATEST/search-index?q="authorized participants"&forms=497`). If none, record: "state cannot be attached to ETF from public filings; IDEA-010 not specifiable — untested, not dead". Update G-29, IDEA-010, V-010.
2. **G-27/G-29** — count distinct firms with public capital ratio via X-17A-5 EDGAR, listed 10-Q/10-K XBRL, FR Y-9C; per-firm cadence, regime composition, resulting (ETF,AP,episode) cells. Page with from/size (entity_filter max 30 buckets). Report "untested — not dead" if counts small.
3. **G-28 (IDEA-004)** — keep frozen, V-002 frozen. Test FINRA twice-monthly short-interest (S-127) mapped to pair structure. Record as lead with objections.
4. **IDEA-014 state-free limb** — maintain inconclusive; no effort without new source.
5. **One new mechanism family screen** — (A) eligibility-switch (who may hold, published compliance date, published distance-to-limit); (B) benchmark methodology change with published effective date; (C) Rule 10b-18 daily 25% ADTV cap (already R-019; do not repeat). Apply strict bar, log bounded negatives as R-020+.
6. **Wrap up.** Update idea_register.md, ranked_shortlist.md, source_ledger.md, validation_handoffs.md, rejected_and_parked.md, cycle_notes.md. Score with fixed rubric as research priority. Rewrite `research/next_agent_handoff.md` with re-derived counts, next priorities, fresh verbatim initial task message for Cycle 41.

**Standing rules.** Read handoff+register before generating; preserve prior work. Every external claim → source ledger entry with verification. Re-derive all counts/IDs from files. Leave session with updated handoff and fresh initial task message for next agent.
(End of file)