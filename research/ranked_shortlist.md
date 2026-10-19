# RANKED SHORTLIST — CYCLES 1–2

Scores are a **research-priority heuristic**, not a probability of profit. No numerical probability
of success is attached to any candidate: the retrieved literature offers no defensible, cited base
rate for "ideas of this type that survive out-of-sample validation after costs", so attaching one
would be false precision.

Weighted total = Σ (dimension score × weight) / 5, expressed out of 100.

Rubric weights (fixed by the mission prompt):
Economic mechanism / persistence 25 · Evidence quality and independence 20 · Substantive novelty 15 ·
Falsifiable predictions and clean future test 15 · Resilience to costs, capacity, regime 15 ·
Data availability, simplicity, reproducibility 10.

Cycle 2 added three candidates (IDEA-005, IDEA-006, IDEA-007), all outside listed US equities, and
re-checked the four Cycle-1 candidates against the new material. Cycle 3 added two candidates
(IDEA-008, IDEA-009), both in mechanism families where the decision-time state variable is
published by an institution/venue (securities-lending disclosures and exchange-published funding
rates). No Cycle-1 or Cycle-2 score changed; the reasons are recorded under each candidate.

---

## Table

| Rank | ID | Short name | Mechanism 25 | Evidence 20 | Novelty 15 | Falsifiability 15 | Resilience 15 | Data 10 | **Total /100** | Cycle-1 rank | Hard-stop flags |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | IDEA-001 | RECON-FLOW | 4 → 20.0 | 4 → 16.0 | 2 → 6.0 | 5 → 15.0 | 3 → 9.0 | 5 → 10.0 | **76.0** | 1 (unchanged) | none; premise assumptions unverified (G-03, G-07) |
| 2 | IDEA-004 | SLOWCAP-COND | 5 → 25.0 | 4 → 16.0 | 3 → 9.0 | 3 → 9.0 | 3 → 9.0 | 3 → 6.0 | **74.0** | 2 (unchanged) | none; proxy-validity kill condition (G-04) |
| 3 | IDEA-005 | ROLLCOND | 4 → 20.0 | 3 → 12.0 | 3 → 9.0 | 4 → 12.0 | 3 → 9.0 | 5 → 10.0 | **72.0** | new | effect-may-be-dead condition (S-033); cost-overwhelm condition; G-06 narrowed |
| 4 | IDEA-003 | VRP-STATE | 4 → 20.0 | 4 → 16.0 | 2 → 6.0 | 4 → 12.0 | 3 → 9.0 | 4 → 8.0 | **71.0** | 3 (down 1) | none; tail-concentration warning; G-05 partially open |
| 5 | IDEA-008 | SECURITY-LEND | 4 → 20.0 | 3 → 12.0 | 3 → 9.0 | 3 → 9.0 | 3 → 9.0 | 3 → 6.0 | **65.0** | new | rare-event sample condition; news-confound condition |
| 6 | IDEA-007 | FUNDSTATE-FX | 4 → 20.0 | 3 → 12.0 | 2 → 6.0 | 3 → 9.0 | 3 → 9.0 | 4 → 8.0 | **64.0** | new | carry-channel confound; publication-timing condition; **residual-only after R-006; G-10 mostly closed** |
| 7 | IDEA-009 | PERP-FUND | 4 → 20.0 | 2 → 8.0 | 3 → 9.0 | 4 → 12.0 | 2 → 6.0 | 4 → 8.0 | **63.0** | new | crypto venue risk; momentum-confound condition; venue-transferability condition |
| 8 | IDEA-002 | FUNDSTATE | 4 → 20.0 | 3 → 12.0 | 3 → 9.0 | 3 → 9.0 | 3 → 9.0 | 2 → 4.0 | **63.0** | 4 (down 2) | none; feasibility kill condition (G-01) — **parked, P-004** |
| 9 | IDEA-006 | FIXCLOCK | 4 → 20.0 | 3 → 12.0 | 2 → 6.0 | 3 → 9.0 | 2 → 6.0 | 3 → 6.0 | **59.0** | new (down from 5) | cost-floor condition; proprietary-intraday-data condition; **residual-only after R-007; G-11 partially closed** |

**Cycle-3 rank changes.** IDEA-008 enters at 5 and IDEA-009 at 7, displacing IDEA-007 to 6 and
IDEA-006 to 9. IDEA-002 remains parked (P-004) at 63.0, tied with IDEA-009 but not in the active
ranking because its feasibility precondition (G-01) is open. The parked candidate scoring at the
same level as a new retained candidate is the honest ordering: an unresolved feasibility question
ranks at the same level as a new candidate whose evidence base is thin. The G-09 closure pass
moved IDEA-006 from 5 to 7 (66.0 → 59.0) in Cycle 2; Cycle 3 adds G-11 partially closed and two
new candidates above it.

---

## Rank 1 — IDEA-001 RECON-FLOW (76.0) — *Cycle-1 rank 1, unchanged*

- **Mechanism, causal coherence, persistence (4/5):** The causal chain from provider rules (S-008)
  to scheduled non-price-sensitive demand to a liquidity concession to a partial reversal is
  explicit, and each link is documented by a different body of work. Not 5 because the *differentiated*
  links (flow scaling, capacity asymmetry) are conjectures rather than theory.
- **Quality and independence of supporting evidence (4/5):** Four independent scholarly lines
  (S-001, S-002, S-003, S-004) plus option-market evidence (S-005, S-006, S-007) and primary venue
  rules (S-008). Not 5 because the option-market evidence includes a working paper by authors
  affiliated with the index provider (S-006), and the classic samples predate today's passive scale.
