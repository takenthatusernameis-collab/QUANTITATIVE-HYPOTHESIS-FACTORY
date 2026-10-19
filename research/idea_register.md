# IDEA REGISTER

Every retained candidate lives here with a complete dossier. Status values: `shortlisted`,
`candidate` (retained but not shortlisted), `archived` (retained for reference, not a top
opportunity), `rejected` (see `rejected_and_parked.md`; dossiers are not maintained for those).

Last updated: **Cycle 5 complete** (the Cycle-5 gap-closure and originality pass), 2026-10-19. The
register was empty before Cycle 1; Cycle 2 added three dossiers outside listed US equities.
**Closure passes: five candidates have now been demoted by their own literature.** IDEA-007 was
narrowed to v1.1 after the funding-currency corpus was read — its aggregate version is a published
baseline (S-055, rejected as R-006) and the dossier then claimed only the cross-sectional and
publication-timing residual — and in Cycle 5 that residual was closed against it as well: the
cross-section is a published, positive result (S-064) and the mechanism's literature has closed in
the same direction (S-095, S-096, S-097), so IDEA-007 is **rejected (R-008)**. IDEA-006 was narrowed
to v1.1 after the intraday fixing literature was read — the fix-window price impact is published
(S-074 … S-081, rejected as R-007) — and in Cycle 5 its own gate was met: **G-11 closed against it,
so IDEA-006 is rejected (R-009)** and its dedicated vehicle IDEA-012 is **rejected (R-010)**.
**Cycle-3 gap closures:** G-10 cross-sectional residual remains open; G-11 partially closed —
settlement-side mechanics are a priced friction (S-082, S-071) but the deadline cluster is untested;
G-06 narrowed — the commodity basis-convergence literature (S-032 … S-039) does not condition on
passive share × depth, so IDEA-005's state-conditioned differentiator survives as a conjecture.
**Cycle-5 gap closures (this cycle):** **G-10 closed against IDEA-007** (see the R-008 record);
**G-11 closed against IDEA-006 and IDEA-012** (a settlement deadline cluster is a published price
determinant — S-112; the securities settlement cycle is a published price-impact determinant —
S-113, S-114, S-115; the post-US-close FX window is documented as a cost rather than an edge —
S-117, S-118, S-119, S-120); **G-06 closed as a bounded negative finding** with the papers that had
not been found earlier now located and registered (S-098 conditions spot–futures convergence on
*trader type*; S-099 conditions *commodity returns during roll periods* on the CIT market share and
reports no significant effect — contradicting evidence now recorded against IDEA-005); **G-08 mostly
closed** and **G-05 split** (its single-name 0DTE series is constructible from public OCC data, so
the *data* question is closed and only the *literature* question is open); **G-12 opened** — the
general question of whether a *published* state can change the *sign or existence* of a published
effect, or only its measurement quality, which is now the register's standing test for every
state-conditioned candidate; and **G-13 opened** — a published state is usable as a decision-time
variable only if it is published *before* the decision, an established instance being the EU ETS
aggregate balance (S-121), which was published after the pre-2023 surrender deadline it was meant to
inform. **IDEA-013 was parked (P-008)** after its required full-text check: S-101 does not condition
the premium on the aggregate surplus (so the candidate is not a re-description of published work),
but the published model already implies the conditional structure, the published sample contains a
high-surplus year in which the effect persisted, and the decision-time form of the candidate has
only three observations.

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
- *Gap G-06 result (Cycle 3):* the commodity basis-convergence literature was located
  (S-032 … S-039) and establishes that the roll concession, as an aggregate post-2012 fact, is
  dead (S-033), transient (S-032, S-034), and not predicted by positions (S-036, S-037). It does
  **not** condition the roll-period nearby-to-deferred spread concession on the passive share of
  open interest × contract depth, and it does not establish the concession as a plain
  convergence-to-carry trade with a calendar catalyst rather than a liquidity-provision concession
  around a scheduled roll. G-06 is therefore **narrowed, not closed**: the claim that "nobody has
  conditioned the roll impact on the passive share of open interest" survives as a conjecture,
  not an exhaustive negative finding, and must be re-visited before IDEA-005 is presented as a
  discovery.
- *Confidence in the comparison:* moderate-to-high. The closest work (S-035) and the three
  peer-reviewed studies that contradict it (S-032, S-033, S-034) were read at the level of
  abstracts, publisher records and the CFTC-hosted full text of S-035; S-032 was read in the
  author-hosted PDF.

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
  literature was located in Cycle 3 (S-032 … S-039, gap G-06 narrowed but not closed). If the
  concession is simply a convergence-to-carry trade with a calendar catalyst, it is a variant of a
  known baseline and must be reclassified.

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
- **Date added:** 2026-10-19 · **Cycle:** 2 · **Status:** **rejected (R-009)** ·
  **Version:** 1.2
- **Change notes:** v1.0 — first dossier. The intraday periodicity around the London fix is an
  established fact; the candidate is the *deadline-constrained flow* reading of it, extended to
  the post-US-close settlement window that the T+1 transition created. **v1.1 — reclassified after
  the G-09 closure pass (S-074 … S-081): the *fix* half of the deadline cluster is published —
  the price impact of price-insensitive hedging demand at the fix, its temporary character and
  the pre-fix/post-fix reversal are all in the literature — so the aggregate version of this
  candidate was rejected (R-007) and the dossier was narrowed to two residuals: the
  *settlement-side* deadlines beyond the fix (blocked on G-11) and the post-2015 persistence of
  the published fix effect.**
  **v1.2 — REJECTED after the Cycle-5 G-11 closure (S-112 … S-121).** The candidate's own gate —
  "G-11 must be closed before any of the above is treated as a candidate rather than a hypothesis.
  If a published paper already shows a settlement-side or T+1-window price effect, the candidate is
  rejected, not narrowed" — is now met, in both of its limbs. A settlement deadline cluster is a
  published price determinant: Kraenzlin and Nellen (2010, S-112) show that after CLS "the value of
  intraday liquidity has increased during the hours of the CLS settlement cycle", with a structural
  break at the pay-in schedule and an estimated mark-up of "approximately 0.50bp per hour, leading to
  a total of roughly 1.5bp for the CLS settlement cycle". A T+1-window price effect is also
  published: Baig, Breeze, Cox and Griffith (2022, S-113) find that shortening the US cycle to T+2
  made US securities *more liquid* than matched London-listed securities, and Bhanu, Nath and
  Patnaik (2024, S-114) find that T+1 "significantly improved liquidity" measured by bid-ask
  spreads, Amihud illiquidity and price impact. The residual's own kill condition on the post-2015
  persistence question was answered earlier (S-047, S-080: the benchmark's post-revision quality and
  the 2015–2023 effectiveness of the fix are documented in peer-reviewed work). **The dossier is
  closed; the reasoning is preserved in R-009 and the candidate is not to be presented as an
  opportunity.**

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
  **blocked on G-11**: G-11 is now **partially closed** — Lee, Ranaldo and Tsuruga (2026) (S-082)
  show settlement risk is a *priced friction* in currency markets using Hungary's 2015 CLS
  PvP adoption, and Ranaldo and Santucci de Magistris (2022) (S-071) build CLS-based settlement
  metrics linked to currency risk premia. So settlement-side mechanics matter for pricing, but
  neither paper tests the specific *settlement-side deadline cluster* — the CLS currency-close and
  pay-in cut-offs and the post-US-close window created by the May 2024 T+1 transition — as a
  price determinant. The specific claim IDEA-006's residual rests on remains untested, so
  "unclaimed" is still an *expectation*, not a finding. This dossier must never be described as
  a discovery of the fix's price impact.
- *Confidence in the comparison:* **high for the fix, low for the residual.** Every item in
  S-074 … S-081 was re-verified directly against Crossref, the arXiv record, the NBER record or
  the publisher listing in this pass, and the DOIs that a read-only verification agent reported
  for three of them were wrong and were corrected (the errors are recorded in the G-09 gap
  entry). S-082 adds a published settlement-side result (the closest located work to IDEA-006's
  residual) but does not close the deadline-cluster claim. The residual side is weaker: G-11 is
  partially closed, and the fix literature's own data (administrator- and dealer-provided tick
  data) mean that a "nobody has tested this" claim about the settlement side must be earned, not
  assumed.

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
window created by the May 2024 T+1 transition — as a price determinant rather than as an operational
schedule, and if not, does the settlement window show a directional imbalance that survives removal of
the published fix effect?

