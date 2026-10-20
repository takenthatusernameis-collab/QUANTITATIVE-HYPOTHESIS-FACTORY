# DURABLE HANDOFF — NEXT AGENT

Last updated: 2026-10-20, **Cycle 37**. Cycle 37 executed the five Cycle-37 priorities and, in doing so,
**corrected a false negative**: Cycle 36 had recorded that broker-dealer firm-level regulatory capital is
not publicly available, and that claim was **false**. Form X-17A-5 is a **public** EDGAR form type and the
net-capital figures of broker-dealers — including private, non-listed authorised participants — are in
publicly indexed filings (S-231: 6,131 public X-17A-5 documents match "excess net capital"). **G-27 is
closed in IDEA-010's favour** on state availability, with per-firm cadence, document-level format and
cross-regime comparability registered as part of the verdict; **G-29 is opened** for the ETF → authorised-
participant mapping and the coverage count that now bounds the effective sample. G-28 was confirmed open and
sharpened; G-21 was confirmed null and its comparison written down; IDEA-014's state-free existence limb was
confirmed inconclusive. Two family screens were logged as bounded negatives: **R-017** (the Cycle-36
ex-dividend screen, written for real — it had been recorded in prose only) and **R-018** (the Rule 201
short-sale price-test circuit breaker, a genuinely different template whose effect is published and
peer-reviewed). **No score changed; no candidate was created; no validation specification was added.**

## 1. State of the pipeline

Counts re-derived from the artifact files in this cycle (not carried forward):

| Item | Status |
| --- | --- |
| Idea register | 15 dossiers (IDEA-001 … IDEA-015); **5 active** (IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014), **6 parked** (IDEA-002 P-004, IDEA-003 P-012, IDEA-005 P-009, IDEA-008 P-010, IDEA-013 P-008, IDEA-015 P-011), **4 rejected** (IDEA-001 R-011, IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010) |
| Ranked shortlist | 5 ranked — **IDEA-011 69.0 (rank 1), IDEA-004 69.0 (rank 2), IDEA-010 68.0 (rank 3), IDEA-009 60.0, IDEA-014 52.0**; tie at 69.0 broken in IDEA-011's favour on falsifiability (4 vs 3) |
| Source ledger | **228 verified sources** (S-001 … S-209, S-220 … S-238); S-210 … S-219 reserved and unused |
| Validation hand-offs | 10 specs (V-001 … V-010). **Executable: V-008, V-009, V-010.** V-002 **frozen** (G-28). V-003 **never-to-execute**. Withdrawn: V-001, V-004, V-005, V-006, V-007. V-010 amended in Cycle 37 |
| Rejected / parked | **18 rejections** (R-001 … R-018) and **12 parkings** (P-001 … P-012); P-013 reserved and unused |
| Known-baseline table | **59 rows** (ex-dividend date mechanics and the Rule 201 circuit breaker added in Cycle 37) |
| Gaps | G-01 … G-29 defined (G-17 skipped, G-26 reserved and unused). **Open: G-04, G-21, G-28, G-29, G-01.** G-27 closed in IDEA-010's favour in Cycle 37 |
| Next free identifiers | **IDEA-017, S-239, V-012, G-30, R-019, P-014** |

## 2. Highest-priority unresolved theoretical questions

1. **G-29 (IDEA-010) — which firms arbitrage which ETF, and how many cells can be counted?** *This is
   now the register's most valuable open question, and it is a document-reading question, not a search
   question.* The candidate's identification is a cross-sectional contrast, so the capital state must be
   attached to an ETF through the identity of its authorised participants. Established in Cycle 37: some
   ETF statutory prospectures name their APs (trade-press lead, **not** a verified source — the
   prospectus itself was not read, and it is deliberately *not* in the ledger as one); the AP universe is
   named in the APs' own filings (Virtu's 10-K names Citadel, Susquehanna, Two Sigma, Jane Street, DRW,
   IMC, Optiver). **Not established: whether *corporate-bond* ETF prospectuses name their APs** — the
   summary prospectuses read in Cycle 37 disclose AP risk generically and do not name them — and the
   resulting (ETF, AP) cell count. If no bond ETF names its APs, IDEA-010 is **not specifiable — untested,
   not dead**, and the register must not re-specify around a published crowding proxy (S-026, S-157, S-222
   measure a *different* crowd).