- **Substantive novelty (2/5):** The underlying effect is forty years old and well published.
  What is claimed as new is a conditional, flow-scaled, two-leg specification. This is the lowest
  score in the register and it is deliberately visible: presenting this as a new edge would be false.
- **Clarity of falsifiable predictions and feasibility of a clean test (5/5):** Event dates are
  published in advance by the index provider; the design has no look-ahead risk on the event
  schedule; the flow-size prediction is quantitative; the kill conditions are explicit.
- **Resilience to costs, capacity, financing, adverse selection, regime (3/5):** Per-event capacity
  is small by construction, the reversal leg trades against the same crowd, and the premise depends
  on a trading convention (trade at the effective close) that is not publicly guaranteed (G-03).
- **Data availability, simplicity, reproducibility (5/5):** Public announcements, public index
  weights, public prices. The one missing input — assets tracking the benchmark — is a real but
  addressable gap (G-02, G-07).

**Cycle-2 re-check.** No score change. Cycle 2 did not resolve G-02 (a benchmark-specific
passive-asset series does not exist in the public record; G-07 is opened in its place) or G-03 (the
trading convention remains undocumented; G-03 is re-framed, G-08 opened). The *general* economics
of the family were strengthened rather than the candidate: Cycle 2 established, from the futures
venue, that a scheduled passive flow buys a liquidity concession from the market (S-032, S-034),
which is the same link IDEA-001 relies on. The family-level strengthening does not change IDEA-001's
novelty score, which is capped by the age of the underlying effect.

**Key uncertainties that could change the rank.** If G-03 resolves against the candidate (index
funds no longer trade at the effective close), leg 1 disappears and the score falls toward the
mid-50s. If G-07 cannot be closed, the flow-scaling prediction becomes untestable and the score
falls further. If the effect has been arbitraged away at current passive scale, the candidate is
dead regardless of score.

**Role in the portfolio.** Strongest *first* candidate to validate (cleanest test, published
schedule, cheap falsification), weakest *new* mechanism. It is a good entry point for the pipeline
and a poor engine of discovery.

---

## Rank 2 — IDEA-004 SLOWCAP-COND (74.0) — *Cycle-1 rank 2, unchanged*

- **Mechanism, causal coherence, persistence (5/5):** The deepest theoretical backing in the
  register: a coherent chain from equilibrium slow capital (S-017, S-018, S-019) through mandates
  and reputation (S-020, S-021) to flow-driven momentum/reversal (S-024) and synchronised exits
  (S-022, S-023), with a measurable crowding proxy already in the literature (S-026). The 5 is
  for the mechanism; the *conditioning* is separately scored below.
- **Quality and independence of supporting evidence (4/5):** Independent theory groups (Shin and
  co-authors; He–Xiong; Duffie; Kondor; Abreu–Brunnermeier) and independent empirics (S-025, S-026,
  S-024). Not 5 because the specific two-sided conditioning has no supporting empirical work
  located in this cycle.
- **Substantive novelty (3/5):** The family is textbook; the crowd-depth gate with a *non-monotone*
  conditioning is a genuinely different claim from "avoid crowded trades" (S-026). Modest, but the
  most defensible novelty claim in the register.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  sharp — prediction 1 (non-monotonicity) is a single, decisive test — but the crowd proxy is
  lagged and noisy, and the fundamental-break confounder is not addressed by the rule.
- **Resilience to costs, capacity, financing, regime (3/5):** The hardest candidate to survive
  costs: market-neutral pairs pay twice, carry can exceed the payoff, and the left tail comes from
  the anchor failing, which the rule does not hedge.
- **Data availability, simplicity, reproducibility (3/5):** Prices and the anchor are easy; the
  crowd proxy is the bottleneck (G-04).

**Cycle-2 re-check.** No score change. Cycle 2 found what a *timely, public* crowd-depth proxy
looks like — the CFTC's weekly "Index Traders" positions (S-030, S-031), which is exactly the
measure IDEA-004's conditioning wants, but in a different venue. For equities nothing equivalent
was found, so G-04 stands and the proxy-validity kill condition stands. Two indirect consequences
are recorded rather than scored: (a) IDEA-005 is now a venue in which the *same* crowd-state
question can be tested with public data, which is a research asset, not a score change; and (b)
the S-038 finding that futures-market participant positions do not predict futures risk premia is
a caution about using position data as predictors in general.

**Key uncertainties that could change the rank.** Prediction 1 turning out monotone-and-negative
collapses the candidate into a known baseline and drops it below IDEA-003. Failure to validate the
proxy against a holdings-based crowding measure (S-026) makes it untestable as specified.

**Role in the portfolio.** Strongest *new-mechanism* candidate. This is where discovery value
sits, and it is the candidate the next cycle should deepen.

---

## Rank 3 — IDEA-005 ROLLCOND (72.0) — *new in Cycle 2*

- **Mechanism, causal coherence, persistence (4/5):** The chain is unusually well documented at
  *both* ends: the participant and the constraint are the regulator's own words (S-030: index
  traders replicate an index and roll "from future to future using a fixed methodology"), the
  calendar is the provider's own published rule (S-029), and the economics of a concession paid
  for supplying liquidity to a predictable trade are established (S-032, S-034). Not 5 because the
  *differentiated* link — that the concession survives only where the passive share of open
  interest is high and depth is thin — is a conjecture that no located work tests.
