# THEORY-TO-VALIDATION HANDOFFS — CYCLE 1

**Status: specification only.** Nothing in this file has been executed. No test code, no data
acquisition, no metrics, no simulations and no jobs were produced for these candidates in this
repository. The designated validation repository must make its own data, implementation,
accounting and result checks, and must not treat any statement here as a result.

Three specifications are provided, in shortlist order: V-001 (IDEA-001), V-002 (IDEA-004),
V-003 (IDEA-003). IDEA-002 is not specified for validation this cycle because its feasibility
precondition (source gap G-01) is open; see `next_agent_handoff.md`.

---

## V-001 — RECON-FLOW (IDEA-001)

### Frozen hypothesis
Index-provider reconstitution creates a scheduled, deadline-driven passive demand shock. The part
of the price move attributable to the compensation paid to the arbitrageur who supplies that demand
partly reverses after the passive flow has been executed. The magnitude of both legs scales with
the size of the required passive flow (index weight change × assets tracking the benchmark).

### Frozen conceptual rules
- Event universe: announced S&P 500 / S&P MidCap 400 / S&P SmallCap 600 constituent changes with a
  public announcement timestamp and a published effective date.
- Leg 1 (pre-effective): long the affected name after the announcement, held to the effective-date
  close. Deletions: short or no position — the validator must pre-register which side is traded;
  the hypothesis predicts an asymmetric result (additions harvestable, deletions not).
- Leg 2 (post-effective reversal): the position is exited, and the pre-specified reversal window is
  1 to 20 trading sessions after the effective date, with the exit schedule fixed in advance.
- The flow-size variable is the weight change scaled by assets tracking the benchmark. The assets
  series must be sourced, dated and defended (gap G-02) — if no defensible series exists, the
  scaling test is dropped and the validator must report that it was dropped.
- No look-ahead: only information published at or before the decision timestamp may enter the rule.

### Ambiguities the validator must resolve and record
1. Whether index funds execute at the effective close or pre-position (gap G-03). If the validator
   has evidence of pre-positioning, leg 1 must be re-specified or dropped, with the reason recorded.
2. Whether the announcement after-close (05:15 ET) can be traded at all; if not, leg 1's entry must
   be the next session's open or a defined VWAP window, and this changes the realised return.
3. Whether "assets tracking the benchmark" is measured as of the announcement date, the effective
   date, or interpolated.
4. Whether the effective-date close print can be traded (auction participation, halts, limit
   moves) and what the fill assumption is.
5. Whether corporate actions inside the announcement-to-effective window change the required
   weights (share freeze, M&A, secondary offerings).

### Target universe, time frame, sampling frequency
- Universe: US-listed common stocks subject to S&P 500 / MidCap 400 / SmallCap 600 changes.
- Time frame: the validator must choose and justify a start date; the classic literature covers
  1978–2014 and the modern passive era differs, so a pre-2010 / post-2010 split must be reported.
- Sampling frequency: event-driven at daily resolution, with a stated rule for events that overlap
  the effective date.

### Data fields required
Announcement timestamp and content; effective date; pre- and post-event index weights; daily
OHLC and closing auction prices/volumes; quoted spread and depth around the event; index
membership history; assets tracking the benchmark; a borrow series for any short leg; and a
flag set for halts, corporate actions and index-futures rolls.

### Timing, execution and survivorship
Decision timestamps must be strictly after the announcement publication. Event samples must
include failed and removed names (deletions, and names removed shortly after addition) to avoid
survivorship bias. Corporate-action-driven constituent changes should be reported separately from
discretionary index-committee changes.

### Cost and execution assumptions the validator must justify independently
Auction versus open-versus-close execution; the borrow cost for any short leg; the market-impact
assumption relative to the stock's typical auction depth; and a statement of whether the assumed
cost is consistent with the size of the expected edge.

### Pre-specified primary outcome and guardrails
- Primary: the average abnormal (market- and industry-adjusted) leg-1 return, and the average
  abnormal leg-2 return conditional on leg 1, both as functions of the flow-size variable.
