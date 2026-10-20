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

---

## Cycle 3 — gap closures and new mechanism families, 2026-10-19

**Cycle objective.** Close the three remaining blocking originality gaps (G-06, G-11, G-10 residual)
that can kill a candidate; then produce 2–3 new dossiers in mechanism families not yet in the
register, chosen by the Cycle-2 rule that the decision-time state variable must be *published by an
institution*; write the state-proxy methodological note; re-rank; and hand off.

### Three-pass task-framing loop (required before generation)

**Pass 1 — draft.** Objective: (a) close G-06 (commodity basis-convergence literature for IDEA-005),
G-11 (settlement-side deadline cluster for IDEA-006) and the G-10 residual (cross-sectional funding
state for IDEA-007), each by reading the closest published work and recording a ledger entry with
the verification method; (b) choose a frontier from handoff section 3 where the state is published
by a venue, regulator, benchmark administrator or settlement utility; (c) write 2–3 dossiers with
a participant, a binding constraint, a dated flow, a decision-time-observable state, falsifiable
predictions and verified sources; (d) write the state-proxy methodological note as a closing
section of `idea_register.md`; (e) rank with the fixed rubric and add V-007+ specs for any new
top-three candidate. Key uncertainty: whether a new family can be specified whose state variable is
genuinely published at decision time, rather than constructed from quotes or inferred.

**Pass 2 — framing.** Cycle 1 covered scheduled non-price-sensitive flows in listed US equities
(IDEA-001…IDEA-004). Cycle 2 added commodity futures (IDEA-005), the FX fixing clock (IDEA-006)
and the FX funding state (IDEA-007), and established the venue-selection lesson: the state-proxy
problem is largely a venue-selection problem. The two closure passes demoted IDEA-007 (aggregate
version published, R-006) and IDEA-006 (fix effect published, R-007). For Cycle 3, the open
families from handoff section 3 are: (1) corporate credit index/ETF flow vs dealer balance sheet;
(2) securities lending / short-sale constraints / recall-driven forced selling — the state
(borrow availability, recalls, short-position disclosures) is a documented, disclosable operational
fact rather than a latent variable; (3) crypto perpetual funding rate — the funding rate is settled
every few hours and published by the exchanges, the clearest instance of "the state is published by
the venue"; (4) slow information diffusion with an event clock (accounting standards adoption);
(5) settlement/payment infrastructure as a dated flow (continuation of IDEA-006's vein).
Known baselines to stay distinct from: the momentum family, the value/carry family, the
attention/PEAD family, the convergence-to-fundamental-anchor family, the commodity
basis-convergence family (S-032…S-039), the fix-window literature (S-074…S-081), and the
funding-currency/global-liquidity corpus (S-052…S-073).

**Pass 3 — scope.** Frontier chosen: Family 2 (securities lending / short-sale constraints /
recall-driven forced selling) as IDEA-008 and Family 3 (crypto perpetual funding rate) as IDEA-009.
Both have a decision-time state variable published by an institution/venue: short-interest and
securities-lending disclosures are published (Reg SHO, exchange short-interest reports), and
perpetual funding rates are published by exchanges on a fixed cadence. Both are outside the
register. Both admit a participant-and-constraint story: (IDEA-008) the borrow constraint binds
and recalls force involuntary covering; (IDEA-009) the funding rate is the crowded-leverage state
settled every few hours. In scope: literature reading, verification, dossier writing, state-proxy
note, ranking, validation specs. Out of scope (absolute): backtests, data acquisition, code,
metrics, workflow changes, tests, credentials, infrastructure, trading. No candidate is tested
here; every score is a research priority, not a success probability.

### What was actually done

- **Gap closures:** G-06 narrowed (commodity basis-convergence literature S-032…S-039 located;
  none conditions the roll concession on passive share × depth, so IDEA-005's differentiator
  survives as a conjecture, not an exhaustive negative). G-11 partially closed — settlement-side
  mechanics are a priced friction (S-082 Lee/Ranaldo/Tsuruga IMF WP/26/156; S-071 Ranaldo &
  Santucci de Magistris JFE 2022) but the specific CLS deadline cluster / T+1 post-US-close
  window is untested; IDEA-006 v1.1 survives but unproven. G-10 residual open — no located paper
  tests the cross-sectional funding-state claim; IDEA-007 v1.1 survives but unproven.
- **Source ledger:** added S-082 with full verification record; updated G-06, G-10, G-11 verdicts.
- **Idea register:** updated IDEA-005/006/007 originality sections with gap results; updated
  register header change notes.
- **New dossiers:** IDEA-008 (SECURITY-LEND / short-sale constraints / recall-driven forced
  selling) and IDEA-009 (PERP-FUND / crypto perpetual funding rate as a published funding state).
- **State-proxy note:** written as a closing section of `idea_register.md`.
- **Ranking:** new candidates added to `ranked_shortlist.md` with per-score justification and
  hard-stop flags; existing ranks re-checked.
- **Validation specs:** V-007 (IDEA-008) and V-008 (IDEA-009) added to `validation_handoffs.md`.
- **Rejected/parked:** no new rejections or parkings this cycle.
- **Handoff:** `next_agent_handoff.md` rewritten with new state.

### Artifact history (Cycle 3)

- `research/source_ledger.md` — S-082 added; G-06 narrowed, G-10 residual open, G-11 partially
  closed.
- `research/idea_register.md` — IDEA-005/006/007 originality sections updated; IDEA-008 and
  IDEA-009 added; state-proxy methodological note added as closing section; header updated.
- `research/ranked_shortlist.md` — IDEA-008 and IDEA-009 added with scores and justifications;
  existing ranks re-checked.
- `research/validation_handoffs.md` — V-007 and V-008 added.
- `research/next_agent_handoff.md` — rewritten.
- `research/cycle_notes.md` — this entry.

### Deviations and honest limits

- The funding rate literature base is thinner than the equity short-sale literature; IDEA-009's
  evidence score reflects that, and the venue risk (crypto) is stated honestly.
- Every identifier was re-derived from Crossref/arXiv/publisher before use; the phantom-citation
  and fabricated-bibliography findings from the Cycle-2 closure passes are treated as standing
  warnings.
- No candidate has been tested; no number in any dossier is a performance estimate.

---

## Cycle 4 — new mechanism families, 2026-10-19

**Cycle objective.** Add three new dossiers in mechanism families not yet in the register
(corporate-credit ETF flow vs dealer balance sheet as IDEA-010; accounting-standards adoption as a
slow-information event clock as IDEA-011; settlement-side deadline cluster as a price determinant
as IDEA-012), re-rank the register with the fixed rubric, write V-009 for the new top-three
candidate, and update the state-proxy methodological note to cover the new candidates' data-access
profile.

### Three-pass task-framing loop (required before generation)

**Pass 1 — draft.** Objective: (a) add three dossiers each naming a participant, a binding
constraint, a dated flow, a decision-time-observable state, falsifiable predictions and verified
sources; (b) re-rank all twelve candidates under the fixed rubric; (c) write V-009 for IDEA-011
(which enters the top three at rank 3 tied at 72.0); (d) extend the state-proxy methodological
note to cover IDEA-010's partial data-access problem (ETF flow public, AP-level balance-sheet data
commercial) and IDEA-012's hard data-access block (intraday order-book data not public). Key
uncertainty: whether each new family's state variable is genuinely published at decision time, or
whether the binding constraint is commercial or proprietary data.

**Pass 2 — framing.** Cycle 1 covered scheduled non-price-sensitive flows in listed US equities
(IDEA-001…IDEA-004). Cycle 2 added commodity futures (IDEA-005), the FX fixing clock (IDEA-006)
and the FX funding state (IDEA-007), and closed G-09 and G-10 as blocking originality gaps. Cycle
3 added securities-lending equities (IDEA-008) and crypto perpetuals (IDEA-009), both with
decision-time state variables published by an institution/venue, and wrote the state-proxy note.
Cycle 4 extends into: corporate credit (ETF flow vs dealer balance sheet), slow information
diffusion with an event clock (accounting standards adoption), and settlement-side deadlines as a
structural dated flow — continuing IDEA-006's vein but as a separate candidate (IDEA-012).
Known baselines to stay distinct from: all previously registered families plus the ETF arbitrage
limits family (Pan & Zeng 2019; Eisfeldt et al. 2024) and the accounting-standards adoption
literature (Armstrong et al. 2010; Beuselinck et al. 2009).

**Pass 3 — scope.** Frontier chosen: Family 1 (corporate-credit index/ETF flow vs dealer balance
sheet) as IDEA-010, Family 2 (slow information diffusion with an event clock — accounting
standards adoption) as IDEA-011, and Family 3 (settlement-side deadline cluster as a price
determinant) as IDEA-012. In scope: literature reading, verification, dossier writing, re-ranking,
V-009, state-proxy note extension. Out of scope (absolute): backtests, data acquisition, code,
metrics, workflow changes, tests, credentials, infrastructure, trading. No candidate is tested
here; every score is a research priority, not a success probability.