- **Quality and independence of supporting evidence (3/5):** The sourcing is primary and
  independent (a regulator, a provider, and four separate peer-reviewed groups), but the
  *direction* of the evidence conflicts: S-032, S-033, S-034, S-036 and S-037 all cut against a
  naive version of the claim, and the supporting work (S-035) is a non-refereed dissertation with
  a sample ending in March 2010. The 3 reflects a well-documented but contested family.
- **Substantive novelty (3/5):** The family is documented and the *unconditioned* trade is logged
  as rejected (R-004). What is claimed is new: the state (the passive flow relative to liquidity,
  read from the regulator's own Index Trader positions), the *sign* prediction that follows from
  it, the provider-side rather than front-runner-side expression, and the reconciling claim that
  the published aggregate null is a composition effect.
- **Clarity of falsifiable predictions and feasibility of a clean test (4/5):** Strong. The dates
  are published years ahead; the state variable is public with a known five-day lag; the
  cross-sectional prediction is decisive in one test; and the two rival decay channels make
  mutually distinguishable predictions. Not 5 because the state is contaminated by the regulator's
  own caveats and the cross-section is thin in some commodities.
- **Resilience to costs, capacity, financing, regime (3/5):** The passive's own execution cost is
  documented at about three percent per year (S-032), which bounds what can be harvested; capacity
  per contract per roll is small; the trade consumes exactly the liquidity it prices; and the
  effect is documented to have decayed (S-033).
- **Data availability, simplicity, reproducibility (5/5):** Public futures prices, open interest
  and volume; public weekly CFTC reports (S-030, S-031); a public provider methodology (S-029). No
  proprietary input is required.

**Key uncertainties that could change the rank.** If the cross-section is flat — that is, if the
concession does not vary with the passive share of open interest — the candidate is dead and the
published null (S-033) becomes a statement about the whole market rather than a composition effect.
If the concession is uniformly smaller than round-trip cost, the candidate is dead for a different
reason. The blocking originality check is **G-06**: the commodity basis-convergence literature has
not been read, and if the concession is a plain convergence trade with a calendar catalyst, the
candidate must be reclassified.

**Role in the portfolio.** The Cycle-2 *discovery* candidate: a new venue, a new participant, a
public state variable, and a live scientific disagreement that the candidate is designed to
resolve. It is also the register's first candidate whose *kill condition* is published by
independent researchers rather than inferred by the project.

---

## Rank 4 — IDEA-003 VRP-STATE (71.0) — *Cycle-1 rank 3, down 1*

- **Mechanism, causal coherence, persistence (4/5):** Insurance demand → skewed premium → state
  gate is a coherent, well-anchored chain (S-016, S-014, S-012, S-013, S-015). The gate itself is
  an inference, not a theorem, which keeps it below 5.
- **Quality and independence of supporting evidence (4/5):** Strong and independent (S-012, S-013
  from one group; S-014, S-015, S-016 from others). Not 5 because the measure of the premium
  depends on realized-variance estimation, and the "crash compensation" reading is a model-based
  interpretation with a documented rival (a variance risk factor, S-012).
- **Substantive novelty (2/5):** Short variance is a known baseline. The claim is about the
  *gate*, and even that is partly anticipated by S-015. Honest score.
- **Clarity of falsifiable predictions and feasibility of a clean test (4/5):** The gate is
  computable ex ante from option data only, which is a genuine methodological advantage; the
  downside is that the gate must be validated out of sample and the whole result lives in a few
  extreme events.
- **Resilience to costs, capacity, regime (3/5):** Tail concentration, margin that rises exactly
  when the position loses, and a harvest that lives in a handful of crisis events.
- **Data availability, simplicity, reproducibility (4/5):** Aggregate version is data-friendly;
  the single-name version and the post-2010 structural question (G-05) are not.

**Cycle-2 re-check.** No score change, and the displacement to rank 4 is caused by IDEA-005's
entry, not by any new evidence against it. G-05 is now **partially closed** (S-043): the
post-2010 change in option market structure is characterised (same-day expiries from about 5% of
SPX options volume in 2016 to 59–62% in 2025, roughly half retail, about 98% electronically
traded), and the exchange's own estimate is that net market-maker gamma is de minimis. That
*weakens* the alternative worry that the single-name channel has been distorted by 0DTE gamma,
but it does not settle whether the single-name insurance-demand channel changed size — which is
why G-05 remains open on the single-name side and the candidate keeps a 4 on data.

**Key uncertainties that could change the rank.** The decay of the predictive power that S-013
themselves flag, and the possibility that post-2010 option market structure (0DTE) changed the
mechanism's size or sign (G-05).

---

## Rank 5 — IDEA-008 SECURITY-LEND (65.0) — *new in Cycle 3*

- **Mechanism, causal coherence, persistence (4/5):** The causal chain from borrow constraints and
  recall risk to forced covering and a temporary price spike is explicit, and each link is
  documented by a different body of work (S-083, S-084). Not 5 because the *differentiated* links
  (the two-legged reversal specification, the news-confound separation) are conjectures rather
  than theory, and the event is rare (~2% of loans per month in S-084).
- **Quality and independence of supporting evidence (3/5):** S-083 (JFE, 704 citations) and S-084
  (JFE, same issue) are verified and independent; S-085 (SEC 2021) is regulator documentation.
  Not 4 or 5 because the *joint* two-legged liquidity-provision specification has no supporting
  empirical work located in this cycle, and S-084's DOI could not be independently re-derived.
- **Substantive novelty (3/5):** The short-sale-constraints family is well documented (S-083), and
  the "expensive-to-short predicts low returns" effect is the opposite direction. What is claimed
  is new: the recall-driven forced-covering spike on the *long* side, the two-legged and
  time-boxed expression, and the published state (short interest, lending fees). Modest but
  defensible novelty.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions
  are sharp (event spike, state scaling, news confound, cost floor), but the event is rare and
  the recall itself is not published — it must be inferred from fee spikes and volume anomalies.
  Not 4 because the small effective sample makes clean inference difficult.
- **Resilience to costs, capacity, financing, regime (3/5):** The covering is concentrated in
  minutes, so spread and slippage are first-order; capacity per name is small; the fundamental
  news confounder is severe (a recall driven by lost confidence is a directional loss, not a
  liquidity event).
- **Data availability, simplicity, reproducibility (3/5):** Short interest is public but biweekly
  and lagged; borrow fees are commercial; the recall event must be inferred; a fundamental-news
  calendar is needed. No proprietary input is strictly required, but the inference layer adds
  friction.

**Cycle-3 re-check.** New candidate; no prior rank.

**Key uncertainties that could change the rank.** If the news confounder explains the entire
event spike (recalls driven by fundamental re-pricing, not liquidity), the candidate is dead. If
the biweekly lagged short-interest series is too stale to be a decision-time state, the candidate
fails on observability. If the effect cannot be distinguished from noise given the ~2% monthly
event rate, it is untestable as specified.

**Role in the portfolio.** The Cycle-3 *discovery* candidate in a new venue family (equities, but
the securities-lending segment rather than index events). It shares the "dated, price-insensitive
institutional flow" logic with IDEA-005 and IDEA-006 but in the short-sale venue, where the state
(borrow cost/availability) is published by exchanges and lending agents rather than inferred.

---

## Rank 6 — IDEA-007 FUNDSTATE-FX (64.0) — *new in Cycle 2; demoted by Cycle-2 closure pass*

**Cycle-3 rank change:** down from 5 to 6 (displaced by IDEA-008's entry); score unchanged at 64.0.

- **Mechanism, causal coherence, persistence (4/5):** The funding-liquidity channel is modelled
  and supported (S-052), and the state is published (S-054). Not 5 because the cross-sectional
  step — that dependence, not the aggregate, drives the response — is an inference from the
  mechanism, not a result.
- **Quality and independence of supporting evidence (3/5):** The Cycle-2 source closure read the
  funding-currency and global-liquidity corpus (S-052 … S-073), so the evidence base is now
  documented rather than assumed: the mechanism is supported by central-bank staff work (S-052), a
  peer-reviewed version (S-053), the CIP/hedging-demand literature (S-056, S-057, S-059) and
  official crisis documentation (S-058, S-060, S-072). Not 4 or 5 because the *cross-sectional
  claim itself* has no supporting evidence at all — everything cited supports the parent
  mechanism, not the refinement.
- **Substantive novelty (2/5):** **Reclassified in the Cycle-2 closure pass.** The aggregate
  funding-constraint-state → carry-return relation is published, peer-reviewed and positive
  (S-055), and the dollar-funding-liquidity → dollar-forecast relation is published in both
  working-paper and peer-reviewed form (S-052, S-053); the aggregate versions were therefore
  rejected (R-006). What is left is the **cross-sectional** structure and the publication-timing
  test — a narrow, unclaimed residual, not a discovery of the channel. 2/5 is retained, not
  raised, and it is tied for the lowest novelty in the register with IDEA-001: presenting the
  residual as if it were the channel would be false.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  clear, the publication-timing test is clean, and the data are public — but the state is
  quarterly while the market is daily, so the effective sample is small and the cross-section must
  do the work. A further constraint found in the closure pass: the *fast* version of the state
  (the cross-currency basis) is not published anywhere and must be built from market quotes.
- **Resilience to costs, capacity, regime (3/5):** Slow horizon and liquid instruments are
  favourable; the tail (the funding-contraction state is the carry-crash state) is not, and
  emerging-market currencies — the most funding-dependent — are the least liquid and the least
  two-way borrowable.
- **Data availability, simplicity, reproducibility (4/5):** All inputs are public and published on
  a known calendar (S-054); no proprietary data is required.

**Cycle-2 closure re-check.** G-10's verdict is **MOSTLY CLOSED**: the aggregate version of this
candidate is a published baseline (R-006), and the dossier has been narrowed (v1.1) to the
cross-sectional and publication-timing residual only. The score is unchanged at 64.0, but its
*composition* has changed: the evidence is now stronger and better sourced while the novelty is
now demonstrably confined to a narrow residual. That is a demotion in substance and a wash in
arithmetic, and the ranking should be read accordingly.

**Key uncertainties that could change the rank.** Whether the cross-sectional structure exists at
all; whether it survives the carry-channel control (the published result claims separation, but
that claim must be re-verified in any validation); and whether the slow edge exceeds financing
and turnover costs. If the cross-section turns out to be published, the candidate is not
downgraded — it is **rejected**, and the register would hold no FX candidate at all.

**Role in the portfolio.** The register's *novelty-closure* exhibit: it demonstrates that
IDEA-002's mechanism is testable in a venue where the state is published, which is the Cycle-2
answer to the state-proxy question, and it demonstrates the closure process demoting the
register's own candidate when the literature turns out to already contain the result. It is a
candidate, but a weakly novel one with a narrow residual.

---

## Rank 7 — IDEA-009 PERP-FUND (63.0) — *new in Cycle 3*

- **Mechanism, causal coherence, persistence (4/5):** The causal chain from the exchange-published
  funding rate to the crowded-leverage state to the forced unwind and basis mean reversion is
  explicit, and the funding-rate mechanism is documented by the exchanges and by academic work
  (S-086, S-087). Not 5 because the *differentiated* links (the funding-rate-level reversal
  specification, the separation from momentum feedback) are conjectures rather than theory, and
  the crypto venue carries venue-specific risks.
- **Quality and independence of supporting evidence (2/5):** S-086 (arXiv:2212.06888) and S-087
  (Wharton working paper) are verified, but the literature base is thin; S-088 (SSRN) and S-089
  (Blockchain Research and Applications, 2026) are preprints or recent publications with
  author-reported results not reproduced here. Not 3 because the *joint* reversal specification
  has no supporting empirical work located in this cycle, and several sources are pending
  re-verification of identifiers.
- **Substantive novelty (3/5):** The funding-rate mechanism and the funding-rate arbitrage are
  published (S-086, S-087). What is claimed is new: taking the side opposite the funding-rate
  crowd as a reversal trade keyed to the funding-rate *level* (not the basis), with a pre-specified
  exit after a few funding periods. Modest but defensible novelty.
- **Clarity of falsifiable predictions and feasibility of a clean test (4/5):** The predictions
  are sharp (reversal, state scaling, funding-carry contribution, venue transferability, cost
  floor), the state is published with zero lag every funding period, and observations are
  frequent (every 8 hours). Not 5 because momentum feedback (past returns predict basis
  deviations with R² above 50% in S-086) is a severe confound that must be separated.
- **Resilience to costs, capacity, financing, regime (2/5):** Crypto venue risk (custody, exchange
  risk, 24/7 trading) is real and unquantified; the position's own funding cost moves with the
  same state variable that generates the signal (a self-referencing hazard); large altcoins have
  thin books; spread and slippage accumulate on frequent intraday trades.
- **Data availability, simplicity, reproducibility (4/5):** All inputs are published by the venue
  with zero lag (funding rates, prices, open interest, volume); no proprietary input is required.
  Venue risk is the constraint, not data availability.

**Cycle-3 re-check.** New candidate; no prior rank.

**Key uncertainties that could change the rank.** If momentum feedback explains the apparent
reversal (high funding rates coincide with upward momentum that continues), the candidate is
dead. If the effect is exchange-specific (a venue artefact rather than a mechanism), it fails
the venue-transferability test. If crypto venue risk (custody, exchange failure, funding-cadence
changes) makes the trade unexecutable at scale, the candidate fails on resilience.

**Role in the portfolio.** The Cycle-3 *venue-selection* exhibit: the funding rate is the
clearest possible instance of "the state is published by the venue", which is the Cycle-2
selection rule. It shares the "crowded-position unwind" logic with IDEA-008 (recall-driven forced
covering) but in a derivatives venue with a zero-lag published state. It also leaves the
operator's stated crypto breakout experience area while using a different mechanism (funding, not
breakout structure) — which is honest about the departure, not a return to the parked breakout
family (P-001).

---

## Rank 8 — IDEA-002 FUNDSTATE (63.0) — *Cycle-1 rank 4, down 2; parked*

- **Mechanism, causal coherence, persistence (4/5):** The chain is coherent and each link is
  well-founded (S-009, S-010, S-011); the joint link is conjectural.
- **Quality and independence of supporting evidence (3/5):** Excellent components, but no located
  work on the *combination*, and the proxy's validity is unestablished (G-01).
- **Substantive novelty (3/5):** A synthesis of three established literatures around a state
  variable that does not appear in any of them. Novel enough to be interesting, not established as
  unclaimed.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  clear; volatility is a severe confound; the proxy is the obstacle.
- **Resilience to costs, capacity, regime (3/5):** The strategy consumes exactly the liquidity it
  is trying to measure, and its own financing cost moves with the state that generates the signal.
- **Data availability, simplicity, reproducibility (2/5):** The binding constraint. Order-flow data
  are obtainable; a defensible public funding-state proxy is not currently identified (G-01).

**Cycle-2 re-check.** No score change; the rank is 8 because two candidates were added above it
in Cycle 3 (IDEA-008 at 65.0 and IDEA-009 at 63.0, tied on score but not parked). IDEA-002
remains **parked** (P-004): G-01 was **narrowed, not closed**: four public funding-state
ingredients were verified (SOFR and the related GC repo rates, S-041; standing-repo-facility
take-up and the primary dealer statistics, S-042), but the *validation target* — a published,
continuous series of dealer funding value adjustments — still does not exist in the public
record, so the candidate cannot yet be tested as specified. The parking therefore stands.
**IDEA-002 and IDEA-009 are tied at 63.0; IDEA-002 is parked, IDEA-009 is retained.** The honest
ordering: an unresolved feasibility question parks a candidate even when its score matches a
retained one.

**Key uncertainties that could change the rank.** If G-01 cannot be closed, this candidate should
remain **parked, not re-specified** — re-specifying it around a weaker proxy would convert a good
idea into a disguised baseline. Cycle 2's IDEA-007 makes the reason sharper: the *same mechanism*
is testable in FX because the state is published there, which is an argument for changing venue
rather than for weakening the proxy.

---

## Rank 9 — IDEA-006 FIXCLOCK (59.0) — *new in Cycle 2; demoted by the G-09 closure*

**Cycle-3 rank change:** down from 7 to 9 (displaced by IDEA-008 and IDEA-009); score unchanged at
59.0.

- **Mechanism, causal coherence, persistence (4/5):** The deadline chain is documented by three
  independent institutional bodies — a global regulator (S-044), the benchmark administrator
  (S-045) and the settlement utility (S-048, S-049) — and the flow's concentration is quantified
  by the FSB (over 10% of a platform's daily volume in the fix window on some days for some
  currencies). Not 5 because the link from a documented deadline to a *price* concession is now
  documented for the fix but remains an inference for the settlement-side deadlines, which are
  the candidate's residual.
- **Quality and independence of supporting evidence (3/5):** Down from 4 after the G-09 closure.
  The evidence base is now genuinely strong — five independent lines on the fix effect (S-075,
  S-076, S-077, S-074, S-081), the institutional documentation (S-044, S-045, S-046, S-048,
  S-049) and a post-revision benchmark study (S-080) — but every one of them supports the
  *parent* effect, not the candidate's residual claim, and the settlement-side literature has not
  been searched at all (G-11). Not 4 or 5 for that reason.
- **Substantive novelty (2/5):** **Reclassified by the G-09 closure.** The headline claim — a
  price-insensitive, deadline-driven flow that moves the price at the fix, temporarily, and
  reverses — is published (S-075, S-076, S-077, S-074, S-081), and the aggregate version was
  rejected (R-007). What is left is the settlement-side extension and the post-2015 persistence
  question: narrow, and not yet cleared of the literature (G-11). 2/5 ties for the lowest novelty
  in the register with IDEA-001 and IDEA-007, and it is deliberately visible.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  stated, the published fix result is available as a baseline to reproduce, and a no-macro-release
  discriminator exists; but the test requires proprietary intraday order-book data, the published
  literature's own datasets are administrator- and dealer-provided (S-074, S-076, S-080), and a
  daily-data substitute would measure a different object.
- **Resilience to costs, capacity, regime (2/5):** The weakest dimension in the register alongside
  IDEA-002: the concession is measured in pips inside a few minutes, so spread and slippage are
  first-order; the flow may already be arbitraged by the liquidity providers who are stationed
  there by construction; and the 2015 widening of the calculation window from one minute to five
  may have diluted the very effect the candidate was built on.
- **Data availability, simplicity, reproducibility (3/5):** The clock is public; the flow
  measurement is not. The benchmark administrator's own tick data is not freely available (S-047,
  S-080).