- Guardrails to pre-register: maximum drawdown of the event book, per-event and per-name position
  concentration, turnover, gross and net exposure, and a capacity ceiling expressed as a fraction
  of the estimated passive flow requirement and of the name's typical daily volume.
- Tail guardrail: the worst single event, and the loss distribution in calendar windows containing
  market-wide stress.

### Baselines, separation and controls
- Baselines: zero-return events; events of the opposite sign; and a placebo calendar of
  non-announcement dates matched by month and index-size bucket.
- Separation: a selection window, a validation window, and a final holdout window, all defined in
  advance; rules and thresholds frozen before the holdout is touched.
- Controls against peeking: no re-estimation of the flow-size threshold after seeing holdout
  results; every rule change logged with a date and a reason; a family-wise accounting for the
  number of event-type/leg/window combinations searched.

### Stress cases, regime slices, ablations
- Regime slices: pre- vs post-2010; high vs low passive assets; crisis vs calm windows; index
  futures roll weeks; months containing reconstitution plus macro announcements.
- Ablations: drop the flow-size conditioning; drop the reversal leg; restrict to "outsider"
  additions versus intra-family promotions (the flow-size difference is an order of magnitude);
  add a control for pre-announcement abnormal options volume (S-005) to separate anticipation from
  price pressure; and an attention control (S-027) to test the awareness explanation.

### Pass / fail / uncertain
- **Pass:** leg 1 abnormal return is positive for additions and scales with flow size; leg 2 shows a
  partial reversal; both survive the costs the validator justifies; the result is not explained by
  the anticipation or attention controls.
- **Fail:** no flow-size scaling, or no reversal, or the effect vanishes net of justified costs, or
  the anticipation control explains the announcement effect.
- **Uncertain:** the flow-size series cannot be constructed (G-02) or the trading convention cannot
  be established (G-03) — the validator then reports the event study without the scaling test and
  does not conclude either way.

### Kill criteria and follow-up justification
Kill if the announcement effect is fully explained by informed anticipation, or if the effect does
not scale with the passive flow requirement. Justify follow-up research if the effect survives
costs and controls but the reversal leg is unstable — that would indicate a state-dependence worth
a follow-up cycle.

---

## V-002 — SLOWCAP-COND (IDEA-004)

### Frozen hypothesis
Because arbitrage capital is slow to arrive and exits in synchronisation, the expected return of a
convergence trade is a function of the deviation *relative to the depth of the crowd already
running it*, and that relation is non-monotone: returns are larger in moderate crowding than in low
crowding (deviations persist) and smaller in high crowding (the edge is competed shut), while
tail severity rises with crowding.

### Frozen conceptual rules
- The convergence universe and the fundamental anchor must be defined ex ante, before any results
  are seen, and must be stated in the specification, not chosen after the fact.
- Crowd depth must be constructed from lagged public proxies and validated against at least one
  holdings-based crowding measure (S-026). If validation fails, the candidate is untestable as
  specified and must be reported as such rather than re-specified on the fly.
- The crowding state is a first-class input to both entry and exit, including the pre-specified
  suspension of new positions during market-wide liquidity events.
- Sizing is inversely related to crowd depth.

### Ambiguities the validator must resolve and record
1. The anchor: which deviation, and against which fundamental or market-based benchmark.
2. The proxy set: which lagged observables constitute crowd depth, and the reporting lag of each.
3. Whether "moderate crowding" is defined ex ante (e.g. by terciles of the proxy computed on a
   training window only) rather than by inspecting the outcome.
4. The exit-capacity model: how the strategy's own size interacts with the crowd's exit.
5. Whether the observed effect is a momentum exposure (S-024) rather than a convergence effect.

### Target universe, time frame, sampling frequency
- Universe: a pre-specified cross-sectional relative-value universe with an explicit pairing rule
  (for example industry-neutral pairs with a pre-defined fundamental anchor).
- Time frame: at least one full market cycle, with at least one crisis window included, and with
  pre-specified regime labels that are not constructed from the outcome.