2. **G-27 (IDEA-010) — the effective-sample and coverage count.** The state is now known to be public but
   it is **firm-dependent and document-level**: annual for most private broker-dealers (fiscal year end,
   filed Feb–Mar, so 40–90 days stale at any decision date), quarterly for listed broker-dealers (XBRL,
   S-233) and bank holding companies (FR Y-9C, S-226), and quarterly for at least one private filer
   (S-231 records a period ending 2024-09-30). FOCUS net capital is **not commensurable** with bank
   risk-based ratios, and asset-manager APs have no equivalent. The count of usable (ETF, AP, episode)
   cells is **not yet computed**.

3. **G-28 (IDEA-004) — which crowd is the state?** Still open, now with the route named and the reasons
   stated: a **Form 13F holdings-matching** construction (a manager disclosing long holdings in both legs
   of a pair is by construction running convergence capital) fails because it is a construction rather than
   a published measure; it captures only the visible long leg (13F reports longs only — no shorts, swaps
   or credit instruments); it cannot separate convergence capital from a coincident directional holder; and
   the register's already-established 45-day filing lag makes it a quarter-slow against a rule anchored to
   its own cadence. V-002 stays frozen. The unfreezing condition is written out in the Cycle-37 blocks of
   `idea_register.md` and `validation_handoffs.md`.

4. **G-21 (IDEA-011) — the first-adopter versus second-adopter drift comparison.** A second cycle has
   found no published study running it: a **null**, meaning untested rather than refuted. The comparison
   is now written down exactly (first-time adopters versus second-time adopters of an IFRS-equivalent
   standard; same calendar window; controlling for size, industry and market; abnormal return in a fixed
   post-earnings-announcement window), so it can be handed to a validator rather than re-searched.

5. **IDEA-014's state-free existence limb.** Bounded search inconclusive on whether the RFS compliance
   deadline moves prices at all. Retained, not resolved; no further effort justified without new sources.

6. **G-04 (IDEA-004) and G-01 (IDEA-002, parked).** G-04's validity limb is downstream of G-28. G-01's
   blocker (no public continuous dealer funding-value-adjustment series) is indefinite.

## 3. Best next research task (Cycle 38)

1. **Priority 1 — G-29 (IDEA-010): does a corporate-bond ETF's statutory prospectus name its authorised
   participants, and what is the coverage count?** This is the highest-value task available: it is a
   primary-document reading task with a decisive outcome, it gates the register's rank-3 candidate, and it
   is now *cheap* because the tooling works. Read the prospectus or SAI of the major US corporate-bond
   ETFs (iShares Core U.S. Aggregate Bond ETF, iShares Core 1–5 Year USD Bond ETF, and one fund from each
   of two other issuers). **Technique that works where direct `sec.gov/Archives` fetches are blocked**
   (they returned HTTP 403 in Cycle 37): the EDGAR full-text search JSON API —
   `https://efts.sec.gov/LATEST/search-index?q="authorized participants"&forms=497` — returns matching
   document metadata and highlights; `&ciks=` restricts to a filer, `&dateRange=custom&startdt=&enddt=`
   bounds the period, `&from=`/`size=` pages the hits. A phrase query for "authorized participants"
   restricted to a bond-ETF registrant settles the question without fetching a PDF. Then produce the
   **coverage count**: the number of corporate-bond ETFs whose AP set is reconstructable from a public
   filing, and the number of (ETF, AP) cells in which the AP also has a public capital ratio. Record
   "not specifiable — untested, not dead" if no bond ETF names its APs; do **not** substitute a proxy.