### What was actually done

- **New dossiers:** IDEA-010 (CREDIT-ETF / corporate-bond ETF flow vs AP balance-sheet constraint),
  IDEA-011 (ACCTCLOCK / accounting-standards adoption as a slow-information event clock) and
  IDEA-012 (CLS-CLOSE / settlement-side deadline cluster as a price determinant). Each carries a
  participant, a binding constraint, a dated flow, a decision-time-observable state, falsifiable
  predictions, confounders, data requirements, theory/evidence status and verified sources.
- **Re-ranking:** `ranked_shortlist.md` re-scored all twelve candidates; IDEA-011 enters at rank 3
  (tie, 72.0), IDEA-010 at rank 6 (68.0), IDEA-012 at rank 12 (56.0); IDEA-003 moves to rank 5,
  IDEA-008 to rank 7, IDEA-009 to rank 9, IDEA-006 to rank 11; IDEA-002 remains parked (P-004).
- **Validation spec:** V-009 added to `validation_handoffs.md` for IDEA-011; executable as specified
  (adoption calendars are regulator-published; all inputs public); binding constraint is the small
  event sample and the concurrent-macro confound.
- **Source ledger:** added S-090 (Bianchi/Bigio/Engel "Scrambling for Dollars" NBER w29457,
  verified via NBER + CEPR), S-091 (CLS Group T+1 documentation), S-092 (Brogaard/Han/Won 0DTE
  volatility SSRN), S-093 (Almeida/Freire/Hizmeri 0DTE asset pricing SSRN), S-094 (Vilkov 0DTE
  trading rules SSRN). G-10 residual remains open (Bianchi/Bigio/Engel confirms the aggregate
  channel, not the cross-section). G-11 remains open (CLS documentation confirms the deadline
  window exists operationally but no located paper tests it as a price determinant). G-06 remains
  narrowed but not closed exhaustively. T5–T8 remain open with recorded verdicts.
- **State-proxy note:** extended to cover IDEA-010's partial data-access problem and IDEA-012's
  hard data-access block; the venue-selection lesson is restated with the new candidates included.
- **Rejected/parked:** no new rejections or parkings this cycle; IDEA-002 stays parked (P-004),
  IDEA-006 v1.1 stays blocked on G-11, IDEA-007 v1.1 stays blocked on the G-10 residual.
- **Handoff:** `next_agent_handoff.md` rewritten with new state.

### Artifact history (Cycle 4)

- `research/source_ledger.md` — S-090 … S-094 added; G-10 residual open, G-11 open, G-06 narrowed
  but not closed exhaustively; T5–T8 verdicts recorded.
- `research/idea_register.md` — IDEA-010, IDEA-011 and IDEA-012 dossiers added; register header
  updated; state-proxy methodological note extended.
- `research/ranked_shortlist.md` — all twelve candidates re-scored with per-score justifications and
  hard-stop flags; cross-cutting notes extended; per-candidate Cycle-4 sections added.
- `research/validation_handoffs.md` — V-009 added for IDEA-011; header paragraph updated.
- `research/next_agent_handoff.md` — rewritten.
- `research/cycle_notes.md` — this entry.

### Deviations and honest limits

- Bianchi, Bigio and Engel's "Scrambling for Dollars" (S-090) confirms the aggregate dollar-funding
  → currency response channel but not the cross-sectional claim that would make IDEA-007's
  cross-sectional residual publishable; the cross-section remains unverified.
- IDEA-012 is blocked on G-11: the settlement-side deadline cluster / T+1 post-US-close window is
  untested as a price determinant; if a published paper tests it, IDEA-006 and IDEA-012 are both
  rejected rather than narrowed.
- IDEA-010's binding data constraint is commercial AP-level balance-sheet data; if that cannot be
  validated against public disclosures, the candidate is untestable as specified.
- Every identifier was re-derived from Crossref/arXiv/publisher before use; phantom-citation and
  fabricated-bibliography findings from earlier cycles are standing warnings.
- No candidate has been tested; no number in any dossier is a performance estimate.

---

## Cycle 5 — closure passes and the frontier after the settlement window closes, 2026-10-19

**Cycle objective.** Cycle 5 was run in two halves, and the handoff now records both. *First half*:
close the blocking originality gaps that the previous handoff identified (G-10 residual, G-11, G-06,
T5–T8), add new dossiers in mechanism families not yet in the register, and re-rank. *Second half*
(this session): close G-11 decisively, resolve the outstanding full-text check on IDEA-013's cited
published work, re-rank the register against the fixed rubric, update every downstream artifact and
rewrite the handoff.

### Three-pass task-framing loop (required before generation)

**Pass 1 — draft.** Objective: (a) close G-10, G-11 and G-06 with published work, recording each
source with the method by which it was verified; (b) answer IDEA-013's outstanding first check by
reading the full text of the published work it claims to differ from; (c) add candidates in
mechanism families not yet in the register, with the decision-time state published by a venue,
regulator, benchmark administrator or settlement utility; (d) re-rank everything under the fixed
rubric; (e) write validation specifications for any new top-three candidate; (f) rewrite the
handoff. Key uncertainty for the second half: whether G-11's literature, when actually searched,
would *narrow* the two settlement-window candidates or *kill* them — and whether a published state
is ever available **before** the decision it is meant to inform.

**Pass 2 — framing.** Cycle 1 covered scheduled non-price-sensitive flows in listed US equities
(IDEA-001 … IDEA-004); Cycle 2 added commodity futures and two FX candidates and closed G-09 and
G-10 as blocking gaps; Cycle 3 added securities-lending equities and crypto perpetuals and wrote
the state-proxy note; Cycle 4 added corporate-bond ETFs, accounting-standards adoption and FX
settlement. At the start of Cycle 5 the register held twelve candidates and the frontier was
narrowing: the remaining originality gaps were all in the *settlement and funding* family, and the
second-half objective had to be decided by the outcome of one literature check rather than chosen
freely. The framing that governed the second half was the register's own rule — "if a published
paper already shows the effect, the candidate is rejected, not narrowed" — and the standing
rediscovery guard's three conditions (G-12, G-13, and the closure rule).

**Pass 3 — scope.** In scope: literature reading and verification, dossier maintenance, gap
verdicts, re-ranking, validation-specification status, artifact consistency, and the handoff. Out of
scope (absolute, and honoured): backtests, simulations, parameter sweeps, significance testing,
performance or risk metrics, market-data acquisition or processing, strategy or signal
implementation, executable research infrastructure, job or workflow launches, changes to workflow
files or tests, credentials or infrastructure, work in other repositories, and any trading. The
canonical mission prompt was not modified. No candidate was tested; every score is a research
priority, not a success probability.

### What was actually done

- **First half (previous session, recorded for completeness):** G-10 closed against IDEA-007 (R-008);
  G-06 closed as a bounded negative finding with contradicting evidence registered (S-098, S-099);
  G-08 mostly closed and G-05 split; IDEA-013 (EU-ETSCOMP) added as a new candidate at 70.0;
  S-095 … S-111 registered; G-12 opened as the general question of whether a published state can
  change the sign or existence of a published effect.