**v1.2 closure (Cycle 5). The question above was answered, and the answer is disqualifying.**
Published work does test settlement deadlines as price determinants (S-112: the CLS settlement cycle
raises the price of intraday liquidity in the Swiss franc repo market; S-113, S-114: the securities
settlement cycle is a published price-impact determinant, with the *liquidity-improvement* sign),
and the institutional record shows the post-US-close window to be structurally illiquid and expensive
rather than concession-rich (S-117, S-118, S-119, S-120: "less than 1% of trades in the $7 trillion
OTC FX market are carried out in this window"; "bid/ask spreads widen and liquidity shrinks"; the
market's own answer was custodian cut-off extensions and pre-funding). The candidate's rule is
explicit that this outcome rejects rather than narrows. **Status: rejected (R-009).** The mechanism
is real and now partly owned by published work; the *trading* claim was never supported and the cost
structure of the target window makes it unsupportable. This dossier is retained only so that the
negative reasoning is not re-derived.

---

## IDEA-007 — FUNDSTATE-FX: the dollar as the funding currency, and the cross-section of who feels it

- **ID / short name:** IDEA-007 / FUNDSTATE-FX
- **Date added:** 2026-10-19 · **Cycle:** 2 · **Status:** **rejected (R-008)** · **Version:** 1.2
- **Change notes:** v1.0 — first dossier (the venue answer to the state-proxy question). v1.1 —
  reclassified after the funding-currency corpus was read: the aggregate funding-state → carry-return
  relation is a published, peer-reviewed baseline with a positive result (S-055), the aggregate
  version was rejected as R-006, and the dossier was narrowed to the cross-sectional dependence
  structure plus a publication-timing test. **v1.2 (Cycle 5) — REJECTED.** The cross-sectional
  residual is a published, positive result (S-064) and the mechanism's own literature has closed in
  the same direction (S-095, S-096, S-097). The dossier is retained as a compact record only; the
  full reasoning is in `rejected_and_parked.md` (R-008).

**What was claimed.** The dollar is the world's funding currency, so the growth of
dollar-denominated liabilities of the intermediaries who supply that funding is a public, slow-moving
state that moves the dollar. The aggregate version of that relation is published (S-052, S-055). The
candidate's residual claim was therefore the *cross-sectional* version: which currencies' exchange
rates move when dollar funding expands and by how much, measurable *ex ante* from the published BIS
locational banking statistics (S-054) on their quarterly calendar, and identifiable by a
publication-timing test (the effect must appear from the publication date and not before).

**Why it is rejected.** The cross-section is published, and published *positively*. Wang (2026),
"Deviations from Covered Interest Parity, Dollar Funding Pressure, and Currency Risk Premia"
(S-064), states the hypothesis in the register's own words — "Currencies with higher dollar funding
pressure (higher unconditional level of basis) earn higher expected excess returns" — and reports a
global high-minus-low basis factor that earns a 4–4.5% annual risk premium, explains a large share
of the cross-sectional variation in currency excess returns, and subsumes carry and several other
factors. The mechanism's literature closed in the same direction during the same cycle: Moskowitz,
Ross, Ross and Vasudevan are now peer-reviewed as "Risk, Specialization, and Covered-Interest
Parity" (*Journal of Finance*, S-095) and document the cross-section of CIP bases and its
pass-through to prices; Cenedese, Della Corte and Wang (2021, S-096) show that a binding regulatory
balance-sheet constraint prices currency funding at the dealer level; Adrian, Etula and Muir (2014,
S-097) establish the general intermediary-state → cross-section-of-returns mechanism.

**What survives, and what does not.**
- *Does not survive:* the cross-sectional claim as a **discovery**. It is published, and the
  published version has a positive result. A dossier claiming it would be presenting a published
  baseline as an original result, which is the register's rediscovery rule.
- *Does not survive:* the **publication-timing test** as a source of novelty. A published state on a
  known calendar is a *feasibility* property — it makes the published effect implementable without
  look-ahead or vendor data. It is not a source of novelty, and it does not change the *sign* or the
  *existence* of the effect (the register's rediscovery guard for candidates that differ from a
  baseline only in the state variable). This generalisation is now logged as **G-12**.
- *Survives as a baseline:* the funding-constraint state prices carry (S-055) and the cross-section
  of currency risk premia (S-064); the state is published quarterly (S-054) while the *fast* state
  — the cross-currency basis — is **not published anywhere** and must be built from paid vendor
  forwards (a scoped negative finding from G-10 finding (a), unchanged in Cycle 5).
- *Survives as a lead for a different candidate:* "does the level of forward points predict the future
  level of forward points, on a state constructed from public data?" (the "forward points predict
  forward points" residual identified in the Cycle-2 G-10 pass) is **not** answered by S-064 and is
  carried forward as a lead, not as a candidate. It would be a different mechanism from the
  cross-section, and it would need its own dossier and its own originality check.

**Consequences recorded in the register.**
1. The register now holds **no FX candidate** — a diversification cost the shortlist had explicitly
   pre-registered as the consequence if the cross-section turned out to be published.
2. The funding-state family is not dead; it is *published*. Any future FX candidate must be a
   **new mechanism** (a new venue, a new participant, a new constraint) and must state in advance
   how it differs from S-055, S-064, S-095, S-096 and S-097. A new *state variable* on the same
   channel is not enough (G-12).

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

---

## IDEA-008 — SECURITY-LEND: borrow constraints, recall-driven forced covering, and the short-interest state

- **ID / short name:** IDEA-008 / SECURITY-LEND
- **Date added:** 2026-10-19 · **Cycle:** 3 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. New mechanism family not previously in the register.

**One-sentence hypothesis.** When a stock's borrow becomes expensive or scarce and lenders recall
loaned shares, short sellers are forced to cover involuntarily; the resulting buying pressure
creates a temporary price spike that decays as the covering is completed, so a rule that buys
into borrow-constraint and recall events and exits on a pre-scheduled basis captures a
liquidity-provision premium paid by the forced coverers.

**Plain-language description.** Some stocks are hard or expensive to borrow. Short sellers who
borrowed those shares can be asked to give them back at any time — the lender can recall the
loan. When that happens, the short seller must buy the stock back to close the position, often in
a rising market and often all at once with other short sellers in the same stock. That forced
buying pushes the price up temporarily, and the spike fades once the covering is done. A
participant who is ready to buy into that forced covering and sell afterward collects the
temporary price concession.

**Mechanism (causal chain).**
1. To sell a stock short, an investor must first borrow it; the lender charges a fee (the loan
   rate or "specialness") and can recall the shares at any time (Jones & Lamont, 2002, S-083).
2. Stock loans are not term loans: the lender has the right to demand the shares back at any
   moment, and if the short seller cannot find replacement shares, the position must be covered
   — bought back — at whatever the market price is (S-083).
3. Recall risk is real and measurable: in a large lending-intermediary sample, about 2% of loans
   on loan were recalled in an average month, and days with involuntary covering saw volume more
   than twice the stock's average and elevated intraday volatility (D'Avolio, 2002, S-084;
   referenced in S-083).
4. When many short sellers are recalled at once — or when borrow becomes expensive enough that
   new shorts cannot be initiated — the forced covering is concentrated and price-insensitive:
   the short seller must buy regardless of price (S-083).
5. A participant who supplies liquidity into that forced buying — buying as the coverers buy and
   selling into the subsequent normalization — earns the temporary price concession. The edge is
   a *liquidity-provision premium* paid by the forced coverers, not a risk premium for systematic
   exposure.
6. The state is observable at decision time: short interest (shares sold short, published
   biweekly by exchanges), securities-lending fees and availability (reported by lending agents
   and data vendors), and recall events themselves are documented operational facts rather than
   latent variables (SEC, 2021, S-085).

**Expected return source.** A temporary liquidity-provision premium paid by short sellers who are
forced to cover (by recall or by prohibitively expensive borrow), collected by a participant who
is scheduled to be present at the covering event and exits after it, net of execution costs and
the risk that the recall is driven by fundamental news rather than a pure liquidity event.

**Originality.**
- *Closest known work:* Jones & Lamont (2002) "Short-Sale Constraints and Stock Returns" (S-083),
  JFE 66(2-3):207-239; D'Avolio (2002) "The Market for Borrowing Stock" (S-084), JFE
  66(2-3):271-306; Duffie, Garleanu & Pedersen (2002) "Securities Lending, Shorting, and Pricing"
  (SSRN 302015); SEC (2021) on securities lending market opacity (S-085); and the broader
  limits-to-arbitrage literature (S-022, S-023).
- *What is already known:* that stocks expensive to short or newly entering the borrowing market
  have low subsequent returns (S-083); that loan supply, fees and recalls are real and measurable
  (S-084); that short-sale constraints are a limit to arbitrage and bind only for certain
  ("special") stocks; and that recall-driven forced covering produces volume and volatility spikes
  (S-084).
- *Substantive differentiator claimed here:* (i) the candidate is *not* the well-documented
  "expensive-to-short predicts low returns" effect (which is the opposite side of the trade);
  it is the **recall-driven forced-covering spike** on the *long* side, which is a distinct,
  event-timed, short-horizon phenomenon; (ii) the state (borrow cost/availability and recall
  risk) is published by exchanges and lending agents on a known calendar, so no proxy
  construction is needed — this is the venue-selection lesson applied to a new family; and
  (iii) the trade is explicitly two-legged and time-boxed (buy into the cover, exit on schedule),
  not a directional short-sale-constraints position.
- *Honest classification:* **mechanism documented in parts, candidate specification new.** The
  components (borrow cost, recall risk, forced covering) are published; the joint specification —
  buying into recall events as a liquidity-provision trade with a pre-specified exit — is not a
  known baseline in the register or in the located literature.
- *Confidence in the comparison:* moderate. S-083 and S-084 were verified directly (Crossref and
  publisher record); S-084's DOI could not be re-derived and is logged as a working-paper
  reference cited within S-083. The claim that no published work tests the recall-event liquidity
  provision as a tradeable two-legged rule is a search result, not a proof.

**Target scope.** US equities with publicly reported short interest and active securities-lending
markets; holding horizon intraday to a few sessions around a recall or borrow-cost spike event;
per name; regime conditions: exclude names with fundamental news (earnings, M&A, FDA decisions)
inside the event window; exclude names under a short-sale restriction (Reg SHO SSR threshold).

**Observables (knowable at decision time, conceptually).**
- Short interest (shares sold short), published biweekly by exchanges (NASDAQ, NYSE) with a
  known lag — the change in short interest is the flow proxy.
- Securities-lending fee ("specialness") and borrow availability, reported by lending agents and
  data vendors — the state variable.
- Recall events: not published as a time series, but the *risk* of recall is priced into the loan
  fee, and spikes in the fee are observable (S-084).
- Reg SHO threshold securities list (stocks that have failed to deliver for five consecutive
  settlement days) — published by exchanges and by FINRA — a regulatory signal that borrowing is
  constrained (S-085).
- *Timing hazards to flag for the validator:* short interest is reported biweekly with a lag, so
  the state is stale by design; the recall event itself is not published and must be inferred from
  fee spikes and volume anomalies; a recall can be driven by fundamental news (the lender selling
  because they lost confidence), which is the dominant confounder; and the event is rare (about
  2% of loans per month in S-084), so the sample is small.

**Rule sketch (descriptive, non-executable).** Each day, for each name in scope: compute the
change in short interest and the securities-lending fee relative to its own history; flag names
where the fee spikes into the top decile of its own distribution (a borrow-constraint event) or
where short interest rises sharply with a simultaneous fee increase; exclude names with scheduled
fundamental news inside the window; take a long position sized as a small fraction of the name's
daily volume; exit on a pre-specified schedule (e.g. T+1 to T+5) after the event, with the exit
rule fixed in advance. Exclusions: names under Reg SHO threshold, names with earnings or M&A
news inside the window, names in the bottom liquidity quintile.

**Persistence thesis.** Stock loans are not term loans and lenders can recall at any time, so
recall risk is structural; short-sale constraints bind only for certain stocks and are not
competed away because the supply of lendable shares is limited by the holdings of long-term
investors (S-083). It decays if securities lending becomes centralized and transparent (reducing
recall risk and fee spikes), if short selling becomes so constrained that few shorts exist to be
recalled, or if the recall-event premium is arbitraged by participants already stationed to
supply liquidity into recalls.

**Constraints.** Cost/liquidity: the covering is concentrated in minutes, so spread and slippage
are first-order; this is the binding constraint. Capacity: bounded by the size of the forced
covering and by the name's liquidity; small-cap names have the highest fees but the least
liquidity. Financing/margin: a long position held for days is a spread cost, not a
balance-sheet constraint. Borrow: not a short-sale-constrained trade (it is long), but the
underlying event is about borrow constraints. Market impact: buying into a concentrated
forced-covering window is an impact machine. Venue/operational: short-interest data are biweekly
and lagged; the recall event itself must be inferred.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the constraint state
is the regime — the candidate predicts an edge only when borrow is constrained. Tail: a recall
driven by fundamental news is a directional loss, not a liquidity event; this is the dominant
failure mode. Crash behaviour: in a market-wide squeeze, recalls cluster across names and the
position is long into a rising market (which is the payoff), but the covering may extend beyond
the pre-scheduled exit. Hidden beta: the long position carries market beta and idiosyncratic
news risk; beta must be controlled explicitly. Correlated risks: recalls can cluster in the same
sector (e.g. after a sector-level negative development), so the book is not fully diversified.