**Cycle-2 closure re-check (G-09).** The verdict is **MOSTLY CLOSED**, and it went against the
candidate: the fix's price impact is published (S-075, S-076, S-077, S-074, S-081), the aggregate
version was rejected (R-007), and the dossier was narrowed to v1.1. The score falls from 66.0 to
59.0 — evidence 4 → 3 and novelty 3 → 2 — because the closure found the effect published, and
because the residual it leaves behind is unsearched (G-11). The seven-point fall is the largest
single-cycle change in the register, and it is the process working as intended.

**Key uncertainties that could change the rank.** Whether the settlement-side deadlines have any
separable price effect at all (G-11, on which the candidate is blocked — G-11 is now *partially
closed*: settlement-side mechanics are a priced friction per S-082 and S-071, but the specific
CLS deadline cluster / T+1 post-US-close window remains untested); whether the published fix
effect survived the 2015 methodology revision, which would remove the need for any new state
condition; and whether any of it is harvestable after costs by a participant who is not already
stationed at the fix. If G-11 closes against the candidate, it is rejected, not re-scored.

**Role in the portfolio.** No longer a structural candidate in its own right: it is now a *narrow
residual* attached to a published effect, blocked on a literature check. Its value in the register
is now the second demonstration of the closure process (after IDEA-007), and the register's only
candidate whose constraint is a *funding* deadline rather than a price-setting event — the part of
the clock that no fix paper covers.