2. **Priority 2 — complete G-27/G-29 with the coverage and effective-sample counts.** Using the EDGAR
   API and the routes in the Cycle-37 amendment to V-010, count: distinct firms with publicly indexed
   X-17A-5 net capital; listed broker-dealers with XBRL-tagged quarterly net capital; bank APs with FR
   Y-9C; the number of corporate-bond ETFs with a reconstructable AP set; and the resulting (ETF, AP,
   episode) cells. **Trap to avoid:** the API's `entity_filter` aggregation returns only the top 30
   buckets per response, so a firm missing from that list is **not** evidence of absence — page with
   `from=`/`size=` or narrow by CIK. Report "untested — not dead" if the counts are too small; a
   small-sample null must not be upgraded into a kill.

3. **Priority 3 — G-28 (IDEA-004): keep the candidate frozen; test one specific new lead.** The 13F
   holdings-matching route is now documented as insufficient. The one *published* state that could attack
   two of the four objections (long-leg-only; coincidental holder) is **the short leg**: FINRA requires
   firms to report short interest twice a month and publishes it on a dated schedule (S-127, fetched
   directly), so a convergence trade's short leg is observable at a published, lagged cadence. Test whether
   a *pair-structure* mapping (short interest in the acquirer around the announcement date) can separate
   convergence capital from a directional bear. Record it as a **lead**, not a solution: it leaves the
   "construction, not a published measure" objection untouched, it is bi-monthly, and it covers equities
   only — so it can only address the equity part of the candidate's universe. **Do not write a candidate
   on it unless it meets the full register bar.**

4. **Priority 4 — IDEA-014's state-free existence limb.** Maintain the inconclusive status. No effort
   unless a new source appears.

5. **Priority 5 — one new mechanism family screen on a genuinely different template.** The
   compliance-deadline template is exhausted and Cycle 37's Rule-201 screen (R-018) is the template to
   beat: *a regulatory switch that disables a participant, triggered by a published, observable threshold
   with a published, bounded duration*. Three families the register has **not** screened, each a
   different template in kind:
   - **(A) Rate-limited price-insensitive demand.** Rule 10b-18's safe harbour caps an issuer's daily
     repurchase volume at 25 % of four-week ADTV, so a price-insensitive buyer's demand is *rate-limited*
     and deferred across days rather than converging on a date. The register's own **R-005** preserved
     this lead ("a dated, capacity-constrained rule whose bindingness is observable"). **Correction to
     carry forward: the cap is DAILY, not monthly** — do not build a monthly capacity clock. The state
     would be the issuer's remaining capacity, published only in the monthly repurchase table of the
     10-Q/10-K. There is **no 10b-18 source in the ledger yet**; add one (S-239 or later) with the rule
     text. Also note the buyback literature is dense and price-sensitive, so the bar is high.
   - **(B) Eligibility-switch families.** A regulator changing *who may hold* an asset, with a published
     compliance date and a published distance-to-limit state (for example CFTC speculative position limits
     with per-contract compliance dates and published weekly position data, or concentration/large-exposure
     limits). Template: a constrained party's forced repositioning on a published date.
   - **(C) Benchmark methodology changes.** An index provider publishing a methodology change with an
     effective date (rather than a membership change) forces passive repositioning on a published date.
     Different in kind from reconstitution, which is already a baseline.
   Apply the strict bar and log bounded negatives; a bounded negative is a legitimate outcome.

6. **Priority 6 — theory only; re-derive state each cycle.** No backtests, no data acquisition or
   processing, no strategy or signal implementation, no performance or risk metrics, no significance
   testing on strategy results, no workflow/test/infrastructure edits, no changes to the canonical
   prompt, no trading, no work outside this repository. Read `research/next_agent_handoff.md` first, then
   `research/idea_register.md`, `research/ranked_shortlist.md` and `research/source_ledger.md`. New IDs
   start at **IDEA-017, S-239, V-012, G-30, R-019, P-014**; call this **Cycle 38**. Re-derive every count
   from the files before writing it down, and write a verbatim initial task message for Cycle 39.

## 4. Initial task message for the next agent (copy verbatim)

