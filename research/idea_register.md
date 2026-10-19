# IDEA REGISTER

Every retained candidate lives here with a complete dossier. Status values: `shortlisted`,
`candidate` (retained but not shortlisted), `archived` (retained for reference, not a top
opportunity), `rejected` (see `rejected_and_parked.md`; dossiers are not maintained for those).

Last updated: Cycle 2 (including the Cycle-2 closure passes), 2026-10-19. The register was empty
before Cycle 1; Cycle 2 added three dossiers outside listed US equities. **Closure passes: two
candidates were demoted by their own literature. IDEA-007 was narrowed to v1.1 after the
funding-currency corpus was read — its aggregate version is a published baseline (S-055, rejected
as R-006) and the dossier now claims only the cross-sectional and publication-timing residual.
IDEA-006 was narrowed to v1.1 after the intraday fixing literature was read — the fix-window
price impact is published (S-075, S-076, S-077, S-074, S-081, rejected as R-007) and the dossier
now claims only the settlement-side residual (blocked on G-11) and the post-2015 persistence
question.**

---

## IDEA-001 — RECON-FLOW: announcement-timed, flow-scaled reconstitution pressure with a post-effective reversal leg

- **ID / short name:** IDEA-001 / RECON-FLOW
- **Date added:** 2026-10-19 · **Cycle:** 1 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. Effect family is documented in prior literature; the
  candidate is the *conditional, flow-scaled, two-leg specification*, not the effect itself.

**One-sentence hypothesis.** Index-provider reconstitution creates a scheduled, deadline-driven
passive demand shock that is knowable in advance, and the part of the resulting price move that
reflects the arbitrageur's compensation for providing liquidity to that shock partly reverses after
the passive flow has been executed.

**Plain-language description.** When S&P announces that a stock will join the S&P 500, index funds
must buy it at the effective close, five days later. Somebody has to sell that stock to the funds
before the deadline, and the market's price moves up to compensate the seller for the risk of
carrying the position and for the fact that their exit is crowded. After the funds have bought,
that seller unwinds and part of the price move goes back the other way.

**Mechanism (causal chain).**
1. S&P DJI fixes an announcement timestamp and an effective date; constituent changes are
   announced one to five days ahead, S&P 500 announcements are published at 05:15 ET, changes
   take effect after the close on the third Friday of the quarter-end month, and a share freeze
   applies in the preceding week (S-008).
2. Funds tracking the benchmark must trade to the new weights on the effective date; the required
   dollar flow for a given name is a deterministic function of the index weight change and the
   assets tracking the index. This is a *scheduled* demand curve shock, not an information shock.
3. The passive flow is not price-sensitive (the funds must trade at the close regardless of price),
   so the price must move to ration a finite liquidity supply. The price concession paid to the
   counterparty is the compensation.
4. A risk arbitrageur ("the S&P game", S-002) supplies the stock ahead of the effective date and
   sells into the passive demand. That is a *business* for the arbitrageur, not a free lunch.
5. The arbitrageur must eventually unwind; the unwind is itself a scheduled, correlated sale in
   the same name. If the fundamental value has not changed, part of the initial concession
   reverses (S-002, S-004).
6. The magnitude of both legs should scale with the *size of the passive flow requirement* —
   i.e. with the index weight change multiplied by the assets tracking the index — and with the
   liquidity of the affected name. This scaling is the differentiator: the classic literature
   treats index events largely as one homogeneous type.

**Expected return source.** A compensation for providing liquidity to a deadline-driven,
non-price-sensitive buyer (a structural liquidity-provision premium), plus the arbitrageur's
scheduled-unwind reversal, net of execution costs and adverse selection. This is a *flow* premium
and a *timing* premium, not a risk premium for systematic exposure.

**Originality.**
- *Closest known work:* the index-inclusion literature — Harris & Gurel (1986) [S-001], Beneish &
  Whaley (1996) [S-002], Chen/Noronha/Singal (2004) [S-003], Woglom (2002) [S-004]; option-market
  evidence [S-005, S-006, S-007]; and the "holdings effect" debate summarised in [S-004].
- *What is already known:* the announcement price increase, the announcement-to-effective drift, a
  partial post-effective reversal, the asymmetry between additions and deletions, and the fact that
  the effect grew with index-fund assets.
- *Substantive differentiator claimed here:* (i) conditioning every leg on the **size of the
  passive flow requirement** rather than treating events as homogeneous; (ii) specifying the
  **post-effective reversal as a separately tradable leg** with its own entry/exit rule rather
  than as a description of a price path; (iii) an explicit **asymmetry of who can arbitrage** —
  on additions an arbitrageur can pre-position and be paid; on deletions the index fund must sell
  into a one-sided book and no comparable arbitrageur exists — which is a flow-and-capacity
  explanation for the addition/deletion asymmetry that [S-003] attributes to investor awareness.
- *Honest classification:* **documented effect, incremental conditional refinement.** This is not
  a new effect and must never be presented as one. Its value is that it is unusually clean to
  test and to falsify, with published event dates that require no look-ahead.
- *Confidence in the comparison:* high. The classic papers are directly on point and were read
  (abstracts plus full text for S-002 and S-004).

**Target scope.** US large-cap equities (S&P 500, S&P MidCap 400, S&P SmallCap 600 additions and
deletions); event-driven holding from the announcement after-close to the effective close (leg 1)
and from the effective close to roughly 1–20 sessions after (leg 2); monthly frequency of events
(quarterly reconstitution plus intra-quarter changes). Regime conditions: intact index futures
market, low index-futures basis stress, no venue outage at the effective close.

**Observables (known at decision time, conceptually).**
- Announcement timestamp and the announced change (published; S-008).
- Effective date and the index weight change implied by the reconstitution.
- Assets tracking the benchmark (needed as a scale variable; see source gap G-02).
- The affected name's liquidity: quoted spread, depth, average daily volume around the event.
- Whether the name is an "outsider" addition (moving in from outside the S&P 1500 family) versus
  an intra-family promotion — the flow requirement differs by an order of magnitude [S-007].
- **Timing hazards to flag for the validator:** the announcement is published after the close
  (05:15 ET), so leg 1 cannot be entered at the announcement close without trading in the
  after-hours/overnight session; the effective-date close is the passive execution moment, so
  leg 2 must be entered *after* the passive flow is done (next session onwards) and its exit must
  be scheduled to avoid the crowded window; a share-freeze week and corporate actions can change
  the required weights between announcement and effective date; a name can be added and later
  removed within the same window; and index-option expiries and index-futures rolls coincide with
  the effective date, contaminating the flow.

**Rule sketch (descriptive, non-executable).** At the announcement after-close, for each announced
addition (and separately for deletions), compute the required passive flow as a function of the
weight change and the assets tracking the benchmark; screen for the affected name's liquidity and
for a non-degenerate announcement-to-effective window. Leg 1: establish a long position in the
affected name after the announcement, sized so that the position is small relative to the expected
passive flow requirement, and hold to the effective-date close. Leg 2: close or reverse the
position after the effective date over a pre-specified number of sessions. Exclusions: names
trading below a minimum dollar volume, names with a corporate action inside the window, events
inside a scheduled index-futures roll week.

