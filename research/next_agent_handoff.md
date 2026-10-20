# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and `research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the superseded text is summarised into `research/cycle_notes.md`.

Last updated: 2026-10-20, **Cycle 6 complete** · The two standing screens (**G-13** publication-before-decision, **G-12** sign-or-existence) were applied to every active candidate and **parked two** (IDEA-005 as P-009, IDEA-008 as P-010) and re-scored one (IDEA-010, 68.0 → 65.0); the five frontier families were screened and produced **one new candidate, IDEA-014 RIN-DEADLINE (60.0)**; the register was re-ranked to **seven active candidates**; the top three are unchanged, so **no new validation specification was required**; **V-004 and V-007 are withdrawn** and **V-001 and V-002 amended**. Next: **Cycle 7**.

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | **14 dossiers (IDEA-001 … IDEA-014)** — 7 active candidates, 4 parked (IDEA-002 P-004, IDEA-005 P-009, IDEA-008 P-010, IDEA-013 P-008), 3 rejected (IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010; dossiers retained only so the reasoning is not re-derived) |
| Ranked shortlist | **7 ranked** (76 / 74 / 72 / 71 / 65 / 63 / 60) + 4 parked (63, 63, 60, 58) + 3 withdrawn (64, 59, 56) |
| Source ledger | **145 verified sources (S-001 … S-145)**, source gaps G-01 … G-16 |
| Validation hand-offs | **9 specifications (V-001 … V-009)**, of which **V-004, V-005, V-006 and V-007 are withdrawn** (their candidates are parked or rejected); **5 executable** (V-001, V-002, V-003, V-008, V-009) |
| Rejected / parked | **10 rejected (R-001 … R-010)**, 10 parked (P-001 … P-010), 34-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged** |
| Validation performed | **None.** No candidate has been tested. Every score is a research priority, not a probability of profit. |

Cycle 6 did the work the Cycle-5 handoff had been holding open. **The two standing general questions were turned into screens and run on every active candidate for the first time.** The result was not cosmetic: the screens **parked two candidates** and **re-scored a third**.

- **IDEA-005 ROLLCOND — parked (P-009) on G-12.** Its own formulation is an *existence* claim, which is what G-12 asks for, but the screen asks what the candidate *demonstrates*. The closest published test of its **own state variable** — the CFTC Index Traders' share of open interest, conditioned on commodity returns in roll periods — reports **no significant effect** (S-099); the trader-type literature conditions convergence *speed* rather than the nearby-to-deferred concession (S-098); the aggregate effect the joint state would rescue is documented as decayed after 2012 (S-033, S-037, S-036). It is parked rather than rejected because **nothing published shows the candidate's effect**; two unblocking conditions are recorded and both are required. Score 72.0 → 60.0.
- **IDEA-008 SECURITY-LEND — parked (P-010) on G-13, with a dated unblocking condition.** The failure is a calendar, not a judgement: the SEC's December 2025 order exempts Rule 10c-1a compliance "with respect to the reporting date until September 28, 2028, and with respect to the dissemination date until March 29, 2029" (S-126), so the earliest public availability of a borrow-cost state is **29 March 2029**; the short-interest fallback is twice-monthly and published roughly seven to eight business days after its settlement date (S-127). The register's Cycle-3 belief that "lending fees are published" was **wrong about the calendar**. Score 65.0 → 63.0; gap **G-14** records the dated condition.
- **IDEA-010 CREDIT-ETF — re-scored 68.0 → 65.0.** Its mechanism's core (AP inventory and balance-sheet constraints driving ETF–NAV dislocations) is published institutionally at S-123, so novelty falls 3 → 2; G-13 passes only partially because the differentiating state is commercial and the published substitutes are unvalidated — gap **G-16**.
- **IDEA-001, IDEA-003, IDEA-004, IDEA-009 and IDEA-011 passed both screens with no score change**, but two passes were not costless. IDEA-001's G-12 pass holds **only on the existence limb** (the side asymmetry and the second leg); the flow-scaling limb conditions size only, and V-001 is amended. IDEA-004's G-13 pass **resolves** the question Cycle 5 left open: the 13F-based crowd state is published on EDGAR within 45 days of each quarter end, so a filing-anchored rule is decision-time feasible and the binding constraint is proxy *validity* (G-04), not timing — and V-002 is amended to re-anchor its rebalance grid to the filing cadence.