You are continuing a **theory-only** hypothesis-generation and research-prioritisation repository. Read
`research/next_agent_handoff.md` first, then `research/idea_register.md`, `research/ranked_shortlist.md`,
`research/source_ledger.md`, `research/validation_handoffs.md`, `research/rejected_and_parked.md` and
`research/cycle_notes.md`, before generating anything. The mission is defined by the canonical prompt
`research_prompts/systematic_edge_discovery_agent_prompt.txt`, which is maintainer-owned and must not be
edited.

**Absolute scope boundary.** Not allowed: backtests, simulations, parameter sweeps, optimisation,
significance testing on strategy results, performance or risk metrics, market-data acquisition or
processing, strategy or signal implementation, executable research infrastructure, job or workflow
launches, changes to workflow files, tests, credentials or infrastructure, work in other repositories, and
any trading. Allowed: reading and summarising literature, market-structure and venue documentation, exchange
and regulator material, and this repository's own notes; specifying hypotheses, falsifiable predictions,
observables and data requirements; maintaining the theory-only artifacts. If a question can only be answered
by running something, write the question down precisely and hand it off — that is the correct output, not a
failure.

**Current state (re-derived from the files — re-derive it again yourself).** 15 dossiers: 5 active
(IDEA-011 69.0 rank 1, IDEA-004 69.0 rank 2, IDEA-010 68.0 rank 3, IDEA-009 60.0, IDEA-014 52.0),
6 parked, 4 rejected. 228 verified sources (S-001 … S-209, S-220 … S-238; S-210 … S-219 reserved and
unused). 10 validation specs (V-001 … V-010): V-008, V-009, V-010 executable; V-002 frozen; V-003
never-to-execute; V-001, V-004, V-005, V-006, V-007 withdrawn. 18 rejections (R-001 … R-018), 12 parkings
(P-001 … P-012; P-013 reserved and unused), 59 baseline rows. Gaps G-01 … G-29 defined (G-17 skipped,
G-26 reserved and unused); open: G-04, G-21, G-28, G-29, G-01. Cycle 37's central finding was a
**correction**: Cycle 36's claim that broker-dealer firm-level regulatory capital is not publicly available
is **false** — Form X-17A-5 is a public EDGAR form type and the net-capital figures of private,
non-listed authorised participants are in publicly indexed filings (S-231) — so G-27 is closed in
IDEA-010's favour on state availability, and G-29 is opened for the ETF → authorised-participant mapping.
Next free identifiers: **IDEA-017, S-239, V-012, G-30, R-019, P-014**. This cycle is **Cycle 38**.

**Execute these priorities in order.**
1. **G-29 (IDEA-010) — does a US corporate-bond ETF's statutory prospectus or SAI name its authorised
   participants?** Read primary filings for the major corporate-bond ETFs (iShares Core U.S. Aggregate Bond
   ETF, iShares Core 1–5 Year USD Bond ETF, and one fund from each of two other issuers). Where direct
   `sec.gov/Archives` fetches fail (HTTP 403), use the EDGAR full-text search JSON API:
   `https://efts.sec.gov/LATEST/search-index?q="authorized participants"&forms=497` (add `&ciks=` to
   restrict to a filer, `&dateRange=custom&startdt=&enddt=` to bound the period, `&from=`/`size=` to page).
   Then compute the coverage count: how many corporate-bond ETFs have a publicly reconstructable AP set,
   and how many (ETF, AP) cells exist in which the AP also has a public capital ratio. If no bond ETF names
   its APs, record the verdict "**the state cannot be attached to an ETF from public filings; IDEA-010 is
   not specifiable — untested, not dead**" and do **not** re-specify around a published crowding proxy
   (S-026, S-157, S-222 measure a different crowd). Update G-29, IDEA-010's dossier and V-010.
2. **G-27/G-29 — the effective-sample and coverage counts.** Using the routes in the Cycle-37 amendment to
   V-010 (Form X-17A-5 on EDGAR for private broker-dealers; 10-Q/10-K XBRL for listed ones; FR Y-9C for
   bank APs), count distinct firms with a public capital ratio, the per-firm filing-cadence distribution,
   the capital-regime composition, and the resulting (ETF, AP, episode) cells. Trap: the EDGAR API's
   `entity_filter` aggregation is truncated to 30 buckets per response, so absence from that list is not
   evidence of absence. Report "untested — not dead" if the counts are too small; never upgrade a
   small-sample null into a kill, and never extend the 1–10 session horizon.