- Sampling frequency: daily marks with weekly or monthly rebalances; the validator must pre-specify
  the rebalance rule and stick to it.

### Data fields required
Pair constituents' prices, borrow availability and borrow cost, the anchor variable, the
crowd-depth proxies (holdings-based crowding, short interest, option open interest, analyst target
dispersion, comparable-trade counts), the market and sector series for de-meaning, and a
liquidity-event calendar for the suspension rule.

### Timing, execution and survivorship
- All state variables must be lagged by their true reporting lag; a proxy computed from a
  quarterly holdings file used on a daily decision rule is a look-ahead and must be handled as one.
- Universe construction must be point-in-time (no survivors, no backfilled index membership or
  borrow availability).
- The crowding proxy validation must itself be out of sample relative to the trading test.

### Cost and execution assumptions the validator must justify independently
Two-sided spread cost, borrow cost and availability, the financing/carry drag of a market-neutral
pair, and the impact of the pair's own size relative to the liquidity of its legs. The validator
must justify whether the assumed cost can be reconciled with the size of the hypothesised edge.

### Pre-specified primary outcome and guardrails
- Primary: the average net abnormal return of the convergence leg, bucketed by crowd-depth
  tercile computed on the training window only.
- Guardrails: drawdown, per-name and per-sector concentration, gross and net exposure, turnover,
  the loss in the worst market-wide liquidity window, and a capacity ceiling scaled by the
  observable depth of each leg.

### Baselines, separation and controls
- Baselines: unconditional convergence trades; crowd-avoidance rules of the form "trade only when
  crowding is low" (the known-baseline version of this idea — this is the decisive comparison);
  and a momentum-matched control.
- Separation: training, selection and holdout windows fixed in advance; tercile cut-points
  estimated on the training window only; all threshold choices logged with dates.
- Controls against peeking: an explicit count of every configuration examined; a pre-registered
  stopping rule for the research process; and a holdout that is opened once.

### Stress cases, regime slices, ablations
- Regime slices: crisis vs calm; high vs low market-wide volatility; quarters around large
  index reconstitution flows; periods of benchmark-wide arbitrage activity.
- Ablations: (a) drop the crowd state and use unconditional convergence — if the result survives,
  the candidate collapses into the baseline; (b) use the holdings-based crowding measure directly
  in place of the fast proxy — this isolates the proxy's contribution; (c) remove the
  market-wide-event suspension rule; (d) replace the anchor with a pure relative-price anchor to
  test how much of the result is fundamental-break risk.

### Pass / fail / uncertain
- **Pass:** returns are non-monotone in crowd depth with the predicted ordering, the ordering
  survives the crowd-avoidance baseline comparison, net of justified costs, and the tail severity
  ordering holds.