- **Mechanism, causal coherence, persistence (4/5):** The funding-liquidity channel is modelled
  and supported (S-052), and the state is published (S-054). Not 5 because the cross-sectional
  step — that dependence, not the aggregate, drives the response — is an inference from the
  mechanism, not a result.
- **Quality and independence of supporting evidence (3/5):** The Cycle-2 source closure read the
  funding-currency and global-liquidity corpus (S-052 … S-073), so the evidence base is now
  documented rather than assumed: the mechanism is supported by central-bank staff work (S-052), a
  peer-reviewed version (S-053), the CIP/hedging-demand literature (S-056, S-057, S-059) and
  official crisis documentation (S-058, S-060, S-072). Not 4 or 5 because the *cross-sectional
  claim itself* has no supporting evidence at all — everything cited supports the parent
  mechanism, not the refinement.
- **Substantive novelty (2/5):** **Reclassified in the Cycle-2 closure pass.** The aggregate
  funding-constraint-state → carry-return relation is published, peer-reviewed and positive
  (S-055), and the dollar-funding-liquidity → dollar-forecast relation is published in both
  working-paper and peer-reviewed form (S-052, S-053); the aggregate versions were therefore
  rejected (R-006). What is left is the **cross-sectional** structure and the publication-timing
  test — a narrow, unclaimed residual, not a discovery of the channel. 2/5 is retained, not
  raised, and it is tied for the lowest novelty in the register with IDEA-001: presenting the
  residual as if it were the channel would be false.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  clear, the publication-timing test is clean, and the data are public — but the state is
  quarterly while the market is daily, so the effective sample is small and the cross-section must
  do the work. A further constraint found in the closure pass: the *fast* version of the state
  (the cross-currency basis) is not published anywhere and must be built from market quotes.