**Persistence thesis.** The opportunity exists because the passive buy is not price-sensitive and
is scheduled, so the price concession is not competed away: the arbitrageur is *paid* to absorb the
flow, and payment is a cost to the index fund, not a loss to an informed counterparty. It decays if
(a) index funds shift to pre-positioning (which would remove the pre-effective leg), (b) passive
assets grow so large that the arbitrage becomes the dominant participant (which would compress the
concession and increase the risk that the arbitrageur's own exit crowds it), or (c) execution
becomes cheap enough (fractional/algorithmic closing-auction participation) that the concession
disappears. All three are observable in principle.

**Constraints.**
- *Cost/liquidity:* the affected names are large-cap and liquid, but the trade must be small
  relative to the passive flow, so the per-event dollar capacity is small; the reversal leg is
  executed in a name where the arbitrage crowd is also unwinding.
- *Capacity:* capacity is bounded by the size of the flow requirement, so the strategy scales with
  passive assets, not with the arbitrageur's balance sheet.
- *Financing/borrow:* a long-only leg 1 has no borrow requirement; a long/short reversal variant
  (short the affected name against the market) does, and the affected name is typically easy to
  borrow, but borrow can be scarce exactly in the crowded window.
- *Market impact:* the trade is small relative to the passive flow by construction, but the
  reversal leg trades *against* the same crowd.
- *Venue/operational:* a single close on a single exchange; a venue outage or a limit-up/limit-down
  halt at the effective close breaks the premise; index funds and the arbitrageur compete for the
  same closing-auction liquidity.
- *Financing of the event:* the position is held for at most a few days, so financing is a spread
  cost, not a balance-sheet constraint.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.**
- Regime: the effect depends on index-fund trading convention and passive scale; it should be
  weakest when passive funds pre-position and strongest when they trade at the effective close.
- Tail exposure: leg 1 is a long position held for days with an event-driven exit; it carries
  market beta and overnight gap risk, and the announcement-to-effective window contains
  idiosyncratic news.
- Crash behavior: additions to an index performed during a crisis recovery can gap; the price
  concession and the fundamental news are confounded.
- Hidden beta: the leg is a long-only small-cap-of-index event position; sizing must control
  market beta explicitly, otherwise the "alpha" is a beta bet.
- Correlated risks: all events in a reconstitution window share the same date; a single market
  shock dominates many small event-level results.

**Falsifiable predictions and rejection conditions.**
1. *Announcement-to-effective drift:* additions drift up and deletions drift down, with magnitude
   increasing in the required passive flow. **Kill:** the drift is not monotone in flow size, or
   disappears once announcement-window abnormal options volume is controlled for (which would
   indicate the announcement is being anticipated by informed option flow rather than by
   price pressure — see [S-005]).
2. *Post-effective partial reversal:* a non-zero fraction of the leg-1 move reverses within
   1–20 sessions after the effective date, and the reversal is larger when leg 1 was larger.
   **Kill:** no reversal at all, or a reversal that is fully explained by a change in the
   fundamental news environment or by an index-option/futures roll.
3. *Flow scaling:* effect size scales with weight change × assets tracking the benchmark, not just
   with "being in the index". **Kill:** no relation to flow size.
4. *Asymmetry:* additions give a harvestable spread; deletions do not, because the passive seller
   faces a one-sided book. **Kill:** deletions show an equally large and equally harvestable move
   in the passive direction.
5. *Crowding null:* if the post-effective reversal is entirely explained by a broad reversal in
   additions, the mechanism is a common factor, not a liquidity concession.

**Main confounders and rival explanations.**
- *Informed trading ahead of the announcement:* options markets and insiders may trade the
  announcement; [S-005] finds pre-announcement abnormal options volume predicts smaller
  announcement returns. Any flow-scaling result must separate price pressure from anticipation.
- *Awareness/attention:* the addition makes the name visible; a retail attention flow (cf. [S-027])
  is an alternative explanation for the announcement response, and it would not predict the
  post-effective reversal or the flow scaling.
- *Fundamental news:* additions are not random — companies with rising market value, M&A activity
  and index eligibility change together. This is the single most important confounder.
- *Index-option and index-futures mechanics* on the effective date, and the "sell the news" of
  the arbitrageur's own unwind.
- *Survivorship in the event sample:* deleted names often fail, so the deletion leg is contaminated
  by fundamental news in a way the addition leg is not.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: S&P DJI announcements and index-weight changes
(S-008 gives the schedule; the provider publishes constituent and weight files), daily OHLCV and
closing-auction data, index membership history, and a series for assets tracking the benchmark
(gap G-02). Feasibility: high for the event study, medium for the flow-scaling test (depends on
G-02) and medium for the reversal leg (needs precise close-to-close and auction data).

**Theory/evidence status.**
- *Conceptual rationale:* supported by the price-pressure and liquidity-provision mechanism
  [S-001, S-002, S-004] and by the venue's own rules [S-008].
- *Mechanism supported by sources:* yes for the announcement drift; the flow-scaling
  specification and the arbitrage-capacity asymmetry are **unresolved conjectures** added here.
- *Prior empirical support reported by others:* yes, extensively [S-001, S-002, S-003, S-004,
  S-005, S-006, S-007] — reported by their authors, not reproduced here.
- *Unresolved:* whether the effect is still present at post-2024 passive scale and under modern
  closing-auction practice.

**Remaining uncertainty / confidence.** Confidence in the *core effect*: high (published,
repeatedly). Confidence in the *differentiated specification* (flow scaling + two-leg trade +
side asymmetry): moderate; the components are individually unproven. Priority score 76/100;
rank 1 of 7 (rank 1 of 4 at Cycle 1; score and rank unchanged at Cycle 2). **Concrete next
question:** does the announcement-to-effective drift scale with the
required passive flow (a quantitative, publicly checkable prediction), and is the post-effective
reversal statistically separable from awareness and information-leakage explanations?

---

## IDEA-002 — FUNDSTATE: intermediary funding cost as a state variable for flow-driven price impact

- **ID / short name:** IDEA-002 / FUNDSTATE
- **Date added:** 2026-10-19 · **Cycle:** 1 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. The components are well established; the *combination*
  (funding state × order-flow impact asymmetry) is the candidate.

**One-sentence hypothesis.** When intermediary funding costs are high and dealers' balance sheets
are constrained, flow-driven price impact is larger and more persistent than when funding is cheap,
so the *sign and size* of the expected price response to a given order-flow shock depends on an
observable funding state.

**Plain-language description.** The same order-flow imbalance moves a price more, and moves it back
more slowly, when the dealers who absorb that flow are expensive to fund. So a directional signal
built on order flow should be scaled by a funding-state variable, and short-horizon flow strategies
should expect worse exit liquidity precisely when their signals work best.

**Mechanism (causal chain).**
1. Dealers intermediate client flow on their balance sheet; the cost of doing so is a funding
   cost that the dealer's shareholders bear as a debt overhang, and dealer quotations therefore
   embed it (S-010).
2. Funding costs are state-dependent: they reflect the marginal cost of balance sheet, which
   rises with volatility, with balance-sheet congestion, and with the discount rate applied to
   encumbered assets.
3. Under Brunnermeier–Pedersen (S-009), margin and funding constraints make market liquidity
   state-dependent and can make it "dry up" and become self-reinforcing; speculators' capital and
   volatility are state variables for liquidity and for risk premia.
4. Order-flow imbalance explains short-horizon price changes with an impact slope inversely
   proportional to market depth (S-011) — the impact relation is therefore not a constant; it
   inherits the liquidity state.
5. Combining: the flow-impact coefficient and the subsequent reversal are functions of the
   funding/liquidity state. A flow signal conditioned on the funding state should have a
   time-varying, state-dependent expected value, and the *dealer-intermediated* segment of the
   market should behave differently from internally managed assets in the same state.

**Expected return source.** Compensation for intermediation and liquidity provision that varies
with the funding state, plus a short-horizon reversal of temporary price pressure that is larger
when the pressure was larger.

**Originality.**
- *Closest known work:* Brunnermeier & Pedersen [S-009]; Andersen, Duffie & Song [S-010]; Cont,
  Kukanov & Stoikov [S-011]; Hasbrouck-style dealer inventory work; and the broader
  "liquidity premium" literature.
- *What is already known:* that funding constraints and market liquidity are linked; that dealer
  funding costs are a real, quantified wedge; that order flow drives short-horizon prices with a
  depth-dependent slope; that liquidity is a state variable with nonlinear effects.
- *Substantive differentiator claimed here:* a *joint* state model in which a publicly observable
  funding-state proxy is used to predict the **asymmetry between flow-driven continuation and
  reversal**, and to distinguish the dealer-intermediated part of the market from the
  self-cleared part. I am not aware of a published result that conditions flow-impact asymmetry on
  a funding state; the retrieved literature treats funding (S-009) and impact (S-011) separately.
- *Honest classification:* **informed synthesis; the linking relation is an unresolved conjecture.**
- *Confidence in the comparison:* moderate. The three components are solid; my claim is about the
  absence of a published *combination*, which I cannot establish exhaustively from a limited search.

**Target scope.** US equities and ETFs with substantial dealer intermediation; intraday to
multi-day horizons; daily rebalancing of a flow signal; regime conditions: exchange-traded,
clearing-fee and margin schedules observable; stress episodes (margin hikes, futures-basis
stress) are part of the state, not an exception to it.

**Observables.** Order-flow imbalance from trades and quotes; quoted depth; a funding-state proxy
(constructed from observable funding instruments — see below); market and sector volatility;
dealer-intermediation intensity (share of volume executed against dealers; the fraction of the
universe with listed options and active market makers); margin and clearing-fee schedules as
discrete funding shocks.

**Rule sketch (descriptive, non-executable).** Compute a daily order-flow imbalance signal per
name. Estimate the state-dependence of the impact coefficient by conditioning on the funding-state
proxy (a composite of observable funding spreads, basis, and margin/collateral policy dates).
Trade the continuation leg scaled by the state; stand aside, or reduce exposure, in states where
the estimated impact-to-reversal ratio is unfavourable; restrict the tradable universe to
dealer-intermediated names in states where the funding constraint binds.

**Persistence thesis.** The funding wedge is a *price* for balance-sheet risk, not an error; it
persists because balance-sheet risk is real and because dealers' funding is scarce in exactly the
states when their intermediation is most valuable. It decays if balance-sheet capacity becomes
elastic (e.g. through a permanently abundant capital base or non-dealer liquidity provision) or
if dealer economics stop embedding funding cost in quotes.

**Constraints.** Costs: intraday spreads and adverse selection are precisely what the strategy
consumes, so cost sensitivity is extreme. Capacity: flow-based strategies are capacity-limited in
exactly the states where the signal is strongest. Financing: a long/short intraday book is
capital-intensive and margin-sensitive — the strategy's own funding cost moves with the same state
variable that generates the signal, which is a self-referencing hazard that must be handled
explicitly. Borrow: short legs are subject to recall in stress. Venue/operational: intraday
execution quality, queue position, and message latency. Market impact: the signal is *about*
impact, so slippage estimation error is the central risk.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Strongly regime-dependent by
construction: the state variable *is* the regime. Tail: in the tightest funding states, the
book is short exactly the liquidity it needs to unwind, and gaps are large. Crash behaviour: the
reversal leg can fail violently in a dislocation, because the temporary pressure becomes permanent
fundamental news. Hidden beta: a long/short book built from flow signals is nearly beta-neutral by
construction but not risk-neutral; funding-state conditioning may load on credit and duration
factors. Correlated risks: all positions respond to the same state variable, so the book is a
single macro bet in stress.

**Falsifiable predictions and rejection conditions.**
1. *State-dependent impact:* the estimated flow-impact slope is larger in high-funding-cost states
   than in low-cost states. **Kill:** no monotone relation, or the relation is fully explained by
   contemporaneous volatility and depth.
2. *State-dependent reversal:* the post-shock reversal is proportionally larger when the
   funding state is tight. **Kill:** reversal is state-independent once volatility and spread are
   controlled.
3. *Intermediation differential:* the effect is present in dealer-intermediated names and absent
   (or materially weaker) in self-cleared names in the same state. **Kill:** no differential.
4. *Proxy validity:* the constructed funding proxy must be validated against disclosed dealer
   funding costs; if the proxy carries no information about them, the candidate is untestable and
   must be dropped rather than re-specified.

**Main confounders and rival explanations.** Volatility (a funding-state proxy and an impact driver
simultaneously — the hardest confound); spread and depth as mediators rather than confounds;
liquidity as a *cause* of both funding stress and price impact (so conditioning may be
over-controlling); index and ETF rebalance flows; and the possibility that the apparent effect is
an unmodelled news/attention state.

**Data requirements and feasibility for a future independent validation.** TAQ or equivalent
order-level data (trades, quotes, order-book) for a multi-year sample; a constructed funding-state
proxy from public funding instruments; dealer balance-sheet disclosures for proxy validation
(gap G-01). Feasibility: **medium-low** — the binding constraint is the funding-state proxy, not
the flow data.

**Theory/evidence status.** Conceptual rationale: supported [S-009, S-010, S-011]. Mechanism
supported by sources: for each component; the joint relation is an unresolved conjecture. Prior
empirical support reported by others: for the components (S-009, S-011); not for the combination.
Unresolved: whether a public, defensible funding-state proxy exists (G-01).

**Remaining uncertainty / confidence.** Confidence in the components: high. Confidence in the
joint relation: low-to-moderate. **The principal risk to this candidate is feasibility, not
mechanism** — if G-01 cannot be closed, the candidate must be parked rather than re-specified.
Priority score 63/100; rank 6 of 7 (rank 4 of 4 at Cycle 1; the score is unchanged, and the rank
fell only because three candidates were added above it — and rose back one place when IDEA-006
fell below it after the G-09 closure — the parking stands, P-004). **Concrete
next question:** is there a public funding-state
proxy that demonstrably predicts disclosed dealer funding value adjustments over a multi-year
sample? (If not, park the candidate.)

---

## IDEA-003 — VRP-STATE: the variance risk premium as crash-state compensation, and the state gate on harvesting it

- **ID / short name:** IDEA-003 / VRP-STATE
- **Date added:** 2026-10-19 · **Cycle:** 1 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. The aggregate variance risk premium is a known baseline;
  the candidate is the *state gate* on harvesting it.

**One-sentence hypothesis.** The variance risk premium is compensation for bearing crash risk
rather than a free annuity, so a strategy that harvests it should only be run in states where the
crash is not imminent, and the premium's sign in normal times is not evidence that it can be
harvested unconditionally.

**Plain-language description.** Investors pay up for insurance against crashes; that is why
implied variance exceeds realized variance. A strategy that sells variance earns that insurance
premium — but only gets paid if the world does not crash, and the states in which the premium is
largest are often the states in which the crash is coming. The premium is only harvestable with a
state gate.

**Mechanism (causal chain).**
1. Asset pricing with rare disasters implies that investors demand an insurance premium for
   bearing disaster risk, and that demand generates a negatively skewed risk premium (S-016).
2. Skew laws and the differential pricing of individual equity options show the same demand
   operating at the single-name level (S-014).
3. The variance swap rate is a near-exact model-free synthesis of option prices and approximates
   the risk-neutral expected variance; realized minus implied variance is the variance risk
   premium, which is strongly negative for US equity indices (S-012).
4. The premium is a *state variable* for aggregate equity returns, with the strongest predictive
   power at a quarterly horizon (S-013) — and crash risk is itself a state that commands an
   elevated equity premium (S-015).
5. Therefore the premium-harvesting payoff is negatively skewed: it is earned in the many
   ordinary states and lost in the rare state, and the *conditional* value of harvesting depends
   on the state. A gate on the crash state is part of the mechanism, not an optimisation overlay.

**Expected return source.** Compensation for absorbing crash risk in the left tail, plus the
time-varying pricing of variance as a risk factor (S-013).

**Originality.**
- *Closest known work:* the variance risk premium literature [S-012, S-013]; disaster insurance
  pricing [S-016]; single-name skew and insurance demand [S-014]; crash-risk and the equity
  premium [S-015].
- *What is already known:* the premium exists, is large, predicts aggregate returns, and is
  associated with crash-risk states.
- *Substantive differentiator claimed here:* the *state-gated harvesting specification* — that
  the premium should be harvested only outside crash-imminent states, that the unhedged harvest is
  a crash-state bet, and that the gate should be an explicit, pre-specified, ex-ante-observable
  state (implied crash measures, not realized crash outcomes). Part of this is anticipated by
  [S-015] (crash-risk states carry higher premia) and by the tail-hedge-fund evidence; the
  candidate's claim is narrower: the *unconditional* harvesting strategy is a state-contingent
  bet, and the gate is the mechanism.
- *Honest classification:* **known baseline with a state-conditioning refinement.** Not a new
  premium. Any claim of novelty for "short variance" would be false; the candidate is about *when*
  to short it.
- *Confidence in the comparison:* high for the baseline; moderate for the gate specification.

**Target scope.** US equity index options and variance swaps; single-name options for the
cross-sectional version; monthly to quarterly holding horizons for the aggregate version; regime
conditions: the gate must be computable from option data only (no realized crash variables).

**Observables.** Model-free implied variance and variance-swap rate from listed options (S-012);
model-free realized variance for post hoc measurement only; option-implied crash measures (e.g.
out-of-the-money put-implied crash probabilities) as the gate; skew; term structure; liquidity of
the option surface (spread and depth at the strikes used).

**Rule sketch (descriptive, non-executable).** Each period, compute the model-free implied variance
and the variance risk premium; compute the gate from option-implied crash-risk measures. In states
where the gate indicates an elevated crash probability relative to its own history, hold no
variance-shortening position (or hold a reduced position); in ordinary states, take the
variance-shortening position, scaled by the premium and by the liquidity of the option surface.
Report the harvest net of option spreads, margin and financing, and vega risk.

**Persistence thesis.** The demand for crash insurance is structural (S-016) and is amplified by
the growth of index and single-name option usage; the premium persists because the supply of
insurance is limited by the balance sheet and risk tolerance of the writers. It decays if insurers
expand capacity, if retail flow dominates option volumes, or if the option market's own tail
becomes a crowded trade.

**Constraints.** Costs: option spreads on the traded strikes; vega and gamma risk on the position;
the P&L is a variance-swap-like payoff that must be replicated or directly accessed, and both
routes have their own basis risk. Financing/collateral: variance positions consume margin that
moves with volatility, i.e. exactly when the position loses. Liquidity: far out-of-the-money
options are cheap but wide; the liquid ATM/OTM region is where the premium is smallest. Capacity:
the premium harvest is capacity-limited at exactly the sizes where the supply of insurance is
scarce. Venue/operational: OTC variance swaps introduce counterparty and documentation risk;
listed-option replication introduces tracking error. Shorting constraints: not a short-sale-constrained
strategy in the equity sense, but writing options requires exchange-level approvals and margin.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Extremely regime-sensitive:
the strategy is short the thing that spikes in a crisis. Tail exposure: the defining feature — a
single crash can dominate many years of premium. Crash behaviour: gap risk, exchange halts, and
the fact that the premium's *realisation* is a small number of large negative events. Hidden beta:
a variance-short book is long gamma and short vega, and it has a negative exposure to volatility
increases; the equity market beta of the harvest can be state-dependent. Correlated risks: all
variance positions across the surface are the same trade.

**Falsifiable predictions and rejection conditions.**
1. *Gate works:* the unconditioned harvest has a materially worse risk-adjusted outcome and a
   fatter left tail than the state-gated harvest, on a pre-specified gate. **Kill:** the gate
   provides no incremental risk-adjusted benefit out of sample.
2. *Premium predictability:* the premium state predicts subsequent aggregate returns in the
   direction reported by [S-013]. **Kill:** no predictive relation in the modern sample (note
   [S-013]'s own caveat that the power of other predictors has decayed).
3. *Crash-state linkage:* the premium and the option-implied crash state co-move such that
   harvesting is least attractive exactly when the premium is highest. **Kill:** the premium is
   highest in states where crashes are *less* likely.
4. *Cost threshold:* the harvest survives option-spread and financing costs at a plausible
   institutional cost. **Kill:** the gross premium is mostly transaction cost.
5. *Structural change:* post-2010 single-name option structure (0DTE, retail flow) has not
   eliminated the mechanism. **Kill:** the single-name insurance channel has been arbitraged
   away or reversed (gap G-05).

**Main confounders and rival explanations.** The premium may be compensation for a variance risk
factor rather than for crash risk per se (S-012's own alternative) — these are hard to separate;
the measured "premium" partly reflects the volatility risk of the *hedging* programme; a
volatility-feedback story can generate similar options-pricing patterns; measurement error in
realized variance (closing-price noise) can inflate the estimated premium; and the gate can be
overfitted to the same history that defines the premium.

**Data requirements and feasibility for a future independent validation.** Listed option chains
(option quotes with model-free implied variance) and intraday prices for realized variance
(S-012, S-013 use OptionMetrics-like data); for the single-name version, a large options
database. Feasibility: high for the aggregate version if a survivorship-clean option history is
available; medium for the single-name version; the gate's ex-ante computability is the design
constraint to enforce.

**Theory/evidence status.** Conceptual rationale: supported [S-016, S-014]. Mechanism supported by
sources: for the premium's existence and measurement [S-012, S-013]; the "compensation for crash
risk" reading is a model-based interpretation [S-016, S-015]. Prior empirical support reported by
others: yes [S-012, S-013, S-015]. Unresolved: the *gate* specification and the post-2010
structural change (G-05).

**Remaining uncertainty / confidence.** Confidence in the premium's existence: high. Confidence
that a state gate materially improves the harvest: moderate — this is the candidate's whole
content, and it is not directly evidenced. Priority score 71/100; rank 4 of 7 (rank 3 of 4 at Cycle 1; the score is unchanged, and the rank
fell only because IDEA-005 was added above it). **Concrete next
question:** in a pre-specified ex-ante gate, does the crash-state-gated variance harvest dominate
the unconditioned harvest on a risk-adjusted basis, and does the gate need any information beyond
the option surface itself?

---

## IDEA-004 — SLOWCAP-COND: capacity-conditional convergence trades under slow-moving capital

- **ID / short name:** IDEA-004 / SLOWCAP-COND
- **Date added:** 2026-10-19 · **Cycle:** 1 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. The limits-to-arbitrage family is heavily studied; the
  candidate is the *observable crowd-depth state* used to condition the trade.

**One-sentence hypothesis.** Because arbitrage capital is slow to arrive and exits in
synchronisation, a convergence trade's expected return and its crash risk are both functions of
how crowded the convergence crowd already is, and the crowd depth can be partially observed.

**Plain-language description.** When a stock is mispriced, the money that should fix it does not
come instantly — it comes slowly, and only if the mispricing gets deep enough. So the bigger the
gap and the thinner the crowd, the longer the gap can persist, but when the crowd is already
heavy, the same gap will be competed shut faster and everyone's exit will collide.

**Mechanism (causal chain).**
1. Equilibrium with slow-moving capital: arbitrage capital only moves when fire-sale discounts are
   deep enough; stand-by capital is limited, and contagion arises when unrelated assets draw on a
   common pool of arbitrage capital (S-017); capital is empirically and theoretically slow
   (S-018, S-019).
2. Mandates, delegation and career concerns bind capital (S-020); manager reputation can make
   capital slow sometimes and fast other times, moving prices with no fundamental news (S-021).
3. Flow-driven price pressure of exactly this kind produces momentum when flow inertia makes
   prices underreact to expected future flows, and reversal when the same flows push prices away
   from fundamental value (S-024) — the sign depends on the state of the flow process.
4. Arbitragers who fail to act in time are forced to synchronise later, raising the price of
   liquidity and amplifying deviations (S-023).
5. The strategy that trades convergence is therefore exposed to a *crowding* risk: as more capital
   runs it, the price effect that generates the profit shrinks and the risk of a simultaneous exit
   rises (S-022, S-025). Crowding itself is measurable at the security level (S-026) and is
   associated with tail risk.
6. Hence: the expected value of a convergence trade is a function of (deviation, crowd depth,
   exit capacity), not of the deviation alone. The candidate's claim is that crowd depth is
   partially observable and is a *first-order* conditioning variable, not a risk-management overlay.

**Expected return source.** Compensation for supplying capital/liquidity to slow-moving,
constraint-bound arbitrageurs and institutions, plus the slow unwinding of price pressure away
from fundamental value (S-019, S-024).

**Originality.**
- *Closest known work:* the limits-to-arbitrage literature — Shleifer & Vishny's framing, Kondor
  [S-022], Abreu & Brunnermeier [S-023], Acharya/Shin/Yorulmazer [S-017], Duffie [S-019], plus
  empirical work on risk arbitrage [S-025] and on measurable crowding [S-026].
- *What is already known:* deviations persist; arbitragers are synchronised; crowding is a risk
  factor; crowding is measurable with slow, stale data.
- *Substantive differentiator claimed here:* a *trade specification* in which the crowd-depth state
  is the gate on both entry and exit, and in which the claim is about the **direction of the
  conditioning** (crowding raises expected convergence return in the short run because capital is
  slow, and lowers it while raising tail risk in the exit) — a two-sided relation that a simple
  "avoid crowded trades" rule does not capture. The related published result [S-026] finds
  crowdedness is associated with worse tail outcomes; it does not (to my knowledge) exploit the
  slow-capital mechanism to argue for *when* to take the convergence side.
- *Honest classification:* **informed variant of a documented family with a new conditioning
  variable.** The risk is that the conditioning variable is unobservable in a timely way (G-04), in
  which case this is a re-description of a known baseline.
- *Confidence in the comparison:* moderate.

**Target scope.** Cross-sectional equity pairs (industry-relative and single-name), merger-spread
and index-convergence style relative-value where measurable; holding horizons of days to months;
regime conditions: excluded during market-wide liquidity events where the crowd exits together.

**Observables.** The deviation (a concept-dependent spread); the crowd-depth state, in principle
from: reported holdings of arbitrage and multi-strategy funds (lagging, S-026), the dispersion of
analyst targets as a proxy for disagreement crowding, the concentration of option open interest
around the trade's strikes, aggregate short interest, the count and size of recently announced
comparable trades, and the fund-flow state of the strategy complex. All must be available with
their reporting lag accounted for.

**Rule sketch (descriptive, non-executable).** Identify convergence candidates (a specified
relative-value universe with a pre-defined fundamental anchor). Compute the deviation. Compute the
crowd-depth state from lagged observable proxies, and the exit-capacity state. Take the
convergence side only when the deviation is large *relative to the crowd depth* (i.e. the gap is
not already the consensus trade), size inversely to the crowd depth (capacity of the exit), and
pre-specify an exit that is spread over time and is suspended during market-wide liquidity events.
Maintain the crowd state as a first-class input to the sizing rule, not merely as a risk limit.

**Persistence thesis.** Slow capital, mandates, and reputation-driven capital immobility are
structural features of delegated asset management (S-017, S-020, S-021) and change slowly; the
deviations they create unwind slowly (S-019, S-024). It decays if capital becomes mobile
(electronically distributed advice, retail arbitrage platforms, internalised crossing), if
crowd depth is observable and therefore arbitraged away, or if the anchor itself becomes
contestable.

**Constraints.** Cost/liquidity: convergence trades are often in less liquid names; the spread is
paid on both legs and the trade is a market-neutral pair, so the cost is doubled. Capacity: the
capacity of the trade is the capacity of the *exit*, which is shared with the crowd — the
candidate's own sizing rule handles this, but it also caps the strategy's size at exactly the
moments the signal is strongest. Financing/financing cost: carry on a market-neutral pair is a
direct drag and can exceed the convergence payoff. Borrow: short legs in crowded names are the
most expensive to borrow exactly when the trade is most attractive. Market impact: taking the
crowded side of a small-cap pair is an impact machine. Venue/operational: paired execution adds
leg-risk. Short-sale constraints: borrow recalls can force early, adverse exits.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime-sensitive: the crowd
state itself is the regime. Tail: convergence trades have a classic left tail — the fundamental
anchor breaks (M&A fails, an accounting restatement) and the trade becomes a directional loss,
which is unrelated to the crowd state and therefore not hedgeable by the rule. Crash behaviour:
the crowd exits together, so the crowd state should be read as a *warning*, not merely a size
modifier. Hidden beta: convergence pairs in equities carry residual market, sector and factor
exposures; the state rule does not remove them. Correlated risks: all names in one crowded
strategy are the same trade.

**Falsifiable predictions and rejection conditions.**
1. *Conditioning direction:* convergence returns are larger when the deviation is large relative to
   crowd depth, and the relationship is non-monotone in crowd depth (higher in moderate crowding
   than in low crowding, lower in high crowding). **Kill:** the relation is monotone and
   negative throughout, in which case the candidate collapses into "avoid crowded trades" and
   should be reclassified as a known baseline.
2. *Tail asymmetry:* the left-tail severity of the strategy is higher in high-crowd states, and the
   rule's crowd gate reduces expected return but also reduces tail severity. **Kill:** no
   difference in tail severity across crowd states.
3. *Exit-capacity effect:* the reversal is faster in high-crowd states (the crowd's exit accelerates
   the convergence) but with worse gap risk. **Kill:** convergence speed is unrelated to crowd
   depth.
4. *Proxy validity:* the crowd proxy must be shown to carry information about the *actual* position
   concentration of arbitrage capital (validation against a holdings-based measure such as
   [S-026]). **Kill:** the proxy has no relation to the holdings-based crowding measure — in which
   case the candidate is not testable as specified (G-04) and must be parked.

**Main confounders and rival explanations.** Fundamental-break risk (the anchor is wrong) is the
dominant confounder and is not addressed by the crowd state; momentum is a rival explanation for
any positive convergence-return pattern (S-024) — the crowd state and momentum loadings must be
separated; liquidity premia (S-009-style) explain pairs returns without any slow-capital story;
crowding proxies are stale and may simply proxy for size, value or momentum factor exposures;
and the "crowdedness" literature already documents worse tail outcomes [S-026], so a naive
crowding-avoidance result is not evidence for this candidate.

**Data requirements and feasibility for a future independent validation.** Pair-level prices and
borrow costs; a defined universe and anchor; holdings-based crowding data [S-026] (or an
equivalent institutional holdings database) for proxy validation; optionally short interest and
option open interest. Feasibility: **medium** — the prices and the anchor are easy, the crowd
proxy is the bottleneck, and its reporting lag is a design constraint, not an implementation detail.

**Theory/evidence status.** Conceptual rationale: strongly supported [S-017, S-019, S-020, S-021,
S-023, S-024]. Mechanism supported by sources: yes for the slow-capital and synchronisation
channels; the *joint* crowd-depth conditioning of a convergence trade is an unresolved conjecture.
Prior empirical support reported by others: for crowding and tail risk [S-026]; for risk-arbitrage
characteristics [S-025]. Unresolved: the timely observability of crowd depth (G-04) and the
direction of the conditioning (prediction 1).

**Remaining uncertainty / confidence.** Confidence in the mechanism: high. Confidence in the
two-sided conditioning: moderate-to-low — this is the falsifiable core. Confidence in timely
observability: low-to-moderate. Priority score 74/100; rank 2 of 7 (rank 2 of 4 at Cycle 1;
unchanged). **Concrete next question:** is
the relation between convergence returns and crowd depth non-monotone as predicted, and can a
timely proxy for crowd depth be validated against a holdings-based measure?

---

## IDEA-005 — ROLLCOND: the scheduled commodity-index roll as a size-conditional liquidity demand, and the state that decides whether the concession survives

- **ID / short name:** IDEA-005 / ROLLCOND
- **Date added:** 2026-10-19 · **Cycle:** 2 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — first dossier. The underlying event (a scheduled passive roll) is
  documented, and the *headline* trade (front-running the roll) is documented as having decayed.
  The candidate is the **state-conditioned, provider-side** specification: the concession is
  predicted to survive only where the passive share of open interest is high and depth is thin.

**One-sentence hypothesis.** Commodity index trackers must move a long futures position from the
expiring contract into the deferred contract on a published calendar; because that demand is
price-insensitive, dated and knowable in advance, it buys a liquidity concession that a
*scheduled* provider can earn — but the concession exists only where the passive flow is large
relative to the contract's liquidity, a condition that is publicly observable and that has become
the binding constraint since electronification.

**Plain-language description.** Every month, on days the index provider has published years in
advance, a large pile of passive money has to move from one futures contract to the next. It does
not care what the price is; it has to be done. Whoever is standing on the other side of that
order gets a better price than the fundamentals justify, and the passive pays for it in
transaction costs. But the concession is only worth anything where the passive is a large share of
the market and the market is thin — in the deep, heavily arbitraged contracts, other dealers
supply that liquidity faster than the passive arrives, and the premium has disappeared.

**Mechanism (causal chain).**
1. Passive commodity exposure is obtained by holding long futures positions and rolling them; the
   index provider publishes the contract schedule and the roll schedule, and the S&P GSCI rolls
   monthly from the **5th to the 9th business day**, in fixed proportions 80/20 → 60/40 → 40/60 →
   20/80 → 0/100, with a documented procedure for holding roll weights if a market disruption
   event occurs (S-029). The clock is public and stable.
2. The regulator names the participant and the constraint: the CFTC's own explanatory notes define
   the "Index Traders" category in the Supplemental Commitments of Traders report as traders
   "replicating a commodity index by establishing long futures positions in the component markets
   and then rolling those positions forward from future to future using a fixed methodology"
   (S-030). The mechanism is documented by the regulator, not inferred from a price pattern.
3. The passive flow is not price-sensitive — exposure must be maintained whatever the price — so
   the price must move to ration a finite liquidity supply. The concession is the compensation
   paid to whoever supplies that liquidity, and it is a *cost* to the passive rather than a
   transfer from an informed counterparty.
4. The economically correct expression of "supply liquidity to a predictable large trade" is
   supplied *before* the trade, on a schedule, not raced against other speculators.
   Bessembinder, Carrion, Tuttle and Venkataraman (2016) model strategic trading around a
   predictable liquidation and find that competition among such traders improves market quality
   and increases the liquidator's proceeds (S-032) — the channel that the later literature labels
   "sunshine trading" (S-034). In their USO evidence the price imbalance around the roll "is
   almost entirely reversed within one minute in the expiring contract and within three minutes in
   the second nearest-to-expiration contract on roll days", and the passive fund pays real money
   for the privilege — they estimate roll trading costs averaging about three percent per year
   (S-032).
5. The size of the concession must scale with the passive flow relative to the *available
   liquidity* in the affected contract, and the relevant components are publicly observable:
   the passive's own position in the expiring contract (CFTC "Index Traders" positions, weekly,
   positions as of Tuesday, published Friday), the arbitrage/liquidity-supply state (managed money
   and swap dealer positions in the Disaggregated COT report), the contract's open interest,
   volume and depth, and the curve (whether the roll is into a more or less expensive deferred
   contract).
6. The state is not constant, and its evolution is the reason the published literature disagrees.
   Mou (2011) found the front-running profit depends on the size of index investment net of the
   arbitrage capital employed (S-035); Stoll & Whaley (2010) found index rolls have little futures
   price impact (S-036); Hamilton & Wu (2015) found that index-trader positions do not predict
   near-contract excess returns and that the oil relation breaks down out of sample (S-037); Yan,
   Irwin & Sanders (2022) find the impact of predictable rebalancing flows to be "modest and
   temporary" (S-034); and Irwin, Sanders & Yan (2023) find that the roll's impact on the
   nearby-versus-deferred spread **disappears in 2012–2019**, attributing this to the increase in
   liquidity supply from electronification (S-033).
7. These results are not inconsistent — they are measurements of an average dominated by the
   deepest contracts, in a period when the marginal liquidity supplier was a human on a floor. The
   candidate's claim is a *cross-sectional* one: the concession survives in the contracts where
   the passive share of open interest is high and the liquidity supply is thin, and vanishes in
   the deep ones. That is a prediction the aggregate time-series studies are not powered to see,
   and it is contradicted if the cross-section is flat.

**Expected return source.** Compensation for supplying liquidity to a dated, price-insensitive
demand shock — a *liquidity-provision premium* paid by the passive — collected by a participant
who is scheduled to be present rather than one who has to guess. The premium is bounded by the
passive's own execution cost (documented at roughly three percent per year for one large ETF's
roll in S-032), which is the ceiling on what can be harvested and also the reason the residual
after costs is hard to establish.

**Originality.**
- *Closest known work:* Mou (2011) "Front-Running the Goldman Roll" (S-035); Stoll & Whaley
  (2010) (S-036); Hamilton & Wu (2015) (S-037); Bessembinder, Carrion, Tuttle & Venkataraman
  (2016) (S-032); Yan, Irwin & Sanders (2022) (S-034); Irwin, Sanders & Yan (2023) (S-033);
  Tang & Xiong (2012) on index investment and the financialisation of commodities; and the
  inventory-based risk-premium literature (S-038, S-039).
- *What is already known:* that the passive exists, rolls on a published schedule, and is large
  in some contracts; that the roll moved the nearby-deferred spread before 2012 and that this
  reversed after the roll completed; that the impact in the deepest contract is transient and
  that the passive's execution cost is large; that the aggregate effect disappeared after 2012;
  and that index-trader positions do not predict near-contract excess returns.
- *Substantive differentiator claimed here:* (i) the **state** — the passive flow relative to
  liquidity, read directly from the regulator's own Index Trader positions — as a first-class
  conditioning variable, with a *sign* prediction (survival only in high-passive-share, thin
  contracts) that aggregate studies cannot produce; (ii) the **provider-side** expression rather
  than the front-runner-side one, which is the expression consistent with the "sunshine trading"
  evidence and with the documented decay of the front-running effect; and (iii) the
  **reconciling** claim: the published null is a composition effect of deep contracts, not a
  statement that the mechanism is dead everywhere.
- *Honest classification:* **documented and contested effect family; the candidate is a
  state-conditioned, provider-side refinement.** This is not a new effect and must never be
  presented as one. Its value is that the *state* is public, the *dates* are public, and the
  family has a documented, peer-reviewed null that the candidate must survive.
- *Confidence in the comparison:* moderate-to-high. The closest work (S-035) and the three
  peer-reviewed studies that contradict it (S-032, S-033, S-034) were read at the level of
  abstracts, publisher records and the CFTC-hosted full text of S-035; S-032 was read in the
  author-hosted PDF. The claim that "nobody has conditioned the roll impact on the passive share
  of open interest" is **not** established exhaustively and is labelled a conjecture.

**Target scope.** US-traded commodity futures (CME, CBOT, NYMEX, ICE US) that are components of
passive commodity benchmarks; the first-nearby (expiring) and second-nearby (deferred) contracts;
holding horizon intraday to a few sessions around each monthly roll; per commodity and per
contract; regime conditions: not in delivery months, not when a price limit or a market
disruption event suspends the roll (the provider's own roll-weight adjustment rule applies),
and not in a contract whose liquidity has collapsed in the roll week.

**Observables (knowable at decision time, conceptually).**
- The published roll calendar, per-day roll weights and the market-disruption adjustment rule
  (S-029) — known years ahead, so no look-ahead.
- The CFTC Supplemental "Index Traders" position in the expiring contract, from the report
  published on Friday for positions as of the prior Tuesday (S-030, S-031) — available with a
  known five-day lag, and applied to a *scheduled* future date, so the lag is not a look-ahead.
- Managed money and swap dealer positions for the same contracts (Disaggregated COT), as the
  arbitrage/liquidity-supply state (S-030, S-031).
- Contract open interest, traded volume, quoted spread, depth, and the size of the passive flow
  implied by the index weight change and index scale.
- The nearby-to-deferred price spread and the cost-of-carry bound it is measured against.
- *Timing hazards to flag for the validator:* weekly COT data with a five-day publication lag
  (a decision taken on a roll day uses the previous Friday's report); the roll can be extended or
  held by a market disruption event (S-029); contract specifications and index methodologies
  change (the S&P GSCI Enhanced family uses a different, partly dynamic roll schedule, S-029);
  delivery months and first notice days distort the expiring contract; and the COT "Index Traders"
  category itself contains classification error and includes some non-index activity (S-030).

**Rule sketch (descriptive, non-executable).** For each component commodity of the passive
benchmark universe, on each roll day: compute the passive-flow-to-liquidity ratio from the most
recent published Index Trader position in the expiring contract divided by that contract's open
interest; screen to contracts where the ratio is high and the contract's depth is small relative
to the expected roll notional; take the position on the side *opposite* the passive's roll — that
is, supply the liquidity the passive requires — with the size bounded by a fraction of the
expected roll notional and by the contract's depth; exit on a pre-specified schedule tied to the
completion of the roll, with the exit window defined in advance. Exclusions: delivery months,
contracts under a price limit, contracts in which the passive share is small, and any contract
where the liquidity in the roll window has visibly collapsed.

**Persistence thesis.** The passive's need to trade is a mandate, not a view, and it is renewed
every month, so the demand recurs; a provider who can be *scheduled* rather than reactive keeps a
structural edge over a front-runner who must locate the flow in real time. The premium persists
where the alternative liquidity supply is thin. It decays — and has decayed, on the published
evidence — where liquidity supply becomes elastic (electronification, S-033) or where arbitrage
capital pre-positions the roll in advance (the alternative explanation for the post-2012 null).
Both decay channels are observable, which is the point of the state variable.

**Constraints.** Cost/liquidity: thin contracts have wide spreads, and the passive's own execution
cost (~3% per year in the USO case, S-032) bounds the harvestable premium; the strategy consumes
exactly the liquidity it is trying to price. Capacity: per contract and per roll the capacity is
bounded by the passive flow actually present, so it scales with passive assets, not with the
strategy's own balance sheet. Financing/margin: futures require margin, and a position that is
short the deferred contract carries margin that moves with volatility. Market impact: taking the
opposite side of a large scheduled flow in a thin contract is an impact machine. Venue/operational:
exchange position limits, delivery rules and price limits; a market disruption event can change
the roll schedule mid-flow (S-029). Shorting constraints: not a borrow-constrained trade, but
futures shorting is margin- and limit-constrained, and in a thin contract the position can be
expensive to exit exactly when it must be unwound.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: entirely state-
dependent by construction — in deep, liquid, heavily arbitraged contracts the candidate predicts
no edge at all, which is the majority of contracts by notional. Tail: the position is short one
leg of a curve; a sudden supply shock (a real production failure, a policy change, a war) moves
the whole curve, and the position is short the deferred contract into a rising price. Crash
behaviour: in a liquidity crisis the thin contracts are the least liquid and the position is
hardest to exit; the passive's own roll is also least well executed then, which cuts both ways.
Hidden beta: the position is short a deferred commodity contract, i.e. it is a short position in
the "carry" component of commodity returns, and will load on the momentum/carry factors and on
the dollar. Correlated risks: every commodity's roll falls in the same five days of the month, so
the book is a single month-end-dated bet on the passive complex; a single contract blow-up
dominates many small contract-level results.

**Falsifiable predictions and rejection conditions.**
1. *Cross-sectional survival:* the roll-period price concession (the deviation of the
   nearby-to-deferred spread from its no-arbitrage carry bound) is larger in contracts with a
   high passive share of open interest than in contracts with a low passive share, in the same
   period and the same commodity. **Kill:** the relation is flat or reversed across contracts.
2. *Liquidity condition:* the concession is larger in the thinnest contracts (measured by depth or
   by the passive flow relative to open interest) and negligible in the deepest. **Kill:** the
   concession is proportional to the passive flow but not to liquidity, or is present in the deep
   contracts too.
3. *Post-roll reversal:* the deviation reverses after the roll completes, and the reversal is
   larger the larger the deviation was. **Kill:** no reversal, or a reversal fully explained by
   the carry bound moving (a change in storage/financing costs) rather than by the flow.
4. *Modern-period survival:* the effect is not absent in 2012–present in the thin, high-passive-
   share contracts, notwithstanding the published aggregate null (S-033). **Kill:** the effect is
   absent in every contract in the modern period — in which case the candidate is dead and the
   published null is a statement about the whole market, not a composition effect.
5. *Discriminating the decay channel:* if the decay is due to *arbitrage capital pre-positioning*,
   the concession should be smallest in contracts where managed money positioning in the deferred
   contract is already high before the roll; if it is due to *electronification and liquidity
   supply*, the concession should be smallest in contracts with the deepest order books and
   unchanged in thin contracts with little pre-positioning. **Kill:** neither pattern holds.
6. *Cost floor:* the realised concession per contract exceeds the round-trip cost of the trade
   (spread, commission, slippage, margin financing) in the contracts the rule selects.
   **Kill:** the gross concession is smaller than the cost in every selected contract.

**Main confounders and rival explanations.**
- *Electronification and liquidity supply* (S-033) — the leading rival: the effect may be gone
  everywhere, and the cross-section may be a story about measurement rather than about markets.
- *Arbitrage capital pre-positioning* — the roll may be pre-absorbed by spread traders, so there
  is nothing to supply; Mou (2011) found profitability depends on the balance of index
  investment against arbitrage capital (S-035), which is a state, not a constant.
- *Fundamental news* — commodity fundamentals move on the same calendar as the roll (USDA, EIA,
  OPEC, weather); a spread move that coincides with a fundamental repricing is not a liquidity
  concession.
- *Carry and storage economics* — the nearby-deferred spread is driven by convenience yield and
  storage costs, which are themselves state-dependent (S-038); a "deviation from the carry bound"
  must be measured against a *state-dependent* bound, not a constant.
- *Hedging pressure* — producer hedging is a separate, documented driver of futures risk premia
  (S-039) and can move the same spread for the same calendar reasons.
- *Classification error in the COT data* — the Index Traders category contains non-index activity
  and excludes some index traders (S-030), and it is reported at the trader level with a weekly
  lag.
- *The candidate may be a dressed-up basis-convergence trade* — the commodity basis-convergence
  literature was not retrieved this cycle and must be checked (gap G-06). If the concession is
  simply a convergence-to-carry trade with a calendar catalyst, it is a variant of a known
  baseline and must be reclassified.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: futures settlement and trade prices by contract
month, open interest and volume (exchange data); CFTC Supplemental CIT and Disaggregated COT
reports (S-030, S-031); the index's contract weights, roll schedule and index scale (S-029, and
a passive-asset scale series — see G-07). Feasibility: **medium-high** for the cross-sectional
event study (all inputs are public and the calendar is fixed); **medium** for the state
construction (COT classification error and a five-day lag); **medium** for the cost model (thin
contract fills are the binding assumption and must be justified independently).

**Theory/evidence status.**
- *Conceptual rationale:* supported — price pressure from non-price-sensitive scheduled demand
  (S-038, S-039) and the economics of liquidity provision around predictable large trades (S-032).
- *Mechanism supported by sources:* **yes** for the participant, the constraint and the dated
  schedule — the regulator documents the Index Trader roll methodology (S-030) and the provider
  documents the roll calendar (S-029).
- *Prior empirical support reported by others:* mixed and contested. Support for a pre-2012
  effect: S-035 (working paper, non-refereed). Support for transience and high costs: S-032.
  Support for modest and temporary impact: S-034. Evidence of an aggregate null post-2012: S-033.
  Evidence that index-trader positions do not predict near-contract excess returns: S-037 and
  S-036. None of these is reproduced here.
- *Unresolved:* whether any cross-sectional residual survives in the modern period, and which
  decay channel (liquidity supply or pre-positioning) is responsible for the published null.

**Remaining uncertainty / confidence.** Confidence that the participant, the constraint and the
schedule are real and publicly dated: **high** (regulator and provider documentation).
Confidence that a *harvestable* concession survives today: **low-to-moderate** — three
independent peer-reviewed lines point the other way for the aggregate and for the deep contract.
Confidence in the state-conditioning as the right way to resolve the disagreement: **moderate** —
it is the only formulation found that both (a) uses a public variable and (b) predicts a
*sign* change rather than a smaller magnitude. Priority score **72/100**; rank 3 of 7 at the time
of writing. **Concrete next question:** is the roll-period concession in the nearby-to-deferred
spread a function of the passive share of open interest and of contract depth, and does it survive
in 2012–present in the thin, high-passive-share contracts where the published aggregate null
(S-033) says it should not exist?

---

---

## IDEA-006 — FIXCLOCK: the end-of-day deadline cluster, and the concession that the clock rents

- **ID / short name:** IDEA-006 / FIXCLOCK
- **Date added:** 2026-10-19 · **Cycle:** 2 · **Status:** retained (not in the top three),
  **blocked on G-11** · **Version:** 1.1
- **Change notes:** v1.0 — first dossier. The intraday periodicity around the London fix is an
  established fact; the candidate is the *deadline-constrained flow* reading of it, extended to
  the post-US-close settlement window that the T+1 transition created. **v1.1 — reclassified after
  the G-09 closure pass (S-074 … S-081): the *fix* half of the deadline cluster is published —
  the price impact of price-insensitive hedging demand at the fix, its temporary character and
  the pre-fix/post-fix reversal are all in the literature — so the aggregate version of this
  candidate was rejected (R-007) and the dossier was narrowed to two residuals: the
  *settlement-side* deadlines beyond the fix (blocked on G-11) and the post-2015 persistence of
  the published fix effect.**

**One-sentence hypothesis.** The FX day ends with a cluster of hard, published deadlines — the
16:00 London benchmark fix, the CLS currency-close and pay-in deadlines, and, since May 2024, the
need to arrange currency for US securities settlement in the two hours after the US equity close —
and the flows those deadlines force are not price-sensitive; **the fix's own concession is already
published**, and the candidate's residual claim is that the *settlement-side* deadlines impose a
separable, additional price-insensitive demand in a window that is not a benchmark, and that the
published fix effect survives the 2015 methodology revision and the post-2013 enforcement regime
at a cost a new participant can still capture.

**Plain-language description.** Once a day, the world's currencies have to be struck. Funds that
are valued at the London fix, mandates that must transact at it, and settlement members who have
to have the right currency in the right place by a cut-off all have to trade in a very short
window whether they want to or not. That is a predictable, dated, price-insensitive demand for
liquidity, and it is the same economics as a futures roll, but repeated every single day and
concentrated in minutes.

**Mechanism (causal chain).**
1. The benchmark is documented and dominant. The FSB's review of FX benchmarks states that the
   "WM/Reuters (WMR) 4pm London fix … is by far the dominant benchmark being used, not just in
   FX, but also as a key input in multi-currency equity, bond and credit indices", that "most
   investment mandates are benchmarked against global equity indices … or credit indices … that
   use the WMR 4pm London fixing for FX valuation and transaction purposes", and that "while
   management type pension trusts commonly reference the WMR 4pm London fix to execute FX
   transactions", investment trusts tend to transact without referencing the benchmark (S-044).
2. The clock is published and hard. The benchmark administrator publishes the closing spot rates
   "daily Monday–Friday at 4:00 pm London time", the calculation window was widened from one
   minute to five minutes on 15 February 2015 after the IOSCO/FSB recommendations, and the FCA
   brought the 16:00 fix into its regulatory regime (S-045, S-046).
3. The flow is large enough to matter and is measurable in the data: "for several currencies,
   there are a few days when the 1-minute WMR 4pm London trading window can account for over 10%
   of the platform's daily trading volume" (S-044). On those days the fix window is not a
   footnote; it is a tenth of the day's turnover executed in one minute.
4. The settlement side adds a second, harder deadline. CLS requires payment instructions to meet
   "stringent requirements in terms of payment deadlines"; the final pay-in schedule is
   disseminated at 06:30 CET, funds are called from 07:00 CET, currency close deadlines fall at
   midday, and — since the US and Canadian move to T+1 settlement in May 2024 — instructions must
   be submitted by 00:00 CET on day T+1, so that "when the US equity market closes at 16:00 EST
   (22:00 CET), time is limited for the associated currency trading" and "in extremis, there is a
   reduced window of only two hours to arrange the submission to CLS" (S-048, S-049).
5. The flow is not price-sensitive: a fund that must transact at the fix, and a settlement member
   that must fund a payment instruction by a cut-off, transact to satisfy a deadline, not a view.
   The price must therefore move to ration the available liquidity in the window, and the
   concession is the compensation for supplying it — the same economics as the futures roll in
   IDEA-005 (S-032) and as the "sunshine trading" literature (S-034).
6. **The fix half of this chain is already published, in the form the candidate claimed.** Melvin
   and Prins (2015) show that passive hedging flows executed at the fix "predict the direction of
   temporary exchange rate movements at this time of day", concentrated at end of month, where
   "hedging demand has a strong, but temporary, impact on exchange rates" (S-075); Evans (2018)
   documents "negative serial correlation in price changes around the WRM Fix" and models the fix
   order as an optimal-execution problem (S-076); Ito and Yamada (2015) document "the negative
   autocorrelation of the Forex rate between the pre- and post-fixing periods, particularly at the
   end-of-month trading day" (S-077); Michelberger and Witte (2016) document the increased
   volatility and size of movements around 4pm (S-074); and He (2026) reports a W-shaped pattern in
   which "the dollar climbs before FX fixes and falls after them" for the nine most traded
   currencies over 21 years (S-081). **Consequence:** the price-insensitive-deadline-flow
   concession, its temporary character, its end-of-month concentration and the pre-fix/post-fix
   reversal are all established results. The candidate cannot be the fix.
7. Because the clock repeats every day, a participant can be *scheduled* into it rather than
   having to detect it, and the object of study is the intraday price path around a known
   timestamp, not a multi-year return.
8. The macro-news confound is manageable and is itself a discriminator: the standard US releases
   (08:30 and 10:00 ET) and the European releases (09:00–10:00 London) fall before 16:00 London,
   so the fix window is not *typically* a scheduled-information window. Some releases can still
   fall close to it, which is why the rule excludes any day with a scheduled release inside the
   window rather than relying on the average. That exclusion is what makes any residual pressure
   attributable to the institution rather than to the news.

**Expected return source.** The liquidity-provision concession paid by deadline-constrained flow
to the participant who supplies liquidity into the deadline; equivalently, the price at which
deadline-driven demand is rationed. On the equity side of the same clock, the analogous object is
the concession the passive pays in the closing auction. **For the fix, this source is already
documented and the price effect is published (S-075, S-076, S-077) — the residual's return source
is therefore the settlement-side deadline flow, whose effect is not established in any located
paper.**

**Originality.**
- *Closest known work:* the FSB/IOSCO benchmark reviews and the FSB's 2014 final report, which
  itself lists "the behaviour of market participants around the time of the major FX benchmarks
  (primarily the WMR 4pm London fix)" as a workstream (S-044); the BIS account of the benchmark
  reform (S-046); the CLS documentation of the settlement schedule (S-048, S-049); and — read in
  the G-09 closure pass — **the fix literature itself**: Melvin and Prins (2015) on equity hedging
  and the London fix (S-075), Evans (2018) on trading around the WMR fix (S-076), Ito and Yamada
  (2015) on pre/post-fixing autocorrelation (S-077), Michelberger and Witte (2016) on the
  microstructure of the fix window (S-074), Benenchia, Galati and Lepone (2025) on the
  post-revision benchmark (S-080), Evans and Lyons (2002) on order flow in FX generally (S-078),
  Osler (2003) on order clustering as a rival mechanism (S-079), and He (2026) on the
  W-shaped pattern around global fixings (S-081).
- *What is already known:* that the fix window is a distinct, heavy, institutionally-driven slice
  of the trading day; **that the price-insensitive flow at the fix moves the price in a
  predictable direction and only temporarily; that the effect is strongest at end of month; that
  the pre-fix/post-fix return autocorrelation is negative; and that the 4pm window is
  distinguishable from the rest of the day by larger moves and higher volatility.** All of that
  is published (S-074 … S-077, S-081).
- *Substantive differentiator claimed here — the residual, and only this:* (i) the
  **settlement-side** deadlines — the CLS currency-close and pay-in cut-offs and the post-US-close
  window that T+1 created (S-048, S-049) — as a *separable* source of price-insensitive currency
  demand that is **not** a benchmark and is therefore not covered by any of the fix literature
  located in the G-09 pass; (ii) whether the **published fix effect survives the 2015 methodology
  revision** (the calculation window was widened from one minute to five) and the post-2013
  enforcement and remediation regime — the fix literature read so far largely predates or does not
  price the reform; and (iii) whether any of it is **harvestable after costs by a new participant**,
  which none of the located papers addresses.
- *Honest classification:* **a published effect with a narrow, unclaimed extension — and an
  extension that is not yet cleared of the literature.** The aggregate version of this candidate
  (a deadline-driven concession at the end-of-day clock) is published (S-075, S-076, S-077,
  S-074, S-081) and was therefore **rejected as a candidate (R-007)**. What remains is the
  settlement-side residual and the post-reform persistence question, and the first of those is
  **blocked on G-11**: no search of the settlement-side or T+1-window literature has been
  performed, so "unclaimed" is currently an *expectation*, not a finding. This dossier must never
  be described as a discovery of the fix's price impact.
- *Confidence in the comparison:* **high for the fix, low for the residual.** Every item in
  S-074 … S-081 was re-verified directly against Crossref, the arXiv record, the NBER record or
  the publisher listing in this pass, and the DOIs that a read-only verification agent reported
  for three of them were wrong and were corrected (the errors are recorded in the G-09 gap
  entry). The residual side is weaker: G-11 is open, and the fix literature's own data
  (administrator- and dealer-provided tick data) mean that a "nobody has tested this" claim
  about the settlement side must be earned, not assumed.

**Target scope.** Spot and forward FX in the major pairs and the most fix-traded crosses; the
16:00 London fix window and the 16:00–18:00 ET post-US-close window; holding horizon intraday
(minutes to hours); per currency pair; regime conditions: exclude days with scheduled macro
releases inside the window, exclude days around benchmark methodology changes or fix suspensions
(the administrator publishes holiday and methodology notices, S-045), exclude periods of market
disruption.

**Observables (knowable at decision time, conceptually).**
- The published benchmark calendar and methodology, including the five-minute calculation window
  and the holiday/methodology notices (S-045) — known in advance.
- The published CLS settlement timeline: pay-in schedule issue, currency close deadlines,
  rescission deadlines, and the 00:00 CET initial-pay-in deadline introduced with T+1 (S-048,
  S-049).
- The fix-window volume share of daily volume by platform and currency (S-044 reports that this
  can exceed 10% on some days) — the *state* that should scale the effect.
- The month-end and quarter-end calendar, and the equity-close-to-CLS-deadline interval.
- Intraday prices, spreads and depth around the fix and around the post-US-close window.
- *Timing hazards to flag for the validator:* proprietary data (the tick data used in S-047 were
  provided by the benchmark administrator; platform-level volume shares are not public time
  series); benchmark holidays and method changes; the interaction with macro releases; the
  migration to T+1 in May 2024, which is a *regime break* in the data; and the fact that the
  benchmark administrator's own surveillance function may alter behaviour at the fix.

**Rule sketch (descriptive, non-executable).** Each day, for each currency pair in scope:
identify the **settlement-side** windows from the published CLS schedule (the currency-close
deadline, the 00:00 CET initial-pay-in deadline on day T+1 and the post-US-close interval) and,
separately, the fix window (16:00 London ± the published five-minute calculation window) as the
*control* to be reproduced, not traded; determine from the published calendar whether the day
carries deadline-amplifying features (month-end, quarter-end, ex-dividend date, T+1-related
settlement peak) and exclude days with scheduled macro releases inside the window; measure the
recent fix-window volume share for the pair as the state variable; take the position on the side
that *supplies* liquidity to the settlement-deadline demand — that is, against the direction in
which deadline-constrained flow must transact — sized as a small fraction of the pair's normal
depth; exit at a pre-specified time after the window closes, with the exit rule fixed in advance
of the trade.

**Persistence thesis.** The deadlines are contractual and institutional: benchmark mandates,
settlement obligations and the T+1 settlement cycle do not go away, so the flow recurs every
single day and re-amplifies at month-end. The concession is competed away only if liquidity
supply becomes perfectly elastic at the exact timestamp — the same decay channel as IDEA-005
(S-033) and the same reason the state variable is essential.

**Constraints.** Cost/liquidity: the concession is measured in pips inside a few minutes, so
spread and slippage are first-order; this is the binding constraint of the whole candidate.
Capacity: bounded by the fix-window depth of the pair and by the size of the deadline-constrained
flow. Market impact: trading *into* a concentrated deadline window is an impact machine.
Venue/operational: the fix is a benchmark calculation, not an execution venue — the trade must be
executed around it, not at it; execution infrastructure around the fix is expensive.
Financing/margin: negligible for spot, relevant for leveraged forward positions. Shorting
constraints: not a borrow-constrained trade.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: entirely
deadline-dependent — on an ordinary day the deadline flow is small; at month-end or on a T+1
settlement peak it is not. Tail: a market disruption (a failed settlement, a benchmark
suspension, a forced closure) is exactly when the deadline binds hardest and when liquidity is
worst, so the position is most likely to be held exactly when it cannot be exited — the same
"most crowded, least liquid" trap that governs IDEA-002. Crash behaviour: a benchmark
suspension removes the trade entirely; a settlement stress can force the deadline to bind on
multiple currencies simultaneously. Hidden beta: the position is a short/long in the *funding
currency* around a deadline, so it loads on the funding-coinage and the basis trade, and can
carry an event risk that is not visible in the return.

**Falsifiable predictions and rejection conditions.**
*Baselines to reproduce, not predictions (the published fix results; a validator must reproduce
them and must never report them as a finding):* the directional pre-fix move in the direction of
net deadline-constrained demand, the partial post-fix reversal, the end-of-month amplification, and
the elevated volatility in the fix window (S-075, S-076, S-077, S-074, S-081).
*The candidate's own, residual predictions:*
1. *Settlement-side separability:* the post-US-close / settlement-deadline window shows an
   imbalance in the direction of the funding requirement, **after** the fix-window effect has been
   removed, and the pre-T+1 sample does not. **Kill:** the window shows no imbalance, or the
   pre- and post-T+1 samples are indistinguishable, or the effect vanishes once the published fix
   effect is controlled for.
2. *Post-reform persistence:* the published fix effect (S-075, S-076) is materially smaller after
   the 2015 widening of the calculation window from one minute to five and after the post-2013
   enforcement and remediation regime than before it. **Kill:** the effect is unchanged across the
   break, which would mean the pre-reform result is either still live or was never a regime
   artefact — either way, the *new* state conditioning this candidate would need is not there.
3. *State scaling:* the size of the pre-fix move is increasing in the fix-window volume share
   (S-044). **Kill:** no relation, or the relation is only with the currency's overall liquidity
   rather than with the fix-window share.
4. *Calendar amplification:* the effect is larger at month-end, quarter-end and on high-settlement
   days. **Kill:** no calendar dependence.
5. *Cost floor:* the realised concession exceeds round-trip cost in the pairs selected.
   **Kill:** the gross concession is smaller than the spread plus slippage in every pair.
6. *Reflexivity:* the effect weakens over the sample as more participants learn it. **Kill:** no
   decay, which would suggest the mechanism is something else (for example a macro-news artefact
   that the exclusion rules failed to remove, or the Osler-style order-clustering mechanism,
   S-079, which produces the same pattern without any deadline story).
7. *Gate:* **G-11 must be closed before any of the above is treated as a candidate rather than a
   hypothesis.** If a published paper already shows a settlement-side or T+1-window price effect,
   the candidate is rejected, not narrowed.

**Main confounders and rival explanations.**
- *Macro news timing* — the dominant rival; the discriminator is the no-release day, and the
  exclusion rule must be applied before any result is read.
- *Benchmark administrator surveillance and fix engineering* — the calculation window was widened
  in 2015 and the methodology has changed repeatedly, so the "fix" is not a constant object across
  the sample (S-045, S-046).
- *Market-making and internalisation* — a large share of FX volume is internalised and never
  prints; the observed print-level flow is not the true flow.
- *Statistical artefact of daily data* — most public FX data are daily, so an apparent
  "intraday" effect measured on daily data is a different object; a validator must not
  substitute daily for intraday data.
- *The same deadline economics already priced* — if the fix-window concession is fully arbitraged
  by the liquidity providers who are already present (the "sunshine" equilibrium of S-032, S-034),
  there is nothing left; the candidate must show the concession accrues to a *new* participant
  rather than to those already stationed there.
- *T+1 as a one-off* — the settlement-window claim rests on a structural change that has already
  happened; a claim that depends on the *change* is a one-off event study, not a candidate.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: the benchmark calendar and methodology (S-045);
the CLS settlement timeline (S-048, S-049); the macro calendar. Commercial: intraday tick and
order-book data for the major pairs from at least one platform contributing to the fix — the
dataset used in the peer-reviewed work was provided by the benchmark administrator (S-047) and is
**not** freely available, and the fix literature read in the G-09 pass used a decade of
tick-by-tick data for 21 currency pairs (S-076) and administrator-provided high-frequency data
(S-074, S-080), none of which is public; this is the single largest feasibility constraint on
this candidate, and it applies to the *residual* test as much as to the reproduction of the
published fix result. Feasibility: **low-to-medium** for a rigorous intraday test; the public
proxy (fix-window volume share) is not published as a time series.

**Theory/evidence status.**
- *Conceptual rationale:* supported — price pressure from non-price-sensitive demand and the
  economics of liquidity provision around predictable large trades (S-032, S-034).
- *Mechanism supported by sources:* **yes** — the participant set, the deadline and the size of
  the flow are documented by an international regulator (S-044), the benchmark administrator
  (S-045) and the settlement utility (S-048, S-049).
- *Prior empirical support reported by others:* the fix-window price effect is **published and
  strong** — the temporary, end-of-month-concentrated impact of passive hedging demand at the fix
  (S-075), the negative serial correlation around the fix (S-076), the negative pre/post-fixing
  autocorrelation (S-077), the elevated volatility and movement size around 4pm (S-074), the
  W-shaped dollar pattern around global fixings (S-081), and the benchmark's own post-revision
  reassessment (S-080). **None of it is reproduced here, and none of it supports the residual.**
- *Unresolved:* whether the *settlement-side* deadline flow has a separable price effect (blocked
  on **G-11**), whether the published fix effect survives the 2015 methodology revision and the
  post-2013 enforcement regime, and whether any of it survives the cost of trading it.

**Remaining uncertainty / confidence.** Confidence that the deadlines, the participant set and the
flow concentration are real and published: **high**. Confidence that the *fix's* flow moves prices
in a predictable direction: **high, and it is no longer a discovery** (S-075, S-076, S-077,
S-074, S-081). Confidence that the *settlement-side* residual is real and unclaimed: **low** —
G-11 is open, so this is an expectation rather than a finding. Confidence that any of it is
*harvestable* after costs: **low** (this is the decisive weakness; the candidate may be a
structural understanding with no exploitable residual, and the fix half of it is now a published
effect that the liquidity providers who are already stationed there will have arbitraged).
Priority score **59/100** (down from 66 after the G-09 closure); rank 7 of 7 at the time of
writing, below the parked IDEA-002. **Concrete next question:** does any published work test the
*settlement-side* deadlines — the CLS currency-close and pay-in cut-offs, and the post-US-close
window created by the May 2024 T+1 transition — as a price determinant rather than as an
operational schedule, and if not, does the settlement window show a directional imbalance that
survives removal of the published fix effect?

---

## IDEA-007 — FUNDSTATE-FX: the dollar as the funding currency, and the cross-section of who feels it

- **ID / short name:** IDEA-007 / FUNDSTATE-FX
- **Date added:** 2026-10-19 · **Cycle:** 2 · **Status:** retained (not in the top three) ·
  **Version:** 1.1
- **Change notes:** v1.0 — first dossier. This is IDEA-002's mechanism taken to the venue where
  the funding state is *published*; the register's answer to the state-proxy question is that the
  venue, not the proxy, determines feasibility. **v1.1 — reclassified after the funding-currency
  source closure (S-055 … S-073): the aggregate funding-state → carry-return relation is a
  published, peer-reviewed baseline with a positive result, so the aggregate version was rejected
  (R-006) and this candidate's residual claim was narrowed to the cross-sectional dependence
  structure.**

**One-sentence hypothesis.** The dollar is the world's funding currency, so the growth of
dollar-denominated liabilities of the intermediaries who supply that funding is a public,
slow-moving state that moves the dollar; the aggregate version of that relation is already
published (S-055), and the candidate's residual claim is that the *cross-sectional* version — which
currencies' exchange rates move when dollar funding expands, and by how much — is a distinct,
testable object that the literature read so far does not establish, and that it is tradeable
because the state is published on a known calendar.

**Plain-language description.** When the world's banks and borrowers take on more dollar
liabilities, the dollar tends to appreciate against most other currencies. The interesting part is
not that the dollar moves on average but that it should move *more* against the currencies whose
own borrowers depend most on dollar funding — and that dependence is measurable from published
banking statistics.

**Mechanism (causal chain).**
1. The dollar is the funding currency: the largest and most central funding market in the world
   is a dollar market, and dollar liabilities of financial intermediaries are the balance-sheet
   expression of that fact.
2. The mechanism is documented and modelled: "we present evidence that the growth of
   U.S.-dollar-denominated banking sector liabilities forecasts appreciations of the U.S. dollar,
   both in-sample and out-of-sample, against a large set of foreign currencies" and "we provide a
   theoretical foundation for a funding liquidity channel in a global banking model where exchange
   rates fluctuate as a function of banks' balance sheet capacity"; the authors further note that
   "this channel is separate from the more familiar 'carry trade' channel" (S-052). The closely
   related peer-reviewed work amplifies the same channel (S-053).
3. **The aggregate version of this idea is already published, with a positive result.** Filipe,
   Nissinen and Suominen (2023) measure funding constraints by deviations from covered interest
   parity, define funding risk as the dispersion of those deviations, and find that funding risk
   explains carry trading activity, carry returns and carry-long/short correlations, with a model
   in which the investment and the funding currency crash together relative to a safe asset when
   constraints bind (S-055). The state variable's own determinants are understood: covered
   interest parity has been systematically violated since the crisis because dollar hedging demand
   meets balance-sheet-constrained arbitrage (S-056, S-057), and the dollar's strength moves with
   both CIP deviations and cross-border dollar lending contraction (S-059). **Therefore the
   candidate cannot be the aggregate version.** It must be the cross-section: which currencies
   respond to a given dollar funding expansion, and by how much.
4. The state is *published*: the BIS locational banking statistics publish cross-border positions
   by residence, currency and counterparty sector on a fixed quarterly calendar, and the BIS
   publishes regular statistical releases on international banking statistics and the global
   liquidity indicators (S-054). The state therefore has a known, slow, publication schedule — no
   look-ahead, no proprietary data. **Important constraint discovered in the source-closure pass:**
   the *fast* version of this state — the cross-currency basis itself — is **not published
   anywhere**: the BIS statistics catalogue contains no cross-currency basis series, and the
   published funding-constraint studies construct it from paid vendor forwards (S-055). A candidate
   that wants a daily funding state must build it from market quotes and must say so.
5. The cross-section follows from the mechanism rather than from the correlation: if a dollar
   funding expansion tightens the balance sheet of the intermediaries who supply dollar funding,
   the currencies whose own borrowers rely on that funding should adjust more than currencies
   whose borrowers are insulated from it. The candidate's claim is that this heterogeneity is
   the object of study, and that it is measurable *ex ante* from the same published statistics.
6. The signed prediction is the discriminator: the published time-series result has the dollar
   appreciating when dollar funding liquidity expands (S-052). That is the *opposite* sign to the
   familiar carry-crash mechanism, in which a funding squeeze forces the funding currency to
   appreciate and high-carry currencies to collapse. A candidate must therefore specify which
   channel it is trading and must not blend them.
7. The dated flow element: the state updates on a published calendar (quarterly), and the funding
   book itself rolls on the international value dates, so the state is revised at known dates and
   the position is a slow, calendar-driven holding rather than a fast signal.

**Expected return source.** Compensation for supplying dollar funding in the states where the
funding premium is positive, and the corresponding movement of the currencies whose funding
dependence is highest — a *funding premium*, distinct from the level of carry, and distinct from
the FX risk premium.

**Originality.**
- *Closest known work:* **Filipe, Nissinen and Suominen (2023)**, who already use covered interest
  parity deviations as a funding-constraint state and show that the resulting "funding risk" drives
  carry returns and carry activity (S-055) — this is the single closest work and it is
  peer-reviewed with a positive result; Adrian, Etula and Shin's funding-liquidity channel (S-052),
  with the related peer-reviewed version (S-053); the cross-currency-basis literature that explains
  what the state *is* (S-056, S-057, S-058, S-059, S-069); the carry-crash and global-liquidity
  literature (S-065, S-066, S-067, S-068, S-070, S-072); the explicit "funding currency" construct
  and its recent formalisations (S-061, S-062, S-063, S-064); and the published banking statistics
  (S-054).
- *What is already known:* that the growth of dollar-denominated intermediary liabilities forecasts
  dollar appreciation in and out of sample, at weekly, monthly and quarterly horizons (S-052); that
  the channel is distinct from the carry channel in that paper (S-052); that covered interest parity
  has been systematically violated since the crisis and that the violation reflects dollar hedging
  demand against balance-sheet-constrained arbitrage (S-056, S-057); that the dollar's strength
  tracks CIP deviations and cross-border dollar lending contraction (S-059); that the funding
  constraints implied by CIP deviations predict carry returns, carry activity and carry
  correlations (S-055); that the "funding currency" is a named and defined concept whose pricing
  kernel anchors currency-specific risk–return relations (S-061, S-062); that hedging demand is an
  exchange-rate determination channel in its own right (S-063); that the dollar dominates
  cross-border banking and that dollar funding is raised in different places from where it is
  provided (S-054, S-070); and that the crisis-period funding state is an official, documented
  phenomenon (S-058, S-060, S-072).
- *Substantive differentiator claimed here:* (i) the *cross-sectional* version — the response of
  individual currencies conditional on their own dollar-funding dependence — rather than the
  published time-series version against a large set of currencies, and rather than the published
  *level* version in S-055; (ii) the *sign discipline*, making the funding-liquidity channel and the
  carry-crash channel explicitly separate and separately testable; and (iii) the *venue* argument —
  this is IDEA-002's mechanism in a market where a state variable is published, which is what makes
  it testable at all.
- *Honest classification:* **known baseline, with a residual claim.** The aggregate version — carry
  conditioned on a publicly observable funding-constraint state — is published, peer-reviewed and
  positive (S-055), and the aggregate version of this candidate has therefore been logged as a
  rejection (R-006). What remains claimed here is narrow: the *cross-sectional* dependence
  structure, and the *publication-timing* test. This dossier must never be described as a
  discovery of the funding-state → carry relation.
- *Confidence in the comparison:* **moderate-to-high for the baseline, low for the residual.**
  S-055 and S-059 were re-verified directly against their publisher records in this cycle; the rest
  of the corpus was verified by a dedicated verification pass (S-056 … S-073) whose bibliographic
  details are corroborated by the reference lists inside the two directly fetched records. What
  could *not* be established is that the cross-sectional claim is unpublished — the residual
  question in G-10.

**Target scope.** Spot FX in a set of currencies whose borrowers' dollar-funding dependence
differs materially — for example a group of dollar-funding-dependent emerging-market currencies
and a group of currencies whose borrowers fund domestically; holding horizon one quarter to two
quarters, aligned to the publication calendar of the funding statistics; regime conditions:
exclude quarters with a large change in the regulatory treatment of dollar funding, and exclude
quarters in which the funding aggregates are structurally revised (a stated data hazard).

**Observables (knowable at decision time, conceptually).**
- The published cross-border and dollar-denominated liability aggregates by residence, currency
  and counterparty sector, on the quarterly publication calendar (S-054) — known in advance, with
  a known lag.
- The *cross-sectional* dependence measure: for each currency, the share of its cross-border
  borrowing that is dollar-denominated, from the same published tables (S-054).
- The policy rate differential and the forward-implied rate differential, as the control for the
  ordinary carry channel (the published result explicitly separates the two, S-052).
- The VIX or an equivalent risk state, and the *sign* of the dollar's move, as the discriminator
  between the funding-liquidity channel and the carry-crash channel.
- *Timing hazards to flag for the validator:* revisions and breaks in the banking statistics;
  the quarterly frequency of the state against a market that reprices daily; the fact that the
  published time-series result is *in-sample and out-of-sample* over a specific vintage
  (2007–09 induced a structural shift) and that the 2020 and 2022 episodes may be different.

**Rule sketch (descriptive, non-executable).** On each scheduled publication of the banking
statistics, for each currency in scope: compute the change in dollar-denominated cross-border
liabilities attributable to borrowers resident in that currency, and the currency's
dollar-funding-dependence share; form a cross-sectional score combining the funding-state change
with the dependence share; take the position, with a size set by the cross-sectional dispersion of
the score and by a pre-specified cap; hold until the next scheduled publication, when the
position is re-formed on the same rule; carry the price differential as an explicit cost, and
exclude any period in which the carry channel and the funding channel point in opposite
directions unless the rule specifies which dominates.

**Persistence thesis.** The dollar's role as the funding currency is structural, and the
statistics that measure it are produced by a standing international committee; the state therefore
persists and refreshes on a known calendar. The premium does not need to be large — it needs to
be measurable and not competed away, and the fact that the state is published at a known date is
what makes the trade implementable without look-ahead.

**Constraints.** Cost/liquidity: a quarterly-horizon position in liquid currency pairs is
cheap to hold, but the edge is slow, and a slow edge must survive financing and the cost of
turnover. Capacity: high in the majors, lower in the emerging-market currencies whose funding
dependence is the object of study; that is the direct capacity trade-off of the candidate.
Financing/margin: material for the carry cost of the positions. Market impact: high for the
emerging-market currencies, and the currencies with the highest funding dependence are often
the least liquid and the most intervention-prone. Venue/operational: the state is published by
international bodies with a known calendar, but the *timing* of the publication within the day
must be pinned down before any same-day effect is claimed. Shorting constraints: several
emerging-market currencies have limited two-way borrow, which directly constrains the short leg.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the candidate is
*defined* by regime — a funding expansion versus a funding contraction, and the two have
different signs for the currency. Tail: the funding-contraction state is exactly the carry-crash
state, in which the crowded position unwinds violently; a position sized for a slow premium can
meet a violent deleveraging. Crash behaviour: in a global dollar squeeze, the currencies with the
highest funding dependence should be the most violent, which is the prediction that would make the
candidate dangerous to hold through the tail it is designed to anticipate. Hidden beta: the
positions are long the funding currency and short high-dependence currencies, which is
substantially a short-carry position and can load on the momentum factor.

**Falsifiable predictions and rejection conditions.**
1. *Cross-sectional ordering:* when dollar funding liquidity expands, the currencies with the
   highest dollar-funding dependence appreciate more (against the dollar) than the currencies with
   the lowest dependence, in the same period. **Kill:** the cross-sectional ordering is flat, or
   the dependence measure has no incremental explanatory power over the interest differential.
2. *Sign discipline:* the predicted sign is opposite to the carry-crash channel, and the
   candidate's periods must not overlap the carry-unwind episodes; if the result only holds in
   episodes where the carry channel dominates, the candidate has not identified its own channel.
   **Kill:** the effect is fully explained by the interest differential.
3. *Publication-timing test:* the effect must appear from the *publication date* of the
   statistics and not before it. **Kill:** the effect is present before the data were public,
   which would mean the state is not the cause.
4. *Out-of-sample stability:* the cross-sectional relation holds in a held-out period, and the
   relationship is not driven by a single crisis episode. **Kill:** it is.
5. *Cost floor:* the cross-sectional spread of the predicted returns exceeds the round-trip cost
   and the carry cost over the holding period. **Kill:** it does not, in which case the candidate
   is a description rather than a trade.

**Main confounders and rival explanations.**
- *The carry channel* — the most important rival, and the published result claims separation from
  it (S-052) but the separation must be re-verified in any validation.
- *Dollar invoicing and trade exposure* — a currency's trade-weighted dollar invoicing share
  predicts its dollar move for reasons unrelated to funding; the candidate must control for it.
- *Risk-off and safe-haven flows* — in stress the dollar appreciates against everything, which
  can masquerade as the funding channel.
- *Interest-rate expectations* — the state may proxy for the expected policy path.
- *Data revisions and structural breaks* — the published time-series result notes a structural
  shift induced by the 2007–09 crisis; the statistics themselves are revised.
- *The candidate may be a repackaged carry trade with extra steps* — the honest null.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: the BIS locational banking statistics and the
global liquidity indicators on their published calendar (S-054); BIS and national FX reference
rates; the policy rate differential; a volatility series. Commercial: none required. **Data-
construction constraint to pass to the validator:** the *fast* version of the state — the
cross-currency basis — is **not published in any official statistical release** (a scoped
negative finding: the BIS statistics catalogue contains no such series, and the published
funding-constraint studies construct it from paid vendor forwards, S-055). A validator must
therefore choose explicitly between the published quarterly state and a self-built daily state,
must say which, and must price the second option's data cost; a daily-state variant of this
candidate is a *different* candidate with a different data budget. Feasibility:
**high** for the data; **medium** for the identification, because the state is quarterly while the
market is daily, so the effective number of independent observations over a multi-decade sample
is small and the cross-section must be built out of currency heterogeneity rather than time
series variation.

**Theory/evidence status.**
- *Conceptual rationale:* supported — the funding-liquidity channel is modelled and empirically
  supported (S-052, S-053).
- *Mechanism supported by sources:* **yes** — the channel, its sign and its separation from carry
  are documented (S-052); the state variable is published (S-054).
- *Prior empirical support reported by others:* the aggregate funding-state → carry-return result
  is the authors' own and is not reproduced here (S-055); the dollar funding-liquidity forecasting
  result is likewise the authors' own (S-052, S-053); the basis and hedging-demand mechanism is
  documented in the central-bank and peer-reviewed literature (S-056, S-057, S-059, S-069); the
  crisis-period funding state is documented officially (S-058, S-060, S-072). **None of this is
  reproduced here, and none of it supports the cross-sectional claim.**
- *Unresolved:* whether the cross-sectional structure exists, whether it survives the
  carry-channel control, and whether the residual claim survives the fact that the aggregate
  version is published.

**Remaining uncertainty / confidence.** Confidence that the channel exists and the state is
published: **high**. Confidence that the *aggregate* application of this channel to carry is
new: **none — it is published** (S-055). Confidence that the *cross-sectional* refinement is
correct: **low-to-moderate** — it is plausible from the mechanism, and it was not found in the
corpus read, but the corpus is not exhaustive and the residual question in G-10 is still open.
Confidence that it is tradeable after costs: **moderate** (slow horizon, liquid instruments, but a
slow edge). Priority score **64/100**; rank 5 of 7 at the time of writing. **Concrete next
question:** when dollar funding liquidity expands, do the currencies whose borrowers are most
dependent on dollar funding appreciate more than the others, conditional on the interest
differential, and does the relation appear from the publication date rather than before it —
and, as a lead for a *new* candidate rather than for this one: does the level of forward points
predict the future level of forward points, on a state constructed from public data, given that
no published cross-currency basis series exists (G-10)?

---

## Cross-idea dependency and correlation map

- **IDEA-001 and IDEA-002 share a microstructure dependency:** both assume impact and reversal are
  measurable from order-flow and event data. A validation of one supplies the plumbing for the
  other, but their mechanisms are independent (scheduled passive flow vs. funding-constrained
  intermediation). If either is falsified, the other is not affected.
- **IDEA-002 and IDEA-004 both condition on a latent state variable** (funding state, crowd depth).
  If a general lesson emerges — that state conditioning requires a *fast* proxy — it applies to
  both, and a shared "state proxy methodology" note is warranted (see the handoff).
- **IDEA-003 is structurally independent** of the other three: its state variable is the option
  surface, and its risk is a left tail rather than a liquidity spiral. It is the only candidate
  whose failure mode is a single catastrophic event rather than a decay of the effect.
- **Common exposure:** IDEA-001, IDEA-002 and IDEA-004 are all long-short or event-driven equity
  strategies that will load on equity market beta and on volatility in different ways. A combined
  validation would need explicit factor attribution; the candidates should be validated
  independently first.
- **IDEA-005 and IDEA-006 are the same mechanism in two venues.** Both are "a dated,
  price-insensitive institutional flow buys a liquidity concession, and the concession is a
  function of the flow's size relative to liquidity". IDEA-005 is the monthly futures roll with
  the state published by the CFTC; IDEA-006 is the daily end-of-day deadline cluster with the
  state published by the benchmark administrator and the settlement utility. A validation of the
  *economics* (the concession accruing to a scheduled provider) is shared; the *rules* are not.
  If the concession economics fail in one venue, that is evidence about the other, but the
  candidates must still be validated separately.
- **IDEA-007 is IDEA-002's mechanism in a venue where the state is published.** The two are not
  independent ideas: IDEA-002 is parked (P-004) precisely because the equity-market funding state
  is not observable, while IDEA-007 is feasible because the dollar funding state is published
  (S-052, S-054). This is the register's answer to the Cycle-1 state-proxy question: **the
  state-proxy problem is largely a venue-selection problem.** Validating IDEA-007 tests the
  *mechanism* that IDEA-002 would have tested if a proxy had existed.
- **IDEA-005 and IDEA-004 share the crowd-state idea in a way that matters.** IDEA-004's known
  weakness is that its crowd-depth proxy is quarterly-stale (S-026, G-04). IDEA-005 shows what a
  *timely public* crowd proxy looks like: the CFTC's weekly Index Trader positions (S-030). A
  negative result for IDEA-005's state conditioning would be indirect evidence against the
  feasibility of IDEA-004's proxy, though the instruments and horizons differ.
- **IDEA-003 and IDEA-006 are exposed to the same end-of-day window.** If the equity closing
  auction and the FX fixing window are both institutionally concentrated, then a position sized
  for one is exposed to the other's flow. They should not be validated with a shared risk budget
  without attribution.
- **Cycle-2 common exposure:** IDEA-005, IDEA-006 and IDEA-007 are all non-equity candidates, and
  two of them (IDEA-006, IDEA-007) are FX positions that will load on the dollar and on the
  funding-coinage factor, and both can be short the funding currency. The register now has
  *market* diversification but a *factor* concentration in the dollar; that concentration should
  be stated in any portfolio-level discussion.