**Falsifiable predictions and rejection conditions.**
1. *Event spike:* a borrow-fee spike or sharp short-interest increase is followed by a temporary
   price increase that decays within 1–5 sessions. **Kill:** no price increase after the event,
   or the increase does not decay.
2. *State scaling:* the size of the post-event price move is increasing in the fee spike magnitude
   and in the change in short interest. **Kill:** no relation to the state variables.
3. *News confound:* the effect is present on no-news days and absent (or reversed) on days with
   fundamental news inside the window. **Kill:** the effect is driven entirely by news days,
   which would mean it is a fundamental-repricing event, not a liquidity event.
4. *Cost floor:* the realised temporary spike exceeds round-trip cost (spread, commission,
   slippage) in the selected names. **Kill:** the gross spike is below cost in every selected
   name.
5. *Rarity:* the event is rare (about 2% of loans per month), so the effective sample is small;
   if the effect cannot be distinguished from noise given the sample size, the candidate is
   untestable as specified.

**Main confounders and rival explanations.**
- *Fundamental news on the recall:* the lender recalls because they lost confidence and are
  selling; the short covering coincides with a fundamental re-pricing. This is the single most
  important confounder and is addressed only partially by the no-news exclusion.
- *Short-sale constraint overpricing:* expensive-to-short stocks have low subsequent returns
  (S-083) — the opposite direction; the candidate must show its effect is distinct from and not
  explained by this baseline.
- *Reg SHO threshold effects:* stocks on the threshold list behave differently for regulatory
  reasons unrelated to recall risk.
- *Liquidity as cause and effect:* a thin stock has both high borrow fees and large price moves
  for any flow; the conditioning may be over-controlling.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: short interest (biweekly, exchange-published),
Reg SHO threshold list (exchange/FINRA-published), daily OHLCV, borrow-fee and availability data
(from lending agents and data vendors — commercial), and a fundamental-news calendar. Feasibility:
**medium** — the prices and short interest are public; the borrow-fee data are commercial and the
recall event must be inferred; the rarity of the event makes the sample small.

**Theory/evidence status.**
- *Conceptual rationale:* supported — short-sale constraints as limits to arbitrage (S-083),
  recall risk as a real cost of shorting (S-084), and the securities-lending market as
  documentation-heavy but economically real (S-085).
- *Mechanism supported by sources:* yes for the participant, the constraint and the recall risk
  (S-083, S-084); the *joint* two-legged liquidity-provision specification is an unresolved
  conjecture.
- *Prior empirical support reported by others:* for the components (S-083, S-084); not for the
  joint trade specification.
- *Unresolved:* whether the recall-driven forced-covering spike is large enough to exceed costs
  after the news confound is removed, and whether the biweekly lagged short-interest series is a
  sufficiently timely state variable.

**Remaining uncertainty / confidence.** Confidence that borrow constraints, recall risk and forced
covering are real and documented: **high**. Confidence that a tradeable two-legged rule can be
built on them: **low-to-moderate** — the event is rare, the recall itself is not published, and
the news confounder is severe. Priority score **66/100**; rank **4 of 9** at the time of writing.
**Concrete next question:** does a securities-lending fee spike or a sharp short-interest increase
predict a temporary price increase that decays within a week, on no-news days, after costs?

---

## IDEA-009 — PERP-FUND: the perpetual-futures funding rate as a daily-settled, published funding state

- **ID / short name:** IDEA-009 / PERP-FUND
- **Date added:** 2026-10-19 · **Cycle:** 3 · **Status:** shortlisted · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. New mechanism family not previously in the register.

**One-sentence hypothesis.** The perpetual-futures funding rate is settled every few hours and
published by the exchange; because it measures the crowded-leverage state directly, a rule that
takes the side opposite to the funding-rate crowd — short when the funding rate is high and
positive (longs paying shorts), long when it is low or negative — captures a mean-reversion
premium in the futures-spot basis that decays as the crowd unwinds.

**Plain-language description.** Crypto perpetual futures have no expiry. To keep the futures
price close to the spot price, exchanges make the long and short sides pay each other a funding
rate every few hours. When the funding rate is high and positive, lots of people are long and
paying the shorts — the market is crowded on the long side. That crowd is leveraged and can be
forced to unwind. A participant who goes short when the funding rate is very positive (betting
against the crowded long side) and long when it is very negative (betting against the crowded
short side) captures the mean reversion in the basis, funded by the funding-rate payments
themselves.

**Mechanism (causal chain).**
1. Perpetual futures have no expiry date, so there is no guaranteed convergence to spot; instead,
   exchanges use a funding rate — a periodic payment between longs and shorts proportional to the
   futures-spot gap — to keep the futures price close to spot (He et al., 2022/2024, S-086;
   Jermann et al., 2024, S-087).
2. The funding rate is typically settled every 8 hours and equals approximately the average
   futures-spot spread over the preceding period (S-086). It is published by the exchange on a
   fixed cadence — the state is published by the venue, with no look-ahead and no proxy
   construction.
3. A high positive funding rate means longs are paying shorts: the market is crowded on the long
   side, and the crowd is leveraged (perpetuals are leveraged instruments). A high negative rate
   means the reverse: the crowd is on the short side.
4. The crowded side is exposed to unwinding: when the funding rate reverses or the price moves
   against the crowd, leveraged positions are liquidated, which accelerates the move in the
   opposite direction — a forced-deleveraging spiral in the same family as recall-driven forced
   covering (IDEA-008) but in a derivatives venue (He et al., S-086).
5. Taking the side opposite the funding-rate crowd — short when longs are paying and crowded,
   long when shorts are paying and crowded — means supplying liquidity to a crowd that must
   unwind, collecting the funding-rate payments and the basis mean reversion. The edge is a
   *crowded-leverage reversal premium*, not a trend-following or breakout signal.
6. Because the funding rate is published every few hours, the state is observable at decision
   time and the trade can be scheduled around each settlement — this is the clearest instance of
   the Cycle-2 venue-selection rule: "the state is published by the venue."

**Expected return source.** The funding-rate payment itself (collecting the rate by being on the
receiving side) plus the mean reversion of the futures-spot basis as the crowded leveraged
position unwinds — a liquidity-provision/crowded-leverage reversal premium paid by the leveraged
crowd, net of execution costs, funding costs, and liquidation-spike risk.

**Originality.**
- *Closest known work:* He, Kelly, Lu, and Manela (2022/2024) "Fundamentals of Perpetual Futures"
  (arXiv:2212.06888, S-086); Jermann, Phelps, and Zhang (2024) "Perpetual Futures Pricing"
  (S-087); Christin, Routledge, Soska, Zetlin-Jones "The crypto carry trade" (preprint, cited in
  S-086); Emre Inan "Predictability of Funding Rates" (SSRN, S-088); and the "Exploring risk and
  return profiles of funding rate arbitrage" study (Blockchain Research and Applications, 2026,
  S-089).
- *What is already known:* the funding rate keeps perpetual futures close to spot (S-086);
  deviations from no-arbitrage prices in crypto are larger than in traditional markets, comove
  across currencies, and diminish over time (S-086); past returns predict futures-spot deviations
  with R² above 50% (momentum feedback in S-086); funding-rate arbitrage strategies (long spot,
  short perpetual when futures are expensive) have been documented (S-086, S-088); and funding
  rates contain information about future spot volatility beyond fixed-maturity futures measures
  (S-089).
- *Substantive differentiator claimed here:* (i) the candidate is *not* the well-documented
  funding-rate arbitrage (long spot, short expensive perpetual) — which is an arbitrage, not a
  state-conditional reversal — but a **crowded-leverage reversal** keyed to the funding-rate
  level as a state variable; (ii) the state is published by the exchange every few hours with
  zero lag, which is the venue-selection ideal; and (iii) the holding horizon is a few funding
  periods (intraday to multi-day), not the perpetual arbitrage's indefinite hold.
- *Honest classification:* **mechanism documented in parts, candidate specification new.** The
  funding-rate mechanism and the funding-rate arbitrage are published; the joint specification —
  taking the side opposite the funding-rate crowd as a reversal trade keyed to the funding-rate
  *level* (not the basis) — is not a known baseline in the register or in the located literature.
  The venue risk (crypto) is real and is stated honestly.
- *Confidence in the comparison:* moderate-to-low. S-086 was verified via arXiv (2212.06888);
  S-087 via the Wharton/arXiv PDF; S-088 via SSRN. The funding-rate literature base is thinner
  than the equity short-sale literature, and the crypto venue carries venue-specific risks
  (custody, exchange risk, 24/7 trading). The claim that no published work tests the
  funding-rate-level reversal as a tradeable rule is a search result, not a proof.

**Target scope.** Crypto perpetual futures on major exchanges (Binance, Bybit, OKX, etc.) for
liquid underlyings (BTC, ETH and a small set of large altcoins); holding horizon one to several
funding periods (8-hour to multi-day); per underlying; regime conditions: exclude periods of
exchange outage or severe congestion; exclude underlyings with thin perpetual order books.

**Observables (knowable at decision time, conceptually).**
- The funding rate, published by the exchange every funding period (typically every 8 hours) —
  the state variable, with zero lag.
- The futures-spot basis (perpetual price minus spot price) — the object that mean-reverts.
- Funding-rate extremes: the funding rate relative to its own history (e.g. top/bottom decile)
  — the entry signal.
- Open interest and volume in the perpetual — the size of the crowded position.
- *Timing hazards to flag for the validator:* funding rates can clamp at a minimum (e.g. 0.01%
  per period in S-086), so small rates are not informative; the exchange can change the funding
  cadence or clamp rules; crypto markets trade 24/7 so the "session" concept does not apply;
  and exchange-specific funding-rate implementations differ (clamp regions, calculation methods),
  so results are not transferable across venues without restatement.

**Rule sketch (descriptive, non-executable).** For each underlying in scope, at each funding
settlement: read the published funding rate; if the rate is in the top decile of its own trailing
distribution (longs paying, crowded long side), take a short perpetual position sized as a small
fraction of open interest; if the rate is in the bottom decile (shorts paying, crowded short
side), take a long position; exit after a pre-specified number of funding periods (e.g. 1–3) or
when the funding rate crosses zero, whichever comes first, with the exit rule fixed in advance.
Exclusions: thin order books, exchange outages, clamp-region rates, and underlyings with
insufficient open interest.

**Persistence thesis.** Perpetual futures are leveraged instruments with no expiry, so the
funding rate is the mechanism that keeps the crowd aligned with spot; the crowded side is always
exposed to unwinding; and the funding rate is published by the exchange, so the state is always
observable. It decays if the funding-rate crowd becomes sophisticated enough to pre-position
against reversals, if exchange funding implementations change to reduce the signal, or if
liquidity in thin underlyings dries up. Both decay channels are observable.

