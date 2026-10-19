# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading
it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and
`research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the
superseded text is summarised into `research/cycle_notes.md` so the pipeline history survives.

Last updated: 2026-10-19, end of Cycle 2 plus two closure passes · Cycle 2 closed · Next cycle:
Cycle 3

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | 7 dossiers (IDEA-001 … IDEA-007) — 4 listed US equities, 3 outside them; **two narrowed to v1.1 after their own literature was read** |
| Ranked shortlist | 7 ranked, scored out of 100 (76 / 74 / 72 / 71 / 64 / 63 / 59) |
| Source ledger | **81 verified sources (S-001 … S-081)**, 11 source gaps (G-01 … G-11); **G-09 and G-10 both MOSTLY CLOSED**, G-11 newly opened |
| Validation hand-offs | 6 specifications (V-001 … V-006); V-004 required by the top-three rule, V-005 and V-006 released only as residual tests, V-006 also blocked on G-11 |
| Rejected / parked | **7 rejected (R-001 … R-007)**, 7 parked (P-001 … P-007), 15-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged, must stay unchanged** |
| Validation performed | **None.** No candidate has been tested; no number here is a performance estimate. |

Cycle 1 built the pipeline and four candidates in one family (listed US equities). Cycle 2 moved
the register into two new venue families, produced three new dossiers, re-ranked everything, and
attempted the four bounded supporting tasks. **The most important Cycle-2 output is not a
candidate but a finding: the state-proxy problem that blocks IDEA-002 and IDEA-004 is largely a
*venue-selection* problem.** IDEA-002's mechanism is testable in FX (IDEA-007) because the dollar
funding state is published; IDEA-004's crowd-state idea is testable in futures (IDEA-005) because
the regulator publishes the passive positions. The next cycle should search for candidates in
venues where the state is *already published by an institution*, rather than continuing to hunt for
proxies.

**The two closure passes are the second-most-important Cycle-2 output, and they went against the
register.** Reading the closest published work twice demoted **two of the register's own
candidates**:
- **G-10 (IDEA-007).** The aggregate funding-constraint-state → carry-return relation is
  **published, peer-reviewed and positive** (Filipe, Nissinen & Suominen 2023, S-055). The
  aggregate version was rejected (R-006); IDEA-007 was narrowed to v1.1 and now claims only the
  *cross-sectional* and *publication-timing* residual. A second, scoped negative finding: **no
  published cross-currency basis series exists in the BIS statistics catalogue** — the slow state
  is published, the fast one must be built from quotes.
- **G-09 (IDEA-006).** The fix-window price effect is **published** — the temporary,
  end-of-month-concentrated impact of passive hedging demand at the fix (S-075), the negative
  serial correlation around it (S-076), the negative pre/post-fixing autocorrelation (S-077), the
  elevated volatility around 4pm (S-074) and the W-shaped dollar pattern around global fixings
  (S-081). The aggregate version was rejected (R-007); IDEA-006 was narrowed to v1.1 and now
  claims only the *settlement-side* residual and the post-2015 persistence question, and its score
  fell from 66 to 59. **The fix is now a known baseline.**
- **Process finding.** A read-only verification agent returned **three wrong identifiers and one
  paper that does not exist** ("Rime, Sarno & Sojli — *Exchange rate forecasting and the New York
  close*, JFI 19(1)" — a phantom; the correct DOI is for Bruno & Claessens on corporate
  governance). Every identifier was re-derived against Crossref/arXiv/NBER before use, and the
  errors are recorded in the ledger's G-09 entry. Separately, a registered 2026 working paper
  (S-081) was found to have a **fabricated 39-item bibliography**; none of its references may be
  cited. **Never enter an agent-supplied citation without re-deriving it yourself.**

### Candidates in one line each
- **IDEA-001 RECON-FLOW (rank 1, 76)** — announcement-timed, flow-scaled reconstitution pressure
  with a post-effective reversal leg. *Documented effect, conditional refinement.* Best first
  **test**, weakest **discovery**.
- **IDEA-004 SLOWCAP-COND (rank 2, 74)** — convergence trades conditioned on observable crowd
  depth, with a predicted non-monotone relation. Strongest **new mechanism**.
- **IDEA-005 ROLLCOND (rank 3, 72)** — the scheduled commodity-index roll buys a liquidity
  concession that survives only where the passive share of open interest is high and depth is
  thin; the state is the CFTC's published Index Trader positions. *Contested published effect,
  state-conditioned, provider-side.*
- **IDEA-003 VRP-STATE (rank 4, 71)** — the variance risk premium is crash-state compensation;
  harvest it only behind an ex-ante crash-state gate. *Known baseline, state-conditioned.*
- **IDEA-007 FUNDSTATE-FX (rank 5, 64)** — the dollar funding-liquidity channel in FX, with the
  *cross-section* of dollar-funding dependence as the claim and the published banking statistics
  as the state. *The aggregate version is a published baseline (S-055, rejected as R-006); the
  dossier now claims only the cross-sectional and publication-timing residual (v1.1).*
- **IDEA-002 FUNDSTATE (rank 6, 63)** — funding cost as a state variable for flow-driven impact
  asymmetry. Blocked on a proxy (G-01); **park, do not re-specify** — Cycle 2 shows the same
  mechanism works in a venue where the state is published (IDEA-007).
- **IDEA-006 FIXCLOCK (rank 7, 59)** — the end-of-day deadline cluster and the concession the
  clock rents. *The fix's price impact is published (S-075, S-076, S-077, S-074, S-081, rejected
  as R-007); the dossier now claims only the settlement-side residual and the post-2015
  persistence question (v1.1), and it is **blocked on G-11**.*

---

## 2. Highest-priority unresolved theoretical questions

**Blocking originality checks — each can kill a candidate, and both are cheap to close.**
These are now the highest-value work in the pipeline.

1. **G-06 — is IDEA-005's concession just a commodity basis-convergence trade with a calendar
   catalyst?** The commodity basis-convergence literature was not retrieved in Cycle 2. If the
   roll-period concession is a plain convergence-to-carry trade, IDEA-005 must be reclassified as a
   variant of a known baseline; if the *cross-sectional* state condition is already published,
   IDEA-005's novelty claim collapses. Until G-06 is closed, IDEA-005 must be described as
   "state-conditioned refinement of a contested published effect", never as a discovery. **This is
   the last untouched blocking check on the register's newest candidate and should be closed
   first.**
2. **G-11 — has anyone tested the *settlement-side* deadline cluster as a price determinant?**
   The G-09 closure established that the **fix** half of IDEA-006's cluster is published
   (S-075, S-076, S-077, S-074, S-081), but the search covered the fix literature, not the
   settlement side: the CLS currency-close and pay-in deadlines, and the post-US-close window
   that the May 2024 T+1 transition created (S-048, S-049). The distinction is real — the fix is
   a *price-setting* event whose participants must trade at a published price, whereas the
   settlement deadlines are *funding* constraints that generate price-insensitive demand in a
   window that is not a benchmark. **IDEA-006 v1.1 is blocked on this.** If a published paper
   already shows a settlement-side price effect, the candidate is rejected, not narrowed. Note the
   asymmetry that must be respected: the fix literature is dense and partly built on
   administrator- and dealer-provided tick data, so "nobody has looked at the settlement side"
   has to be earned with the same rigour, not assumed from the density of the fix papers.

**One residual check left over from the first closure pass (narrow, cheap, and it can kill a
candidate).**

3. **G-10 residual — is the *cross-sectional* funding-state claim already published?** The closure
   pass read the funding-currency, cross-currency-basis, global-liquidity and carry-crash
   literature (S-055 … S-073) and did **not** find a published cross-sectional result: that the
   currencies whose borrowers depend most on dollar funding respond most to a dollar funding
   expansion, conditional on the interest differential. That negative finding is scoped to the
   corpus read, so it is a search result, not a proof. The residual check is to look for it in the
   FX cross-section and currency-return literature specifically. **If it is found, IDEA-007 is
   rejected, not downgraded** — the register would then hold no FX candidate at all, and the
   state-proxy/venue-selection lesson would still stand, but on a different mechanism.

**Substantive questions, in priority order.

4. **Is the crowd-depth conditioning in IDEA-004 non-monotone?** Prediction: convergence returns
   are higher at moderate crowding than at low crowding (deviations persist because capital is
   slow) and lower at high crowding (the edge is competed shut), while tail severity rises with
   crowding. If the relation is monotone and negative, IDEA-004 collapses into the known
   "avoid crowded trades" baseline and must be reclassified.
5. **Does the announcement-to-effective drift in IDEA-001 scale with the size of the required
   passive flow**, rather than with "being in the index"? A quantitative, publicly checkable
   prediction that separates price pressure from anticipation and awareness. **G-02 is not
   closed** — there is no verified benchmark-specific passive-asset series; G-07 records it.
6. **Is the variance risk premium only harvestable outside crash-imminent states**, and can the
   gate be computed from the option surface alone? G-05 is only *partially* closed: the post-2010
   option-market structure is characterised (S-043), and the exchange's own estimate is that net
   dealer gamma is de minimis, but the single-name insurance channel is not settled.
7. **Does IDEA-005's concession survive the post-2012 boundary in the thin, high-passive-share
   contracts?** The published aggregate result says the roll's spread impact *disappears* in
   2012–2019 (S-033); IDEA-005's claim is that this is a composition effect of deep contracts.
   This is the decisive experiment of the Cycle-2 family.
8. **Did the published fix effect survive the 2015 reform?** The calculation window was widened
   from one minute to five on 15 February 2015 (S-045, S-046), and the benchmark was the subject
   of a regulatory and enforcement cycle (S-044). The price-effect literature located in the G-09
   pass largely predates the reform or does not price it (S-075, S-076, S-077), while the
   post-revision benchmark-quality work exists (S-080). If the effect is unchanged across the
   break, then IDEA-006's residual has no *new* state condition to trade, and the candidate should
   be killed rather than re-scoped. This is the second half of IDEA-006 v1.1's claim.
9. **What is a defensible public proxy for a latent state variable in general?** Cycle 2 answered
   part of this (see section 3 of `ranked_shortlist.md`, note 1), but the *methodological note*
   itself — how to choose, build and validate a state proxy, and when to abandon a candidate
   because no proxy exists — **has still not been written down**. Doing so is cheap and would serve
   every future candidate.
10. **Does the *level* of forward points predict the future *level* of forward points, in a state
    constructed from public data?** This is the lead the first closure pass produced: the BIS
    statistics catalogue contains **no published cross-currency basis series** (a scoped negative
    finding recorded under G-10), and the published funding-constraint studies build the state
    from paid vendor forwards (S-055). A candidate that must *construct* the fast state from public
    quotes is unattractive; a candidate whose claim is that the **level** of a market-implied state
    predicts its own future level — a state-continuation claim rather than a flow-claim — is a
    different object, is adjacent to what the published literature does *not* test, and is cheap
    to specify. It is a lead, not a candidate: it has not been searched, and it must first be
    checked against the FX predictability literature, which is dense.

---

## 3. Next distinct mechanism families to investigate (not yet in the register)

Cycle 2 covered: forced/dated flows in commodities (IDEA-005), the end-of-day deadline clock in FX
(IDEA-006), and the funding-currency channel in FX (IDEA-007). The families below remain open.
They are suggestions with reasons, not quotas — a cycle that produces one excellent candidate from
an unlisted family is better than four weak ones from these. **Weigh each candidate by the
Cycle-2 lesson: prefer venues where the state variable is published by an institution.**

1. **Corporate credit: index and ETF flow against dealer balance-sheet capacity** — the credit
   version of IDEA-002 in a market where dealer capacity and passive flow both matter and where
   issuance calendars are explicit. *Why now:* it is the one Cycle-1-recommended family still
   untouched, and credit has published calendars (issuance, index rebalances) and, since the
   CFTC's dealer position reporting rules, published positions.
2. **Securities lending, short-sale constraints and recall-driven forced selling** — a family in
   which a *borrow* constraint rather than a flow drives the price. The constraint is observable
   (borrow availability, recalls, and now securities-lending and short-position disclosures).
   *Why now:* it is the one mechanism family in which the state is a *documented, disclosable*
   operational fact rather than a latent variable.
3. **Crypto: the perpetual-futures funding rate as a daily-settled, published funding state** —
   the funding rate is settled every few hours, published by the exchanges, and is a direct
   measure of the crowded-leverage state. *Why now:* it is the clearest possible instance of
   "the state is published by the venue", which is the Cycle-2 selection rule; it also leaves the
   operator's stated experience area (breakouts) while using a different mechanism (funding, not
   breakout structure). The evidence base is thinner and the venue risk is real; both must be
   stated honestly.
4. **Slow information diffusion with an identifiable event clock** — distinct from the attention
   baseline (S-027): the staggered, published adoption dates of accounting standards (each
   filer's own fiscal-year date) create a dated, cross-sectional read-across in which the market
   learns the new numbers from the early adopters. *Why now:* it is the last Cycle-1-recommended
   family still untouched, and the event clock is published years in advance.
5. **Settlement and payment infrastructure as a dated flow** — the continuation of IDEA-006's
   vein: the T+1 transition, the CLS settlement deadlines, and the currency funding that must
   follow them, as a *structural* (not intraday) candidate with a documented schedule. *Why now:*
   IDEA-006 identified the mechanism but could not measure the price effect; a structural version
   may be measurable with public data.

---

## 4. Best next research task (Cycle 3)

> **Close the two remaining blocking originality gaps (G-06, G-11) and the narrow G-10 residual —
> each can kill a candidate — and then produce 2–3 new dossiers in mechanism families not yet in
> the register, chosen by the Cycle-2 rule that the decision-time state variable must be *published
> by an institution*.**

Concretely, Cycle 3 should:

1. **Close G-06, G-11 and the G-10 residual first** (literature verification only; no new
   candidates needed). For each, read the closest published work, add a ledger entry with how it
   was verified, and then **update the affected dossier's originality section** with the result —
   including *reclassifying a candidate if the gap closes against it*. Record the outcome in
   `rejected_and_parked.md` if a candidate does not survive. The two closure passes of Cycle 2
   are the precedent: reading the literature **demoted two of the register's own candidates**
   (IDEA-007 to v1.1 with R-006; IDEA-006 to v1.1 with R-007, score 66 → 59), and that was
   worth more than two new weak dossiers. A cycle that closes three gaps and kills or narrows one
   candidate is worth more than a cycle that adds three weak dossiers.
   **Method rule carried forward from the closure passes: re-derive every identifier yourself.**
   A read-only verification agent produced three wrong DOIs and one non-existent paper in the
   last pass, and one registered working paper (S-081) was found to have a fabricated
   bibliography.
2. **Choose the frontier** from section 3 (or a better one you can justify), and state the choice
   and the reason in `cycle_notes.md` *before* generating candidates. Apply the three-pass
   task-framing loop and record it.
3. **Search primary sources** for the participant and constraint — venue, regulator, benchmark
   administrator and settlement-utility documentation, plus primary academic work — and verify
   every citation exactly as Cycle 2 did (S-029 … S-054 set the standard: full reference, DOI/URL,
   type, what it supports, caveat, and **how it was verified**, including how a document was read
   when a publisher's bot protection blocked a direct fetch).
4. **Write 2–3 dossiers** in the same field structure as `idea_register.md`, each with an explicit
   **honest classification** against the whole register and the known-baseline table, and each with
   a **state-variable line that says who publishes it and on what calendar**.
5. **Write the state-proxy methodological note** that Cycle 1 and Cycle 2 both deferred (question 8
   above) — as a closing section of `research/idea_register.md`, so it stays with the candidates it
   governs. It should answer: how to choose a state proxy; how to build it without look-ahead;
   how to validate it against an independent measure; and when the honest answer is "no public
   proxy exists — park the candidate rather than re-specify it".
6. **Red-team and rank** with the fixed rubric, adding the new candidates to `ranked_shortlist.md`
   with per-score justification and hard-stop flags, and re-check the existing ranks (the new
   candidates may legitimately displace them).
7. **Add validation hand-off specifications** (V-007 onward) for any new candidate that reaches the
   top three, in the same structure as `validation_handoffs.md`.
8. **Update this handoff** with the new state, the new best next task, and a fresh initial task
   message for the following agent.

**Bounded supporting tasks** (each closes a named gap; do these *in addition*, not instead of the
main work):

- **T5 (G-03 / G-08):** determine whether the passive equity flow concentrates in the closing
  auction, using exchange-published closing-auction volume statistics. This decides whether
  IDEA-001's premise (trade at the effective close) is a fact or an assumption.
- **T6 (G-01):** write the composite funding-state specification for IDEA-002 (SOFR and the GC
  repo rates, S-041; standing-repo-facility take-up and the primary dealer statistics, S-042) and
  state precisely what validation against disclosed dealer funding value adjustments would require.
  If that validation is impossible with public data, keep IDEA-002 parked and say so.
- **T7 (G-05, single-name side):** establish whether the single-name option market's post-2010
  structure changed the size of the insurance-demand channel; S-043 characterises the index side
  only.
- **T8 (G-07):** find a defensible benchmark-specific passive-asset series (or demonstrate that
  none is published), and record the verdict. This blocks IDEA-001's flow-scaling test (V-001).

---

## 5. Operating rules for the next session

1. **Read this file first.** Then the register, the shortlist, the source ledger, and the rejected
   log before generating anything.
2. **Theory only, absolutely.** No backtests, no data acquisition or processing, no executable
   strategy code, no performance metrics, no parameter sweeps, no jobs, no workflow/test/infra
   edits, no cross-repository work, no trading. If a question can only be answered by running
   something, write the question down and hand it off — that is the correct output, not a failure.
   *Note: the mission prompt permits reading and summarising literature and market-structure
   documentation; that is what source verification is, and it is the only external action taken in
   Cycle 2 as well as Cycle 1.*
3. **Do not modify** `research_prompts/systematic_edge_discovery_agent_prompt.txt`.
4. **Preserve prior work.** Add, do not delete or renumber. New IDs: `IDEA-008`+, `S-082`+,
   `V-007`+, `G-12`+, `R-008`+, `P-008`+, and call the next cycle `Cycle 3`. (R-001 … R-007,
   S-001 … S-081, V-001 … V-006 and G-01 … G-11 are already in use.)
5. **Never invent a citation — and never accept one unverified.** Every external claim points to
   a ledger entry; every ledger entry records how it was verified, and **every identifier must be
   re-derived from the publisher, Crossref, arXiv, NBER or the institution's own site**, because
   the last verification agent returned three wrong DOIs and one paper that does not exist. Also
   treat an agent-supplied *bibliography* as unverified: one registered working paper (S-081) has a
   fabricated 39-item reference list, and none of its references may be cited. Unverifiable claims
   are labelled conjectures and become source gaps.
6. **Locate the contradicting evidence deliberately.** Cycle 2's rule, and it changed the outcome:
   for every candidate, find the peer-reviewed work that *contradicts* it and record it in the
   dossier. A candidate whose contradiction has not been searched for is not ready to be ranked.
7. **Scores are research priority, not success probability.** No numerical probability of profit.
8. **Update this handoff last**, and keep the initial task message below current and self-contained.

---

## 6. Environment observations (reported, not actioned — outside the agent's scope)

These are maintainer items. The mission prompt forbids the agent from changing workflow files,
tests, credentials or execution infrastructure, so they are recorded here for the operator and
were deliberately not acted on. **Carried forward from Cycle 1 and not re-verified in Cycle 2.**

- The workflow `.github/workflows/main.yml` references `scripts/controller_progress.py` (used to
  decide whether a session produced meaningful repository progress) and four test modules under
  `tests/`. **None of these exist in the repository.** The most recent completed run recorded in
  `research_state/workflow_run_diagnostics.jsonl` (run id 39263963610, head sha `e3fa662`) failed
  with `file or directory not found: tests/test_controller_progress_accounting.py` and
  `TEST_OUTCOME: failure`.
- Consequence to be aware of: because `scripts/controller_progress.py` is missing, the
  controller's project-progress accounting cannot succeed even when a checkpoint is committed and
  pushed, so a run can report "no meaningful repository change" and exit non-zero despite the work
  being durably persisted. The work itself is still committed by the controller and pushed — check
  `git log` and the remote SHA rather than the job conclusion.
- A workflow-file push is a diagnostics-only activation; the worker loop runs on schedule and on
  `workflow_dispatch`.

---

## 7. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. This is a research-prioritisation
environment only.

1. Read the durable handoff at research/next_agent_handoff.md first, then
   research/idea_register.md, research/ranked_shortlist.md,
   research/source_ledger.md and research/rejected_and_parked.md. Do not
   regenerate what already exists and do not renumber or delete existing IDs.

2. Execute the best next research task stated in section 4 of the handoff. The
   first and highest-value part is closing the remaining originality gaps by
   reading the closest published work and recording it in the source ledger:
   G-06 (the commodity basis-convergence literature, for IDEA-005), G-11 (has
   anyone tested the settlement-side deadline cluster - the CLS currency-close
   and pay-in cut-offs and the post-US-close window created by T+1 - as a price
   determinant rather than as an operational schedule, for IDEA-006) and the
   G-10 residual (whether the cross-sectional funding-state claim is already
   published, for IDEA-007). Each of these can kill a candidate, so update the
   affected dossier's originality section with the result and reclassify,
   narrow or park the candidate if the gap closes against it. The two Cycle-2
   closure passes are the precedent to follow: they demoted two of the
   register's own candidates (IDEA-007 to v1.1 with R-006; IDEA-006 to v1.1
   with R-007, score 66 -> 59) and produced a new gap (G-11) in the process.
   Then produce 2-3 new dossiers in mechanism families not yet in the register,
   choosing families where the decision-time state variable is published by a
   venue, regulator, benchmark administrator or settlement utility. Each dossier
   must name the participant, the binding constraint, a decision-time-observable
   state variable (with who publishes it and on what calendar), a dated or
   state-dependent flow, the expected return source, an honest originality
   comparison against the whole register and the known-baseline table,
   falsifiable predictions with explicit rejection conditions, confounders, data
   requirements, a theory/evidence status, and verified sources. Also write the
   state-proxy methodological note that both previous cycles deferred, as a
   closing section of research/idea_register.md, and attempt the bounded
   supporting tasks T5-T8, recording any gap you cannot close as a new source
   gap.

3. Apply the three-pass task-framing loop (draft, critique, revise and
   red-team) before the research cycle and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file at
   research_prompts/systematic_edge_discovery_agent_prompt.txt.

4. Rank the new candidates with the fixed rubric in
   research/ranked_shortlist.md (re-checking the existing ranks, which the new
   candidates may legitimately displace), write validation hand-off
   specifications for any new candidate reaching the top three (V-007 onward,
   same structure as research/validation_handoffs.md), and log anything
   rejected or parked in research/rejected_and_parked.md with the reason.

5. Absolute scope boundary: theory and discovery only. Do not run or
   commission backtests, simulations, parameter sweeps, significance tests on
   strategy results or any performance calculation. Do not download or process
   market data, build a research notebook, implement a strategy, write a
   signal generator or any executable research infrastructure, or launch any
   job, workflow or CI run. Do not change workflow files, tests, credentials or
   infrastructure, and do not touch other repositories. You may read public
   literature, venue and regulator documentation, and market-structure
   documentation in order to verify citations. If a question can only be
   answered by running something, document the question precisely and hand it
   off instead of relaxing the boundary.

6. Cite every external claim with a verifiable URL or DOI, and never invent a
   citation. Re-derive every identifier yourself from the publisher, Crossref,
   arXiv, NBER or the institution's own site, and do not accept an identifier
   or a bibliography supplied by a search or research agent: the last
   verification pass produced three wrong DOIs and one paper that does not
   exist, and one registered working paper (S-081) turned out to carry a
   fabricated reference list whose entries must not be cited. Record for each
   source how it was verified, including the cases where a publisher's bot
   protection blocked a direct fetch. Distinguish authors' reported results
   from independently reproduced results, label unresolved claims as
   conjectures, and deliberately search for the evidence that contradicts each
   new candidate. Scores are research-priority weights, not probabilities of
   profit; attach no numerical probability of success.

7. Finish by rewriting research/next_agent_handoff.md: current pipeline state,
   the highest-priority unresolved theoretical questions, the next mechanism
   families to investigate, the open source gaps, the best next research task,
   any environment observations for the maintainer, and a fresh, self-contained
   initial task message for the following agent. Summarise the superseded
   handoff into research/cycle_notes.md.
```

