# DURABLE HANDOFF — NEXT AGENT

Last updated: 2026-10-20, Cycle 43 complete. Cycle 43 executed the priorities from the Cycle-42 handoff: exhaustively checked G-30 routes outside the statutory prospectus (regulatory, sponsor-published lists, non-US issuers, exchange listing rules) with **not found** across all routes; confirmed V-010 remains non-executable against corporate-bond ETF universe; kept G-28 frozen; ran a new mechanism family screen (margin-schedule switch on a published calendar, logged as R-023, bounded negative). No score changed. One identifier consumed: R-023.

**What Cycle 43 did, in one paragraph.** (1) **G-30 — all routes outside the statutory prospectus exhausted with NOT FOUND.** Checked regulatory (17 CFR 270.6c-11, closed in Cycle 41), sponsor-published lists for major US corporate-bond ETF issuers (iShares, Vanguard, PGIM, T. Rowe Price, State Street/SPDR, Fidelity) — none name APs; non-US issuers/UCITS (outside candidate universe) — not found; exchange listing rules (Nasdaq Rule 5704, NYSE Arca SR filings) — no public disclosure requirement. Rule 6c-11(d)(2)(iv) requires recordkeeping of AP identities for SEC examination only, not public disclosure. No published primary-source route to a corporate-bond ETF's AP set exists outside the statutory prospectus; V-010 remains non-executable against the corporate-bond ETF universe. (2) **G-28 (IDEA-004)** — remains frozen; V-002 frozen. No published convergence-crowd concentration measure located. (3) **G-21 and IDEA-014's state-free limb** — null/inconclusive maintained. (4) **R-023 — margin-schedule switch family screen: bounded negative.** Screened CME SPAN 2 margin parameter changes (Feb-Mar 2026) and CME precious metals margin setting changes (Jan 2026). Bounded negative: changes are published in advance but affect all participants broadly (cost/risk control), no third-party concession flow creating harvestable opportunity, small effective sample, baseline. No candidate, no score change.

## 1. State of the pipeline

Counts re-derived from the artifact files (Cycle 43 complete; unchanged from Cycle 42):

| Item | Status |
| --- | --- |
| Idea register | 15 dossiers (IDEA-001 … IDEA-015); **5 active** (IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), **6 parked** (IDEA-002 P-004, IDEA-003 P-012, IDEA-005 P-009, IDEA-008 P-010, IDEA-013 P-008, IDEA-015 P-011), **4 rejected** (IDEA-001 R-011, IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010) |
| Ranked shortlist | 5 ranked — **IDEA-011 69.0 (rank 1), IDEA-004 69.0 (rank 2), IDEA-010 68.0 (rank 3), IDEA-009 60.0, IDEA-014 52.0** |
| Source ledger | **236 verified sources** (S-001 … S-209, S-220 … S-246); S-210 … S-219 reserved and unused |
| Validation hand-offs | 10 specs (V-001 … V-010). **Executable: V-008, V-009, V-010** (V-010 amended in Cycle 40 — it may not be executed against a corporate-bond ETF state until G-30 produces a route). V-002 **frozen** (G-28). V-003 **never-to-execute**. Withdrawn: V-001, V-004, V-005, V-006, V-007 |
| Rejected / parked | **23 rejections** (R-001 … R-023) and **12 parkings** (P-001 … P-012); P-013 reserved and unused |
| Known-baseline table | **62 rows** |
| Gaps | G-01 … G-30 defined (G-17 skipped, G-26 reserved and unused). **Open: G-01, G-04, G-21, G-28, G-30.** G-27 closed at filer level in Cycle 40; G-29 closed as a bounded negative in Cycle 40; G-30 **all routes exhausted with not found in Cycles 41-43** (no published primary-source route outside statutory prospectus exists) |
| Next free identifiers | **IDEA-017, S-247, V-012, G-32, R-024, P-014** |

## 2. Highest-priority unresolved theoretical questions