- **Resilience to costs, capacity, regime (3/5):** Slow horizon and liquid instruments are
  favourable; the tail (the funding-contraction state is the carry-crash state) is not, and
  emerging-market currencies — the most funding-dependent — are the least liquid and the least
  two-way borrowable.
- **Data availability, simplicity, reproducibility (4/5):** All inputs are public and published on
  a known calendar (S-054); no proprietary data is required.

**Cycle-2 closure re-check.** G-10's verdict is **MOSTLY CLOSED**: the aggregate version of this
candidate is a published baseline (R-006), and the dossier has been narrowed (v1.1) to the
cross-sectional and publication-timing residual only. The score is unchanged at 64.0, but its
*composition* has changed: the evidence is now stronger and better sourced while the novelty is
now demonstrably confined to a narrow residual. That is a demotion in substance and a wash in
arithmetic, and the ranking should be read accordingly.

**Key uncertainties that could change the rank.** Whether the cross-sectional structure exists at
all; whether it survives the carry-channel control (the published result claims separation, but
that claim must be re-verified in any validation); and whether the slow edge exceeds financing
and turnover costs. If the cross-section turns out to be published, the candidate is not
downgraded — it is **rejected**, and the register would hold no FX candidate at all.

**Role in the portfolio.** The register's *novelty-closure* exhibit: it demonstrates that
IDEA-002's mechanism is testable in a venue where the state is published, which is the Cycle-2
answer to the state-proxy question, and it demonstrates the closure process demoting the
register's own candidate when the literature turns out to already contain the result. It is a
candidate, but a weakly novel one with a narrow residual.