- **Second half — G-11 closed against IDEA-006 and IDEA-012.** The settlement-side literature was
  searched and produced four findings: (i) a settlement deadline cluster is a **published price
  determinant** (S-112: Kraenzlin and Nellen, SNB WP 2010/06 — after CLS "the value of intraday
  liquidity has increased during the hours of the CLS settlement cycle", with an estimated "roughly
  1.5bp for the CLS settlement cycle"); (ii) the securities settlement cycle is a **published
  price-impact and market-quality determinant** (S-113, S-114, and S-115 as a preprint), with the
  published sign that shortening the cycle *improves* liquidity; (iii) the FX settlement-risk
  premium is already published (S-082, S-071); and (iv) the **post-US-close window is documented as
  a cost, not an edge** — the New York Fed's own FX Committee material names "NY 4-6pm currency
  liquidity" as the transition's priority FX risk and records an expected "uptick in price premium
  and market impact for trades executed later in the NY trading day" (S-117, S-118), while the
  market record is "less than 1% of trades in the $7 trillion OTC FX market" in that window, a
  half-hour pricing-engine outage at 5pm ET and "bid/ask spreads widen and liquidity shrinks"
  (S-119), and the market's own answer was custodian cut-off extensions and pre-funding (S-120).
  Both candidates had set the rule that this outcome rejects rather than narrows. **IDEA-006 was
  rejected (R-009) and IDEA-012 was rejected (R-010).**
- **IDEA-013's outstanding first check was performed.** The full text of the published work
  (arXiv 2606.03767v2) was fetched and read. Result: the paper does **not** condition the
  surrender-month premium on the aggregate surplus, so the candidate is not a re-description of
  published work; **but** the paper's model already makes the equilibrium price affine in the
  aggregate bank of allowances, its own robustness construction works from operator-level,
  bank-adjusted shortfalls, and its statement that the delayed-trading pattern "persists into the
  most recent phase of the EU ETS" covers Phase IV (2021), a large-surplus year. In addition, the
  Commission's own TNAC communications (S-121) establish that the aggregate balance is published in
  **late May or June of the year following the emissions year**, so under the pre-2023 regime it was
  published *after* the surrender deadline it was meant to inform. The decision-time form of the
  candidate therefore has three observations and no deficit year. **IDEA-013 was parked (P-008),
  with a dated unblocking condition; G-13 was opened and a fifth screening condition added to the
  state-proxy note.**
- **Frontier screening that produced no candidate.** Four further families were screened so that the
  next cycle does not re-derive them, and all four were found to be published or documented:
  exchange-published maintenance-margin schedules (S-122: "I do not find a significant effect of
  margin changes on the futures price level", but a 50% rise in realized variance and funding-
  liquidity spillovers); ETF primary-market arbitrage and AP inventory (S-123: the FCA's own study
  of 128 ETFs, and its proprietary dataset — the same constraint that blocks IDEA-010); crypto
  spot-ETF flow (S-124, S-125: "the ETF channels large, uninformed demand into the spot market,
  making it busier but shallower"); and the benchmark-window-alteration angle (already published,
  S-047, S-080). These are now baseline rows, so the next cycle starts from a wider reference set.
- **Ranking and specifications:** the register was re-ranked under the fixed rubric. The active
  ranking is now eight candidates (IDEA-001 76.0, IDEA-004 74.0, IDEA-005 72.0, IDEA-011 72.0,
  IDEA-003 71.0, IDEA-010 68.0, IDEA-008 65.0, IDEA-009 63.0), with IDEA-002 and IDEA-013 parked
  and three candidates withdrawn. **No new validation specification was required**, because no new
  candidate entered the top three; **V-005 and V-006 were withdrawn** because their candidates were
  rejected.
- **Handoff:** `next_agent_handoff.md` rewritten with the new state, a dated next task and a fresh,
  self-contained initial task message.

### Artifact history (Cycle 5)

- `research/source_ledger.md` — S-095 … S-111 (first half); **S-112 … S-125** (second half: the
  settlement-deadline cluster, the T+1 window, the decision-time state, and the four screened-out
  families); S-101's caveats rewritten with the full-text read; **G-11 rewritten as CLOSED against
  IDEA-006 and IDEA-012**; **G-13 opened**; the Cycle-5 verdict block and the ledger header updated.
- `research/idea_register.md` — IDEA-006 to v1.2 (**rejected**, R-009) with a closure paragraph;
  IDEA-012 to v1.1 (**rejected**, R-010) with a closure paragraph; IDEA-013 to v1.1 (**parked**,
  P-008) with the resolved first check, the contradicting evidence, the decision-time timing
  finding, a revised score (70 → 58) and a dated unblocking question; register header rewritten;
  state-proxy note extended with **condition (e)** on publication timing and with IDEA-013 in the
  governed list.
- `research/rejected_and_parked.md` — **R-009** (IDEA-006) and **R-010** (IDEA-012) added;
  **P-008** (IDEA-013) added; seven baseline rows added (settlement deadlines, settlement cycle
  length, the post-close window, the EU ETS surrender-month premium, margin schedules, ETF
  primary-market arbitrage, crypto spot-ETF flow); rediscovery guard rewritten with the three
  standing screening conditions; header counts corrected.
- `research/ranked_shortlist.md` — header rewritten for Cycles 1–5; the table rebuilt with the
  active ranking, the parked table and the withdrawn table; Cycle-5 rank changes recorded; section
  headers re-labelled for the new ranks; a new section added for IDEA-013; cross-cutting notes
  rewritten (nine notes, including the new "a published state is not automatically a decision-time
  state" note).
- `research/validation_handoffs.md` — header rewritten for Cycles 1–5; **V-005 and V-006 marked
  withdrawn with reasons**; the executable set stated explicitly.
- `research/next_agent_handoff.md` — rewritten.
- `research/cycle_notes.md` — this entry.

### Deviations and honest limits

- **The register shrank rather than grew.** Cycle 5 ended with three rejections, one parking and one
  new candidate, against the previous handoff's request for two to three new dossiers. The reason is
  recorded rather than papered over: the second half of the cycle was spent on the two checks that
  could invalidate candidates (G-11 and IDEA-013's full text), and the frontier families that could
  have supported new dossiers were screened and found to be published (S-122 … S-125). A future cycle
  should treat those families as closed and generate in families the register has not touched.
- **G-11's scope is narrow in one direction.** No located paper measures an **FX-spot** price effect
  specific to the post-US-close window with the published fix effect removed. That gap was not
  converted into a candidate because the window is documented as structurally illiquid (S-119) and
  the data required are commercial. It is recorded as a baseline boundary instead.
- **Two of the new institutional sources are index-rendered rather than directly parsed.** The New
  York Fed FX Committee minutes (S-118) and the Traders Magazine article (S-119) are binary PDFs
  whose text was returned through the search index; the quotes are reproduced as returned, and both
  are used only for market-structure documentation, never as the sole support for an economic claim.
  The peer-reviewed claims that carry the verdict (S-112, S-113, S-114) were metadata-checked
  directly against Crossref.
- **The valuation of IDEA-013 rests on a reading of the published sample's coverage, not on its
  year-by-year numbers.** The published paper states that the pattern persists into Phase IV; it does
  not report the April premium's magnitude by year, so the candidate's existence-flipping hypothesis
  is neither supported nor refuted by it. That ambiguity is recorded as such, and is one reason the
  candidate is parked rather than rejected.
- **No candidate has been tested; no number in any dossier is a performance estimate.** Every
  identifier added this cycle was re-derived from Crossref, the publisher's own record, the issuing
  institution or the primary document before use; the phantom-citation and fabricated-bibliography
  findings from earlier cycles remain standing warnings.

---

## Cycle 6 — the G-13 / G-12 screen and the five frontier families, 2026-10-20

**Cycle objective.** The Cycle-5 handoff left two standing general questions and a secondary
programme. *Primary:* apply **G-13** (is the state published *before* the decision?) and **G-12**
(does the conditioning change the *sign or the existence* of the effect, rather than only its
size?) to every active candidate, and re-score or park whatever failed. *Secondary:* screen the
five mechanism families the handoff named as the frontier — statutory date-bound obligations
outside the EU ETS, sovereign issuance calendars, fast-payment rails, sovereign bond index
inclusion, and physical-delivery calendars in commodity futures — one search round each, recording
**every** verdict including the negative ones, and writing a full dossier only for a family whose
mechanism is unclaimed *and* whose state is published before the decision. *Tertiary:* attempt
T5–T8 and record whatever could not be closed as new source gaps.

### Three-pass task-framing loop (required before generation)

**Pass 1 — draft.** Objective: run the two standing screens across the whole active register; run
one bounded literature round on each of the five frontier families and record the verdicts; write
one dossier if a family earns it; re-rank; update every artifact; rewrite the handoff. Key
uncertainty: whether the two screens, which had been stated as principles since Cycle 5, would
actually *remove* candidates — that is, whether the register's own active set had been passing a
test it had never been subjected to, or whether the screens were doing no work and would change
nothing.

**Pass 2 — framing.** Cycle 1 covered scheduled non-price-sensitive flows in listed US equities;
Cycle 2 added commodity futures and two FX candidates; Cycle 3 added securities-lending equities
and crypto perpetuals and wrote the state-proxy note; Cycle 4 added corporate-bond ETFs,
accounting-standards adoption and FX settlement; Cycle 5 added an EU-allowances candidate,
rejected three and parked one. At the start of Cycle 6 the register held thirteen candidates, of
which eight were active. The framing that governed this cycle was deliberately *narrow*: the
highest-value work was not a new mechanism family but **running the two standing screens across
the existing register**, because a screen that has never been applied to a candidate is a
principle rather than a check, and the register had grown six candidates since the screens were
written. The secondary programme (the five families) was run in parallel, one search round each,
because the handoff had already pre-registered what a negative verdict looks like: a baseline row
in the known-baseline table, not a candidate.

**Pass 3 — scope.** In scope: literature reading and verification, dossier maintenance, gap
verdicts, re-ranking, validation-specification status, artifact consistency, and the handoff. Out
of scope (absolute, and honoured): backtests, simulations, parameter sweeps, significance testing,
performance or risk metrics, market-data acquisition or processing, strategy or signal
implementation, executable research infrastructure, job or workflow launches, changes to workflow
files or tests, credentials or infrastructure, work in other repositories, and any trading. The
canonical mission prompt was not modified. No candidate was tested; every score is a research
priority, not a success probability.

### What was actually done

- **The two screens were run on every active candidate, and they removed two.** The screen was
  applied candidate by candidate, and each verdict is recorded in the candidate's dossier, in the
  ranked shortlist and in the source ledger's "Cycle-6 verdicts" block, so the reasoning survives.
  - **IDEA-005 ROLLCOND — parked (P-009) on G-12.** Its own formulation is an *existence* claim,
    which is what G-12 asks for; but the screen asks what the candidate *demonstrates*, and the
    closest published test of its **own state variable** — the CFTC Index Traders' share of open
    interest conditioned on commodity returns during roll periods — reports **no significant
    effect** (S-099), the trader-type literature conditions convergence *speed* rather than the
    nearby-to-deferred concession (S-098), the aggregate effect the joint state would rescue is
    documented as decayed after 2012 (S-033, S-037, S-036), and G-06 closed as a bounded negative
    finding. It is **parked rather than rejected** because nothing published *shows* the
    candidate's effect; two unblocking conditions are recorded, both required. Score 72.0 → 60.0.
  - **IDEA-008 SECURITY-LEND — parked (P-010) on G-13, with a dated unblocking condition.** The
    failure is a calendar, not a judgement: the SEC's December 2025 order exempts Rule 10c-1a
    compliance "with respect to the reporting date until September 28, 2028, and with respect to
    the dissemination date until March 29, 2029" (S-126), so the earliest public availability of a
    borrow-cost state is **29 March 2029**; the short-interest fallback is twice-monthly and
    published roughly seven to eight business days after its settlement date (S-127). The
    register's Cycle-3 belief that "lending fees are published" was wrong about the calendar.
    Score 65.0 → 63.0; new gap **G-14** records the dated unblocking condition.
  - **IDEA-010 CREDIT-ETF — re-scored 68.0 → 65.0.** Its mechanism's core (AP inventory and
    balance-sheet constraints driving ETF–NAV dislocations) is published institutionally at S-123,
    so novelty falls 3 → 2; G-13 passes only partially because the differentiating state is
    commercial, and the published substitutes are unvalidated — new gap **G-16**.
  - **IDEA-001, IDEA-003, IDEA-004, IDEA-009 and IDEA-011 passed both screens with no score
    change**, but two of the passes were not costless and are recorded. IDEA-001's G-12 pass holds
    **only on the existence limb** (the side asymmetry and the second leg); the flow-scaling limb
    conditions size only, and V-001 is amended accordingly. IDEA-004's G-13 pass **resolves** the
    question the Cycle-5 handoff had left open: the 13F-based crowd state is published on EDGAR
    within 45 days of each quarter end, so a filing-anchored rule is decision-time feasible, the
    binding constraint is proxy *validity* (G-04) and not timing — and V-002 is amended to re-anchor
    its rebalance grid to the filing cadence.
- **The five frontier families were screened, one search round each, and every verdict is
  registered — including the four negative ones.** Families 2 (sovereign issuance calendars), 3
  (fast-payment rails), 4 (sovereign bond index inclusion) and 5 (physical-delivery calendars) are
  **published baselines** and are now rows in the known-baseline table with the sources that
  establish them: S-137, S-138, S-139 (sovereign index inclusion, peer reviewed in *JIE* and
  *JFE*), S-142, S-143, S-144 (issuance calendars), S-140, S-141 (fast payments), S-145 alongside
  S-038, S-039 (delivery calendars).
- **Family 1 produced the cycle's one new candidate: IDEA-014 RIN-DEADLINE (60.0, status
  `candidate`).** The template — a price-insensitive, date-bound obligation whose concession is paid
  by the obligated party — is published for the EU ETS (S-101), so that version is a baseline. The
  **US Renewable Fuel Standard** is the same template with a different regulator, a different
  obligor population, and a state that is published *before* the decision: the obligation's size is
  codified for two future years in 40 CFR 80.1405 (S-128), the deadline is **published by
  regulation** — "The annual compliance reporting deadline will be calculated in accordance with
  paragraph (f)(1)(i) of this section and published on EPA's website" (40 CFR 80.1451(f)(1)(iii),
  S-129) — and the deadline has already been moved once by published rule (the 2025 deadline moved
  from 1 September 2026 to 1 October 2026, with the next stated as 31 March 2027; S-131). The RIN
  price is a studied object (S-134, S-135), with a published weekly price series (S-132) and a
  physically delivered futures venue (S-136). **The sign of the deadline effect is not asserted
  anywhere**: it is the candidate's first empirical test (gap **G-15**), and the published
  market-quality evidence runs against the candidate on cost (S-133), which is why it enters at
  60.0 and not higher.
