# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-20, **Cycle 6 in progress** · Primary task begun: IDEA-005 reconciled with S-098/S-099 (fails G-12 → parked as baseline re-description, P-009 pending); G-13 timing table drafted for 8 candidates; remaining: G-12 for IDEA-001/003/004/008/009/010/011, five-family frontier screen, T5–T8, re-rank, V-010+

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | **13 dossiers (IDEA-001 … IDEA-013)** — 8 active candidates, 2 parked (IDEA-002, IDEA-013), 3 rejected (IDEA-006, IDEA-007, IDEA-012, dossiers retained only so the reasoning is not re-derived) |
| Ranked shortlist | **8 ranked** (76 / 74 / 72 / 72 / 71 / 68 / 65 / 63) + 2 parked (63, 58) + 3 withdrawn (64, 59, 56) |
| Source ledger | **125 verified sources (S-001 … S-125)**, source gaps G-01 … G-13 |
| Validation hand-offs | **9 specifications (V-001 … V-009)**, of which **V-005 and V-006 are withdrawn** (their candidates were rejected); **7 executable** |
| Rejected / parked | **10 rejected (R-001 … R-010)**, 8 parked (P-001 … P-008), 28-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged** |
| Validation performed | **None.** No candidate has been tested. Every score is a research priority, not a probability of profit. |

Cycle 5 was run in two halves and is now closed. The first half closed G-10 against IDEA-007 (**R-008** —
the cross-sectional funding-state → currency-return claim is a published, positive result, S-064),
closed G-06 as a bounded negative finding with contradicting evidence registered (S-098, S-099), mostly
closed G-08, split G-05, added **IDEA-013 (EU-ETSCOMP)** and registered S-095 … S-111. The second
half — this session — closed **G-11 against IDEA-006 (R-009) and IDEA-012 (R-010)**: a settlement
deadline cluster is a published price determinant (S-112), the securities settlement cycle is a
published price-impact determinant (S-113, S-114, S-115), and the post-US-close FX window is
documented as a **cost** rather than an edge (S-117 … S-120). It also performed IDEA-013's outstanding
full-text check on the published work it claims to differ from: the check resolved **in the
candidate's favour** (the published work does not condition the premium on the aggregate surplus) but
**against it** in three ways, and the decisive finding was a timing one — the EU ETS aggregate balance
is published in late May or June of the year *after* the emissions year (S-121), so under the pre-2023
regime it was published **after** the surrender deadline it was meant to inform. IDEA-013 was therefore
**parked (P-008)** at 58.0 with a dated unblocking condition, and the register opened **G-13**: a
published state is usable as a decision-time variable only if it is published *before* the decision.
Four further frontier families were screened and found published (margin schedules, S-122; ETF
primary-market arbitrage, S-123; crypto spot-ETF flow, S-124, S-125) and are now baseline rows, so the
next cycle does not re-derive them.

## 2. Highest-priority unresolved theoretical questions

1. **G-13 — is every active candidate's state actually published *before* its decision?** This is the
   new screening condition (state-proxy note, condition (e)) and it has **not yet been applied
   systematically** to the eight active candidates. Established instance: the EU ETS aggregate
   balance (S-121). The same question applies to CFTC positioning data for IDEA-005 (published with a
   lag), exchange short-interest and lending-fee filings for IDEA-008, adoption calendars for
   IDEA-011, and the venue funding rate for IDEA-009. **A candidate whose state is published after
   its decision must be re-scored or parked, and the register's rule is that re-specifying around a
   weaker proxy is not allowed.**
2. **G-12 — does each active candidate's state conditioning change the *sign or existence* of the
   effect, rather than only its size?** The register's standing test, introduced in Cycle 5. It has
   not been applied systematically to IDEA-001, IDEA-003, IDEA-004, IDEA-005, IDEA-008, IDEA-009,
   IDEA-010 or IDEA-011. A candidate that fails this test is a baseline re-description and belongs in
   `rejected_and_parked.md`.