The **five frontier families** named by the Cycle-5 handoff were screened, one search round each, and **every verdict is registered, including the four negative ones**. Families 2 (sovereign issuance calendars, S-142 … S-144), 3 (fast-payment rails, S-140, S-141), 4 (sovereign bond index inclusion, S-137 … S-139) and 5 (physical-delivery calendars, S-145 alongside S-038, S-039) are **published baselines** and are now rows in the known-baseline table. **Family 1 produced the cycle's one new candidate: IDEA-014 RIN-DEADLINE (60.0)** — the US Renewable Fuel Standard, where the obligation's size is codified in advance (40 CFR 80.1405, S-128), the deadline is **published by regulation** (40 CFR 80.1451(f)(1)(iii), S-129), and the deadline has already been moved once by published rule (S-131). Its **sign is not asserted anywhere**; that is its first test (gap **G-15**), and the published market-quality evidence (S-133) runs against it on cost, which is why it enters at 60.0 and not higher.

**T5–T8 were revisited and none was closable.** T5: closing-auction **volume** statistics are published by the venues (S-100), so the aggregate participation question is answerable, but the per-security long history is commercial and the *attribution* question is not answerable from aggregate volume. T6: unchanged — no published continuous dealer FVA series exists, IDEA-002 stays parked. T7: the *data* leg is closed and only the *literature* leg remains open. T8: unchanged — no benchmark-specific aggregate passive-asset series exists. **No new task was added.**

## 2. Highest-priority unresolved theoretical questions