**Constraints.** Cost/liquidity: crypto perpetual spreads are narrow for majors but the trade is
intraday and frequent, so spread and slippage accumulate; this is the binding constraint. Capacity:
bounded by perpetual open interest and depth; large altcoins have thin books. Financing: a
leveraged perpetual position incurs funding that moves with the same state variable that
generates the signal — a self-referencing hazard that must be handled explicitly (the position's
own funding cost moves with the state). Borrow: not applicable (perpetuals are not borrows).
Market impact: trading into a crowded funding period is an impact machine. Venue/operational:
exchange custody risk, 24/7 trading, funding-cadence changes, and venue-specific clamp rules are
real risks that must be stated, not assumed away.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the funding-rate
state *is* the regime — the candidate predicts an edge only at funding-rate extremes. Tail: a
leveraged unwind can be violent and fast, and the position is on the side of the unwind (which is
the payoff) but can be stopped out before the reversal completes. Crash behaviour: in a
market-wide deleveraging, funding rates can spike across underlyings simultaneously and the
position is exposed to gap risk at the next funding settlement. Hidden beta: the position is
long/short crypto underlyings and carries crypto market beta; beta must be controlled explicitly.
Correlated risks: funding rates comove across crypto underlyings (S-086), so the book is a single
crypto-leverage bet.

**Falsifiable predictions and rejection conditions.**
1. *Reversal:* a high positive funding rate is followed by a negative futures-spot basis move
   (the crowded long side unwinds), and a high negative rate is followed by a positive basis
   move, within 1–3 funding periods. **Kill:** no mean reversion, or the basis moves in the same
   direction as the funding rate (momentum, not reversal).
2. *State scaling:* the size of the reversal is increasing in the funding-rate extreme (top vs
   bottom decile). **Kill:** no relation to the funding-rate level.
3. *Funding-carry contribution:* a material share of the return comes from the funding-rate
   payment itself (being on the receiving side), not only from the basis move. **Kill:** the
   reversal does not exceed the funding cost of holding the position.
4. *Venue transferability:* the effect holds on at least two exchanges with different funding
   implementations. **Kill:** the effect is exchange-specific, which would mean it is a venue
   artefact rather than a mechanism.
5. *Cost floor:* the gross reversal plus funding received exceeds round-trip cost (spread,
   slippage, funding paid while holding) in the selected underlyings. **Kill:** below cost in
   every selected underlying.

**Main confounders and rival explanations.**
- *Momentum feedback:* past returns predict futures-spot deviations with R² above 50% (S-086) —
  high funding rates may coincide with upward momentum, so the reversal may be a momentum
  continuation in disguise. The candidate must separate reversal from momentum.
- *Exchange-specific implementation:* clamp regions and calculation methods differ by venue, so
  an apparent effect on one exchange may not exist on another.
- *Custody and exchange risk:* crypto venue risk is real and is not diversifiable within the
  strategy.
- *The candidate may be a repackaged funding-rate arbitrage:* the honest null is that the
  documented arbitrage (long spot, short expensive perpetual) already captures the edge, and the
  reversal layer adds nothing.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: exchange-published funding rates (every funding
period, typically 8 hours), perpetual and spot prices, open interest and volume. Commercial:
exchange API access for historical funding rates and order-book data. Feasibility: **high** for
the data (all published by the venue); **medium** for the identification (the reversal must be
separated from momentum, and venue risk is real).

**Theory/evidence status.**
- *Conceptual rationale:* supported — the funding-rate mechanism and its role in keeping
  perpetual futures close to spot (S-086); deviations and arbitrage (S-086, S-087);
  funding-rate predictability (S-088).
- *Mechanism supported by sources:* yes for the funding-rate mechanism and the arbitrage
  (S-086, S-087); the *crowded-leverage reversal* specification is an unresolved conjecture.
- *Prior empirical support reported by others:* for deviations, arbitrage returns and funding-rate
  predictability (S-086, S-088, S-089); not for the joint reversal specification.
- *Unresolved:* whether the funding-rate level predicts a reversal after costs, whether the effect
  transfers across venues, and whether crypto venue risk is manageable.

**Remaining uncertainty / confidence.** Confidence that the funding rate is published, settled
every few hours, and measures the crowded-leverage state: **high** (exchange documentation and
academic work). Confidence that a tradeable reversal rule can be built on it: **moderate** — the
mechanism is real but the literature base is thin, momentum is a severe confound, and crypto
venue risk is unquantified here. Priority score **62/100**; rank **7 of 9** at the time of
writing. **Concrete next question:** does an extreme funding rate (top/bottom decile of its own
trailing distribution) predict a futures-spot basis reversal within 1–3 funding periods, after
costs and after controlling for momentum?

---

## IDEA-010 — CREDIT-ETF: corporate-bond ETF flow against dealer balance-sheet capacity

- **ID / short name:** IDEA-010 / CREDIT-ETF
- **Date added:** 2026-10-19 · **Cycle:** 4 · **Status:** candidate · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. New mechanism family not previously in the register.

**One-sentence hypothesis.** When corporate-bond ETF redemptions force authorised participants (who are also bond dealers) to absorb illiquid bonds onto already-constrained balance sheets, the ETF–NAV discount widens and the underlying bonds cheapen; the state (AP balance-sheet stress and ETF flow) is published, and the trade supplies the liquidity the AP cannot.

**Plain-language description.** Corporate-bond ETFs create and redeem shares through authorised participants — typically big bond dealers. When investors redeem ETF shares, the AP has to take the underlying bonds onto its own balance sheet temporarily. If the AP's balance sheet is already tight (dealers are constrained), the AP will demand a bigger discount to absorb those bonds, so the ETF trades at a wider discount to NAV and the underlying bonds cheapen. A participant who supplies the liquidity the AP cannot — buying the cheapened bonds or the discounted ETF — earns the concession when the AP's balance-sheet stress eases and the discount narrows.

**Mechanism.** APs use creations/redemptions to manage balance sheets; when balance-sheet space is scarce and bonds are costly to intermediate, APs become liquidity seekers in the ETF, widening the ETF–NAV gap and cheapening the underlying bonds (Pan & Zeng 2019). Dealer balance-sheet costs and interdealer capacity are published/measurable proxies (Eisfeldt, Herskovic & Liu 2024). The decision-time state is observable: ETF creation/redemption baskets and AP-level balance-sheet proxies are reported with known lags; the flow itself (ETF shares outstanding change) is published daily.

**Expected return source.** Compensation for bearing intermediary balance-sheet risk in the bond–ETF basis, harvestable when the gap exceeds the cost floor; the basis mean-reverts as AP capacity recovers.

**Originality.** Closest work: Pan & Zeng 2019 (AP balance-sheet constraints limit ETF arbitrage); Eisfeldt et al. 2024 (interdealer price dispersion / dealer capacity). Differentiator: a *state-conditioned, two-legged* specification keyed to published AP-stress proxies and a pre-scheduled exit, rather than a static basis trade. Honest classification: informed synthesis; the joint conditioning is an unresolved conjecture. Confidence: moderate.

**Target scope.** US investment-grade and high-yield corporate bond ETFs vs their creation baskets; daily state; holding 1–10 sessions; regime conditions: stressed dealer capacity, normal-to-high redemption flow.

**Observables (decision time).** ETF shares outstanding change (daily, published); ETF–NAV discount; AP balance-sheet proxies (dealer positions, interdealer price dispersion, SRF take-up); bond liquidity proxies (TRACE volume, dealer inventory); macro release calendar.

**Falsifiable predictions.** (1) ETF–NAV discount widens when AP-stress proxies are high and ETF flow is negative. (2) The discount mean-reverts within 1–10 sessions. (3) The effect is absent when AP capacity is ample (control). (4) Gross discount exceeds round-trip cost in selected ETFs. Kill: no state-dependence, no reversion, or effect below cost.

**Confounders.** Fundamental bond re-pricing during stress; index-rebalance flows; redemption-driven forced selling that is permanent, not temporary; dealer inventory accounting changes.

**Data requirements.** ETF prices/NAV, creation/redemption baskets, TRACE bond data, dealer position proxies, AP balance-sheet data. Feasibility: medium (TRACE is public; AP-level data is commercial).

**Theory/evidence status.** Conceptual rationale supported (Pan & Zeng 2019; Eisfeldt et al. 2024). Joint relation unresolved conjecture. Priority score 68/100; rank TBD.

**Constraints.** Cost/liquidity: corporate bond ETFs and their underlying bonds are less liquid than equities; the spread is crossed twice (ETF and bond); the discount itself is the edge, so transaction costs are first-order. Capacity: bounded by the size of the ETF's creation/redemption flow and by the liquidity of the underlying bonds; high-yield ETFs have the widest discounts but the thinnest underlying markets. Financing/margin: bond positions require margin; a leveraged basis trade consumes balance sheet exactly when dealer capacity is tight — the same constraint that generates the signal. Venue/operational: TRACE is public but with a lag; creation/redemption baskets are published daily by the ETF sponsor; AP-level balance-sheet data is commercial or inferred from dealer disclosures. Shorting constraints: not a borrow-constrained trade, but shorting corporate bonds is costly and recall-risk exposed.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the candidate predicts an edge only when dealer balance-sheet capacity is constrained; in normal times the ETF–NAV basis is narrow and the edge is absent. Tail: a credit stress event widens spreads permanently (fundamental re-pricing, not temporary discount), and the position is long illiquid bonds into a falling market. Crash behaviour: in a dealer balance-sheet crisis (e.g. March 2020), the basis can blow out and not mean-revert within the holding window; the AP may stop making markets entirely. Hidden beta: the position is long corporate credit and short ETF shares — it loads on credit spread duration and on the dollar (for USD-denominated bonds), and can carry event risk from issuer-specific news. Correlated risks: all bond ETFs in the same credit tier share the same dealer-capacity state, so the book is a single credit-cycle bet.

**Remaining uncertainty / confidence.** Confidence that AP balance-sheet constraints widen ETF–NAV discounts: **moderate** (Pan & Zeng 2019 documents the mechanism; dealer capacity is documented by Eisfeldt et al. 2024). Confidence that a tradeable two-legged rule can be built on published AP-stress proxies: **low-to-moderate** — AP-level data is commercial, the discount mean-reversion is unproven at the daily frequency, and the cost floor in thin bond markets is binding. Priority score **68/100**; rank TBD. **Concrete next question:** does the ETF–NAV discount in corporate-bond ETFs widen predictably when published AP-stress proxies are high and ETF flows are negative, and does it mean-revert within 1–10 sessions after costs?

---

---

## IDEA-011 — ACCTCLOCK: accounting-standards adoption as a slow-information-diffusion event clock

- **ID / short name:** IDEA-011 / ACCTCLOCK
- **Date added:** 2026-10-19 · **Cycle:** 4 · **Status:** candidate · **Version:** 1.0
- **Change notes:** v1.0 — initial dossier. New mechanism family not previously in the register.