- **T5–T8 were revisited and none was closable.** T5: closing-auction **volume** statistics are
  published by the venues (S-100), so the aggregate participation question is answerable, but the
  per-security long history is commercial and the *attribution* question is not answerable from
  aggregate volume. T6: unchanged — no published continuous dealer FVA series exists, IDEA-002
  stays parked. T7: the *data* leg is closed (single-name 0DTE is constructible from public OCC
  data) and only the *literature* leg remains open. T8: unchanged — no benchmark-specific
  aggregate passive-asset series exists. **No new task was added.**
- **The re-rank, the artifacts and the validation specifications were updated.** The active
  ranking is now seven candidates: IDEA-001 (76.0), IDEA-004 (74.0), IDEA-011 (72.0), IDEA-003
  (71.0), IDEA-010 (65.0), IDEA-009 (63.0), IDEA-014 (60.0). Four candidates are parked
  (IDEA-002, IDEA-005, IDEA-008, IDEA-013) and three are rejected (IDEA-006, IDEA-007, IDEA-012).
  The top three are unchanged, so **no new validation specification was required**; **V-004 and
  V-007 are withdrawn** with their candidates, and **V-001 and V-002 are amended** with the
  binding consequences of the two screens. The executable set is V-001, V-002, V-003, V-008, V-009.

### Artifact history (Cycle 6)

- `research/source_ledger.md` — **Cycle 6 additions (S-126 … S-145)** written: the SEC Rule 10c-1a
  and Rule 13f-2 exemptive orders (S-126), FINRA's short-interest publication schedule (S-127),
  two **primary regulatory texts read directly** (40 CFR 80.1405, S-128, and 40 CFR 80.1451,
  S-129), three **Federal Register documents** (the Set 2 rule, S-130; the 2025 deadline
  extension, S-131), EPA's published RIN price series (S-132), the NERA market-quality white paper
  (S-133), the peer-reviewed RIN price literature (S-134, S-135), the ICE RIN futures specification
  (S-136), the sovereign-index and issuance-calendar literature (S-137 … S-144) and the roll
  mechanics (S-145). A **"Cycle-6 verdicts"** block was added: the per-candidate G-13/G-12
  verdict table, the five family-screen verdicts including all four negative ones, and the three
  new gaps **G-14, G-15, G-16**. The header was rewritten for Cycles 1–6.
- `research/idea_register.md` — header rewritten for Cycle 6; **a "Cycle 6 screen" block added to
  every active candidate's dossier**, with the G-13 and G-12 verdicts and their consequences for
  the dossier; IDEA-005's status changed to parked (P-009) with its score, unblocking conditions
  and the reason it is a parking rather than a rejection; IDEA-008's status changed to parked
  (P-010) with the dated 2029 unblocking condition; IDEA-010 re-scored with the mechanism's
  published core recorded; **the IDEA-014 RIN-DEADLINE dossier written in full** (60.0,
  `candidate`); the state-proxy methodological note rewritten — its "venue-selection" paragraph
  corrected on two points (IDEA-008's publication calendar and IDEA-004's timing), a new
  condition-(e) paragraph added on what Cycle 6 taught, and two new parking cases added to
  section 5, with the governed-candidate list updated.
- `research/rejected_and_parked.md` — **P-009** and **P-010** added in full, each with the
  evidence, the reason it is a parking rather than a rejection, and its unblocking conditions;
  **seven baseline rows** added for the screened families; the rediscovery guard extended with two
  new standing conditions (a dated future publication calendar is a parking with a date; a
  commercial differentiating state is retained only with an explicit validation precondition); the
  header counts corrected.
- `research/ranked_shortlist.md` — header rewritten for Cycles 1–6; the table rebuilt with the new
  ranking, the enlarged parked table and the withdrawn table; Cycle-6 rank changes recorded; every
  candidate section given a **Cycle-6 re-check** paragraph; section headers re-labelled for the new
  ranks; a new section added for IDEA-014; the cross-cutting notes rewritten (the venue-selection
  note corrected, the decision-time note extended with two further instances, and the
  narrowness, tail-risk, diversification and open-gaps notes updated).
- `research/validation_handoffs.md` — header rewritten for Cycles 1–6; **V-004 and V-007 marked
  withdrawn with reasons**; **V-001 and V-002 amended** with the binding consequences of the two
  screens; the executable set restated.
- `research/next_agent_handoff.md` — rewritten.
- `research/cycle_notes.md` — this entry.

### Deviations and honest limits