- **Fail:** the relation is monotone and negative (i.e. the candidate is just "avoid crowded
  trades"), or the effect disappears net of costs, or it is fully explained by momentum.
- **Uncertain:** the proxy cannot be validated (G-04) — report the holdings-based measurement
  result and state that the fast-proxy version of the candidate is untested.

### Kill criteria and follow-up justification
Kill if the crowd-avoidance baseline performs equivalently, or if proxy validation fails and no
defensible alternative state variable exists. Justify follow-up research if the ordering is
non-monotone but the tail is not manageable — that points to a state-conditional risk budget
rather than a new edge.

---

## V-003 — VRP-STATE (IDEA-003)

### Frozen hypothesis
The variance risk premium is compensation for absorbing crash risk. A strategy harvesting it
therefore earns a negatively skewed payoff and should only be run in states where the crash is not
imminent; the gate must be computable ex ante from the option surface alone.

### Frozen conceptual rules
- Premium: model-free implied variance (or a variance-swap rate synthesised from listed options,
  S-012) minus realized variance, with realized variance used only for post hoc measurement, never
  as an input to the gate.
- Gate: option-implied crash-risk measures, with thresholds pre-registered from the training
  window only.
- The harvest is a variance-shortening position; position construction (direct variance, or a
  listed-option replication) must be pre-specified, and if replication is used, the replication
  error and the tracking basis must be reported.
- In gated states the position is not opened (or is reduced at a pre-registered size).

### Ambiguities the validator must resolve and record
1. Which option universe (SPX vs SPY vs single names) and which strike set.
2. The realized-variance estimator (intraday-aggregated versus close-to-close) and its noise
   properties, including closing-price bid-ask bounce.
3. The crash measure: which implied crash proxy, and how the gate thresholds are set without
   peeking.
4. Whether the harvest is accessed via OTC variance swaps (counterparty and documentation risk) or
   via listed options (replication error, spreads).
5. The margin and financing treatment of a short-variance position.

### Target universe, time frame, sampling frequency
- Universe: a pre-specified index option surface; the single-name extension is a separate,
  separately pre-specified study.
- Time frame: at least one full cycle including at least one crisis window, and a mandatory
  pre-2010 vs post-2010 split to expose structural change (gap G-05).
- Sampling frequency: monthly or quarterly rebalancing of the gate and the position, fixed in
  advance.

### Data fields required
Option quotes with implied volatility (or the inputs to model-free implied variance), intraday
prices for realized variance, the option-implied crash measures used by the gate, transaction
costs on the traded instruments, margin requirements, and financing rates.

### Timing, execution and survivorship
- Option quote survivorship (delisted options, expired contracts) must be handled explicitly.
- The gate must be computed from information available at the rebalance timestamp; the premium
  may only be *measured* afterwards.
- Any parameter estimated from the option surface (for example an ATM strike selection rule) must
  be estimated on the training window only.

### Cost and execution assumptions the validator must justify independently
Bid-ask spreads on the traded strikes, the cost of roll and of replication error, margin funding
costs, financing on the variance position, and the impact of the size taken relative to option
depth. The validator must state whether the harvest survives these assumptions at the pre-specified
size.

### Pre-specified primary outcome and guardrails
- Primary: the average net return of the gated harvest, and the difference between the gated and
  the unconditioned harvest on a pre-specified risk-adjusted measure.
- Guardrails: maximum drawdown, the worst single event, the worst calendar window, the worst
  single-day loss, the total loss attributable to the worst three events as a share of cumulative
  profit, turnover and roll cost, margin utilisation, and the delta/vega/gamma exposure profile.

### Baselines, separation and controls
- Baselines: the unconditioned variance harvest; a constant-size variance-short position; an
  equity-index buy-and-hold; and the equity risk premium itself as a benchmark of what is being
  paid for.
- Separation: training, selection and holdout; gate thresholds frozen on the training window; the
  holdout opened once.
- Controls against peeking: a pre-registered count of gate variants; the "best gate" reported
  honestly as the outcome of a search with N variants.

### Stress cases, regime slices, ablations
- Regime slices: pre- vs post-2010; NBER-style recession windows; episodes of extreme implied
  volatility; periods of retail option-flow dominance.
- Ablations: (a) remove the gate; (b) replace the implied crash measure with a simpler implied
  volatility threshold; (c) replace realized variance with close-to-close variance to expose
  measurement noise; (d) test the harvest on the single-name surface where the insurance demand
  channel is stronger (S-014) and where G-05 is most relevant.

### Pass / fail / uncertain
- **Pass:** the gated harvest dominates the unconditioned harvest on the pre-specified risk-adjusted
  measure, net of justified costs, with the tail guardrails satisfied, and the result holds in the
  holdout.
- **Fail:** the gate adds nothing; the harvest does not survive costs; the premium's predictive
  power has decayed to nothing in the modern sample; the single-name channel has been arbitraged
  away.
- **Uncertain:** the option history is too short or too survivorship-biased to answer the question
  — report the descriptive premium and its state structure without concluding.

### Kill criteria and follow-up justification
Kill if the unconditioned harvest is already optimal, or if the premium is not present in the
modern sample. Justify follow-up research if the gate works only in specific regimes, which would
point to a state-conditional allocation problem rather than a new premium.