---

## Rank 6 — IDEA-002 FUNDSTATE (63.0) — *Cycle-1 rank 4, down 2; parked*

- **Mechanism, causal coherence, persistence (4/5):** The chain is coherent and each link is
  well-founded (S-009, S-010, S-011); the joint link is conjectural.
- **Quality and independence of supporting evidence (3/5):** Excellent components, but no located
  work on the *combination*, and the proxy's validity is unestablished (G-01).
- **Substantive novelty (3/5):** A synthesis of three established literatures around a state
  variable that does not appear in any of them. Novel enough to be interesting, not established as
  unclaimed.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  clear; volatility is a severe confound; the proxy is the obstacle.
- **Resilience to costs, capacity, regime (3/5):** The strategy consumes exactly the liquidity it
  is trying to measure, and its own financing cost moves with the state that generates the signal.
- **Data availability, simplicity, reproducibility (2/5):** The binding constraint. Order-flow data
  are obtainable; a defensible public funding-state proxy is not currently identified (G-01).

**Cycle-2 re-check.** No score change; the rank is 6 because three candidates were added above it
in Cycle 2, and because IDEA-006 subsequently fell back below it when the G-09 closure found
IDEA-006's headline effect published. G-01 was **narrowed, not closed**: four public funding-state
ingredients were verified (SOFR and the related GC repo rates, S-041; standing-repo-facility
take-up and the primary dealer statistics, S-042), but the *validation target* — a published,
continuous series of dealer funding value adjustments — still does not exist in the public record,
so the candidate cannot yet be tested as specified. The parking (P-004) therefore stands.

**Key uncertainties that could change the rank.** If G-01 cannot be closed, this candidate should
remain **parked, not re-specified** — re-specifying it around a weaker proxy would convert a good
idea into a disguised baseline. Cycle 2's IDEA-007 makes the reason sharper: the *same mechanism*
is testable in FX because the state is published there, which is an argument for changing venue
rather than for weakening the proxy.

---

## Rank 7 — IDEA-006 FIXCLOCK (59.0) — *new in Cycle 2; demoted by the G-09 closure*

- **Mechanism, causal coherence, persistence (4/5):** The deadline chain is documented by three
  independent institutional bodies — a global regulator (S-044), the benchmark administrator
  (S-045) and the settlement utility (S-048, S-049) — and the flow's concentration is quantified
  by the FSB (over 10% of a platform's daily volume in the fix window on some days for some
  currencies). Not 5 because the link from a documented deadline to a *price* concession is now
  documented for the fix but remains an inference for the settlement-side deadlines, which are
  the candidate's residual.
- **Quality and independence of supporting evidence (3/5):** Down from 4 after the G-09 closure.
  The evidence base is now genuinely strong — five independent lines on the fix effect (S-075,
  S-076, S-077, S-074, S-081), the institutional documentation (S-044, S-045, S-046, S-048,
  S-049) and a post-revision benchmark study (S-080) — but every one of them supports the
  *parent* effect, not the candidate's residual claim, and the settlement-side literature has not
  been searched at all (G-11). Not 4 or 5 for that reason.
- **Substantive novelty (2/5):** **Reclassified by the G-09 closure.** The headline claim — a
  price-insensitive, deadline-driven flow that moves the price at the fix, temporarily, and
  reverses — is published (S-075, S-076, S-077, S-074, S-081), and the aggregate version was
  rejected (R-007). What is left is the settlement-side extension and the post-2015 persistence
  question: narrow, and not yet cleared of the literature (G-11). 2/5 ties for the lowest novelty
  in the register with IDEA-001 and IDEA-007, and it is deliberately visible.
- **Clarity of falsifiable predictions and feasibility of a clean test (3/5):** The predictions are
  stated, the published fix result is available as a baseline to reproduce, and a no-macro-release
  discriminator exists; but the test requires proprietary intraday order-book data, the published
  literature's own datasets are administrator- and dealer-provided (S-074, S-076, S-080), and a
  daily-data substitute would measure a different object.