- **The register shrank by two and grew by one.** The handoff asked for two to three new dossiers;
  Cycle 6 produced one. The reason is recorded rather than papered over: the primary task was to
  run the two standing screens across the active register, and the screens removed two candidates
  and re-scored a third; the secondary task was one search round per frontier family, and four of
  the five families are published. **A cycle that removes candidates by applying a test is not a
  failed cycle**, but it is a smaller register, and the next cycle's marginal value is again in
  *new mechanism families* rather than in re-ranking what is here.
- **IDEA-014's sign is not asserted, and its cost floor is documented against it.** The published
  market-quality evidence (S-133 — roughly one-tenth the liquidity of comparable commodity
  futures, transaction costs peaking at five times theirs, and a documented tendency to price
  near-expiry vintages above longer-lived ones) is the strongest single piece of evidence against
  the new candidate, and it is a *white paper by a consultancy with a client position*, not a
  peer-reviewed result. It is registered as market-quality evidence, used for a cost floor and a
  prior only, and the register's other RIN sources (S-134, S-135) are peer-reviewed but do not
  speak to the cost structure or to the deadline effect.
- **The novelty check on family 1 is one search round.** The verdict "no located work presents a
  state-conditioned compliance-deadline concession in the US RIN market" is a **bounded negative**,
  not an exhaustive search, and it is logged as gap **G-15** together with the precise question. The
  other four family verdicts carry the same caveat, and each names the sources that establish it.
- **Two of the twenty new sources are index-rendered rather than directly parsed** (the IMF working
  paper S-139 and the Banco Central do Brasil working paper S-140; the Bank of Canada paper S-141
  was also index-rendered). They are used for mechanism-framing and scale claims only, never as the
  sole support for an economic claim, and each entry says so. **The load-bearing sources of this
  cycle were read directly**: the two CFR sections, the three Federal Register documents (two of
  them in their own raw text), FINRA's schedule page and the ICE product page.
- **A web-search provider rate limit truncated one line of work.** The general search provider
  rate-limited partway through the cycle; the remainder of the work was done through the Crossref
  API, the Federal Register API, the eCFR renderer API and direct page fetches, which are not
  rate-limited in the same way. One consequence is recorded: the Fed's FOMC memorandum on the
  refunding statement could not be parsed locally (no text-extraction tooling was available for its
  font encoding) and was therefore **not registered**; the family-2 verdict rests on the two
  published preprints instead.
- **The G-13 screen changed one candidate's characterisation and one candidate's status, and the
  change to IDEA-004 is a correction rather than a new finding.** The register had described
  IDEA-004's proxy as "quarterly-stale"; the screen showed the *publication* is timely on the
  filing cadence and the open question is proxy *validity*. The screen also showed that the
  register's Cycle-3 assessment of IDEA-008 ("lending fees are published") was wrong about the
  calendar. Both corrections are recorded in the dossiers, in the shortlist and in the
  state-proxy note.
- **No candidate has been tested; no number in any dossier is a performance estimate.** Every
  identifier added this cycle was re-derived from the Federal Register API, the eCFR renderer, the
  issuing institution's own page, or Crossref before use; the phantom-citation and
  fabricated-bibliography findings from earlier cycles remain standing warnings.

### Cycle 8 — bounded-negative closures and handoff update (2026-10-20)

- **Primary (a): G-04 closed as bounded negative (literature side).** Bounded search found no freely available, decision-time public crowd-depth proxy for U.S. equities. 13F-based measures are 45-day lagged/stale for the required timing in practical terms and proxy validity is unprovable with public data; borrow depth/exit capacity remain broker-gated. Publication cadence is feasible on a quarterly-anchored rule but validity is the binding unclosable gap; IDEA-004 remains rank 2 constrained by this gap. Recorded in `research/source_ledger.md`.
- **Secondary (b): Five frontier families screened (one round each).** Families 2–5 identified as published baselines (sovereign issuance calendars, fast-payment rails, sovereign bond index inclusion, physical-delivery calendars) with sources recorded. Family 1 (rule 10b5-1 cooling-off / statutory date-bound obligations) did not yield an unclaimed mechanism matching the template beyond what led to IDEA-014; existing findings logged. No new dossier written.
- **Tertiary (c): T5–T8 revisited.** T5 (closing-auction volume/attribution) remains partial; T6 (dealer FVA proxy) remains open (IDEA-002 parked); T7 literature leg for single-name 0DTE remains open; T8 (benchmark-specific passive-asset series) remains open. No closures.
- **Handoff rewritten.** `research/next_agent_handoff.md` updated for Cycle 9 with corrected gap status (G-04 and G-16 closed as bounded negatives). Prior superseded handoff content summarized here.

---
## Cycle 9 — 2026-10-20 — continue discovery per handoff

### Three-pass task-framing loop

**Pass 1 — draft.** Objective: execute the Cycle 9 task from section 4 of the handoff. Investigate open data gaps where feasible (G-01, G-02/G-07, G-03, G-05 literature leg). Screen new frontier families (one search each). For any new candidate that qualifies, write full dossier (unclaimed mechanism, state published before decision, sign decided by published state). Run G-13/G-12 screens on every candidate before ranking. Record results in cycle_notes. Key uncertainty: finding a genuinely unclaimed mechanism with published state before decision and sign decidable by published state.

**Pass 2 — critique.** Must apply G-13 and G-12 as screens on every candidate before ranking, record both verdicts. New IDs start at IDEA-015, S-146, V-010, G-18, R-011, P-011; call this Cycle 9. Every external claim must cite verifiable URL/DOI, distinguish index-rendered from directly fetched verification. Scores are research-priority weights only. Scope is theory and discovery only.

**Pass 3 — revise.** Execute screens on existing candidates, search frontier families, document findings. If no new qualifying candidate emerges, record negative findings. Update artifacts.


### G-13/G-12 screen results (Cycle 9)


**Cycle 9 screening:** Applied G-13 (state published before decision) and G-12 (conditioning changes sign or existence, not just size) to all candidates.

- IDEA-001 (RECON-FLOW): G-13 PASS (announcement published before effective close). G-12 PASS on existence/asymmetry and second-leg, not on pure size-scaling. No change.
- IDEA-002 (FUNDSTATE, parked P-004): G-13 FAIL/PENDING on public proxy (G-01); feasibility blocks. G-12 not directly testable until proxy exists. Parked remains correct.
- IDEA-003 (VRP-STATE): G-13 PASS (option surface available at decision). G-12 PASS (gate can flip sign of harvestability). No change.
- IDEA-004 (SLOWCAP-COND): G-13 PASS on filing cadence (13F) as documented; G-12 PASS on the non-monotonic/sign claim. Proxy validity (G-04) is separate constraint. No change.
- IDEA-005 (ROLLCOND, parked P-009): G-13 PASS (COT reports published before roll). G-12 FAIL - nearest published tests null (S-099) and aggregate effect decayed; parked correct.
- IDEA-006 (FIXCLOCK, rejected R-009): already rejected on G-11; screen moot.
- IDEA-007 (FUNDSTATE-FX, rejected R-008): rejected on published result; moot.
- IDEA-008 (SECURITY-LEND, parked P-010): G-13 FAIL - lending rates not public before 29 March 2029 (S-126); parked correct (dated unblocking G-14).
- IDEA-009 (PERP-FUND): G-13 PASS (funding rate published continuously). G-12 PASS on sign-keyed reversal. No change.
- IDEA-010 (CREDIT-ETF): G-13 partially PASS (flow data public) but AP stress leg commercial (G-16). G-12 PASS conceptually on state-dependent effect. No change to status.
- IDEA-011 (ACCTCLOCK): G-13 PASS (adoption calendars published years ahead). G-12 PASS on state-dependent effect size/sign existence. No change.
- IDEA-012 (CLS-CLOSE, rejected R-010): rejected; moot.
- IDEA-013 (EU-ETSCOMP, parked P-008): G-13 FAIL for pre-2023 regime (TNAC published after surrender deadline); parked correct (dated unblocking). G-12 conditional only with future data.
- IDEA-014 (RIN-DEADLINE): G-13 PASS (obligation/codification published in advance; deadline set by regulation S-128/S-129). G-12 PENDING - sign not asserted (first empirical test G-15); condition on "sign decided by published state" is the open test.


### Frontier families screening (one search each per Cycle 9 task)

Searched for new mechanism families matching template (price-insensitive/deadline-driven flow with published state before decision that determines sign/existence).

Findings:
- Family screening did not yield an unclaimed mechanism meeting all three criteria. The candidate IDEA-014 (family: statutory compliance deadlines with published positions) is already registered and its sign remains the open test (G-15). Other families examined are documented in source ledger as published baselines or blocked by timing/data constraints.
- Open gaps revisited: G-01 (funding proxy) remains open/narrowed; G-02/G-07 (passive asset series) remain open/narrowed; G-03 (closing auction convention) remains open; G-05 literature leg remains open (single-name 0DTE). No new gaps opened beyond those already known.


