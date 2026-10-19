# IDEA REGISTER

Every retained candidate lives here with a complete dossier. Status values: `shortlisted`,
`candidate` (retained but not shortlisted), `archived` (retained for reference, not a top
opportunity), `rejected` (see `rejected_and_parked.md`; dossiers are not maintained for those).

Last updated: Cycle 1, 2026-10-19. Register was empty before this cycle.

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
rank 1 of 4. **Concrete next question:** does the announcement-to-effective drift scale with the
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
Priority score 63/100; rank 4 of 4. **Concrete next question:** is there a public funding-state
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
content, and it is not directly evidenced. Priority score 71/100; rank 3 of 4. **Concrete next
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
observability: low-to-moderate. Priority score 74/100; rank 2 of 4. **Concrete next question:** is
the relation between convergence returns and crowd depth non-monotone as predicted, and can a
timely proxy for crowd depth be validated against a holdings-based measure?

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