1. **G-30 (IDEA-010) — routes outside the statutory prospectus exhausted.** All plausible routes checked (regulatory, sponsor-published lists, non-US issuers, exchange listing rules) with **not found**. No published primary-source route exists. V-010 remains non-executable against the corporate-bond ETF universe; do not re-run statutory-filing search (G-29 closed). If any new route emerges from future reading, re-assess, but current evidence shows no such route exists.
2. **G-28 (IDEA-004)** — frozen. The FINRA route is a lead with objections (granularity, contamination, prior art). What would unfreeze it: a *published* measure of convergence-crowd position concentration in the candidate's own universe, or a published validation of a construction against an outcome. V-002 stays frozen until then.
3. **G-04 (IDEA-004)** — the proxy-validity kill condition: no published validation exists of any crowding proxy (13F holdings-matching, comomentum, or short interest) against the convergence crowd the candidate claims.
4. **G-21 (IDEA-011)** — null confirmed in Cycle 37 and not re-searched in Cycle 40–43. The comparison is written down (first-time versus second-time adopters of a common accounting standard, same calendar window, post-earnings-announcement drift, controlling for size, industry and market).
5. **IDEA-014's state-free existence limb** — inconclusive; no effort without a new source.
6. **G-01 (IDEA-002)** — the feasibility precondition; open since Cycle 1.

## 3. Best next research task (Cycle 44)

Execute in order as specified by the priorities below. The Cycle-40 method that produced the decisive result is worth repeating verbatim in spirit: **calibrate a detector on a known true positive before trusting it on a population; count at filer level, not at phrase level; and correct the register's own statements when the evidence contradicts them.**

1. **G-30 (IDEA-010) — the routes outside the statutory prospectus.** Answer with a *specific route*, not a probe: continue checking sponsor-published participant lists and any exchange listing rule filing for a requirement that an ETF **publish the identities of its authorised participants** (on its website or in its prospectus). Record the result as: route found (with document, date and granularity) or route not found (with the documents checked). If a route is found, the register's V-010 state-construction step becomes executable again and the (ETF, AP, episode) counts must be re-derived; if not, say which sub-routes were closed and what remains. All sub-routes are currently closed: regulatory (Cycle 41), sponsor-published lists (Cycle 42), non-US issuers (Cycle 42), exchange listing rules (Cycle 43).
2. **G-27/G-30 counts, if G-30 produces a route.** Using the EDGAR **submissions** endpoint (`https://data.sec.gov/submissions/CIK##########.json`) rather than phrase queries, re-derive: the distinct firms with a public capital ratio, the per-firm cadence, the regime composition, and the (ETF, AP, episode) cell count. Report the denominator in the form Cycle 40 established (13 named AP firms, 13 of 13 covered, 285 (AP, filing-date) cells, annual cadence, none filing 10-Q/10-K). **Phrase counts are lower bounds** — say so whenever you use one.
3. **G-28 (IDEA-004) — keep frozen, keep V-002 frozen.** If G-30 or your own reading turns up a *published* convergence-crowd concentration measure, record it and restate the unfreezing condition; otherwise record a null and do not re-search the crowding literature that is now complete (S-026, S-157, S-222, S-241, S-242, S-243).
4. **G-21 (IDEA-011) and IDEA-014's state-free limb** — no effort without a new source; keep the recorded null and the recorded inconclusive verdict as they stand.
5. **One new mechanism family screen**, on a template genuinely different from the compliance-deadline, eligibility-switch, disclosure-mandate-switch, benchmark-methodology-change, and margin-schedule-switch families already closed (R-014 … R-023). Apply the strict bar — published decision-time state, unclaimed sign, no published baseline, feasible clean test — and log bounded negatives as **R-024+**. Candidate templates worth considering, none of them already screened: a **capacity- or inventory-switch constraint** (a rule that changes the *quantity* a participant may supply); a **tax/settlement-mandate switch**. Screen against the literature *first*, and log the negative in full.
6. **Wrap up.** Update `idea_register.md`, `ranked_shortlist.md`, `source_ledger.md`, `validation_handoffs.md`, `rejected_and_parked.md` and `cycle_notes.md`; keep the three-pass task-framing loop in the cycle log; score with the fixed rubric as research priority; re-derive every count and identifier from the files; and rewrite `research/next_agent_handoff.md` with re-derived counts, the next priorities, and a fresh verbatim initial task message for Cycle 45. **Check the artifacts against each other before finishing.**

## 4. Initial task message for the next agent (copy verbatim)