3. **IDEA-005's contradicting evidence.** S-099 is the closest published test of IDEA-005's own state
   variable (CIT market share) and reports **no significant effect**; S-098 conditions spot–futures
   convergence on *trader type*. The candidate has not yet been reconciled with either. This is the
   only *active* candidate with published evidence against it, so it should be settled first.
4. **G-01 — a public funding-state proxy** (IDEA-002's feasibility kill condition; T6). The most
   valuable open gap for a *parked* candidate, and the standing instance of the state-proxy problem.
   SOFR, standing-repo and primary-dealer data are public ingredients, but no published, continuous
   series of dealer funding value adjustments exists (S-041, S-042), and the published literature
   prices the constraint with proprietary dealer-level data (S-095, S-096).
5. **G-02 / G-07 — a benchmark-specific passive-asset series** (IDEA-001's data gap; T8). Individual
   ETF assets are public; no aggregate benchmark-specific series for all S&P 500 trackers exists, and
   ICI's series (S-040) is category-level only.
6. **G-03 / G-08 — the trading convention behind the effective close, and closing-auction
   concentration** (T5). No public closing-auction volume statistics have been located.
7. **G-04 — the crowd-depth proxy** for IDEA-004, whose left tail is a broken anchor.
8. **G-05 — the single-name 0DTE literature.** The *data* question is closed (the series is
   constructible from public OCC data, S-100); the *literature* question is open.
9. **IDEA-013's dated unblocking condition.** No effort is to be spent on it before 2029: the next
   TNAC (emissions year 2026) is expected in late May or June 2027, the corresponding surrender
   deadline is 30 September 2027, and the candidate cannot be validated in decision-time form before
   the aggregate balance has crossed a sign change with an observation on each side (P-008).

## 3. Next mechanism families to investigate (not yet in the register)

**Closed by Cycle 5 — do not re-derive:** settlement and payment infrastructure as a price
determinant (published: S-112, S-082, S-071; the window is a cost: S-117 … S-120); securities
settlement cycle length as a price-impact determinant (published: S-113, S-114, S-115);
exchange-published margin schedules (published: S-122); ETF primary-market arbitrage and AP inventory
(published: S-123); crypto spot-ETF flow (published: S-124, S-125); benchmark-window alteration
(published: S-047, S-080).

**Still open — screen first, dossier only if unclaimed:**

1. **Statutory, date-bound obligations outside the EU ETS** — the template IDEA-013 instantiated, but
   in a venue with a different regulator, a different obligor population and a *published* state that
   is available before the decision. Screen before any writing: US RFS/RIN volumes (EPA), shipping
   compliance regimes, the UK's ETS. Note the feasibility trap — a yearly deadline means a yearly
   observation, and a state published after the deadline kills the candidate (G-13).
2. **Sovereign issuance calendars** — the US Treasury's quarterly refunding announcement publishes
   coupon auction sizes and the issuance-duration decision on a known calendar; the state is official
   and in advance. Screen against the published term-premium and duration-of-supply literature before
   writing.
3. **Fast-payment rails as a published structural change** — FedNow, the UK's RTP and the EU's TIPS
   publish usage statistics; the mechanism would be intraday liquidity demand and payment-finality
   pricing. Screen against the BIS/central-bank "fast payments and liquidity demand" literature.
4. **Sovereign bond index inclusion/exclusion** — index administrators publish review calendars and
   the passive-tracking estimates; the flow is scheduled and dated. Screen against the published
   index-flow literature (and note that IDEA-001 already occupies the equity reconstitution instance).
5. **Physical-delivery calendars in commodity futures** — exchanges publish delivery and notice
   calendars and, in some contracts, warehouse stock series; the state is official and in advance.
   Screen against the published inventory/convenience-yield literature (S-038, S-039) and against
   IDEA-005's roll family.

## 4. Best next research task (Cycle 6)

**Primary — apply the two standing screening questions to the active register (highest value per
unit of effort, and required for internal consistency).** For each of the eight active candidates
(IDEA-001, IDEA-003, IDEA-004, IDEA-005, IDEA-008, IDEA-009, IDEA-010, IDEA-011): (a) record, per
observation, the **publication date of the state relative to the decision date** (G-13), and (b) test
whether the state conditioning changes the **sign or existence** of the effect rather than its size
(G-12). Any candidate that fails either test is re-scored or parked, with the reasoning recorded in
`rejected_and_parked.md` and the baseline table. Settle **IDEA-005 first**, because it is the only
active candidate with published evidence against it (S-098, S-099).

**Secondary — frontier generation.** Screen the five families in section 3 against the published
literature *first* (one search each, recording the verdict in the source ledger even when the
verdict is "published — baseline"), and write a full dossier only for a family whose mechanism is
unclaimed and whose state is published **before** the decision.

**Tertiary — the bounded supporting tasks.** T5 (G-03/G-08 closing-auction concentration), T6
(G-01 composite funding spec), T7 (G-05 single-name 0DTE literature), T8 (G-07 benchmark-specific
passive-asset series). Record any gap that cannot be closed as a new source gap with a precise
question.

**Then** re-rank everything under the fixed rubric, write a validation specification for any new
top-three candidate (V-010 onward), log rejections and parkings, and rewrite this handoff.

**Do not** spend effort on IDEA-013 before 2029, and do not re-open G-10, G-11 or G-06 without a new
mechanism.

## 4b. Cycle 6 progress (this session)

- **IDEA-005 (ROLLCOND) settled.** State variable: CIT market share from CFTC COT/DCOT. COT is published Friday 3:30pm ET on the prior Tuesday's positions (3-business-day lag), so it is published before the monthly roll decision calendar — G-13 passes for availability. However, S-099 (Maréchal 2021, J. Futures Markets) conditions commodity returns during roll periods on CIT market share and reports **no significant effect**; S-098 (trader-type conditioning of spot–futures convergence) is the closer published test of the state. IDEA-005 therefore **fails G-12** (state conditioning does not change sign/existence of the effect) and is to be **parked (P-009)** as a baseline re-description; the roll concession itself is absent in the published test. Do not re-specify around a weaker proxy.
- **G-13 timing table (draft)** for the eight active candidates:
  - IDEA-001: S&P announcement published after close, before effective close → passes.
  - IDEA-003: option-implied crash measures from the listed surface → real-time → passes.
  - IDEA-004: crowd depth from lagged institutional holdings → published with lag; G-04 still open; decision-time usability unverified.
  - IDEA-005: COT weekly, 3-day lag, before monthly roll → passes availability; fails G-12 (above).
  - IDEA-008: FINRA short interest published 7 business days after settlement; borrow fees have no public source (SEC Rule 10c-1a exempt until 2029) → lending-fee state fails G-13 unless vendor data; must be re-scored or parked.
  - IDEA-009: venue funding rate published real-time by the venue → passes.
  - IDEA-010: adoption calendars published in advance → passes.
  - IDEA-011: adoption calendars published in advance → passes.
- **Remaining Cycle 6 work:** G-12 for IDEA-001, IDEA-003, IDEA-004, IDEA-008, IDEA-009, IDEA-010, IDEA-011; frontier screen of the five families in section 3; T5–T8; re-rank; V-010+ for any new top-three; log rejections/parkings; rewrite handoff.

## 5. Operating rules for the next session

1. Read this file first, then register, shortlist, source ledger, rejected/parked.
2. Theory only, absolutely. No backtests, data acquisition, code, metrics, workflow/test/infra
   edits, trading.
3. Do not modify the canonical prompt.
4. Preserve prior work; add, do not delete or renumber. New IDs: **IDEA-014+, S-126+, V-010+,
   G-14+, R-011+, P-009+**; call next cycle **Cycle 6**.
5. Never invent a citation; re-derive every identifier; treat agent-supplied bibliographies as
   unverified. Record how each source was verified, and distinguish **index-rendered** verification
   (text returned by a search index) from a directly fetched document.
6. Locate contradicting evidence deliberately — and when a published result is found that tests the
   candidate's own effect, **reject rather than narrow** (the rule that closed IDEA-006, IDEA-007
   and IDEA-012).
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
environment only: no backtests, no data acquisition, no strategy code, no
trading.

1. Read the durable handoff at research/next_agent_handoff.md first, then
   research/idea_register.md, research/ranked_shortlist.md,
   research/source_ledger.md and research/rejected_and_parked.md. Do not
   regenerate what already exists and do not renumber or delete existing IDs.

2. Execute the best next research task in section 4 of the handoff, in this
   order.
    (a) PRIMARY (partly done in Cycle 6 first pass): IDEA-005 is settled — it fails G-12
        and is parked (P-009); apply G-13 and G-12 to the remaining seven active candidates
        (IDEA-001, IDEA-003, IDEA-004, IDEA-008, IDEA-009, IDEA-010, IDEA-011). IDEA-008's
        lending-fee state already fails G-13 on public data (borrow fees not public until 2029)
        and must be re-scored or parked.
   (b) SECONDARY: screen the five mechanism families in section 3 of the
       handoff against the published literature, one search each, recording
       every verdict in the source ledger - including the negative verdicts -
       and write a full dossier only for a family whose mechanism is unclaimed
       and whose state is published BEFORE the decision.
   (c) TERTIARY: attempt the bounded tasks T5-T8 and record any gap you cannot
       close as a new source gap with a precise question.
   Every dossier must name the participant, the binding constraint, a
   decision-time-observable state variable (with who publishes it, on what
   calendar, and when relative to the decision), a dated or state-dependent
   flow, the expected return source, an honest originality comparison,
   falsifiable predictions with explicit rejection conditions, confounders,
   data requirements, a theory/evidence status, and verified sources.

3. Apply the three-pass task-framing loop and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file.

4. Rank the candidates with the fixed rubric in
   research/ranked_shortlist.md (re-checking existing ranks), write validation
   hand-off specifications for any new top-three candidate (V-010 onward), and
   log anything rejected or parked. New IDs start at IDEA-014, S-126, V-010,
   G-14, R-011, P-009; call this cycle Cycle 6.

5. Absolute scope boundary: theory and discovery only. No backtests,
   simulations, parameter sweeps, significance tests, market data
   acquisition/processing, strategy code, executable research infrastructure,
   job/workflow/CI launches, workflow/test/credential/infrastructure changes,
   or trading. If a question can only be answered by running something,
   document it precisely and hand it off.

6. Cite every external claim with a verifiable URL or DOI and never invent a
   citation. Re-derive every identifier yourself; treat agent-supplied
   bibliographies as unverified. Record how each source was verified and say
   explicitly when a document could only be read through a search index.
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
| 4 | 2026-10-19 | IDEA-010/011/012 added; V-009 written; all twelve re-ranked (IDEA-011 at rank 3 tie, IDEA-010 at 6, IDEA-012 at 12); S-090…S-094 added; state-proxy note extended; G-10 residual open, G-11 open, G-06 narrowed but not closed; T5–T8 verdicts recorded. | Yes. |
| 5 (first half) | 2026-10-19 | G-10 closed against IDEA-007 (R-008); G-06 closed as a bounded negative finding (S-098, S-099); G-08 mostly closed, G-05 split; IDEA-013 added at 70.0; S-095…S-111 registered; G-12 opened. | Yes. |
| 5 (second half) | 2026-10-19 | G-11 closed against IDEA-006 (R-009) and IDEA-012 (R-010); IDEA-013's full-text check performed and IDEA-013 parked (P-008, 70→58); G-13 opened and condition (e) added to the state-proxy note; four frontier families screened and registered as baselines (S-122…S-125); register re-ranked to eight active candidates; V-005 and V-006 withdrawn; no new validation specification required. | Yes — this file. |
