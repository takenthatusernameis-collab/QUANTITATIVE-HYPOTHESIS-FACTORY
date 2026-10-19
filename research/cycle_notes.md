# CYCLE NOTES

## Cycle 1 — 2026-10-19 — first cycle, empty register

**Starting state.** The research area did not exist. The repository contained only the canonical
mission prompt (`research_prompts/systematic_edge_discovery_agent_prompt.txt`), the maintainer
workflow, and the diagnostics ledger. No idea register, no source ledger, no handoff. The prior
worker session produced no repository changes (it terminated on a network timeout with no commits
and no artifacts), so Cycle 1 also established the durable handoff mechanism described in
`next_agent_handoff.md`.

**Scope compliance.** This cycle was theory-only. No backtest, simulation, parameter sweep,
performance calculation, market data download, strategy code, workflow edit, test edit, or job
launch was performed. No external system was modified. The only external action was reading public
web pages to verify citations, which is explicitly permitted ("Read and summarize relevant
literature, market-structure documentation, exchange specifications, public research").

---

## Mandatory task-framing loop (three passes)

The mission prompt requires three deliberate passes before each meaningful research cycle. The
canonical prompt file was **not** modified (mission prompt, continuous-loop step 8).

### Pass 1 — Draft
- **Objective.** Build the first ranked pipeline of candidate systematic trading edges for this
  repository, from an empty register.
- **Key uncertainty.** Whether the pipeline can be made genuinely useful — i.e. whether the first
  cycle can produce candidates that are (a) mechanistically grounded, (b) honestly differentiated
  from published baselines, and (c) specified well enough that an independent validation agent
  could execute them without guessing.
- **Research frontier.** Chosen after inspection: the *institutional intermediation* frontier —
  participants whose balance sheets, mandates, or deadlines create predictable, state-dependent
  demand or supply pressure. Chosen over a momentum/reversal/breakout frontier because the
  operator's stated experience is already in that family, and because a first cycle needs
  mechanisms with published institutional rules attached (provable timing constraints) rather than
  mechanisms inferred from price patterns.
- **Deliverables.** Idea register with complete dossiers; ranked shortlist with the rubric;
  source ledger with verified citations; rejected/parked log; validation hand-off specifications;
  durable handoff for the next session.
- **Scope boundaries.** As per the canonical prompt; the additional self-imposed constraint for
  this cycle was to make every citation verifiable by URL/DOI and to mark every unverified claim as
  an explicit conjecture or source gap.

### Pass 2 — Critique
- **Ambiguity:** "systematic trading edge" could pull the cycle toward either (i) asset-class
  breadth (equities, FX, crypto, futures) or (ii) mechanism breadth. Resolved in favour of
  mechanism breadth in a single market, with asset-class breadth deferred to Cycle 2.
- **Confirmation bias risk:** picking well-trodden literature because it is easy to cite, then
  dressing it as discovery. Mitigation: every dossier carries an explicit "honest classification"
  line, and two of the four candidates were deliberately scored 2/5 on novelty.
- **Novelty inflation:** the index-inclusion effect (IDEA-001) is a 40-year-old published effect.
  Mitigation: it is classified as a documented effect with a conditional refinement, its novelty
  score is the lowest in the register, and the shortlist states explicitly that it is the best
  *test* but the weakest *discovery*.
- **Duplication:** three of the four candidates (IDEA-002, IDEA-004, IDEA-003) risk being
  re-descriptions of known baselines. Mitigation: the baseline table in `rejected_and_parked.md`
  and the "closest known work / what is already known / differentiator" structure in each dossier.
- **Hidden implementation assumptions:** the candidates were checked against the disqualifying
  patterns — no look-ahead, no impossible fills, no zero costs, no survivorship-blind universes.
  IDEA-001's announcement-after-close and effective-close-auction issues and IDEA-004's stale
  crowd proxy were both surfaced rather than assumed away.
- **Data-mining temptation:** IDEA-003's gate and IDEA-004's terciles are exactly the places where
  a validation agent could peek. Mitigation: the validation specifications mandate training/
  selection/holdout separation, frozen thresholds, and an explicit count of variants searched.
- **Wording that could encourage practical validation:** all rule sketches are descriptive and
  non-executable, and every file states the theory-only boundary.

### Pass 3 — Revise and red-team
Final task used for this cycle:
> *Produce the first ranked, theory-only candidate pipeline for the institutional-intermediation
> mechanism family, where each candidate must (i) name a participant and a constraint, (ii) state a
> state variable observable at decision time, (iii) survive an explicit comparison against the
> published baseline it resembles, (iv) carry pre-specified falsification conditions, and (v) be
> accompanied by a validation specification that a separate authorised agent could execute without
> guessing. Every citation must be verifiable; every unverified claim must be labelled as a
> conjecture or a source gap. Rank by the fixed rubric, and hand off the best next theory-only
> task, naming the highest-value unresolved questions, the next mechanism families to investigate,
> and the source gaps to close.*

Red-team of the final task against the forbidden-action list: it does not authorise data acquisition,
backtests, code, metrics, workflow changes, cross-repository work, or any claim that a candidate
has been tested. It explicitly requires source-gap labelling rather than gap-filling by assumption.

---

## What this cycle changed

*(This section describes Cycle 1. Cycle 2 is recorded in "Cycle 2" below.)*

- Created the `research/` area and the five canonical artifacts plus this file.
- Added 4 dossiers: IDEA-001, IDEA-002, IDEA-003, IDEA-004.
- Added 28 verified sources (S-001 … S-028) and 5 explicit source gaps (G-01 … G-05).
- Added 3 validation hand-off specifications (V-001 … V-003).
- Logged 3 rejections, 4 parkings, and a 9-row known-baseline reference table.
- Established `research/next_agent_handoff.md` as the durable handoff and pointed at it from
  `AGENTS.md` and `research/README.md`.

## What this cycle did **not** do

*(Cycle 1.)*

- It did not test anything. No candidate has any evidence of working, and no number in the
  register is a performance estimate.
- It did not establish the size of passive assets tracking any benchmark (G-02), the current
  index-fund trading convention (G-03), a public funding-state proxy (G-01), a timely crowd-depth
  proxy (G-04), or the post-2010 single-name option structure (G-05).
- It did not touch the workflow, the tests, or the diagnostics ledger.

---

## Cycle 2 — new mechanism families, 2026-10-19

**Cycle objective.** Move the register out of the single-asset-class, single-mechanism family
that Cycle 1 occupied, and test whether a candidate can be built in a venue where the
*decision-time state variable is publicly published*. Cycle 2 also attempted the four bounded
supporting tasks carried over from Cycle 1 (T1–T4) and re-checked the Cycle-1 ranks against the
new material.

### Three-pass task-framing loop (required before generation)

**Pass 1 — objective.** Produce 2–3 complete dossiers in at least one mechanism family not yet in
the register, each with a participant, a binding constraint, a dated flow, a decision-time
observable state, and falsifiable predictions; then re-rank the whole register with the fixed
rubric and write validation hand-off specifications for any new candidate that reaches the top
three. Secondary objective: close as many of G-01…G-05 as can be closed with verified sources,
and record the verdicts for those that cannot.

**Pass 2 — framing.** Where does Cycle-2 work sit relative to the register and to known baselines?
Cycle 1 established one family — scheduled, non-price-sensitive flows with a published calendar
and a published effect — inside listed US equities. Cycle 2 deliberately targets the *other* half
of the opportunity: the same structural logic in venues where (a) the effect is *contested*
rather than settled, and (b) the state variable is published by a regulator rather than inferred.
The register's two open method questions are also the Cycle-2 targets: what proxy *should* carry
the state (question 4), and does the mechanism survive where a fast public proxy exists (question
1). Known baselines to stay distinct from: the momentum family (S-012), the value and carry family
(S-016), the attention/PEAD family (S-027), the convergence-to-a-fundamental-anchor family
(S-023) — and, newly identified this cycle, the *commodity basis-convergence* family, which has
**not** yet been read and is logged as the blocking gap G-06.

**Pass 3 — scope.**
- *In scope:* reading and summarising literature, venue and regulator documentation, and provider
  methodology; specifying hypotheses, falsifiable predictions, observables and data requirements;
  maintaining the theory-only artifacts; bounded source-gap resolution.
- *Out of scope (absolute):* any backtest, simulation, parameter sweep, optimisation, significance
  test on strategy results, performance or risk metric, market-data acquisition or processing,
  strategy or signal implementation, executable research infrastructure, workflow changes, tests,
  credentials, infrastructure, or trading. Nothing in this cycle was executed; no data was
  acquired or processed; the only computation is the rubric arithmetic recorded in
  `ranked_shortlist.md`.
- *Deliverables:* three dossiers (IDEA-005…IDEA-007), twenty-six new ledger entries (S-029…S-054),
  the Cycle-2 ranking with Cycle-1 rank changes, validation hand-off specifications (V-004 onward)
  for new top-three candidates, new rejection and parking records, gap verdicts, and a rewritten
  handoff.

### What was actually done

- **Frontier chosen:** "scheduled, non-price-sensitive flows whose decision-time state is published
  by a regulator" — instantiated first in commodity futures (the passive index roll), then in two
  non-equity venue families (see the dossiers).
- **Search and verification:** Cycle 1 already used the provider-hosted PDF and the
  Exchange/Commission rulebook as the verification standard; Cycle 2 held to it and added a
  *contradiction standard*: for every new candidate the contradicting peer-reviewed evidence was
  located deliberately and recorded, not just the supporting evidence. That standard changed the
  outcome of the commodity family — see below.
- **Two documented findings that changed the work:**
  1. The regulator's own definitions (S-030) name the participant and the mechanism directly: the
     "Index Traders" category is defined as traders replicating a commodity index and rolling
     "from future to future using a fixed methodology".
  2. The "front-run the roll" trade that dominates the practitioner literature is **documented as
     decayed**: the impact disappears post-2012 in the peer-reviewed evidence (S-033); the impact
     in the deepest contract reverses within minutes while the passive's execution cost is
     documented at about three percent per year (S-032); the annual-rebalancing impact is "modest
     and temporary" (S-034); index-trader positions do not predict near-contract excess returns
     (S-037); and commodity index rolls are found to have "little futures price impact" (S-036).
     Cycle 2 therefore did **not** write a front-running candidate. It wrote a candidate that
     survives this evidence by conditioning on a public state, and it recorded the naive version
     as a rejection (R-004) rather than quietly dropping it.
- **Bounded tasks T1–T4 attempted:** T1 (G-02) narrowed — a public category-level passive-asset
  series exists (S-040) and a *direct* contract-level measure of the passive complex exists in
  futures (S-030); a benchmark-specific series does not (new gap G-07). T2 (G-03) not closed and
  re-framed (G-08). T3 (G-01) narrowed to a specified composite of four verified public series
  (S-041, S-042). T4 (G-05) partially closed from exchange research (S-043), with the
  single-name question explicitly left open.

### Artifact history (Cycle 2)

- `research/idea_register.md` — added IDEA-005, IDEA-006, IDEA-007; rewrote the cross-idea map;
  updated the stale rank lines in the four Cycle-1 dossiers (scores and reasoning untouched).
- `research/source_ledger.md` — added S-029…S-054; rewrote the gap section with verdicts; added
  G-06, G-07, G-08, G-09, G-10.
- `research/ranked_shortlist.md` — re-scored all seven candidates under the fixed rubric; recorded
  Cycle-1 rank changes and per-candidate Cycle-2 re-checks.
- `research/validation_handoffs.md` — added V-004 (required: IDEA-005 reached the top three) plus
  the optional V-005 (IDEA-007) and V-006 (IDEA-006).
- `research/rejected_and_parked.md` — added R-004, R-005, P-005, P-006, P-007; added six new
  known-baseline rows (15 rows in total).
- `research/next_agent_handoff.md` — rewritten.
- `research/README.md` — "next free ID" pointers updated.
- `AGENTS.md` — ID sequences updated to the ranges in use after Cycle 2.

### Deviations from the Cycle-1 pattern, and why

- Cycle 1 read "a candidate" as one entry on the Cycle-1 shortlist and wrote one dossier. Cycle 2
  deliberately wrote **three** dossiers spanning non-equity venue families, because the Cycle-1
  register was concentrated in a single mechanism and a single asset class, and the canonical
  prompt asks for the space of mechanisms to be covered rather than for depth in one.
- Cycle 2 used a stricter rule for "already known": a candidate had to be shown to be distinct not
  only from the register's own baselines but from the *closest published work*, and that work had
  to be located and read. This is why R-004 exists and why IDEA-005 is a state-conditioned
  candidate rather than the front-running candidate the literature would have suggested.
- No market data was acquired, no code was written or run, and no result was computed other than
  the rubric arithmetic. Two read-only web research agents were launched for source verification in
  two of the new families; they did not return usable output within the cycle, so **all** source
  verification was done directly, and every cited item was checked against a publisher, repository,
  regulator or provider page before it entered the ledger. No agent output was used as a citation
  without that check.

### Search log (Cycle 2, abridged)

Queries and page retrievals covered: the S&P GSCI methodology and roll schedule; the CFTC
Commitments of Traders reports, the Disaggregated and Supplemental series and the "Index Traders"
category; the commodity-index-roll literature (Mou; Stoll & Whaley; Hamilton & Wu; Bessembinder
et al.; Yan/Irwin/Sanders; Irwin/Sanders/Yan); the hedging-pressure and inventory-state literature
(Bessembinder 1992; Gorton/Hayashi/Rouwenhorst); the FX end-of-day fixing and closing-clock
literature; the funding-currency and cross-currency-basis literature; the SPIVA scorecards and the
ICI asset series (G-02); the New York Fed reference rates, standing-repo operations and primary
dealer statistics (G-01); and Cboe's 0DTE research and statistics (G-05). Provider and exchange
PDFs were read from the issuer's own domain where the issuer's bot protection permitted: the
S&P DJI methodology PDF returned HTTP 403 to a direct fetch and was read through a text extraction
of the same URL, cross-checked against the provider's Reference Guide PDF — this is recorded in the
ledger entry rather than glossed.

---

---

## Cycle 2 closure pass — 2026-10-19 — G-10 closed *mostly*, and the register demoted one of its own candidates

**Why this pass happened.** Cycle 2 left three blocking originality gaps open (G-06, G-09, G-10).
This pass closed the funding-currency one, G-10, because it was the gap with a decisive
consequence: if the carry-crash and global-liquidity literature already contains IDEA-007's
claim, then IDEA-007 is a published baseline in a new label and the register must say so.

**Three-pass task-framing loop for the closure pass.**
- *Pass 1 — draft.* Read the funding-currency, cross-currency-basis, global-liquidity and
  carry-crash literature (central-bank staff work, BIS statistics and occasional papers, the
  IMF/ECB/Bank-of-England backdrop, and the peer-reviewed FX and international-finance
  literature), register every item, and test IDEA-007's claim against what is there.
- *Pass 2 — critique.* Two objections were raised against the draft. First, that reading a
  literature is not the same as establishing what it says; every claim had to be pinned to a
  quotable line, and a docent-style summary would not be acceptable as a source entry. Second,
  that the "does the literature contain my candidate?" question can be answered wrongly in the
  candidate's favour by searching only for the candidate's own wording — so the search was run
  from the *published papers' side* (what do they claim, what do they leave open?) rather than
  from the candidate's side.
- *Pass 3 — revise and red-team.* Red-team: the strongest possible version of the objection is
  that "no published cross-sectional result" is a *negative* finding about a search, not a
  positive finding about the world, and that a search that fails to find something must be
  recorded as a search with a stated scope, not as a proof of novelty. The pass therefore wrote
  the negative finding into the ledger *with its scope attached* and made the residual claim
  conditional on it.

**What was actually done.**
- Verified and registered **19 further sources** (S-055 … S-073), completing the
  funding-currency / global-liquidity corpus, with the full verification record (how each item
  was reached, and how a document was read when a publisher's bot protection blocked the direct
  fetch).
- Reached the decisive source: **Filipe, Nissinen and Suominen (2023), *Journal of Banking &
  Finance* 149:106800**, which measures funding constraints by covered interest parity
  deviations and shows that funding risk explains carry trading activity, carry returns and
  carry-long/short correlations, with a positive result and a model (S-055). The aggregate
  version of IDEA-007 is therefore **published**.
- **Rejected the aggregate version** as **R-006** and **narrowed IDEA-007 to v1.1**: its claim is
  now the *cross-sectional* structure (which currencies respond most to a given dollar funding
  expansion) and the publication-timing test — nothing else.
- Recorded a **negative data finding with scope**: no published cross-currency basis series
  exists in the BIS statistics catalogue, and the published funding-constraint studies construct
  the state from paid vendor forwards. The *slow* state is published; the *fast* state is not.
- Rewrote the G-10 verdict from OPEN to **MOSTLY CLOSED** and rewrote the shortlist's IDEA-007
  entry, the known-baseline table row, and the V-005 specification accordingly, including a
  blocking condition that a validator must treat the aggregate relation as a **baseline to
  reproduce**, never as a discovery.

**Artifact history (Cycle 2 closure pass).**
- `research/source_ledger.md` — S-055 … S-073 added; G-10 verdict rewritten to MOSTLY CLOSED.
- `research/idea_register.md` — IDEA-007 to v1.1 (mechanism, evidence status, remaining
  uncertainty, and the data-construction constraint in the mechanism chain).
- `research/rejected_and_parked.md` — R-006 added; the funding-currency baseline row rewritten.
- `research/ranked_shortlist.md` — IDEA-007's evidence and novelty justifications rewritten,
  table flags updated, cross-cutting notes 2 and 6 updated; score unchanged at 64.0 because the
  evidence improved while the novelty narrowed.
- `research/validation_handoffs.md` — V-005's blocking condition rewritten as a scope
  restriction; the published aggregate results added to the mandatory baseline list.
- `research/next_agent_handoff.md` — rewritten; G-10 removed from the open-gaps list, R-006 and
  the new leads added.

**Deviations and honest limits.**
- The register's *own* candidate was demoted by a source it did not previously cite. That is the
  intended behaviour of the process, and the arithmetic of the shortlist hides it: IDEA-007's
  total is unchanged at 64.0 while its composition moved from "a published time-series result
  plus an unclaimed refinement" to "a published baseline plus a narrow residual".
- The negative finding (no published cross-currency basis series) is scoped to the BIS statistics
  catalogue and to the studies read; it is not a proof that no such series exists anywhere.
- **G-06 and G-09 remain open.** They are the cheapest high-value work left, and both can kill a
  candidate: G-06 decides whether IDEA-005 is a commodity convergence trade in a new costume,
  and G-09 decides whether IDEA-006's fixing-cluster price effect is already documented.

---

## Cycle 2 closure pass, second round — 2026-10-19 — G-09 closed *mostly*, and the register demoted a second candidate

**Why this pass happened.** The G-10 closure left G-09 as the remaining blocking originality check
on IDEA-006, and a read-only verification agent was launched to locate the intraday FX
microstructure literature around the 4pm fix (the "Evans and Lyons 4pm-fix line" and the
"Michelberger and Witte" work named in S-047). The agent's output arrived at the end of the
session.

**The agent's output was not usable as a citation set, and this is the most important process
finding of the pass.** Of the papers it reported, **three carried wrong identifiers and one paper
does not exist**:
- "Rime, Sarno and Sojli (2010), 'Exchange rate forecasting and the New York close', *JFI* 19(1):
  13–41, DOI 10.1016/j.jfi.2009.10.001" — **does not exist**. That DOI resolves to Bruno and
  Claessens, "Corporate governance and regulation", *JFI* 19(4): 461–482; no Crossref record
  exists under the claimed title; and the *JFI* 19(1) table of contents contains no such article.
  The real paper by those authors is S-051. This is the **third phantom citation** found in this
  register, after "Avalos, Beets, Ehrmann and Leguia — the role of the funding currency" and
  "Bruno and Shin — Global liquidity and the FX market".
- Osler (2003) is DOI 10.1111/1540-6261.00588, not …00589 (the latter is Denis, McConnell,
  Ovtchinnikov and Yu on S&P 500 earnings).
- Evans and Lyons (2002) is DOI 10.1086/324391, not 10.1086/343830.
- The reported DOI for Neely, Rapach, Tu and Zhou (2014) belongs to Tate and Yang (2015) on female
  leadership; that paper is not load-bearing for any dossier and was **not** registered.
Every identifier was therefore re-checked against the Crossref API, the arXiv record and the NBER
record **before** anything entered the ledger, and only the verified forms were used. The wrong
identifiers are recorded in the G-09 gap entry so that no future session repeats them.

**A second integrity finding, this time inside a source.** The 2026 working paper registered as
S-081 ("Currency Returns and Price Discovery around Global FX Fixings", SSRN 7388124) has
verified metadata and a deposited abstract, but **its 39-item reference list is fabricated**: two
spot-checked references — Ben-David et al. (2025, *RFS* 38(1): 188) on ETF flows and intraday FX
price pressure, and Ahmad (2024, *International Review of Economics & Finance* 89: 412) on
intraday order flow and price discovery — cannot be found in Crossref by title, author and
journal. **No reference from that bibliography may be cited in this register**, and the paper is
registered only for its own abstract, which duplicates the published fix results.

**What was actually done.**
- Retrieved and registered **eight further sources** (S-074 … S-081): Michelberger and Witte (2016)
  on the microstructure of the WM/Reuters 4pm fix; Melvin and Prins (2015) on equity hedging and
  the London fix; Evans (2018) on trading around the WMR fix; Ito and Yamada (2015, NBER WP) on
  pre/post-fixing autocorrelation; Evans and Lyons (2002); Osler (2003) on order clustering as
  the rival mechanism; Benenchia, Galati and Lepone (2025) on the post-revision benchmark, which
  also completes the author list of S-047; and the S-081 working paper with its caveat.
- **The finding went against the register's own candidate.** The fix-window price effect is
  published: passive hedging demand at the fix has a "strong, but temporary" impact concentrated
  at end of month (S-075); price changes around the fix are negatively serially correlated
  (S-076); the pre- and post-fixing periods are negatively autocorrelated (S-077); the 4pm window
  has elevated volatility and larger moves (S-074); and the dollar climbs before fixes and falls
  after them across the nine most traded currencies over 21 years (S-081). **That is exactly the
  mechanism and the pattern IDEA-006 claimed to be measuring for the first time.**
- **Rejected the aggregate version as R-007** and **narrowed IDEA-006 to v1.1**: the residual is
  the *settlement-side* deadlines beyond the fix (the CLS cut-offs and the post-US-close window
  that T+1 created) plus the post-2015 persistence of the published fix effect.
- **Scored honestly and dropped the candidate**: evidence 4 → 3 and novelty 3 → 2, so IDEA-006
  falls from 66.0 to 59.0 and from rank 5 to rank 7 — below the parked IDEA-002 (63.0). The
  ranking now shows a parked candidate above a retained one, which is the correct ordering and is
  stated as such in the shortlist.
- **Logged a new blocking gap, G-11**: the settlement-side deadline cluster has never been
  searched. "Unclaimed" is currently an expectation, not a finding, and the dossier says so.
- Narrowed the V-006 specification: the fix window becomes a control to be reproduced, the
  published fix results become mandatory baselines, and the executable test is the residual only.

**Three-pass task-framing loop for this pass.**
- *Pass 1 — draft.* Locate and register the intraday fixing literature; test IDEA-006's originality
  claim against what it says; decide whether the candidate survives as a candidate.
- *Pass 2 — critique.* Two objections. (i) An agent-produced citation list is evidence about the
  agent, not about the literature, so every identifier must be re-derived independently. (ii) A
  search that *finds* the effect is not the same as a search that *establishes* that no paper
  tests the settlement side; the second claim needs a search of its own, and it has not happened.
  Both objections were adopted: the first became a re-verification pass, the second became G-11.
- *Pass 3 — revise and red-team.* Red-team: could the demotion be wrong? The strongest defence of
  IDEA-006 is that the *cluster* is a different object from the fix and that the published papers
  are pre-reform, pre-T+1 and use non-public data. That defence is real, and it is exactly the
  size of the residual the dossier now claims — so the candidate was narrowed rather than killed,
  and its score was set to reflect a narrow, unsearched residual.

**Artifact history (this pass).**
- `research/source_ledger.md` — S-074 … S-081 added (part 4); S-047's author-list caveat closed;
  G-09 verdict rewritten to MOSTLY CLOSED with the mis-reported identifiers recorded; G-11 opened.
- `research/idea_register.md` — IDEA-006 to v1.1 (mechanism chain, originality, expected return
  source, rule sketch, predictions, data requirements, evidence status, remaining uncertainty,
  score 66 → 59); register header updated.
- `research/rejected_and_parked.md` — R-007 added; the fixing baseline row rewritten.
- `research/ranked_shortlist.md` — IDEA-006 moved to rank 7 and re-scored (66.0 → 59.0); rank
  order corrected (IDEA-007 → 5, IDEA-002 → 6, IDEA-006 → 7); notes 2, 3 and 6 updated.
- `research/validation_handoffs.md` — V-006 narrowed to the residual with the published results as
  mandatory baselines; summary paragraph updated.
- `research/next_agent_handoff.md` — rewritten: 81 sources, 7 rejections, G-09 mostly closed, G-11
  opened, and the remaining cheap work is G-06 and G-11.

**Honest limits of this pass.**
- Two of the located fix papers were read at the level of the abstract and the publisher's article
  text, not in full; one (M&W) is open access and could be read in full by a future agent. The
  claims registered here are their *reported* claims, not reproductions.
- The published fix literature is dense and partly built on non-public data (administrator- and
  dealer-provided tick data), so "nobody has looked at the settlement side" cannot be established
  by the same route that established "somebody has looked at the fix". G-11 must be closed with
  that asymmetry in mind.
- The candidate that remains (IDEA-006 v1.1) is **blocked on G-11** and should be treated as a
  hypothesis awaiting a literature check, not as a live candidate.