1. **G-15 — does any published work show a compliance-deadline price pattern in RINs, and what state decides its sign?** This is IDEA-014's first test and the cheapest way to find out whether the new candidate is a discovery or a re-description. It is the direct analogue of the check that killed IDEA-005 (S-099) and it has **not** been run. Until it is run, IDEA-014 rests on a *bounded negative* novelty check (one search round).
2. **G-16 — a validated public proxy for dealer balance-sheet stress in credit.** IDEA-010's precondition. The published substitutes (S-123 and the AP-inventory literature) are different constructs and have not been validated against a dealer-balance-sheet measure. **No validation specification may be written for IDEA-010 until this is done.**
3. **G-01 — a public funding-state proxy** (IDEA-002's feasibility kill condition; T6). The standing instance of the state-proxy problem. SOFR, standing-repo and primary-dealer data are public ingredients, but no published, continuous series of dealer funding value adjustments exists (S-041, S-042), and the published literature prices the constraint with proprietary dealer-level data (S-095, S-096).
4. **G-04 — the crowd-depth proxy** for IDEA-004, whose left tail is a broken anchor. Cycle 6 established that the *publication* is timely on the filing cadence; the *validity* is not established, and it is now the sole binding constraint on the register's rank-2 candidate.
5. **G-02 / G-07 — a benchmark-specific passive-asset series** (IDEA-001's data gap; T8). Individual ETF assets are public; no aggregate benchmark-specific series for all S&P 500 trackers exists, and ICI's series (S-040) is category-level only.
6. **G-03 — the trading convention behind the effective close**, and the closing-auction **attribution** question (T5). Aggregate auction volume is published (S-100); per-security history is commercial; how much of the auction is passive is not answerable from aggregate volume at all.
7. **G-05 — the single-name 0DTE literature.** The *data* question is closed (the series is constructible from public OCC data, S-100); the *literature* question is open.
8. **G-14 — a public borrow-cost series.** **Dated: not before 29 March 2029** (S-126). Do not spend effort on it before then; IDEA-008 stays parked as P-010 until then.
9. **A sharper G-12.** In Cycle 6 most G-12 passes were satisfied *by argument* on the "existence limb" rather than by published evidence. The register now needs a standing answer to: **is the differentiation a hypothesis, or a published result?** A candidate that argues its own existence from theory while a published result already shows the aggregate effect is a baseline re-description. This is the question that closed IDEA-005, and it should be asked explicitly of every new candidate, not argued.
10. **IDEA-013's dated unblocking condition.** No effort before 2029: the next TNAC (emissions year 2026) is expected in late May or June 2027, the corresponding surrender deadline is 30 September 2027, and the candidate cannot be validated in decision-time form before the aggregate balance has crossed a sign change with an observation on each side (P-008).

## 3. Next mechanism families to investigate (not yet in the register)

**Closed by Cycle 5 — do not re-derive:** settlement and payment infrastructure as a price determinant (S-112, S-082, S-071; the window is a cost: S-117 … S-120); securities settlement cycle length as a price-impact determinant (S-113, S-114, S-115); exchange-published margin schedules (S-122); ETF primary-market arbitrage and AP inventory (S-123); crypto spot-ETF flow (S-124, S-125); benchmark-window alteration (S-047, S-080).

**Closed by Cycle 6 — do not re-derive:** sovereign bond index inclusion/exclusion (S-137 … S-139); sovereign issuance calendars / the Treasury quarterly refunding (S-142 … S-144); fast-payment rails and the liquidity-demand channel (S-140, S-141); physical-delivery calendars in commodity futures (S-145, S-038, S-039); the EU ETS surrender-month premium as the *baseline instance* of the compliance-deadline template (S-101); RIN price formation and pass-through as the *market object* for IDEA-014 (S-134, S-135) and its market quality (S-133).

**Still open — screen first, dossier only if unclaimed *and* the state is published before the decision:**

1. **Rule 10b5-1 trading-plan cooling-off periods and expiry.** The SEC's 2023 adopting release sets cooling-off periods (30/90/120 days for directors, officers and issuers) and an expiry cap (2 trading days for issuer plans, 10 trading days otherwise). The calendar is published by regulation, the state is public (Form 4 within two business days), and the flow is date-bound and largely price-insensitive. Screen against the *insider-trading* and *10b5-1* literature before writing. Note the connection to IDEA-001: the announcement-window leg's exposure to insider news is a natural cross-check.
2. **Statutory date-bound obligations in other jurisdictions and sectors** — the family that produced IDEA-014, widened: the **EU ETS maritime phase-in** (a shipping obligor population with a published phase-in schedule), the **UK ETS** (a different regulator), and **US state-level cap-and-trade** (RGGI and California: a state regulator, a public allowance bank, a published surrender deadline). Screen each as a separate instance of the template: different regulator, different obligor population, and a state that decides the sign.
3. **Listing-rule compliance deadlines** (Nasdaq's 180-day bid-price deficiency period, Form 25 / removal-of-listing dates). A date-bound obligation on the issuer with a public calendar and a public state.
4. **Index and benchmark flows in newer asset classes** — private-credit and direct-lending benchmark transitions, where administrators publish review calendars and tracking estimates but the ecosystem is young. The equity instance is IDEA-001's territory and the sovereign instance is published (S-137, S-138); the *private-credit* instance is not covered by either.
5. **A "published state decides the sign" template in a market where the obligation's size is itself a published function.** The register's most general template: a price-insensitive, date-bound obligation whose *direction* is decided by a quantity the regulator publishes in advance. Screen for further instances across commodity-credit, emissions and energy-efficiency-programme regimes (e.g. state energy-efficiency obligations, federal fuel-efficiency standards, agricultural conservation-programme deadlines).

## 4. Best next research task (Cycle 7)

**Primary — close G-15, because IDEA-014 is the newest and least-verified candidate in the register and its sign is entirely unasserted.** Run a bounded literature round on the question: *does any published work identify a price pattern, seasonal effect, or flow signature in the US RIN market around the RFS compliance-reporting deadline, and does any published work identify the state (obligation size, aggregate position, net compliance) that would decide its sign?* Record the verdict in the source ledger **even if negative** — a bounded negative on G-15 is a result, because it converts IDEA-014's novelty from "unsearched" to "searched once and not found", which is the difference between a candidate and a guess. Concretely: (a) search the peer-reviewed RIN literature (S-134, S-135 already locate part of it) and the futures-market literature on credit vintages; (b) check whether the *deadline* rather than the *vintage* is ever the conditioning variable; (c) check what EPA publishes about compliance positions and their timing (the state's own publication calendar is the binding constraint, and 40 CFR 80.1451(f) is the place to start); (d) record the cost floor and the squeeze precedent (the 2013 RIN episode) as pre-conditions on the dossier. Then **re-score, re-rank, or park IDEA-014 on what the search returns.**

**Secondary — screen the new frontier families in section 3** against the published literature *first* (one search each, recording the verdict in the source ledger even when the verdict is "published — baseline"), and write a full dossier only for a family whose mechanism is unclaimed **and** whose state is published **before** the decision, and **and** whose sign is decided by a published state. Run G-13 and G-12 as screens on every new candidate *before* it is ranked, and record both verdicts per candidate in the dossier.

**Tertiary — the bounded supporting tasks.** T5 (G-03/G-08 closing-auction concentration and attribution), T6 (G-01 composite funding spec), T7 (G-05 single-name 0DTE literature), T8 (G-07 benchmark-specific passive-asset series), plus **G-04** (IDEA-004's crowd-depth proxy) and **G-16** (IDEA-010's proxy validation) — the two gaps that now bind the register's rank-2 and rank-5 candidates. Record any gap that cannot be closed as a new source gap with a precise question.

**Then** re-rank everything under the fixed rubric, write a validation specification for any new top-three candidate (V-010 onward), log rejections and parkings, and rewrite this handoff.

**Do not** spend effort on IDEA-008 before 29 March 2029 or on IDEA-013 before 2029, and do not re-open G-06, G-10 or G-11 without a new mechanism.

## 5. Operating rules for the next session

1. Read this file first, then register, shortlist, source ledger, rejected/parked.
2. Theory only, absolutely. No backtests, data acquisition, code, metrics, workflow/test/infra
   edits, trading.
3. Do not modify the canonical prompt.
4. Preserve prior work; add, do not delete or renumber. New IDs: **IDEA-015+, S-146+, V-010+,
   G-17+, R-011+, P-011+**; call next cycle **Cycle 7**.
5. Never invent a citation; re-derive every identifier; treat agent-supplied bibliographies as
   unverified. Record how each source was verified, and distinguish **index-rendered** verification
   (text returned by a search index) from a directly fetched document.
6. Locate contradicting evidence deliberately — and when a published result is found that tests the
   candidate's own effect, **reject rather than narrow** (the rule that closed IDEA-006, IDEA-007
   and IDEA-012). The Cycle-6 refinement: when the closest published test of the candidate's **own
   state variable** is null, the candidate is **parked** with unblocking conditions, not rejected
   (P-009), and when a state's publication calendar is dated in the future, it is parked with the
   date (P-010).
7. **Run G-13 and G-12 as screens on every candidate before ranking it**, and record both verdicts
   in the candidate's dossier, in the ranked shortlist and in the source ledger's verdict block. A
   candidate that fails either screen is re-scored or parked; it is not left in the active ranking
   with the failure noted.
8. Scores are research priority, not success probability.
9. Update this handoff last; keep the initial task message current and self-contained.

## 6. Environment observations

Carried forward unchanged: `.github/workflows/main.yml` references missing
`scripts/controller_progress.py` and test modules; run diagnostics report failure despite durable
commits. Maintainer item; not acted on.

Cycle-6 tooling note for the next session: the general web-search provider **rate-limited** partway
through Cycle 6. The remainder of the work was done through the **Crossref API**, the **Federal
Register API**, the **eCFR renderer API** and direct page fetches, which are not rate-limited in the
same way, and these are the routes to prefer. One document could not be parsed locally and was
therefore **not registered** (the Fed's FOMC memorandum on the refunding statement — no
text-extraction tooling was available for its font encoding); the family-2 verdict rests on the two
published preprints instead.

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
    (a) PRIMARY: close G-15 for IDEA-014 RIN-DEADLINE. Run a bounded
        literature round asking whether any published work identifies a price
        pattern or flow signature in the US RIN market around the RFS
        compliance-reporting deadline, and whether any published work
        identifies the state that would decide its sign (obligation size,
        aggregate compliance position, net position). Record the verdict in
        the source ledger even if the verdict is negative - a bounded negative
        on G-15 is a result. Then re-score, re-rank or park IDEA-014 on what
        the search returns.
    (b) SECONDARY: screen the five new mechanism families in section 3 of the
        handoff against the published literature, one search each, recording
        every verdict in the source ledger - including the negative verdicts -
        and write a full dossier only for a family whose mechanism is unclaimed,
        whose state is published BEFORE the decision, and whose sign is decided
        by a published state.
    (c) TERTIARY: attempt the bounded tasks T5-T8 plus G-04 (IDEA-004's
        crowd-depth proxy) and G-16 (IDEA-010's proxy validation), and record
        any gap you cannot close as a new source gap with a precise question.
    Every dossier must name the participant, the binding constraint, a
    decision-time-observable state variable (with who publishes it, on what
    calendar, and when relative to the decision), a dated or state-dependent
    flow, the expected return source, an honest originality comparison,
    falsifiable predictions with explicit rejection conditions, confounders,
    data requirements, a theory/evidence status, and verified sources.

3. Run G-13 (is the state published BEFORE the decision, per observation?) and
   G-12 (does the conditioning change the SIGN or the EXISTENCE of the effect,
   not merely its size?) as screens on every candidate before it is ranked.
   Record both verdicts in the candidate's dossier, in the ranked shortlist and
   in the source ledger's verdict block. A candidate that fails either screen is
   re-scored or parked; it is not left in the active ranking with the failure
   noted. A failed G-13 with a dated future publication calendar is a parking
   with a date; a G-12 failure where the closest published test of the
   candidate's own state variable is null is a parking, not a rejection. A
   rejection still requires a published result that SHOWS the effect.

4. Apply the three-pass task-framing loop and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file.

5. Rank the candidates with the fixed rubric in
   research/ranked_shortlist.md (re-checking existing ranks), write validation
   hand-off specifications for any new top-three candidate (V-010 onward), and
   log anything rejected or parked. New IDs start at IDEA-015, S-146, V-010,
   G-17, R-011, P-011; call this cycle Cycle 7.

6. Absolute scope boundary: theory and discovery only. No backtests,
   simulations, parameter sweeps, significance tests, market data
   acquisition/processing, strategy code, executable research infrastructure,
   job/workflow/CI launches, workflow/test/credential/infrastructure changes,
   or trading. If a question can only be answered by running something,
   document it precisely and hand it off.

7. Cite every external claim with a verifiable URL or DOI and never invent a
   citation. Re-derive every identifier yourself; treat agent-supplied
   bibliographies as unverified. Record how each source was verified and say
   explicitly when a document could only be read through a search index.
   Scores are research-priority weights, not probabilities of profit.

8. Finish by rewriting research/next_agent_handoff.md: current pipeline
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
| 5 (second half) | 2026-10-19 | G-11 closed against IDEA-006 and IDEA-012 (R-009, R-010); IDEA-013's full-text check performed and IDEA-013 parked (P-008, 70→58); G-13 opened and condition (e) added to the state-proxy note; four frontier families screened and registered as baselines (S-122…S-125); register re-ranked to eight active candidates; V-005 and V-006 withdrawn; no new validation specification required. | Yes. |
| 6 | 2026-10-20 | G-13 and G-12 applied as screens to every active candidate: IDEA-005 parked (P-009, 72→60) on G-12, IDEA-008 parked (P-010, 65→63) on G-13 with a dated 2029 unblocking condition (G-14), IDEA-010 re-scored (68→65) with G-16 opened, five candidates confirmed (IDEA-001 on the existence limb only). Five frontier families screened with all four negative verdicts registered as baselines (S-137…S-144); family 1 produced **IDEA-014 RIN-DEADLINE (60.0)** with G-15 opened. T5–T8 revisited, none closable, no new task. Register re-ranked to seven active candidates; top three unchanged so no new validation specification; V-004 and V-007 withdrawn, V-001 and V-002 amended; S-126…S-145 and G-14…G-16 registered. | Yes — this file. |