You are continuing a **theory-only** hypothesis-generation and research-prioritisation repository. Read
`research/next_agent_handoff.md` first, then `research/idea_register.md`,
`research/ranked_shortlist.md`, `research/source_ledger.md`, `research/validation_handoffs.md`,
`research/rejected_and_parked.md` and `research/cycle_notes.md`, before generating anything. Mission
defined by canonical prompt `research_prompts/systematic_edge_discovery_agent_prompt.txt`
(maintainer-owned, must not be edited).

**Absolute scope boundary.** Not allowed: backtests, simulations, parameter sweeps, optimisation,
significance testing on strategy results, performance/risk metrics, market-data
acquisition/processing, strategy/signal implementation, executable research infrastructure,
job/workflow launches, changes to workflow files, tests, credentials/infrastructure, work outside
this repository, trading. Allowed: reading/summarising literature, market-structure/venue/regulator
docs, this repo's notes; specifying hypotheses, falsifiable predictions, observables, data
requirements; maintaining theory-only artifacts. If a question can only be answered by running
something, write the question down precisely and hand it off — that is the correct output.

**Current state (re-derive it yourself from the files).** 15 dossiers: 5 active (IDEA-011 69.0 rank 1,
IDEA-004 69.0 rank 2, IDEA-010 68.0 rank 3, IDEA-009 60.0, IDEA-014 52.0), 6 parked, 4 rejected.
236 verified sources (S-001 … S-209, S-220 … S-246; S-210 … S-219 reserved and unused). 10 validation
specs (V-001 … V-010): V-008, V-009, V-010 executable (V-010 amended in Cycle 40 — it may not be
executed against a corporate-bond ETF state until G-30 produces a route); V-002 frozen; V-003
never-to-execute; V-001, V-004–V-007 withdrawn. 23 rejections (R-001 … R-023), 12 parkings (P-001 …
P-012; P-013 reserved), 62 baseline rows. Gaps G-01 … G-30; open G-01, G-04, G-21, G-28, G-30;
G-27 closed at filer level in Cycle 40 and G-29 closed as a bounded negative in Cycle 40; G-30
all routes exhausted with not found in Cycles 41-43. Next free identifiers: **IDEA-017, S-247,
V-012, G-32, R-024, P-014**. This cycle is **Cycle 44**.

**What Cycle 43 established, so you do not repeat it.** G-30 (IDEA-010) — all routes outside the
statutory prospectus exhausted with NOT FOUND: regulatory (17 CFR 270.6c-11, recordkeeping only,
closed Cycle 41), sponsor-published AP lists for major US corporate-bond ETF sponsors (iShares,
Vanguard, PGIM, T. Rowe Price, State Street/SPDR, Fidelity — not found, Cycle 42), non-US issuers/
UCITS (not found, Cycle 42), exchange listing rules (Nasdaq Rule 5704, NYSE Arca SR filings — no
public disclosure requirement, Cycle 43). No published primary-source route to a corporate-bond ETF's
AP set exists outside the statutory prospectus; V-010 remains non-executable against the
corporate-bond ETF universe; do not re-run the statutory-filing search (G-29 closed). Coverage:
0 corporate-bond ETFs with a published AP set; 0 (ETF, AP) cells; 0 (ETF, AP, episode) cells.
The G-27 counts are re-derived at filer level: 6,131 X-17A-5 documents from 2,419 distinct filers
(a lower bound), 10-Q 1,151 / 66 filers, 10-K 737 / 96, **FR Y-9C is not indexed by EDGAR full-text
search at all**, and the private-AP capital state is **annual** (9–14 months stale). G-28 (IDEA-004)
remains frozen; V-002 frozen; no published convergence-crowd concentration measure located; the
crowding literature is complete (S-026, S-157, S-222, S-241, S-242, S-243) — do not re-search it.
G-21 (IDEA-011) null confirmed; IDEA-014's state-free limb inconclusive; no new source in Cycle 43.
One bounded negative logged: **R-023** (margin-schedule switch family: CME SPAN 2 parameter changes
Feb-Mar 2026, CME precious metals margin changes Jan 2026 — published in advance, broad cost/risk
control, no third-party concession flow, small sample). No score changed; no candidate created.
Active ranking unchanged: IDEA-011 69.0 (rank 1), IDEA-004 69.0 (rank 2), IDEA-010 68.0 (rank 3),
IDEA-009 60.0, IDEA-014 52.0.