### Cycle 9 outcome

No new dossiers added (new IDs remain IDEA-015, S-146, V-010, G-18, R-011, P-011 unused). Applied G-12/G-13 screens to all candidates; statuses unchanged. Existing gaps confirmed. Updated cycle_notes as required.

---

## Cycle 12 — targeted gap investigation (2026-10-20)

**Pass 1 — draft.** Objective: execute Cycle 12 task (section 3 of handoff): close feasible gaps (G-01, G-02/G-07, G-03, G-05 literature) and run one frontier screening round. New IDs start at IDEA-015, S-146, V-010, G-18, R-011, P-011.

**Pass 2 — critique.** Apply G-13/G-12 screens to all candidates before ranking; record verdicts. Cite every external claim with verifiable URL/DOI; distinguish index-rendered from directly fetched. Theory only.

**Pass 3 — revise.** Execute searches, document findings, update artifacts.

### Gap investigation findings (Cycle 12)

- **G-01 (dealer funding-state proxy):** SCOOS (Fed, quarterly, qualitative net-percentage survey) remains the only public dealer-funding-terms series; SOFR percentile spreads (NY Fed, daily) measure repo market, not dealer funding value adjustments. No continuous public series of dealer funding value adjustments located. Composite (SOFR-percentile-spread × SCOOS) not validated against disclosed dealer funding costs. Gap remains open; IDEA-002 stays parked (P-004).
- **G-02/G-07 (benchmark-specific passive-asset series):** ICI publishes category-level aggregates (indexed mutual funds + ETFs, domestic equity) but no benchmark-specific (e.g. S&P 500) tracked-asset series. 13F filings are quarterly and 45-day lagged; assembly from 13F/ICI category data remains possible but unvalidated as a benchmark-specific series. Gap remains open; IDEA-001 flow-scaling limb still rests on estimated quantity.
- **G-03 (closing-auction convention/attribution):** S&P DJI methodology (S&P US Indices Methodology, 2026-07-07) confirms quarterly reconstitution effective after close of third Friday, share freeze in preceding week, announcements published after close; but no newly located documentation of index funds' effective-close trading convention or attribution of auction volume to index funds vs. arbitrageurs. Gap remains open.
- **G-05 (single-name 0DTE literature leg):** Index-level 0DTE variance risk premium now documented: Almeida/Freire/Hizmeri (2024, SSRN abstract 4701401; 2025 FMA) — high VRP driven by upside risk compensation, negatively predicts market returns; Dim/Eraker/Vilkov (2023, SSRN 4692190) — 0DTE trading, gamma risk, volatility propagation; Vilkov (2023) — 0DTE trading rules; ScienceDirect (2026) — 0DTE SPX option pricing review citing Almeida 2025, Bandi 2026, Khalil 2024 (intraday VRP predictive content). Dew-Becker & Giglio (Chicago Fed WP 2025-17) — decline of VRP, alpha contribution shrunk. No peer-reviewed work located establishing whether the *single-name* variance-gate channel is documented. Literature leg remains open, narrowed.

### Frontier screening (Cycle 12)

One search round across unexamined frontier families for mechanisms matching template (published state before decision, sign decidable by published state). No unclaimed mechanism meeting all three criteria located. No new dossiers. New IDs IDEA-015, S-146, V-010, G-18, R-011, P-011 remain unused.

### Cycle 12 outcome

No new dossiers added. G-01, G-02/G-07, G-03 remain open; G-05 literature leg narrowed (index-level 0DTE VRP documented; single-name gate work still not located). G-14, G-15 remain open. G-13/G-12 screens re-applied: no status changes. Handoff rewritten for Cycle 13.

---

## Cycle 13 — evidence-currency pass on the register's own top candidate, and six frontier screens (2026-10-20)

**Pass 1 — draft.** Objective, taken from the Cycle-12 handoff: (a) close the feasible gaps —
G-01 (composite dealer funding proxy), G-02/G-07 (benchmark-specific tracked assets), G-03
(effective-close convention and attribution), G-05 (single-name 0DTE literature leg); (b) run one
search round per unexamined frontier family for a mechanism matching the template (a
price-insensitive, date-bound obligation with a published state before the decision whose content
decides the sign), writing a full dossier only if the mechanism is unclaimed, the state is published
before the decision, the sign is decidable from that state, and the venue is feasible; (c) apply
G-13/G-12 to any new candidate before ranking. New IDs start at IDEA-015, S-146, V-010, G-18,
R-011, P-011.

**Pass 2 — critique.** Two objections to my own draft plan were recorded before searching. First,
the plan was written as if the gaps were the primary object; the register's *own* ranking was not
in the plan at all, and the rank-1 candidate had not been re-read against literature published since
2023 — which is exactly the failure mode that has just killed a *different* candidate family in
other research programmes. Second, the "new frontier family" instruction needed a sharper filter
after the Cycle-10 and Cycle-12 dry runs: a family that merely *sounds* like the template is not
enough; the family must contain a state whose **content decides the sign**, and the family must
survive the practical question of whether the price-insensitive flow is *actually binding at the
moment it is dated*. I therefore added to the plan a standing question for every family screened:
*is the obligation tight when it falls due, and who is on the other side of it?* That question is
what disqualified California, and it would have disqualified a dozen plausible-sounding candidates
before this.

**Pass 3 — revise.** Execute the searches; record every claim with a source; distinguish
index-rendered from directly fetched; update every artifact; theory only, no tests, no data.

### What was actually done

1. **The rank-1 candidate was re-read against the 2024–2026 literature, and it died.** IDEA-001
   RECON-FLOW (76.0) was killed by three published results: the index effect has collapsed to
   approximately zero in the modern sample (S-146, *Journal of Finance* 2025: additions below 1%
   over the past decade, deletions 0.1% for 2010–2020, an average inclusion effect of −3 basis
   points in 2020); the flow-scaling differentiator has a **published null** (same paper: no
   apparent relationship between net purchases by index trackers and the inclusion effect); and the
   mechanism is published as *anticipatory liquidity provision* that shifts price pressure away from
   the effective date, with short interest rising into implementation and falling afterwards
   (S-147), because the counterparty to passive demand is the issuing firm itself (S-151). Recorded
   as **R-011**; **V-001 withdrawn**. This is the register's first rank-1 rejection, and it is the
   single most important outcome of the cycle.
2. **Two gaps closed *in that candidate's favour* in the same cycle**, which is why the rejection is
   an evidence rejection rather than a technicality: **G-03** (the index manager states in its own
   research that index funds and ETFs are structurally incentivised to execute in the closing
   auction, with MOC orders dominant — S-149; corroborated by peer-reviewed work on closing-auction
   volume share, price impact and passive attribution — S-150) and **G-02/G-07** (a published
   method now exists for inferring the AUM tracking each of five named indices from
   reconstitution-day closing volume, 2000–2021 — S-148).
3. **One gap closed against a variant:** the **G-05** literature leg, closed *against* IDEA-003's
   single-name extension (S-153, S-154 — single-name variance risk premia are frequently zero or of
   the opposite sign to the index premium, with correlation risk doing the pricing). The aggregate
   version of IDEA-003 survives untouched at 71.0.
4. **One gap reopened in part:** **G-04**, because a decision-time, public, price-computable
   crowding measure exists (S-157, comomentum) and has never been validated against the
   holdings-based measure the register uses. This opens **G-18** rather than licensing a
   re-specification, and it puts **V-002 on hold** until it is closed.
5. **Two re-scores:** IDEA-004 74.0 → 69.0 (published, mechanistically explained decay of the base
   effect — S-156 — plus a bounded negative on crowding-conditioned average returns, S-172, preprint;
   the score falls on persistence, not on mechanism or test design) and IDEA-009 63.0 → 60.0 (the
   funding-rate mechanism and its mean-reversion are now published independently — S-158, S-159).
6. **Six frontier families screened; no new dossier.** Crypto token unlocks (documented by an
   interested party, S-170); California Cap-and-Invest's surrender deadline (documented, and the
   price-insensitive demand is satisfied in advance); California Cap-and-Invest's Allowance Price
   Containment Reserve sale (a published, state-triggered, date-bound supply event with a codified
   trigger, published tier prices, published notices and a published schedule — **and it has never
   been used**, S-163, with the regulation at S-164 and S-174); the Treasury General Account → repo
   channel (published, S-160–S-162); accelerated share repurchases (published, S-166, S-167); and
   the perpetual-funding family (published, S-158, S-159). The California reserve-sale screen is
   the cycle's most instructive negative: it is the cleanest *template* found in thirteen cycles of
   screening and it fails on the practical question — a supply valve that never opens cannot carry a
   price effect.
7. **G-01 re-confirmed as open, with a sharper statement:** the construct is peer-reviewed
   (S-155) and the funding-state family is published with a public decision-time measure (TGCR −
   IORB, S-162), but no public, continuous, *dealer-level* funding-value-adjustment series exists and
   none is likely to. IDEA-002 stays parked (P-004).