**One-sentence hypothesis.** Mandatory adoption of a new accounting standard is a dated, regulator-announced information shock whose market reaction diffuses slowly because investors and analysts must re-learn the new numbers; the drift between the adoption announcement and the first full reporting cycle under the new standard is predictable in direction for firms whose pre-adoption information quality was low, and partly reverses once comparability is priced.

**Plain-language description.** When a regulator requires all companies in a market to switch to a new accounting standard (for example, IFRS in the EU in 2005), the announcement date is known years in advance. But the actual numbers under the new standard only appear in companies' first full financial reports after adoption. Until then, investors and analysts must re-learn what the numbers mean, and that learning happens slowly. Firms whose pre-adoption information quality was low — opaque earnings, few analysts, low foreign ownership — should see a bigger drift as the new standards are progressively understood, and part of that drift should reverse once the new numbers are fully digested and comparability is restored. A participant who positions before the first full reporting cycle under the new standard, sized by pre-adoption information quality, captures the slow-diffusion drift.

**Mechanism.** Mandatory IFRS adoption increased earnings information content and reduced stock-return synchronicity in the adoption year, with effects concentrated in firms with lower pre-adoption information quality and in strong-enforcement countries (Armstrong, Barth, Jagolinzer & Riedl 2010; Beuselinck et al. 2009; Lambertides & Mazouz 2013). The adoption dates are published by regulators (IASB/SEC/FASB) years in advance, so the clock is public and ex-ante knowable. The state (pre-adoption information quality, enforcement regime, analyst following) is observable from published filings.

**Expected return source.** Compensation for bearing slow information diffusion and comparability risk across the adoption window; a drift from announcement to first full reporting cycle, with partial reversal once the new numbers are fully digested.

**Originality.** Closest work: Armstrong et al. 2010; Beuselinck et al. 2009; Christensen, Lee & Walker 2007. Differentiator: a *dated, two-legged trade specification* keyed to the adoption calendar and to a pre-registered information-quality state, rather than an event study. Honest classification: informed synthesis of a documented effect; the two-legged specification is an unresolved conjecture. Confidence: moderate.

**Target scope.** Firms in jurisdictions with a mandated adoption date (EU IFRS 2005; other jurisdictions with announced adoption); announcement-to-first-full-reporting-cycle horizon; regime conditions: strong enforcement, no concurrent macro shocks.

**Observables (decision time).** Adoption announcement date and effective date (regulator-published); pre-adoption information quality proxies (earnings quality, analyst following, foreign ownership); enforcement regime (country-level); firm size; reporting lag.

**Falsifiable predictions.** (1) Low pre-adoption information-quality firms drift more from announcement to first full report under the new standard. (2) The drift is larger in strong-enforcement countries. (3) Part of the drift reverses within 1–4 quarters after the first full report. (4) High pre-adoption quality firms show a smaller, possibly negative, drift (convergence benefit). Kill: no information-quality interaction, no reversal, or effect explained by concurrent macro shocks.

**Confounders.** Concurrent macro/regulatory shocks; selection into adoption; the adoption event itself being a proxy for other reforms; size and liquidity differences; analyst coverage changes independent of the standard.

**Data requirements.** Regulator adoption calendars; firm-level returns; accounting-quality proxies; analyst following; country enforcement indices. Feasibility: high (all public, with a known adoption calendar).

**Theory/evidence status.** Conceptual rationale supported (Armstrong et al. 2010; Beuselinck et al. 2009). Two-legged specification unresolved conjecture. Priority score 64/100; rank TBD.

**Constraints.** Cost/liquidity: the affected firms may be small-cap or less liquid; the spread is crossed twice (entry and exit); the holding horizon is quarters, so financing and borrow costs accumulate. Capacity: bounded by the number of adoption events and by the liquidity of the affected firms; a single jurisdiction's adoption creates only one cross-section of firms. Financing/margin: a long/short book across firms is capital-intensive; borrow on the short leg can be scarce in small-cap names. Venue/operational: adoption dates are published by regulators but may change; the first full reporting cycle under the new standard may not align with the effective date (filing lags). Shorting constraints: short legs in small-cap, low-information-quality firms are the most expensive to borrow.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the candidate predicts an edge only around mandated adoption events; outside adoption windows there is no signal. Tail: the fundamental anchor can break if the adoption itself is delayed, watered down, or accompanied by other reforms — the trade becomes a directional loss unrelated to information diffusion. Crash behaviour: a market-wide crash during the adoption window confounds the diffusion drift with broad re-pricing; the exclusion rule (no concurrent macro shocks) must be applied before any result is read. Hidden beta: the long/short book loads on size, value, and momentum factors; low-information-quality firms tend to be smaller and less liquid. Correlated risks: all firms in one adoption jurisdiction share the same event date; a single jurisdiction-level shock dominates many firm-level results.

**Remaining uncertainty / confidence.** Confidence that accounting-standards adoption changes information quality and is dated in advance: **high** (Armstrong et al. 2010; Beuselinck et al. 2009). Confidence that a tradeable two-legged rule can be built on pre-announced adoption calendars: **moderate** — the state is public, the dates are known, but the drift is slow and the sample of adoption events is small (a handful of jurisdictions). Priority score **64/100**; rank TBD. **Concrete next question:** do firms with low pre-adoption information quality show a predictable drift from the adoption announcement to the first full reporting cycle under the new standard, with partial reversal afterward, after costs?

---

---

## IDEA-012 — CLS-CLOSE: the settlement-side deadline cluster as a price determinant (continuation of IDEA-006)

- **ID / short name:** IDEA-012 / CLS-CLOSE
- **Date added:** 2026-10-19 · **Cycle:** 4 · **Status:** **rejected (R-010)** · **Version:** 1.1
- **Change notes:** v1.0 — initial dossier. New mechanism family not previously in the register; a dedicated vehicle for the settlement-side residual of IDEA-006, blocked on G-11.
  **v1.1 — REJECTED after the Cycle-5 G-11 closure (S-112 … S-121).** The candidate existed to be a
  literature check: "if the settlement-side cluster is tested and found priced, IDEA-006 and IDEA-012
  are both rejected; if untested, they remain as narrow, unproven residuals." The check was run and
  returned "tested and found priced": a settlement deadline cluster is a published price determinant
  (S-112 — the CLS pay-in schedule raises the price of intraday liquidity by an estimated "roughly
  1.5bp for the CLS settlement cycle"), the securities settlement cycle is a published price-impact
  determinant (S-113, S-114, S-115), the FX settlement-risk premium is published (S-082, S-071), and
  the post-US-close FX window is documented as a cost, not an edge (S-117, S-118, S-119, S-120). The
  candidate's own "key uncertainties" section stated the consequence in advance: "If G-11 closes
  against the candidate … the candidate is rejected, not re-scored." **The dossier is closed; the
  reasoning is preserved in R-010.**

**One-sentence hypothesis.** Beyond the published 16:00 London fix effect, the CLS currency-close and pay-in deadlines (and the post-US-close window created by T+1) create a separate, dated, settlement-constrained demand/supply pressure in specific currency pairs on no-macro-release days; the state (deadline proximity and fix-window volume share) is published by the benchmark administrator and the settlement utility.

**Plain-language description.** Once a day, the world's currencies have to be settled. CLS members must have the right currency in the right place by hard cut-offs — the currency close at midday CET, the initial pay-in schedule issued at 00:00 CET, the settlement completion target at 09:00 CET. Since the US moved to T+1 in May 2024, when the US equity market closes at 16:00 EST (22:00 CET), there are only about two hours to arrange the currency for US securities settlement. That is a predictable, dated, price-insensitive demand for currency in a window that is not a benchmark — funds must fund their settlement obligations whether they want to or not. Whoever supplies liquidity into that settlement-constrained flow earns a temporary price concession that reverses once the deadline passes.

**Mechanism.** The 16:00 London fix effect is published (Melvin & Prins 2015; Evans 2018; Ito & Yamada 2015). The settlement-side mechanics are documented (CLS pay-in schedule, currency-close deadlines, Banque de France / ECB documentation) and are a priced friction (Ranaldo & Santucci de Magistris 2022; Lee, Ranaldo & Tsuruga 2026 IMF WP), but the specific CLS deadline cluster / post-US-close T+1 window is untested (G-11). The state is published: the CLS settlement timeline, the benchmark administrator's calendar and holiday notices, and the fix-window volume share.

**Expected return source.** A liquidity-provision premium for supplying liquidity to settlement-constrained participants in the post-US-close window; partial reversal once the deadline passes.

**Originality.** Closest work: Melvin & Prins 2015; Evans 2018; Ito & Yamada 2015 (fix window, published). Differentiator: the *settlement-side* residual beyond the fix, which no located paper tests. Honest classification: informed conjecture pending G-11 closure; if a published paper tests the settlement-side cluster, this candidate is rejected, not narrowed. Confidence: low-to-moderate.

**Target scope.** Liquid currency pairs with adequate fix-window volume; no-macro-release days; pre- and post-T+1 (May 2024) split; intraday windows.

**Observables (decision time).** CLS settlement timeline and pay-in deadlines (published); benchmark administrator calendar and holiday notices; fix-window volume share for the pair; macro-release calendar; quoted spread and depth.

**Falsifiable predictions.** (1) On no-release days, the post-US-close settlement window shows a signed move in the funding direction after the fix effect is removed. (2) The effect is absent pre-T+1 (settlement calendar change). (3) The effect is absent in a placebo window of the same length. (4) Gross concession exceeds round-trip cost. Kill: placebo performs the same, effect vanishes net of costs, or G-11 closes against the candidate.

**Confounders.** Macro releases inside the window; the fix effect itself (must be removed); liquidity-provider pre-positioning; non-settlement intraday drift; holiday/alteration days.

**Data requirements.** Intraday order-book or print data for the pairs; published benchmark calendar; CLS timeline; macro-release calendar. Feasibility: medium-low (intraday data is the binding constraint; the published fix literature used administrator-provided data).

**Theory/evidence status.** Conceptual rationale: settlement-side mechanics are a priced friction (S-082, S-071). Specific deadline-cluster price effect: unresolved conjecture (G-11). Priority score 60/100; rank TBD.

**Constraints.** Cost/liquidity: the concession is measured in pips inside a few minutes, so spread and slippage are first-order; this is the binding constraint. Capacity: bounded by the fix-window depth of the pair and by the size of the deadline-constrained flow. Market impact: trading into a concentrated deadline window is an impact machine. Venue/operational: the fix is a benchmark calculation, not an execution venue — the trade must be executed around it, not at it; execution infrastructure around the fix is expensive. Financing/margin: negligible for spot, relevant for leveraged forward positions. Shorting constraints: not a borrow-constrained trade.

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: entirely deadline-dependent — on an ordinary day the deadline flow is small; at month-end or on a T+1 settlement peak it is not. Tail: a market disruption (a failed settlement, a benchmark suspension, a forced closure) is exactly when the deadline binds hardest and when liquidity is worst, so the position is most likely to be held exactly when it cannot be exited. Crash behaviour: a benchmark suspension removes the trade entirely; a settlement stress can force the deadline to bind on multiple currencies simultaneously. Hidden beta: the position is a short/long in the funding currency around a deadline, so it loads on the funding-coinage and the basis trade, and can carry an event risk that is not visible in the return. Correlated risks: all pairs sharing the same funding currency respond to the same deadline, so the book is a single funding-currency bet.

**Remaining uncertainty / confidence.** Confidence that the deadlines, the participant set and the flow concentration are real and published: **high** (CLS documentation S-048, S-049; LSEG methodology S-045). Confidence that the settlement-side deadline cluster has a separable price effect: **low** — G-11 is open, so this is an expectation rather than a finding. Confidence that any of it is harvestable after costs: **low** (the pip-level concession inside minutes is the decisive weakness). Priority score **60/100**; rank TBD. **Concrete next question:** does any published work test the settlement-side deadlines — the CLS currency-close and pay-in cut-offs, and the post-US-close window created by the May 2024 T+1 transition — as a price determinant rather than as an operational schedule, and if not, does the settlement window show a directional imbalance that survives removal of the published fix effect?

**v1.1 closure (Cycle 5).** The question above was run as a literature check and answered
disqualifyingly. Settlement deadlines **are** tested as price determinants in the published
literature: Kraenzlin and Nellen (2010, S-112) show that the CLS pay-in schedule raises the value of
intraday liquidity during the settlement cycle, with an estimated "roughly 1.5bp for the CLS
settlement cycle"; Baig, Breeze, Cox and Griffith (2022, S-113), Bhanu, Nath and Patnaik (2024,
S-114) and Shah and Davda (2026, S-115) make the securities settlement cycle a published
price-impact and market-quality determinant. The FX settlement-risk premium is published (S-082,
S-071). The remaining, narrower question — the *post-US-close window's* own market quality — is
answered by the institutional record as a **cost**: the New York Fed's FX Committee material names
the 4–6pm ET window as the transition's priority FX risk (S-117) and records the market's
expectation of "an uptick in price premium and market impact for trades executed later in the NY
trading day" (S-118); the trade record shows "less than 1% of trades in the $7 trillion OTC FX
market are carried out in this window", pricing engines shut at 5pm for up to half an hour, and
"bid/ask spreads widen and liquidity shrinks" (S-119); the after-action reporting shows the market
solved the constraint with custodian cut-off extensions and pre-funding, not with concession capture
(S-120). A concession priced inside a window with under 1% of volume, widening spreads and a
half-hour pricing-engine outage cannot survive a round trip. **Status: rejected (R-010).** The
mechanism is documented; the *edge* was never evidenced and the cost structure rules it out.