- **Resilience to costs, capacity, regime (2/5):** The weakest dimension in the register alongside
  IDEA-002: the concession is measured in pips inside a few minutes, so spread and slippage are
  first-order; the flow may already be arbitraged by the liquidity providers who are stationed
  there by construction; and the 2015 widening of the calculation window from one minute to five
  may have diluted the very effect the candidate was built on.
- **Data availability, simplicity, reproducibility (3/5):** The clock is public; the flow
  measurement is not. The benchmark administrator's own tick data is not freely available (S-047,
  S-080).

**Cycle-2 closure re-check (G-09).** The verdict is **MOSTLY CLOSED**, and it went against the
candidate: the fix's price impact is published (S-075, S-076, S-077, S-074, S-081), the aggregate
version was rejected (R-007), and the dossier was narrowed to v1.1. The score falls from 66.0 to
59.0 — evidence 4 → 3 and novelty 3 → 2 — because the closure found the effect published, and
because the residual it leaves behind is unsearched (G-11). The seven-point fall is the largest
single-cycle change in the register, and it is the process working as intended.

**Key uncertainties that could change the rank.** Whether the settlement-side deadlines have any
separable price effect at all (G-11, on which the candidate is blocked); whether the published fix
effect survived the 2015 methodology revision, which would remove the need for any new state
condition; and whether any of it is harvestable after costs by a participant who is not already
stationed at the fix. If G-11 closes against the candidate, it is rejected, not re-scored.

**Role in the portfolio.** No longer a structural candidate in its own right: it is now a *narrow
residual* attached to a published effect, blocked on a literature check. Its value in the register
is now the second demonstration of the closure process (after IDEA-007), and the register's only
candidate whose constraint is a *funding* deadline rather than a price-setting event — the part of
the clock that no fix paper covers.

---

## Cross-cutting notes for the next cycle

1. **The state-proxy problem is largely a venue-selection problem.** IDEA-002 fails on the proxy
   and IDEA-007 works on the same mechanism because the dollar funding state is *published*
   (S-052, S-054); IDEA-004 fails on the proxy in equities while IDEA-005 works on the same
   crowd-state idea because the regulator publishes the passive positions in futures (S-030);
   IDEA-008 works because short interest and securities-lending fees are published by exchanges
   and lending agents; IDEA-009 works because the perpetual funding rate is published by the
   exchange every funding period with zero lag. The pattern is deterministic: *do not hunt for a
   proxy; hunt for a venue where the state is already published by a regulator, a benchmark
   administrator, a settlement utility, or the venue itself.* See the state-proxy methodological
   note at the end of `idea_register.md`.
2. **Several candidates are refinements of published effects, and two published aggregates were
   rejected outright.** IDEA-001 must be described as a refinement of a published effect;
   IDEA-005 as a refinement of a contested published effect; IDEA-007 as a **narrow residual** of
   a published funding-constraint result (S-055), after the aggregate version was rejected as a
   known baseline (R-006); IDEA-006 as a **narrow residual** of a published fix-window effect
   (S-075, S-076, S-077, S-074, S-081), after its aggregate version was rejected as R-007; IDEA-008
   and IDEA-009 are **new specifications** whose components are documented but whose joint
   two-legged expressions are not known baselines — they must be described as such, not as
   discoveries of the underlying components. If a future cycle adds a candidate whose only claim
   is "a known effect with a new name", it belongs in `rejected_and_parked.md`.
3. **Tail concentration is the register's main unhedged risk.** IDEA-003's payoff is concentrated
   in a few events; IDEA-001's leg 2 is exposed to announcement-window news; IDEA-004's left tail
   is a broken anchor; IDEA-006's worst case is a settlement or benchmark disruption at exactly
   the deadline the position is held for; IDEA-007's worst case is the funding squeeze it is
   designed to anticipate; IDEA-008's dominant failure mode is a recall driven by fundamental
   news (a directional loss, not a liquidity event); IDEA-009's worst case is a crypto
   deleveraging spike that gaps through the pre-scheduled exit. No single candidate is a complete
   portfolio, and none of them should be described as if it were.
4. **The register now has market diversification and factor concentration.** Cycle 1's candidates
   were all listed US equities; Cycle 2 added commodity futures and two FX candidates; Cycle 3
   added securities-lending equities (IDEA-008) and crypto perpetuals (IDEA-009). Two candidates
   (IDEA-006, IDEA-007) are FX positions short the funding currency, and IDEA-009 adds direct
   crypto-market beta. The register's net dollar exposure and its crypto exposure are
   portfolio-level concerns that no single dossier owns.
5. **No candidate has been tested.** Nothing in this register is evidence that any of these
   hypotheses works, and no number here is a performance estimate.
6. **The three originality gaps on the Cycle-2/3 candidates have been addressed.** G-10
   (IDEA-007) is **MOSTLY CLOSED**: the aggregate version is a published baseline (R-006), the
   cross-sectional residual is open. G-09 (IDEA-006) is **MOSTLY CLOSED**: the fix-window price
   impact is published (R-007), the settlement-side residual is **partially closed (G-11)** —
   settlement-side mechanics are a priced friction (S-082, S-071) but the specific CLS deadline
   cluster / T+1 post-US-close window is untested. G-06 (IDEA-005) is **narrowed, not closed**:
   the commodity basis-convergence literature (S-032 … S-039) was located and none of it
   conditions the roll concession on passive share × depth, so IDEA-005's differentiator survives
   as a conjecture. **G-11 remains the cheapest high-value originality check left:** if a
   published paper tests the settlement-side deadline cluster as a price determinant, IDEA-006 is
   rejected, not narrowed.