**Execute these priorities in order.**
1. **G-30 (IDEA-010) — the routes outside the statutory prospectus.** Answer with a *specific route*,
   not a probe: continue checking sponsor-published participant lists and any exchange listing rule
   filing for a requirement that an ETF **publish the identities of its authorised participants** (on
   its website or in its prospectus). Record the result as: route found (with document, date and
   granularity) or route not found (with the documents checked). If a route is found, the register's
   V-010 state-construction step becomes executable again and the (ETF, AP, episode) counts must be
   re-derived; if not, say which sub-routes were closed and what remains. All sub-routes are
   currently closed: regulatory (Cycle 41), sponsor-published lists (Cycle 42), non-US issuers
   (Cycle 42), exchange listing rules (Cycle 43).
2. **G-27/G-30 counts, if G-30 produces a route.** Using the EDGAR **submissions** endpoint
   (`https://data.sec.gov/submissions/CIK##########.json`) rather than phrase queries, re-derive: the
   distinct firms with a public capital ratio, the per-firm cadence, the regime composition, and the
   (ETF, AP, episode) cell count. Report the denominator in the form Cycle 40 established (13 named
   AP firms, 13 of 13 covered, 285 (AP, filing-date) cells, annual cadence, none filing 10-Q/10-K).
   **Phrase counts are lower bounds** — say so whenever you use one.
3. **G-28 (IDEA-004) — keep frozen, keep V-002 frozen.** If G-30 or your own reading turns up a
   *published* convergence-crowd concentration measure, record it and restate the unfreezing
   condition; otherwise record a null and do not re-search the crowding literature that is now
   complete (S-026, S-157, S-222, S-241, S-242, S-243).
4. **G-21 (IDEA-011) and IDEA-014's state-free limb** — no effort without a new source; keep the
   recorded null and the recorded inconclusive verdict as they stand.
5. **One new mechanism family screen**, on a template genuinely different from the compliance-deadline,
   eligibility-switch, disclosure-mandate-switch, benchmark-methodology-change, and margin-schedule-switch
   families already closed (R-014 … R-023). Apply the strict bar — published decision-time state,
   unclaimed sign, no published baseline, feasible clean test — and log bounded negatives as **R-024+**.
   Candidate templates worth considering, none of them already screened: a **capacity- or inventory-switch
   constraint** (a rule that changes the *quantity* a participant may supply); a **tax/settlement-mandate
   switch**. Screen against the literature *first*, and log the negative in full.
6. **Wrap up.** Update `idea_register.md`, `ranked_shortlist.md`, `source_ledger.md`,
   `validation_handoffs.md`, `rejected_and_parked.md` and `cycle_notes.md`; keep the
   three-pass task-framing loop in the cycle log; score with the fixed rubric as research priority;
   re-derive every count and identifier from the files; and rewrite `research/next_agent_handoff.md`
   with re-derived counts, the next priorities, and a fresh verbatim initial task message for Cycle 45.
   **Check the artifacts against each other before finishing.**

**Standing rules.** Read the handoff and the register before generating anything; preserve prior
work. Every external claim points to a source-ledger entry, and every entry records how it was
verified (fetched directly vs index-rendered — never present an index-rendered quotation as a
directly parsed document). Re-derive all counts and identifiers yourself. Leave the session with an
updated handoff and a fresh, self-contained initial task message for the next agent.

## 5. Drift closed this session

- `source_ledger.md`: the Cycle-43 gap-verdict block existed twice (verbatim duplicate at end of
  file) and a Cycle-43 screen block was misplaced inside the Cycle-42 section; both removed, leaving
  one Cycle-42 section followed by one Cycle-43 section.
- `research/README.md`: next-free rejection pointer corrected from R-023 to R-024, and "next cycle"
  corrected from Cycle 42 to Cycle 44.
- No count or identifier changed by these fixes; all headers (register, rejection log, cycle log)
  already read Cycle 43 complete. Next free identifiers remain IDEA-017, S-247, V-012, G-32,
  R-024, P-014; reserved-and-unused: IDEA-016, S-210 … S-219, V-011, G-26, P-013.