---

---

## IDEA-013 — EU-ETSCOMP: the surrender-deadline concession in the EU ETS, and the published banking position that decides whether it exists

- **ID / short name:** IDEA-013 / EU-ETSCOMP
- **Date added:** 2026-10-19 · **Cycle:** 5 · **Status:** **parked (P-008)** · **Version:** 1.1
- **Change notes:** v1.0 — first dossier. New mechanism family for the register: a **statutory,
  date-bound purchase obligation** with a monetary penalty, in a market whose decision-time state is
  published by a regulator. The *effect* (a surrender-month premium) is published (S-101); the
  candidate claims only the two things the published work does not cover — the **regime change**
  (the deadline moved from 30 April to 30 September from 2024, outside the published sample) and the
  **existence-flipping state** (a pre-deadline published aggregate compliance balance). The full
  text of the published work (NBER WP 35356 / arXiv 2606.03767) **must be read before this candidate
  is retained**; see "Remaining uncertainty".
  **v1.1 — the required full-text check was performed, and the candidate is parked (P-008).** Three
  findings, all verified in this cycle. (i) **The check is resolved in the candidate's favour and
  against it at once:** S-101 does **not** condition the premium on the aggregate surplus (there is
  no occurrence of "TNAC" in the paper; the aggregate balance appears only as a state variable
  *inside the model*, and the paper's "cumulative surplus" measure is used to *construct*
  operator-level shortfalls, not to explain premium variation) — so the candidate is not a
  re-description of published work. But the published model already makes the benchmark price affine
  in the aggregate bank, so the state-conditional structure is **implied by the published model**; what
  the candidate claims is an *empirical* conditional structure that the published work does not
  estimate. (ii) **The published sample does not support the existence-flipping hypothesis and mildly
  cuts against it:** the paper states that "This delayed and frictional trading pattern persists into
  the most recent phase of the EU ETS, indicating limited improvement over time", and its most recent
  phase is Phase IV (2021) — a period of very large aggregate surplus (TNAC 1 134 794 738 for 2022
  and 1 111 736 535 for 2023, S-121). The paper does not report the April premium's magnitude by
  year, so the hypothesis is neither supported nor refuted by the published sample; what the sample
  shows is that a large surplus did **not** switch the effect off. (iii) **The decision-time state
  was, until the regime change, published *after* the deadline it was supposed to inform** — the
  Commission publishes TNAC for emissions year Y in late May or June of year Y+1 (S-121), so under
  the pre-2023 regime (surrender deadline for emissions of year Y: 30 April of year Y+1) the aggregate
  state for the compliance year was published **after** that deadline. Decision-time availability
  begins only with the 2023 compliance year (deadline 30 September 2024), which leaves **three
  decision-time observations to date** (2023, 2024 and 2025 compliance years) and **no observation in
  a deficit year**. This is recorded as the new gap **G-13** and as a new screening condition in the
  state-proxy note: *a published state is usable as a decision-time variable only if it is published
  before the decision.*
  **Why parked rather than retained or rejected.** The effect is published (S-101), so this is not a
  discovery; the claimed residual is not refuted, but the candidate cannot be *validated* in any
  decision-time form: the state switches sign too rarely for a conditional claim to be testable, the
  published model implies the conditional structure rather than leaving it open, and the published
  sample contains a high-surplus year in which the effect persisted. Re-specifying around a weaker
  state (operator-level bank-adjusted shortfalls, which are public only *ex post* in the EUTL) would
  convert the idea into a disguised baseline. The honest position is a **park** with a dated
  unblocking question, not a retention and not a rejection.

**One-sentence hypothesis.** The EU ETS obliges every covered installation, aircraft operator and
shipping company to surrender allowances for the previous year's verified emissions by a statutory
date, penalising failure at €100 per tonne — an obligation that is therefore almost perfectly
price-inelastic — and the resulting deadline-bound demand creates a surrender-month premium paid by
delayed compliance officers to their counterparties; the candidate's claim is that this premium is
**not a standing feature** but an **existence-conditional** one, appearing only in years when the
aggregate compliance balance is short, a balance that is knowable *before* the deadline from
regulator-published data — though, as v1.1 records, that property holds only in the current regime,
from the 2023 compliance year onwards — and that the published result covers only the *old* deadline
regime.

**Plain-language description.** Every year, an installation that emitted a tonne of carbon last year
must hand over one allowance to the government by a fixed date, or pay €100 for every tonne it
fails to cover — roughly the price of the allowance itself, so the obligation is effectively hard.
A firm that has been sitting on its allowance budget all year cannot wait for a better price; it
must buy in the deadline month, and it buys from whoever is willing to sell — usually a bank or a
fund that has been holding the allowance. The buyers pay up. But this only happens when the system
as a whole is *short*: if firms are sitting on a large surplus of banked allowances, nobody is
forced to buy anything in the deadline month and the premium does not exist. Whether the system is
short is not a secret — the regulator publishes, every May or June, the total number of allowances
in circulation, which is a direct read on the surplus. **But** (v1.1) that publication arrives in
late May or June of the year *after* the emissions year, so before the 2023 compliance year it
arrived *after* the surrender deadline it was meant to inform, and the "knowable before the
deadline" property of this state is a property of the **current regime only**.

**Mechanism (causal chain).**
1. **The obligation is statutory and hard.** Under Article 12(3) of Directive 2003/87/EC, "by
   30 September each year" the operator of each installation, each aircraft operator and each
   shipping company must surrender allowances equal to its verified emissions for the preceding
   calendar year (S-102). Failure to surrender on time attracts a penalty of **€100 per tonne** for
   the missing allowances, and the **names of penalised operators are made public** (S-101). A
   penalty of that order relative to the allowance price makes the demand curve almost perfectly
   inelastic in the deadline window — the textbook condition for a concession.
2. **The calendar is published and the timing is a policy variable.** Emissions must be verified by
   an accredited verifier by **31 March**; the surrender deadline was **30 April** under the
   original regime and was moved to **30 September** by Directive (EU) 2023/959, applying from the
   2024 compliance year onwards (S-102, S-103). The market monitors have already observed that the
   shift "spread out demand" and that "December saw the highest volumes, as is typical" (S-104) —
   so the *aggregate* relocation of the pressure is documented; what is not documented is the
   *conditional* structure below.
3. **The published effect.** Borri, Liu, Tsyvinski and Wu find that "purchases concentrate in April
   when returns are systematically high, and operator flow predicts future returns"; that "this
   concentration of compliance demand is associated with systematically high April returns, averaging
   about 10%"; and they estimate "the implied April premium paid by delayed buyers from this
   surrender pattern at about €5 billion" — while being careful that the premium "should be
   interpreted as a financial premium paid in April rather than as a direct measure of aggregate
   resource costs, because part of the higher April price is paid to counterparties" (S-101). Their
   model makes the mechanism explicit: "access determines residual compliance demand, intermediary
   constraints translate residual demand into a surrender-month premium, and the premium feeds back
   into access incentives."
4. **The published sample predates the regime change.** The empirical work covers **2005–2021**
   (S-101). The deadline moved to 30 September for the 2024 compliance year. The published effect
   therefore has **not** been re-established in the regime that is now law, and the market
   structure around it has changed: the MSR has been withdrawing allowances into the reserve since
   September 2024, and the 2027 auction calendars were published on 1 October 2026 with the
   2027 volumes already adjusted for the reserve and for the Social Climate Fund allocation
   (S-105, S-106).
5. **The state is published before the deadline — but only in the current regime — and it flips the
   sign of the effect.** The
   Commission publishes, every year, "the total number of allowances in circulation (TNAC) for the
   previous year" under Article 1(4) of the MSR Decision; the market monitors describe TNAC as "an
   indicator for the surplus" (S-107). The Commission published TNAC for 2023 — 1,111,736,535 — on
   **3 June 2024**, which is after the March verification deadline and before the September
   surrender deadline, and thereby determined that 266,816,768 allowances would be withheld from
   the auction volumes from 1 September 2024 to 31 August 2025 (S-107). Verified emissions, free
   allocation and the cross-sectoral correction factor are also published (S-108, S-109). TNAC,
   the auction calendar and the verified-emissions data therefore allow the **aggregate compliance
   balance for the year whose deadline is approaching** to be estimated before that deadline —
   **in the current regime only** (v1.1: the TNAC publication calendar is late May or June of the
   *following* year, so under the pre-2023 April deadline the balance for the compliance year was
   published after that deadline; see the timing finding below and gap G-13).