8. **IDEA-011's post-2010 evidence base was flagged, not searched** — the mirror image of the check
   that killed IDEA-001 has never been run for the accounting-adoption drift, whose literature of
   record is largely pre-2015. That is the highest-value single task for the next cycle.

### G-13 / G-12 screen results (Cycle 13)

- IDEA-001 (RECON-FLOW): G-13 PASS (and its two qualifications — the effective-close premise and
  the flow-scale quantity — were both closed in the candidate's favour, S-149/S-148/S-150).
  **G-12 FAIL on every limb** (published null on the differentiator, published collapse of the
  effect, published mechanism pointing at a different window) → **rejected, R-011**.
- IDEA-003 (VRP-STATE): G-13 PASS (live option surface). G-12 PASS (the gate flips the
  *harvestability*, i.e. the sign, of the harvest). No score change (71.0); G-05's single-name
  extension foreclosed.
- IDEA-004 (SLOWCAP-COND): G-13 PASS on a filing-anchored rule. G-12 PASS on the sign limb.
  Re-scored 74.0 → 69.0 on persistence; V-002 held until G-18 closes.
- IDEA-009 (PERP-FUND): G-13 PASS (venue-published funding rate, zero lag). G-12 PASS on the sign
  limb. Re-scored 63.0 → 60.0 on novelty (S-158, S-159).
- IDEA-010 (CREDIT-ETF): G-13 PARTIAL PASS (flow leg public; AP-stress leg commercial). G-12 PASS
  on the existence limb. No score change (65.0); G-16 narrowed, still open.
- IDEA-011 (ACCTCLOCK): G-13 PASS, comfortably. G-12 PASS on the existence limb. No score change
  (72.0); rank 3 → 1 by artefact of other candidates' removal.
- IDEA-014 (RIN-DEADLINE): G-13 PASS (obligation codified, deadline published by regulation, moves
  only by published rule). G-12 PASS on the sign limb. No score change (60.0); G-15 still open.
- Parked and rejected candidates: unchanged (IDEA-002 P-004, IDEA-005 P-009, IDEA-008 P-010,
  IDEA-013 P-008; IDEA-006 R-009, IDEA-007 R-008, IDEA-012 R-010).

### Artifact history (Cycle 13)

- `source_ledger.md` — added **S-146 … S-174** (29 entries) and a **Cycle-13 gap-verdicts block**
  (G-01 re-confirmed; G-02/G-07 and G-03 closed; G-04 reopened in part; G-05 closed against the
  single-name variant).
- `idea_register.md` — IDEA-001 v2.0 marked rejected (dossier preserved); Cycle-13 screen blocks on
  IDEA-003, IDEA-004, IDEA-009, IDEA-010, IDEA-011, IDEA-014; a register-header summary; and a new
  **Cycle-13 frontier-family screen log** (six families, six bounded negatives).
- `ranked_shortlist.md` — title and header updated; the ranking table rewritten for six candidates;
  the withdrawn table now carries IDEA-001; Cycle-13 rank-change and validation-rule paragraphs;
  Cycle-13 re-check blocks for IDEA-001 (withdrawal verdict), IDEA-003, IDEA-004, IDEA-009,
  IDEA-011; cross-cutting notes 4, 8 and 9 updated (including the new G-18 and the closure of T5–T8).
- `rejected_and_parked.md` — **R-011** written; **twelve new baseline rows**; the rediscovery guard
  extended with the **evidence-currency condition** and the version-drift warning.
- `validation_handoffs.md` — header updated; **V-001 withdrawn** (with the amendment marked moot);
  the Cycle-13 update paragraph records that no new specification was required and that V-002 is on
  hold pending G-18.
- `cycle_notes.md` — this entry.
- `next_agent_handoff.md` — rewritten for Cycle 14.

### Deviations and honest limits

- **No new candidate was written, and no new ID was consumed** — IDEA-015, S-175, V-010, G-19,
  R-012 and P-011 all remain unused. Three consecutive cycles have produced no new dossier; the
  register's discovery rate is zero and its closure rate is not. That is the honest state of the
  pipeline and the next cycle must say so plainly rather than manufacture a candidate to fill a
  slot.
- **Several sources were read through the search index rather than fetched directly**, because the
  publisher blocked direct fetches (the SEC roundtable PDF returned HTTP 403; the SSRN landing pages
  for S-147 and S-158 returned HTTP 403) or because the item is a working paper whose publisher
  pages are paywalled. Those entries say so explicitly, and their load-bearing numbers are either
  confirmed by a directly fetched abstract (S-146 via the NBER page; S-171 and S-172 via the arXiv
  API) or corroborated by a second independent peer-reviewed source.
- **Two pre-publication numbers were deliberately not used as decisive evidence** (S-152's
  sign-flipped versions, S-158's mean-reversion estimates). The register's rule on version drift is
  now stated explicitly in the rediscovery guard.
- **The peer-review status of every source is recorded**, and two of the cycle's most useful
  findings rest on *working papers* (S-147, S-158) or *preprints* (S-171, S-172); the decisions
  were made so that no candidate's status depends on an unrefereed result alone: R-011 rests on the
  peer-reviewed S-146 and S-151, and IDEA-004's re-score rests on the peer-reviewed S-156.
- **No backtest, simulation, data acquisition, metric, or executable artefact was produced**, in
  line with the repository's theory-only scope.

### Cycle 13 outcome

One rank-1 candidate rejected on published evidence (IDEA-001, R-011; V-001 withdrawn); three gaps
closed (G-02/G-07, G-03, and G-05's literature half — the last against a variant); one gap reopened
in part (G-04) and one opened (G-18); two re-scores (IDEA-004 → 69.0, IDEA-009 → 60.0); six
frontier families screened with six bounded negatives and no new dossier; twelve new baselines
registered. The active ranking is now IDEA-011 (72.0), IDEA-003 (71.0), IDEA-004 (69.0),
IDEA-010 (65.0), IDEA-009 (60.0), IDEA-014 (60.0). Handoff rewritten for Cycle 14.

## Cycle 14 — 2026-10-20 — evidence-currency pass on IDEA-011 + gap work

**Objective (per handoff):** Priority (a) evidence-currency check on remaining candidates starting with IDEA-011's post-2010 accounting-adoption drift; (b) attempt to close G-18 (comomentum vs holdings-based crowding); (c) screen frontier families. Also maintain artifacts and rewrite handoff.

**Three-pass task framing (applied):**
- Pass 1: Read handoff/register/shortlist/source ledger/rejected-parked. Identify that IDEA-011 is rank 1 (72.0), evidence base largely pre-2015 (Armstrong/Beuselinck), need post-2010 check. G-18 open (comomentum S-157 vs holdings-based S-026).
- Pass 2: For IDEA-011, search post-2010 literature on IFRS/adoption effects on drift/information diffusion. Found studies showing adoption improves information environment (reduces synchronicity, increases informativeness) and in some cases reduces PEAD magnitude (e.g. K-IFRS adoption reduces PEAD; PEAD declines in IFRS-adopting countries per Hung et al 2015). That suggests diffusion/slow-learning effects may have weakened post-adoption in many settings, similar to decay patterns seen elsewhere.
- Pass 3: Document findings, update artifacts. Also add S-175 (Armstrong et al 2010) reference noted; conduct bounded check on G-18.

**What was done:**
- Added S-175 (Armstrong et al 2010) and S-176 (Beuselinck et al mechanism notes) to source ledger; also S-177 noted (Dew-Becker & Giglio 2025-17, Chicago Fed WP, re IDEA-003 VRP decline).
- Evidence-currency check on IDEA-011: Post-2010 literature (Hung et al 2015, Song & Woo 2015 on K-IFRS/PEAD, Rosmianingrum et al 2023 Indonesia, etc.) generally finds IFRS adoption improves information quality/transparency and reduces information asymmetry; in several markets PEAD magnitude declines post-adoption. This is consistent with the mechanism improving price discovery (reducing slow diffusion) rather than creating persistent drift - suggesting the tradable announcement-to-first-report drift opportunity may have decayed in many jurisdictions post-2010, similar to patterns seen in other families (momentum decay S-156). The candidate's evidence base remains thin post-2010 and the opportunity appears weakened; however the small-sample/adoption-event constraint remains binding. No score change yet pending more targeted review, but the priority question is now sharper.
- IDEA-003 post-2010 check: Located Dew-Becker & Giglio (2025, Chicago Fed WP 2025-17) "The Decline of the Variance Risk Premium: Evidence from Traded and Synthetic Options" (S-177) showing VRP premium for traded options has declined and alphas became indistinguishable from zero in recent years; the aggregate VRP is documented but the harvestability/alpha contribution has weakened - consistent with IDEA-003 state-gate framing but also with decay of the baseline harvest in some periods. No score change; gate remains key.
- IDEA-010/014 screened: IDEA-010 still constrained by commercial AP data (G-16); IDEA-014 (RIN-DEADLINE) has G-15 open (sign unknown). No new evidence found to change status.
- Reviewed G-18: comomentum (S-157, Lou-Polk return-correlation measure) is return-correlation based proxy for arbitrage activity; holdings-based crowding is S-026 (13F). Literature directly comparing correlation-based crowding to holdings-based crowding not found in bounded search - gap remains open (need validation/comparison). G-18 remains open; V-002 must stay on hold until closed.
- Frontier families screened per handoff (crypto unlocks already screened S-170 as documented but no sign-determining state; CA cap-and-trade screened as inert/practically no tradeable effect; TGA/repo screened as published baseline narrowing G-01; ASRs screened out). No new candidate written up.
- Artifacts maintained: source ledger updated (S-175, S-176, S-177 noted), cycle notes updated. Hand off rewrite completed.

**Outcome:** IDEA-011 remains rank-1 but post-2010 evidence suggests adoption improves information environment (reducing drift opportunity). IDEA-003 baseline harvest weakened per recent literature; gate condition more important. G-18 still open. No new candidates. Next: deeper look at G-18 validation possibilities.

## Cycle 15 — 2026-10-20 — G-18 bounded negative; IDEA-011 post-2010 check complete; IDEA-003 gate review complete

**Objective (per handoff):** (a) close or bound G-18 (comomentum S-157 vs holdings-based crowding S-026); (b) deeper post-2010 evidence-currency check on IDEA-011 (PEAD magnitude around IFRS/adoption, enforcement regimes); (c) review implications of Dew-Becker & Giglio (2025 WP 2025-17, S-177) for IDEA-003 state-gate; maintain artifacts and rewrite handoff.

**Three-pass task framing (applied):**
- Pass 1: Read handoff/register/shortlist/source ledger/rejected-parked. Confirmed IDEA-011 rank 1 (72.0), IDEA-003 rank 2 (71.0); G-18 open; V-002 frozen pending G-18.
- Pass 2: Searched G-18 literature and post-2010 IFRS/adoption PEAD evidence; located S-177 (Dew-Becker & Giglio 2025-17), S-178 (Hung–Li–Wang 2015 RFS), S-179 (Song–Woo 2015 K-IFRS).
- Pass 3: Documented findings, updated artifacts, rewrote handoff for Cycle 15.

**What was done:**
- Added S-177 (Dew-Becker & Giglio 2025, Chicago Fed WP 2025-17: traded-option alphas declined to near zero over ~15 years; synthetic options never negative alpha over 100 years; aggregate VRP unaffected), S-178 (Hung–Li–Wang 2015, RFS 28(4): 1242–1277: PEAD declines after reporting-quality improvement, stronger where enforcement/institutional holdings higher and limits-to-arbitrage lower), S-179 (Song–Woo 2015, K-IFRS: adoption reduced PEAD size) to source ledger (S-001…S-179).
- G-18: BOUNDED NEGATIVE. S-157 (comomentum) is correlated with holdings-based proxies (13F ownership, Chen–Da–Huang NAT) but never tests substitutability; no head-to-head validation of correlation-based vs holdings-based crowding located across thirteen cycles. Closest comparison (Dell "Crowding and Factor Returns", SSRN 3803954) finds the position-based measure subsumes the correlation-based proxy. Comomentum is decision-time and free but NOT a validated substitute for S-026. V-002 (IDEA-004) stays frozen; IDEA-004 not re-specified around an unvalidated proxy. G-18 stands as bounded negative, not closed as a validation.
- IDEA-011 post-2010 check COMPLETE: post-2010 literature indicates IFRS-style adoption improves information environment and shrinks PEAD magnitude — evidence *against* a persistent post-2010 announcement-to-first-report drift, analogous to momentum decay (S-156). Score unchanged 72.0, rank 1; hard-stop (small, non-independent adoption-event sample) unchanged. Enforcement regimes: effects concentrated in strong-enforcement countries (S-178, S-175/S-176).
- IDEA-003 state-gate review COMPLETE: S-177 VRP decline consistent with and reinforcing the state-gate framing (harvestability, not the premium's existence, is the claim); gate viable (G-13 PASS, G-12 PASS sign limb, G-05 closed against single-name extension, aggregate untouched). Score unchanged 71.0, rank 2.
- IDEA-010/014: no new evidence to change status (G-16/G-15 open). No new candidate written up.
- Ranked shortlist updated: IDEA-011 and IDEA-003 hard-stop flags annotated with completed post-2010 checks; no score changes.
- Artifacts maintained: source ledger, idea_register dossiers, ranked_shortlist, next_agent_handoff (Cycle 15), cycle_notes.

**Outcome:** G-18 bounded negative (V-002 stays frozen); IDEA-011 remains rank 1 (72.0) with post-2010 decay evidence documented; IDEA-003 remains rank 2 (71.0) with gate reinforced; no new candidates. Active ranking unchanged: IDEA-011 (72.0), IDEA-003 (71.0), IDEA-004 (69.0), IDEA-010 (65.0), IDEA-009 (60.0), IDEA-014 (60.0). Next cycle: re-score/park decision on IDEA-011 given decay evidence; run G-13/G-12 on evidence-changed candidates; confirm V-002 frozen.

## Cycle 16 — 2026-10-20 — re-score / park decision on IDEA-011; G-13/G-12 recorded

**Objective (per handoff):** (a) re-score / park decision on IDEA-011 given completed post-2010 decay evidence; run G-13 and G-12 on evidence-changed candidates (IDEA-011, IDEA-003) and record both verdicts; re-read nearest published test in post-2010 sample before scoring; (b) confirm V-002 remains frozen; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

- Pass 1: Read handoff/register/shortlist/source ledger/rejected-parked. Confirmed IDEA-011 rank 1 (72.0), IDEA-003 rank 2 (71.0); G-18 bounded negative; V-002 frozen.
- Pass 2: Re-read post-2010 evidence (S-178 Hung–Li–Wang 2015 RFS; S-179 Song–Woo 2015 K-IFRS; S-175/S-176 pre-2010 base). Decay evidence indicates IFRS-style adoption improves information environment and shrinks PEAD magnitude — evidence against a persistent, tradable announcement-to-first-report drift post-2010, analogous to momentum decay (S-156); effects concentrate in strong-enforcement countries. Decision: re-score IDEA-011 72.0 → 69.0. G-13 PASS (adoption calendars published years ahead). G-12 PASS on existence limb; size limb narrowed (drift existence depends on information-quality state, but magnitude decays post-adoption). IDEA-003: G-13 PASS, G-12 PASS on sign limb; score unchanged 71.0 (S-177 reinforces gate framing).
- Pass 3: V-002 confirmed frozen (G-18 bounded negative, not a closure); no new candidates added.

**Outcome:** IDEA-011 re-scored to 69.0 (tied with IDEA-004); IDEA-003 unchanged 71.0 (rank 2); V-002 frozen; no new candidates. Active ranking: IDEA-003 (71.0), IDEA-011 (69.0), IDEA-004 (69.0), IDEA-010 (65.0), IDEA-009 (60.0), IDEA-014 (60.0). Next: resolve IDEA-011/IDEA-004 tie; confirm parking decision; maintain artifacts.

## Cycle 17 (2026-10-20)

- Pass 1: Read handoff/register/shortlist/source ledger/rejected-parked. Confirmed tie at 69.0 (IDEA-011, IDEA-004), V-002 frozen, G-18 bounded negative.
- Pass 2: Re-read nearest published test in post-2010 sample (Hung, Li & Wang 2014/2015 RFS; S-178): PEAD declines after IFRS information shock, decrease more pronounced in strong-enforcement countries, driven by firms with greater reporting changes and higher analyst forecast accuracy/institutional ownership/liquidity. Confirms prior re-score; decay is conditional on information-quality improvement, not a null existence limb. Enforcement-regime concentration is a scope condition, not a rejection — drift survives in weak-enforcement/low-information-quality states. Decision: retain IDEA-011 at 69.0 (no parking P-011); tie with IDEA-004 remains under fixed rubric; IDEA-004 retains rank 3 on originality/mechanism clarity, IDEA-011 rank 4 pending validation of enforcement-regime scope. V-002 confirmed frozen (G-18 bounded negative, not closure); no re-specification around comomentum (S-157).
- Pass 3: No genuine new mechanism family surfaced; no new candidate. IDs unchanged (IDEA-015, S-180, V-010, G-19, R-012, P-011 remain available).

**Outcome:** Cycle 17 complete. IDEA-011 retained at 69.0 (rank 4), IDEA-004 69.0 (rank 3), IDEA-003 71.0 (rank 2). V-002 frozen. No new candidates/parkings. Next: resolve tie via rubric re-read of nearest published test; maintain gap work G-01/G-04/G-16.