3. **G-28 (IDEA-004) — keep the candidate frozen and V-002 frozen; test one lead.** The 13F
   holdings-matching route is documented as insufficient (see the Cycle-37 blocks). Test whether the
   *published* short leg — FINRA's twice-monthly short-interest publication on a dated schedule (S-127) —
   mapped through the pair structure (short interest in the acquirer around the announcement date) can
   separate convergence capital from a directional bear. Record it as a **lead with its objections stated**
   (construction not published measure; bi-monthly cadence; equities only), not as a candidate.
4. **IDEA-014's state-free existence limb — maintain the inconclusive status.** No effort without a new
   source.
5. **One new mechanism family screen on a genuinely different template.** Candidates, in order of
   promise: **(A)** rate-limited price-insensitive demand under Rule 10b-18's daily 25 %-of-ADTV volume
   cap (the cap is **daily**, not monthly; no 10b-18 source exists in the ledger yet, so add one);
   **(B)** eligibility-switch families where a regulator changes *who may hold* an asset, with a published
   compliance date and a published distance-to-limit state; **(C)** benchmark *methodology* changes with
   a published effective date. Apply the strict bar (published decision-time state, dated price-insensitive
   flow, unclaimed sign, no published result showing the effect) and log bounded negatives as R-019 or
   later.
6. **Wrap up properly.** Update `research/idea_register.md`, `research/ranked_shortlist.md`,
   `research/source_ledger.md` (new sources with explicit verification tags — "fetched directly" versus
   "index-rendered" — and **never invent a citation**), `research/validation_handoffs.md` (specifications
   only, never executed), `research/rejected_and_parked.md` and `research/cycle_notes.md` (including the
   three-pass task-framing loop). Score with the fixed rubric as **research priority, never as a probability
   of profit**. Then rewrite `research/next_agent_handoff.md` with re-derived counts, the next priorities,
   and a fresh, self-contained verbatim initial task message for Cycle 39.

**Standing rules that are not optional.** Read the handoff and the register before generating anything, and
preserve prior work. Every external claim points to a source-ledger entry; record how each source was
verified, and never present an index-rendered quotation as a directly parsed document. Re-derive every count
and identifier from the files rather than carrying it forward — a claim that cannot be checked is worse than
no claim, and an unwritten artifact is not a result. Leave the session with an updated handoff and a fresh
initial task message for the next agent.

## 5. Handoff history

- **Cycle 37 (2026-10-20):** executed the five Cycle-37 priorities. **Corrected Cycle 36's false negative**
  on IDEA-010's state availability (G-27 closed in the candidate's favour; S-231 … S-234); opened **G-29**;
  confirmed and sharpened **G-28**; confirmed the **G-21** null and wrote the comparison down; confirmed
  IDEA-014's limb inconclusive; logged **R-017** (the Cycle-36 ex-dividend screen, written for real) and
  **R-018** (Rule 201, bounded negative; S-235 … S-238); wrote the Cycle-36 gap verdicts into the source
  ledger; corrected stale header counts in `rejected_and_parked.md` and a stale status field in IDEA-002's
  dossier. No candidate, no score change, no new validation specification.
- **Cycle 36 (2026-10-20):** executed the five Cycle-36 priorities; recorded G-27 as "untested" on a claim
  about data availability that Cycle 37 showed to be false; G-28 unconstructible; G-21 null; IDEA-014's limb
  inconclusive; one family screen (ex-dividend) logged in prose only, without an entry or an identifier.
  No score changed; no new sources minted.
- **Cycle 35 (2026-10-20):** the state-integrity repair — a prior cycle's claimed sources, candidate,
  specification, rejection and parkings were found never to have existed; R-014 was written for real; G-22,
  G-23, G-18, G-21, G-24 and G-25 were closed or narrowed; G-27 and G-28 were opened.