6. **The sign discipline.** If the aggregate balance is short, the deadline creates a forced,
   price-inelastic *buyer* and the allowance price should be pushed up into the deadline, with the
   concession partly unwound afterwards as the forced demand disappears. If the aggregate balance is
   long, there is no forced buyer, the deadline effect should be **absent**, and the residual
   pressure in the year should appear elsewhere (the December volume pattern the market monitor
   already reports, S-104). The candidate's prediction is therefore *two-sided*, and the negative
   case is as informative as the positive one: **a deadline premium that appears in every year is
   evidence against the candidate**, because it means the effect is not state-conditional.
7. **The counterparty side is not a compliance entity.** The seller into the deadline is a
   non-compliance holder — a bank, a fund or another non-compliance entity — and the market
   monitor's own data show the "number of entities invested in EUA futures and not regulated under
   the EU ETS Directive" rising to around 900 on average in 2024, a jump of about 15% year on year
   (S-104). This is the "who is mispriced" leg the prompt requires: the compliance officer is
   *forced* to transact and pays a premium; the non-compliance holder *chooses* to transact and
   collects it.

**Expected return source.** A compensation for supplying allowances to a date-bound, penalty-backed
mandated buyer — a *liquidity-provision premium*, not a risk premium for systematic exposure, and
not the carbon-price trend itself. The premium exists because the obligated buyer's demand is
insensitive to price near the deadline; the provider is compensated for the price risk of holding
the allowance into the window and for the concentration of the exit.

**Originality.**
- *Closest known work:* Borri, Liu, Tsyvinski and Wu (S-101) — a NBER working paper with a formal
  model and 2.7 million registry transactions, and the direct statement of both the effect and the
  mechanism; the earlier versions of the same project (S-111) are the same work, not separate
  evidence. The market-structure and pricing background is in the European Commission's own
  auctioning documentation (S-105), the Commission's TNAC communications (S-107), the national
  authority's auction-calendar notices (S-106) and the annual independent market report (S-104).
  The venue and rule documentation is S-102, S-103.
- *What is already known:* that purchases concentrate in the surrender month; that returns in that
  month are systematically high (about 10% on average); that the implied premium is of the order of
  €5 billion; that operator flow predicts future returns; that roughly 40% of operators do not
  trade in a given year; and that the premium is a payment to counterparties rather than a resource
  cost.
- *Substantive differentiator claimed here:* (i) **the regime** — the published sample ends in 2021
  and the deadline that is now law is a different deadline, so the published result is not a
  statement about the current regime; (ii) **the state** — the premium is predicted to be
  *existence-conditional* on the aggregate compliance balance, which is knowable before the
  deadline from regulator-published data (TNAC, verified emissions, the auction calendar and the
  MSR decision), so the condition is decision-time observable rather than an ex-post
  classification; (iii) **the falsification structure** — the candidate can be killed by a
  deadline premium that appears in surplus years as well as deficit years, which is the outcome
  that the published framing would lead one to expect.
- *Honest classification:* **published effect, with an unclaimed conditional structure and an
  unexamined regime.** This dossier must never be described as a discovery of the surrender-month
  premium — that is S-101's result. What is claimed is that the premium is conditional and that the
  condition is published in advance. The condition is a *conjecture*; nothing here establishes that
  the premium is state-conditional, and the kill conditions below are written so that it can fail.
- *Confidence in the comparison:* **moderate, and now checked.** The full text of S-101 (arXiv HTML
  rendering, v2) **has been read** in Cycle 5. The verdict: the paper does **not** condition the
  surrender-month premium on the aggregate surplus, so the candidate's central claim is not
  pre-empted; but the paper's *model* already makes the equilibrium price affine in the aggregate
  bank of allowances, so the state-conditional structure is an implication of the published model
  rather than an unclaimed idea about the mechanism; and the paper's own robustness construction
  works from **operator-level, bank-adjusted** shortfalls, which implies the aggregate balance is
  not the object that determines residual demand. The full text also supplies two facts that the
  v1.0 dossier did not have: the statement that the delayed-trading pattern "persists into the most
  recent phase of the EU ETS" (Phase IV, 2021 — a high-surplus year), and the fact that the paper's
  own counterfactual analysis of **staggered surrender deadlines** already reduces the premium by
  about 59%, which is directly relevant to the regime change the candidate relies on. **What remains
  unclaimed** is an *empirical* estimate of how the premium varies with the published aggregate
  balance across the regime change.

**Target scope.** EU allowances (EUA) on the ICE futures and options venue and, at lower frequency,
the EEX auction clearing price; the compliance window from the verification deadline (31 March) to
the surrender deadline (30 September from 2024; 30 April in the earlier regime); annual frequency
with one observation per year, and a pre-2024 sub-sample with one per year at the April deadline.
Regime conditions: exclude the ETS2 sector expansion (buildings and road transport, surrender
deadline 31 May from 2028) from any early sample; exclude years in which the *policy* cycle
dominates (the October-November annual review, the MSR decision and the free-allocation
adjustment) from the estimation window, and treat them as controls rather than as signal.

**Observables (knowable at decision time, conceptually).**
- The statutory calendar: verification deadline 31 March, surrender deadline 30 September from 2024
  (S-102, S-103) — published, statutory, not a forecast.
- The aggregate compliance balance: TNAC for the compliance year (published by the Commission in
  late May or June of the year of the deadline — **available before the deadline only from the 2023
  compliance year**), the verified-emissions dataset, the free-allocation and
  cross-sectoral-correction-factor decisions, and the EEX auction calendar with its volumes
  (S-105, S-106, S-107, S-108, S-109, S-121).
- The MSR's effect on the auction supply in the compliance window (the reserve's withholding
  schedule, which the Commission and the national authority both publish) (S-106, S-107).
- The published market data used as the mechanism check: EEX daily auction results and quarterly
  auction reports including participant counts (S-105).
- *Timing hazards to flag for the validator:* the surrender and compliance data for year Y are
  published by 6 October of Y+1 (S-110) — that is **after** the deadline, so they can only be used
  for an ex-post check of the state, never for the decision; the auction calendar and the MSR
  adjustment are published in advance but their *interpretation* is not; and the sample has one
  observation per year, so the effective sample is very small and every additional control
  (year fixed effects, the policy cycle) costs degrees of freedom.
- **The decisive timing finding of Cycle 5 (G-13):** the aggregate state itself has a publication
  calendar that must be checked against the decision date. The Commission publishes TNAC for
  emissions year Y in **late May or June of year Y+1** — TNAC for 2022 on 15 May 2023, for 2023 on
  3 June 2024 (S-121). Under the pre-2023 regime the surrender deadline for emissions of year Y was
  **30 April of year Y+1**, i.e. the aggregate balance for the compliance year was published
  **after** the deadline it was meant to inform, and the state a rule could have used before that
  deadline was the balance for year Y−2. Under the post-2023 regime (deadline 30 September of year
  Y+1) the balance for year Y is published **before** the deadline. **Consequence:** the
  *decision-time* form of this candidate can only be run from the **2023 compliance year** onwards —
  three observations so far (deadlines of 30 September 2024, 2025 and 2026), all in a period of large
  aggregate surplus, with **no deficit observation**. The *ex-post* form can be run over the whole
  published sample, but an ex-post state is a decomposition, not a rule.

**Rule sketch (descriptive, non-executable).** Once a year, after the Commission has published the
TNAC figure for the compliance year (which, in the current regime, happens in late May or June of
the year of the deadline) and the auction calendar for that year, and before the surrender
deadline: estimate the aggregate compliance balance for the year whose deadline is approaching as
(verified emissions for that year, net of the free allocation and the CSCF adjustment) minus the
allowances the system is holding net of what it has already surrendered — a quantity the published
TNAC series and the surrender data jointly bound. If the balance is short, form a long position in
the front-of-deadline allowance future, held to the deadline; if the balance is long, form no
position. Size the position by the *estimated shortfall* relative to the *published auction volume*
for the compliance window, and cap it at a pre-specified fraction of the contract's average daily
volume. Exit on the settlement of the deadline-week contract. Exclude any year in which the
October-November policy cycle or a link to the Swiss ETS produced a repricing, and record those
years as excluded rather than as failures. **Feasibility note (v1.1):** this rule can only be run
from the **2023 compliance year** onwards, because before that the TNAC for the compliance year was
published after its deadline (G-13) — three observations to date, none in a deficit year, so the
rule as written cannot yet be evaluated on a state switch.

**Persistence thesis.** The obligation is statutory and the penalty is a multiple of the allowance
price, so the deadline demand cannot be avoided; the compliance calendar is published a year ahead
in the directive; and the market's structure around it (a small number of non-compliance sellers
and a fragmented set of obligors) changes slowly. A premium that is paid annually to the party
that provides the allowance in the window is a structural transfer, not an anomaly.

**Constraints.** Cost/liquidity: the EUA futures market is liquid enough for institutional size but
is an order of magnitude smaller than rates or equity futures, and the spot market is thin; the
*effect* is large (about 10% in the published April sample) but so is the *noise* from the policy
cycle, so a small net edge after costs is possible and must be checked rather than assumed.
Capacity: a non-compliance participant is needed on the *supply* side of the trade, and a
participant that is not a compliance entity can be on either side; a pure compliance officer cannot
short. Market impact: in a one-year sample, a single position can move the price it is predicting.
Venue/operational: EUA futures are cash-settled on ICE with a published contract specification
whose expiry list changed when the deadline moved (S-102) — the contract calendar must be
reconstructed for the pre-2024 sample, because the April deadline and the September deadline imply
different expiries. Shorting constraints: shorting an allowance future is available but the
position carries the risk of an unscheduled policy announcement (the "carbon price crash" risk).

**Regime sensitivity, tail exposure, crash behavior, hidden beta.** Regime: the candidate is
*defined* by the compliance regime and by the annual policy cycle. Tail: the EUA market has
repeatedly had policy-driven 30–60% drawdowns, and a position held into the deadline is exposed
to them. Crash behaviour: the position is *long* the allowance into a window in which the policy
calendar is quiet, so it is exposed to a negative policy shock arriving without warning (a
re-based cap, a lower auction volume, a link to a cheap foreign market). Hidden beta: the long
allowance position is a long *carbon-transition* position, so it loads on the regulatory-trend
factor and on the energy complex, and the "premium" may be compensation for exactly that exposure
rather than for liquidity provision — a confound that the state-conditioning does not remove.