---

## 8. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 1 | 2026-10-19 | First cycle: pipeline created, 4 dossiers, 28 sources, 3 validation specs, 3 rejections, 4 parkings, baseline table, durable handoff established. | Yes. |
| 2 | 2026-10-19 | New venue families: 3 new dossiers (commodity futures, FX fixing clock, FX funding state), 26 new sources, gap verdicts on G-01…G-05 and three new gaps, re-ranked shortlist (7 candidates), V-004 required plus two optional specs, 2 new rejections and 3 new parkings, baseline table extended to 14 rows, venue-selection lesson recorded. | Yes. |
| 2 (closure pass 1) | 2026-10-19 | Funding-currency corpus read and registered (S-055 … S-073); G-10 verdict **MOSTLY CLOSED**; IDEA-007's aggregate version found published and **rejected (R-006)**, dossier narrowed to v1.1; scoped negative finding that no published cross-currency basis series exists; V-005 released only as a residual test; shortlist and baseline table rewritten for IDEA-007. | Yes. |
| 2 (closure pass 2) | 2026-10-19 | Intraday fixing literature read and registered (S-074 … S-081); G-09 verdict **MOSTLY CLOSED**; IDEA-006's aggregate version found published and **rejected (R-007)**, dossier narrowed to v1.1, score 66 → 59 and rank 5 → 7; new blocking gap **G-11** opened; three agent-reported identifiers found wrong and one paper found not to exist; a fabricated bibliography found inside a registered working paper; V-006 narrowed to the residual. | Yes — this file. |