**Falsifiable predictions and rejection conditions.**
1. *Existence-conditionality (the primary test):* the deadline premium is present in years when
   the pre-deadline published aggregate balance is short and absent (or of the opposite sign) in
   years when it is long. **Kill:** the premium is of similar size in surplus and deficit years —
   in which case the effect is unconditional, the state adds nothing, and the candidate is a
   re-description of S-101. **Cycle-5 status: untestable in decision-time form, and partly
   pre-answered.** The decision-time test has at most three observations, none in a deficit year
   (G-13); and the published sample contains a high-surplus year (Phase IV, 2021) in which the
   delayed-trading pattern persisted, which is evidence against the sign flip. Both facts are
   recorded here rather than buried, and they are the reason the candidate is parked.
2. *Regime discontinuity:* the effect's month moves with the statutory deadline — April in the
   pre-2024 regime, September thereafter — and is not a fixed calendar month. **Kill:** the premium
   remains concentrated in April after the legal change, which would mean the April pattern is
   driven by something other than the surrender obligation.
3. *Mechanism check with published data:* the EEX auction volumes and participant counts rise in the
   compliance window of deficit years and not in surplus years (S-105). **Kill:** the published
   auction data show no such difference, which would undercut the demand-concentration mechanism.
4. *Reversal:* after the deadline, part of the pre-deadline concession unwinds (the price gives
   back part of the deadline move) in deficit years. **Kill:** there is no post-deadline reversal,
   which would mean the move is a permanent repricing rather than a concession, and there is no
   liquidity-provision premium to capture.
5. *Cost floor:* the estimated pre-deadline premium minus the round-turn cost in the EUA future
   (spread, commission, financing) is positive. **Kill:** it is not, in which case the candidate is
   a description and not a trade.
6. *Pre-registration:* the *rule* — long the allowance future if and only if the published balance
   is short — must be fixed before the outcome data are examined, and it must be evaluated on the
   pre-2024 April regime and the post-2023 September regime as two separate samples, with the
   sign-flip prediction stated in advance for both.

**Main confounders and rival explanations.**
- *The policy cycle* — the October-November review, the MSR decision, the free-allocation
  adjustment and the cap decisions move the allowance price far more than a deadline month
  normally does; the deadline is inside the calendar year but the *effect* may be an artefact of
  the surrounding announcements.
- *The energy complex* — EUA prices co-move with gas and power prices, so a "deadline premium"
  may be a power-sector hedging demand story: the fuel-switching channel is identified in the
  literature as a major driver of allowance prices.
- *Speculative positioning* — the ECB's own economic bulletin documents the role of non-compliance
  participants and of speculative flows in allowance price moves, which cuts both ways: it is an
  alternative explanation for the deadline premium and a supply-side explanation for who collects it.
- *Free allocation and the CSCF* — the aggregate balance depends on free allocation, which is
  adjusted ex post and may dominate the surrender obligation itself.
- *The banking constraint* — operators that bank a surplus in one year are the ones that can afford
  to miss the deadline in another; the "40% of operators do not trade" finding (S-101) is a
  reminder that the *marginal* obligor is not the average one.
- *Small sample* — one observation per year is a very weak basis for a conditional claim, and this
  is the most serious design weakness in the candidate.

**Data requirements and feasibility for a future independent validation.** (Specification only —
nothing is acquired or processed here.) Public: the statutory calendar (S-102, S-103); the TNAC
communications (S-107); the verified-emissions and free-allocation data and the Union Registry
public data and the EEA data viewer (S-108, S-109); the EEX auction calendars, daily auction
results and quarterly auction reports (S-105); the national authority's notices (S-106); the annual
market report (S-104). Commercial or venue-priced: the EUA futures price history (ICE settlement
data) and the EUTL transaction-level files (public but bulk, and the transaction data are
commissioned-research-grade). Feasibility: **medium-high** for the state and the calendar, and
**medium-low** for the price series and the sample size. The binding constraint is not data
availability but the **number of independent observations**: one per year against a state that
must be estimated, not observed — and, after the Cycle-5 timing finding (G-13), **only three
years in which the state was published before the decision at all**.

**Theory/evidence status.**
- *Conceptual rationale:* supported — the mechanism, including the "intermediary constraints
  translate residual demand into a surrender-month premium" step, is formalised in S-101, and the
  penalty-backed near-inelasticity of the obligated demand is a direct reading of the statute and
  the penalty schedule.
- *Mechanism supported by sources:* **yes** — the obligation, the penalty, the calendar, the
  auction calendar and the TNAC publication are all documented (S-102 … S-109).
- *Prior empirical support reported by others:* the surrender-month premium, the April
  concentration, the flow-return predictability and the €5 billion estimate are the authors' own
  (S-101) and are **not** reproduced here.
- *Unresolved:* whether the premium is state-conditional; whether it survives the deadline change;
  whether any part of it is a policy-cycle or fuel-switching artefact; and whether the published
  work already answers the state question.

**Remaining uncertainty / confidence.** Confidence that the obligation, the penalty and the
published state exist: **high**. Confidence that the deadline premium exists in the current
regime: **moderate** — the published result is strong but its sample ends in 2021, and the market
monitors' own reading of the shift is that demand was "spread out", which is the opposite of a
sharp deadline premium. Confidence that the premium is *state-conditional*: **low** — this is the
candidate's conjecture; the full text of S-101 (read in Cycle 5) neither tests it nor supports it,
and its Phase IV persistence statement shows that a very large surplus did not switch the effect
off. Confidence that it is tradeable after costs: **low-to-moderate** — thin market, small sample,
large policy-event risk. **Feasibility of the decision-time rule: low** — the state is published
before the decision only from the 2023 compliance year, leaving three observations, none of them in
a deficit year (G-13). Priority score **58/100** (down from 70: the first check was resolved
favourably, but the model-implied conditional structure, the contradicting persistence statement
and the decision-time sample cut the other way); rank 10 of 10 retained-or-parked candidates at the
time of writing. **Status: parked (P-008).** **Concrete next question (dated, and it is a
data-accumulation question, not a research question):** the unblocking event is the accumulation of
enough post-2023 compliance years for the *ex-post* balance to move across a sign change with at
least one observation on each side. The next published TNAC is for emissions year 2026, expected in
late May or June 2027 (S-121's calendar); the corresponding surrender deadline is 30 September
2027. **Before 2029, the candidate cannot be validated in any decision-time form, and the register
should not spend further effort on it.** A secondary question, worth one search only: whether the
published literature has yet replicated the April premium in the post-2023 September regime — if a
replication exists, the *regime* residual is closed too and the candidate should be rejected rather
than parked.

---

## State-proxy methodological note (closing section)

**Purpose.** This note answers the question deferred by Cycles 1 and 2: how to choose, build and
validate a state proxy, and when the honest answer is "no public proxy exists — park the
candidate rather than re-specify it." It governs every candidate in the register whose mechanism
depends on a latent state.

**1. The state-proxy problem is largely a venue-selection problem.**
IDEA-002 (equities, funding state) is parked because no public funding-state proxy exists
(G-01); IDEA-007 (FX, dollar funding state) works because the BIS publishes the state on a known
calendar (S-052, S-054). IDEA-004 (equities, crowd depth) is blocked because the crowd proxy is
quarterly-stale (G-04); IDEA-005 (futures, passive share) works because the CFTC publishes Index
Trader positions weekly (S-030). IDEA-008 (securities lending, borrow cost) works because short
interest and lending fees are published; IDEA-009 (crypto perpetuals, funding rate) works because
the exchange publishes the funding rate every few hours. The pattern is deterministic: *do not
hunt for a proxy; hunt for a venue where the state is already published by an institution.*

**2. How to choose a state proxy.**
A state proxy must satisfy all five conditions:
(a) **Observable at decision time:** the value must be knowable before the trade is executed,
   with the true publication lag respected. A quarterly holdings file used on a daily rule is
   look-ahead, not a proxy.
(b) **Published by an institution:** an exchange, regulator, benchmark administrator, settlement
   utility, or official statistics body releases it on a fixed calendar. Vendor-constructed
   series are proxies of proxies and must be labelled as such.
(c) **Causally connected to the mechanism:** the proxy must measure the binding constraint or
   flow that generates the edge, not a correlated variable. The carry channel is a rival
   explanation for the funding channel; the proxy must separate them.
(d) **Changes the sign or existence of the effect:** conditioning on the proxy must change the
   *sign* or the *existence* of the predicted return, not merely its size (per the rediscovery
   guard in `rejected_and_parked.md`).
(e) **Published before the decision, not after it** (added in Cycle 5, gap **G-13**): the state must
   be released *before* the decision date it informs, not merely before the end of the sample. An
   official state published on a calendar that runs *after* the decision it is supposed to inform
   can support an explanatory decomposition but can never support a decision-time rule. This is not
   a technicality: in the EU ETS the aggregate compliance balance is published in late May or June
   of the year *after* the emissions year (S-121), so under the pre-2023 April deadline it was
   published *after* the deadline, and the decision-time form of IDEA-013 begins only with the 2023
   compliance year. **Every candidate must now record, for each observation, the publication date of
   the state relative to the decision date.**

**3. How to build it without look-ahead.**
- Use only vintages available at the decision timestamp; if the series is revised, state whether
  real-time or latest-vintage data are used.
- Respect the true publication lag: a decision on day T may use only reports published on or
  before day T.
- Make the proxy construction point-in-time: no backfilled index membership, no survivorship,
  no future information in the selection of the universe.
- Freeze the proxy definition on the training window; do not re-estimate it after seeing holdout
  results.

**4. How to validate it against an independent measure.**
- Validate the fast proxy against at least one holdings-based or institution-reported measure
  (e.g. IDEA-004's proxy against S-026's holdings-based crowding; IDEA-002's proxy against
  disclosed dealer funding value adjustments). If validation fails, the candidate is untestable
  as specified — report that, do not re-specify on the fly.
- The validation itself must be out of sample relative to the trading test.

**5. When to park rather than re-specify.**
The honest answer is "no public proxy exists" when:
- the binding constraint is not published by any institution (IDEA-002's equity funding state,
  G-01);
- the only available measure is stale relative to the decision frequency (IDEA-004's crowd
  proxy, G-04);
- the fast version of the state must be constructed from paid vendor quotes (IDEA-007's
  cross-currency basis, G-10);
- the validator cannot confirm access to the required proprietary data (IDEA-006's intraday fix
  data).
In each case, park the candidate. Re-specifying around a weaker proxy converts a good idea into a
disguised baseline. Change venue, not proxy.

**6. Candidates governed by this note.**
IDEA-002 (parked, P-004, G-01), IDEA-004 (G-04), IDEA-005 (S-030, public — passes), IDEA-007
(S-054, public — passes), IDEA-008 (short interest/lending fees, public — passes), IDEA-009
(funding rate, published by venue — passes), IDEA-013 (published state, but **fails condition (e)**
for the pre-2023 regime — parked, P-008).

---
