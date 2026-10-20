# THEORY-TO-VALIDATION HANDOFFS — CYCLES 1–32

**Status: specification only.** Nothing in this file has been executed. No test code, no data
acquisition, no metrics, no simulations and no jobs were produced for these candidates in this
repository. The designated validation repository must make its own data, implementation,
accounting and result checks, and must not treat any statement here as a result.

Cycle 1 provided three specifications, in shortlist order: V-001 (IDEA-001), V-002 (IDEA-004),
V-003 (IDEA-003). IDEA-002 is not specified for validation because its feasibility precondition
(source gap G-01) is open; see `next_agent_handoff.md`.

Cycle 2 adds **V-004 (IDEA-005)**, which reached the top three, plus two **optional**
specifications for candidates that did not: V-005 (IDEA-007) and V-006 (IDEA-006).

Cycle 3 adds **V-007 (IDEA-008)** and **V-008 (IDEA-009)**, both new candidates that entered the
top three (ranks 5 and 7). Cycle 4 adds **V-009 (IDEA-011 ACCTCLOCK)**, a new top-three candidate
(rank 3, tie at 72.0). All validation specifications are provided because pre-specifying them is
cheap now and expensive later, and because a validation agent can execute them without re-reading
the dossiers. **V-007 is executable as specified** (short interest and lending fees are public; the
recall event must be inferred). **V-008 is executable as specified** (funding rates are published
by the venue with zero lag); the binding constraint is venue risk, not data access. **V-009 is
executable as specified** (adoption calendars are regulator-published years in advance; all inputs
are public); the binding constraint is the small sample of adoption events and the concurrent
macro confound. **Superseded in Cycle 6: V-007 was withdrawn — see the Cycle-6 update below, which
corrects the "lending fees are public" premise.**

**Cycle 5 update — two specifications withdrawn, none added.** The Cycle-5 G-10 closure rejected
IDEA-007 (**R-008**) and the Cycle-5 G-11 closure rejected IDEA-006 (**R-009**) and IDEA-012
(**R-010**); the optional specifications **V-005 and V-006 are therefore WITHDRAWN** and must not be
executed. No new specification was required in Cycle 5 because **no new candidate entered the top
three**: the top three remain IDEA-001 (76.0), IDEA-004 (74.0) and the tie at 72.0 between IDEA-005
and IDEA-011, and all four already have specifications (V-001, V-002, V-004, V-009). IDEA-013 was
added as a candidate in the first half of Cycle 5 and **parked (P-008)** in the second half, so it
has no specification and should not be given one before its dated unblocking condition is met. The
executable set is therefore **V-001, V-002, V-003, V-004, V-007, V-008, V-009**, with **V-005 and
V-006 withdrawn**.

**Cycle 6 update — two specifications withdrawn, none added, one amended.** The Cycle-6 G-13/G-12
screen **parked** IDEA-005 (**P-009**) and IDEA-008 (**P-010**), so **V-004 and V-007 are
WITHDRAWN** and must not be executed: V-004's candidate fails G-12 (the closest published test of
its own state variable is null — S-099 — and the family result is null post-2012 — S-033), and
V-007's candidate fails G-13 (the securities-lending rate state is not publicly disseminated
before **29 March 2029** — S-126 — so the specification's data plan cannot be executed on public
data). **No new specification was required**, because the top three are unchanged — IDEA-001
(76.0), IDEA-004 (74.0) and IDEA-011 (72.0) — and all three already have specifications
(V-001, V-002, V-009). The executable set is therefore **V-001, V-002, V-003, V-008, V-009**, with
**V-004, V-005, V-006 and V-007 withdrawn**. Two specifications carry **Cycle-6 amendments**:
**V-001** must test the *side asymmetry* and the *second leg* separately, because the G-12 screen
established that the flow-scaling limb conditions only the size of a published effect; and
**V-002** must re-anchor its rebalancing grid to the 45-day holdings-filing cadence, because the
G-13 screen established that the crowd state is published on that cadence. IDEA-010 gained no
specification and must not be given one until gap **G-16** is closed; **IDEA-014 (new in Cycle 6)
has no specification and must not be given one** until gap **G-15** — the RIN compliance-deadline
price pattern — is closed.

**Cycle 13 update — one specification withdrawn, none added, one frozen pending a new gap.** The
Cycle-13 evidence closure **rejected IDEA-001 (R-011)**: the S&P 500 index effect has collapsed to
approximately zero in the modern sample (additions below 1% over the past decade, about −3 basis
points in 2020), the candidate's flow-scaling differentiator has a **published null**, and the
mechanism is published as anticipatory liquidity provision that shifts price pressure away from the
effective date (S-146, S-147, S-151). **V-001 is therefore WITHDRAWN and must not be executed** —
including its Cycle-6 amendment, which is now moot. **No new specification was required**, because
the top three are now IDEA-011 (72.0), IDEA-003 (71.0) and IDEA-004 (69.0) and all three already
have specifications (V-009, V-003, V-002); the top-three *membership* changed only in that IDEA-001
left it and IDEA-011 and IDEA-003 took its place, and both were already specified. The executable
set is therefore **V-002, V-003, V-008, V-009**, with **V-001, V-004, V-005, V-006 and V-007
withdrawn**. One specification now carries a **binding hold**: **V-002 (IDEA-004) must not be
executed until the new gap G-18 is closed** — the only *timely, decision-time* crowding proxy
found in thirteen cycles (S-157, comomentum) has never been validated against the holdings-based
crowding measure (S-026) that the specification is frozen on, and re-specifying around an
unvalidated proxy is forbidden by the register's own method. V-002's existing Cycle-6 amendment
(re-anchor the rebalancing grid to the 45-day filing cadence) stands.

**Cycle 30 update — no specification withdrawn, none added, one amended.** The Cycle-30 prior-art and
convention audit produced **no change to the ranking**, so the top three are still IDEA-003 (71.0),
IDEA-011 (69.0) and IDEA-004 (69.0) and **no new specification is required — V-010 remains free**.
**V-003 (IDEA-003) carries a Cycle-30 amendment**: the variance risk premium's *measurement
convention* is now fixed ex ante. The candidate's claim is about the **expected** premium
(model-free implied variance minus the physical conditional expectation of variance); the published
literature contains at least two constructions that measure a different quantity (S-180 extracts the
premium from variance-swap quotes with a horizon distinction; S-181 measures implied minus
*subsequently realized* variance), and the two can move in opposite directions in the same state. The
amendment therefore (i) names the convention in the frozen rules, (ii) states that a null or a
positive result on the **ex-post** convention is **not a kill**, and (iii) adds an ablation that
reports both conventions side by side as a descriptive control. **V-002 (IDEA-004) remains frozen**
— G-18 was *restated*, not closed, in Cycle 30 (the newest peer-reviewed 13F-crowding work,
S-186, makes the holdings-based construction an active published object but associates crowding with
prices, comovement and fragility rather than with a return-predictive rule), and the Cycle-6
re-anchoring amendment stands. **V-008 (IDEA-009)** and **V-009 (IDEA-011)** are unchanged. No
specification may be written for **IDEA-015** while it is parked (P-011, G-21).

**Cycle 32 update — one specification added, one amended, one frozen, one candidate's specification
barred.** The Cycle-32 evidence cycle closed three gaps and moved three scores, so the top three changed:
they are now **IDEA-011 (69.0), IDEA-004 (69.0) and IDEA-010 (68.0)**. **IDEA-010 enters the top three
for the first time, and — because G-16 is now closed in its favour — the register's rule requires a
specification and permits one: V-010 is written below.** IDEA-003 falls from rank 1 to rank 4 with a
**Cycle-32 amendment to V-003** (its sign limb is closed against it by published evidence; the surviving
claim is a tail-management claim, and the premium's level and sign become descriptive controls under both
conventions). IDEA-014 falls to 52.0 with its sign-determining state unusable as specified, so **no
specification may be written for it** until the replacement-state gap G-24 is closed. **V-002 (IDEA-004)
remains frozen** pending G-18/G-21, which Cycle 32 leaves open. The executable set is therefore **V-002
(frozen), V-003 (amended), V-008, V-009, V-010**, with **V-001, V-004, V-005, V-006 and V-007
withdrawn**.

---

## V-001 — RECON-FLOW (IDEA-001) — **WITHDRAWN in Cycle 13 (candidate rejected, R-011)**

**Cycle-13 withdrawal (binding).** IDEA-001 was rejected in Cycle 13 on published evidence: the
index-inclusion effect the specification would have measured has collapsed to approximately zero in
the modern sample (additions below 1% over the past decade, an average inclusion effect of about
−3 basis points in 2020), the flow-scaling prediction has a published null, and the front-running
structure is published as competitive anticipatory liquidity provision (S-146, S-147, S-151).
**This specification must not be executed in any form, including the Cycle-6 amendment below.**
The text of the specification is retained unchanged for the audit trail.

**Cycle-6 amendment (G-12 narrowing — superseded by the withdrawal above, retained for the record).** The Cycle-6 G-12 screen established that the
candidate's **flow-scaling** limb conditions only the *size* of a published effect and does not
by itself survive the rediscovery guard, while the **side asymmetry** (additions yield a harvestable
concession, deletions do not) and the **existence of the second leg** (a non-zero fraction of the
leg-1 move reverses within 1–20 sessions) are the claims that do survive it. **The primary outcome
of this specification must therefore be stated as two separate tests — the asymmetry (does the
announced-to-effective price reaction differ in sign or in harvestability between additions and
deletions?) and the reversal leg (is there a separately dated, separately tradeable reversal?) —
and the flow-scaling prediction must be reported as a secondary magnitude result, not as the
candidate's claim.** A result that establishes only that the drift is larger when the passive flow
is larger has not tested IDEA-001.

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

**Cycle-6 amendment (G-13 resolution — binding).** The Cycle-6 G-13 screen established that the
crowd state built from institutional holdings filings **is** published before the decision: a Form
13F must be filed within 45 days of the end of the calendar quarter and is filed to EDGAR, so a
rule anchored to a quarter boundary can use everything filed up to its decision date. Two changes
follow, and both are binding on this specification. (i) **The rebalance grid must be re-anchored
from daily or monthly to the filing cadence**: the decision dates are the 13F filing dates, and the
crowd proxy must be assembled **point-in-time** from filings published on or before the decision
date — no backfill, no use of a filing that had not yet been made. (ii) **The daily-frequency
proxies (short interest, option open interest, analyst targets) must not be used as the crowd
state**; they may be used only as additional conditioning variables with their own lags. The
binding constraint on this candidate remains **proxy validity** (G-04) — the proxy must still be
validated against a holdings-based measure such as S-026, and if that validation fails the
candidate is untestable as specified and must be reported as such rather than re-specified on the
fly.

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

**Cycle-32 design amendment (specification only; not executed here).** Cycle 32 closed **G-19** — the
question of whether any published work states the expected-premium convention explicitly *and* tests its
sign in crash-imminent states — and the answer is yes, with a published sign of **positive**. The
convention is stated explicitly and independently by Zhou's Annual Review (S-191: "VRP_t ≡
E^Q_t(Var_{t,t+1}) − E^P_t(Var_{t,t+1})"), by Rombouts, Stentoft & Violante (S-190: the difference
between the risk-neutral and physical expectations) and by Bekaert, Engstrom & Ermolov (S-192). Its sign
in bad states has been tested: S-190 reports that the literature's naive ex-post estimator "systematically
becomes negative, rather than largely positive, in periods of market distress" — and that this is a
measurement artefact — while their latent decomposition finds the continuous component "systematically
positive and is higher in periods of market turmoil"; S-192 reports the expected premium is "positive"
and that "high variance risk premiums coincide with the left tail of the consumption growth distribution
shifting down". The closest published sign-flip in a variance-premium quantity in distress is in the
**term** premium (S-193). **The candidate's original sign claim — that in a crash-imminent state the
*expected* premium collapses and short-volatility is uncompensated there — is therefore not supported;
it is contradicted under the candidate's own convention.** The surviving claim is a **tail-management**
claim: the expected premium is positive in every state, but the *realised* payoff of a short-volatility
harvest is catastrophically left-tailed in crash states. The amendment therefore does four things:
(1) it withdraws the sign limb from the frozen hypothesis and states the tail-management claim in its
place; (2) it makes the premium's **level and sign under both conventions descriptive controls**, with
the published expectation registered as a prior; (3) it makes the **primary outcome** the risk-adjusted
difference between the gated and the unconditioned harvest, which was already the pre-specified primary
outcome below, and adds a **state-exposure** outcome so that the claim cannot be reduced to "the gated
trade lost less this quarter"; and (4) it adds a **falsification criterion**: if the gated harvest does
not improve the pre-specified risk-adjusted measure *and* the gate's state does not concentrate the
harvest's worst outcomes, the candidate is rejected under the register's own rule that a published
result showing the effect absent closes the candidate. The amendment does not change the candidate's
score (66.0) or its rank (4), and it does not authorise any execution.

### Frozen hypothesis
The variance risk premium is positive, large and persistent in all states — including crash-imminent
ones — so it is compensation that is *earned* ex ante but realised with an irreducible left tail. A
strategy harvesting it should therefore be **gated** on an option-surface-implied imminent-crash measure
not because the premium's sign flips there, but because the *realisation* is catastrophic there; the gate
changes the trade's state exposure and tail, not the sign of its expected compensation.

### Frozen conceptual rules
- Premium: model-free implied variance (or a variance-swap rate synthesised from listed options,
  S-012) minus realized variance, with realized variance used only for post hoc measurement, never
  as an input to the gate.
- **Convention (fixed ex ante in Cycle 30, mandatory).** The candidate's premium is the **expected**
  premium: model-free implied variance minus the *physical* conditional expectation of variance over
  the same horizon — i.e. the quantity a risk-neutral holder would be paid relative to what the
  realised distribution says will happen, conditional on the state. The **ex-post** premium
  (implied minus *subsequently realised* variance, the convention used by S-181) is **not** the
  candidate's quantity: it is retained only as a descriptive control, and a null, or a positive
  result, on the ex-post convention is **not a kill of the candidate**. The validator must record,
  in the training-window documentation and again in the holdout report, which convention each
  reported number uses. Any statement of the form "the premium collapses" is invalid unless it names
  the convention.
- **Cycle-32 amendment (mandatory, superseding the sign limb).** The premium's **level and sign are
  descriptive controls in this specification, not the candidate's claim.** Under the expected
  convention, the published prior is that the premium is positive in every state and *wider* in bad
  states (S-190, S-192); under the ex-post convention, the published prior is that the premium
  *narrows or turns negative* in stress (S-190, S-181). Both are registered as priors. The validator
  must report both conventions' level and sign as **controls**, and must not present a sign flip in
  either as the candidate's result. A test whose conclusion depends on the premium's sign in some
  state is **invalid under this specification**.
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
6. **The estimator of the physical conditional expectation of variance** used in the expected-premium
   definition above: the horizon, the conditioning set, the estimator, and its sampling error, all
   fixed on the training window; and the mapping from the option surface's risk-neutral implied
   distribution to that expectation. The validator must state how the two conventions are reconciled
   in one table so that a reader can see which quantity any reported number refers to.

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
- **Cycle-32 amendment (mandatory).** The primary outcome is **unchanged in form and is now the
  claim**: the risk-adjusted difference between the gated and the unconditioned harvest. Two
  additions are binding. (i) A **state-exposure outcome** must be reported: the distribution of
  the harvest's returns *conditional on the gate's state*, and the share of the gated harvest's
  cumulative loss that falls in the gated-out (crash-imminent) states — without this, "the gated
  trade lost less" could be a period effect rather than a state effect. (ii) A **falsification
  criterion** is fixed: if the gated harvest does not improve the pre-specified risk-adjusted
  measure **and** the gate's state does not concentrate the harvest's worst outcomes in the
  pre-registered window, the candidate is **rejected** under the register's rule that a published
  result showing the effect absent closes the candidate (the IDEA-001 precedent, R-011). A null on
  the risk-adjusted difference, with the state-exposure outcome also null, is a rejection, not a
  narrowing.
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
  channel is stronger (S-014) and where G-05 is most relevant; **(e) recompute the premium under the
  ex-post convention (implied minus subsequently realized) as a descriptive control and report both
  conventions side by side — the ex-post result is not a pass/fail input and must not be used to
  select the gate**.

### Pass / fail / uncertain
- **Pass:** the gated harvest dominates the unconditioned harvest on the pre-specified risk-adjusted
  measure, net of justified costs, with the tail guardrails satisfied, and the result holds in the
  holdout.
- **Fail:** the gate adds nothing; the harvest does not survive costs; the premium's predictive
  power has decayed to nothing in the modern sample; the single-name channel has been arbitraged
  away. **A null on the ex-post convention alone is not a fail** (Cycle-30 amendment): the
  candidate's claim is about the expected premium, and a negative or positive ex-post premium is a
  statement about a different quantity.
- **Uncertain:** the option history is too short or too survivorship-biased to answer the question
  — report the descriptive premium and its state structure without concluding.

### Kill criteria and follow-up justification
Kill if the unconditioned harvest is already optimal, or if the premium is not present in the
modern sample. Justify follow-up research if the gate works only in specific regimes, which would
point to a state-conditional allocation problem rather than a new premium. **Do not kill on the basis
of the ex-post premium's sign or absence** — that is the quantity S-181 measures, and the candidate's
claim is about the expected premium (Cycle-30 amendment).

---

## V-004 — ROLLCOND (IDEA-005) — **WITHDRAWN in Cycle 6 — do not execute**

**Status: withdrawn.** The candidate was **parked (P-009)** in Cycle 6 after the G-12 screen was
applied to it. The screen asks what the candidate *demonstrates*, and the demonstration runs the
other way on three counts: the closest published test of the candidate's **own state variable** —
the CFTC Index Traders' share of open interest conditioned on commodity returns during roll
periods — reports **no significant effect** (S-099); the published work on the trader-type channel
conditions *rate of convergence* rather than the nearby-to-deferred concession (S-098); and the
aggregate effect the candidate's joint state would rescue is documented as decayed, with the
roll's impact on the nearby-versus-deferred spread "disappears in the 2012–2019 subperiod" (S-033)
and index-trader positions not predicting near-contract excess returns (S-037, S-036). G-06 closed
as a bounded negative finding: no located paper conditions the joint state on the concession. The
specification below is retained **only** so that the reasoning is not re-derived. **No validator
should execute it as a candidate test.** If it is run at all, it is a *reproduction check* of the
published nulls (S-033, S-099), never a discovery, and its result must be reported as such. The
candidate's unblocking conditions are recorded in `rejected_and_parked.md` under **P-009**: a
published or constructible test of the **joint** state (passive share × contract depth), and
evidence that the concession survives 2012–present in the thin, high-passive-share contracts.

### Frozen hypothesis
The scheduled monthly roll of commodity index trackers creates a price concession in the expiring
and deferred contracts of the rolled commodities. The concession's size is a function of the
passive flow relative to the contract's liquidity, it is therefore observable in advance from the
regulator's published Index Trader positions, and it survives in the modern period only in
contracts where the passive share of open interest is high and depth is thin. Part of the
concession reverses after the roll completes.

### Frozen conceptual rules
- **Event universe:** the monthly roll of the S&P GSCI, from the 5th to the 9th business day, per
  the provider methodology in force on the event date (S-029). Sibling families (S&P GSCI Pre-Roll;
  S&P GSCI Enhanced, with a partly dynamic schedule) are **separate pre-specified sub-studies and
  must not be pooled** with the spot-index roll.
- **Position:** supply the liquidity the passive requires. The passive is long and rolls out of the
  expiring contract and into the deferred contract; the position is therefore **long the expiring
  (first-nearby) contract and short the deferred (second-nearby) contract**, entered during the
  roll window and exited on a pre-specified schedule tied to the completion of the roll. The
  measured object is the change in the nearby-minus-deferred spread, which falls during the roll
  and reverts afterwards (the pattern measured in S-033).
- **State variable:** passive share of open interest = the CFTC "Index Traders" long position in the
  expiring contract divided by that contract's open interest, from the most recent published report
  (positions as of the prior Tuesday, published the prior Friday), combined with a liquidity
  measure (depth, or the passive flow relative to open interest).
- **No look-ahead:** the roll calendar is known years ahead; the COT publication lag must be
  respected exactly, and a decision taken on a roll day may use only reports already published.
- **Carry bound:** the deviation must be measured against a *state-dependent* no-arbitrage bound
  (storage and financing costs, convenience yield), not a constant (S-038, S-039).

### Ambiguities the validator must resolve and record
1. Which benchmark family and which roll-weight schedule applies on each event date (the provider
   revises the methodology; S-029).
2. How "thin" is defined, and on which of the several liquidity measures (depth, quoted spread,
   open interest, volume) the state is computed — the choice must be made on the training window.
3. Whether the passive executes the roll as a block or algorithmically, and whether the observable
   spread move is a single event or a sequence (the provider's per-day roll weights, S-029, allow
   a five-day path).
4. How to handle market disruption events, in which the provider's own rule changes the roll
   (S-029) — these events must be excluded or analysed separately, not silently treated as normal.
5. The contamination of the COT "Index Traders" category in both directions (S-030) and the
   question of whether swap-dealer hedging of OTC index exposure should be included.
6. The treatment of delivery months, first notice days and price limits.

### Target universe, time frame, sampling frequency
- Universe: the commodity futures contracts that are components of the benchmark, restricted to
  contracts that are liquid enough to trade; the validator must state the inclusion rule.
- Time frame: from the earliest date on which the required CFTC series (Disaggregated and
  Supplemental CIT) exists for the contracts concerned, with a **mandatory pre-2012 / post-2012
  split** because the published aggregate result changes character at that boundary (S-033).
- Sampling frequency: event-driven around each monthly roll, at the contract level, with a
  pre-specified intraday or daily resolution and a stated rule for overlapping events.

### Data fields required
Contract-level settlement and trade prices by delivery month; open interest, volume, quoted spread
and depth per contract per day; CFTC Supplemental (Index Traders) and Disaggregated COT positions
by contract; benchmark contract weights, roll schedule and roll-weight path; delivery calendars and
price limits; and a measure of the carry/convenience-yield bound for each contract-month.

### Timing, execution and survivorship
- COT data must be used with their true lag; a decision rule that uses a report published after the
  decision is a look-ahead and must be reported as such.
- Contract universes must be point-in-time: contracts that have been delisted or have expired must
  not be backfilled, and the selection of tradeable contracts must not use information from after
  the event (a contract excluded because it was illiquid *after* the roll is a survivorship error).
- The classification error in the Index Traders category must be quantified and reported.

### Cost and execution assumptions the validator must justify independently
Bid-ask spread crossed twice, commission, slippage and market impact in thin contracts, margin
financing on a two-leg futures position, and the settlement/roll mechanics of the deferred leg.
The validator must show the **gross concession per contract exceeds the round-trip cost** at the
pre-specified size, or report that it does not. The published anchor for the size of the passive's
own cost is roughly three percent per year for one large ETF's roll (S-032), which bounds what can
be harvested and should be used as a sanity ceiling.

### Pre-specified primary outcome and guardrails
- Primary: the mean change in the nearby-minus-deferred spread during the roll window, and the
  mean reversion over the pre-specified post-roll window, each estimated as a function of the
  passive-share and liquidity state variables.
- Guardrails: maximum drawdown of the event book; concentration in a single commodity, a single
  contract and a single calendar week (all commodity rolls fall in the same five days, so the book
  is one month-end-dated bet); gross and net exposure; margin utilisation; turnover; the worst
  single event; and the loss in the worst calendar month.
- Tail guardrail: the loss distribution in windows containing a market disruption event or a
  commodity supply shock, in which the position is short one leg of a rising curve.

### Baselines, separation and controls
- **Baselines (the decisive comparisons):** (a) the *unconditional* roll effect — the published
  aggregate null for 2012–2019 (S-033) is the number the candidate must beat, and a validator
  must reproduce that baseline before reporting anything about the state condition; (b) a
  placebo roll calendar in the middle of the month; (c) the same contracts in months without a
  roll; and (d) the "passive roll has little price impact" result (S-036) as a null to be
  contradicted or confirmed.
- **Separation:** training, selection and holdout windows fixed in advance; all tercile
  cut-points and thresholds estimated on the training window only; the holdout opened once.
- **Controls against peeking:** an explicit count of every (state definition × event window ×
  sub-sample) combination examined; every rule change logged with a date and a reason.

### Stress cases, regime slices, ablations
- Regime slices: pre- vs post-2012; pre- vs post-electronification in the contract's own
  history; calendar quarters containing a commodity supply shock; months containing a
  market-disruption event.
- Ablations: (a) drop the state conditioning and estimate the unconditional effect (this is the
  baseline, and if the state adds nothing the candidate is dead); (b) replace the passive-share
  variable with a liquidity-only variable, to test whether the passive is doing the work or
  liquidity is; (c) add managed-money positioning in the deferred contract as a covariate, which
  is the discriminating test between the two rival decay channels — *arbitrage capital
  pre-positioning* versus *electronification and liquidity supply*; (d) exclude delivery months and
  price-limited contracts; (e) replace the state-dependent carry bound with a constant one, to
  expose the convenience-yield confound.

### Pass / fail / uncertain
- **Pass:** the concession is larger in high-passive-share, thin contracts than in low-passive-
  share, liquid contracts within the same commodity and period; the relation survives the
  post-2012 split; the reversal after the roll is present and larger when the concession was
  larger; and the gross concession exceeds the justified round-trip cost in the selected
  contracts.
- **Fail:** the cross-section is flat or reversed; the effect is absent in every contract in the
  modern period (in which case the published null is a statement about the market, not about
  composition); the reversion is explained by a moving carry bound rather than by the flow; or the
  gross concession is below cost in every selected contract.
- **Uncertain:** the CFTC series do not cover enough of the benchmark's contracts, or the
  classification error dominates the signal — the validator then reports the descriptive
  roll-window behaviour with the state variable and states that the candidate is untested rather
  than concluding.

### Kill criteria and follow-up justification
Kill if the unconditional baseline cannot be reproduced, if the state conditioning adds nothing
after costs, or if the effect does not survive the post-2012 split. Justify follow-up research if
the effect is present in the modern period but only in a handful of thin contracts — that points
to a capacity-and-selection problem and a different, more specialised candidate rather than a
general edge.

---

## V-005 — FUNDSTATE-FX (IDEA-007) — **WITHDRAWN in Cycle 5 — do not execute**

**Status: withdrawn.** The candidate was **rejected (R-008)** in Cycle 5: the cross-sectional
funding-state → currency-return relation is a published, positive result (S-064 — "Currencies with
higher dollar funding pressure (higher unconditional level of basis) earn higher expected excess
returns"), and the mechanism's own literature has closed in the same direction (S-095, S-096, S-097).
The specification below is retained **only** so that the reasoning is not re-derived and so that a
future validator can see what was specified and why it was withdrawn. **No validator should execute
it as a candidate test.** If it is run at all, it is a *reproduction check* of S-064, never a
discovery, and its result must be reported as such.

**Blocking condition (updated after the Cycle-2 source closure).** The literature gap that
blocked this specification is now **mostly closed**: the funding-currency and global-liquidity
corpus has been read and registered (S-052 … S-073), and the verdict on G-10 is MOSTLY CLOSED.
The consequence for this specification is a **scope restriction, not a release**: the *aggregate*
funding-constraint-state → carry-return relation is a published, peer-reviewed, positive baseline
(S-055) and was rejected as a candidate (R-006). The validator must therefore execute **only the
cross-sectional and publication-timing residual** below, and must report the aggregate relation as
a **reproduction of a published result, never as a discovery**. A validator who reports "the
funding state predicts carry" has reproduced S-055 and has tested nothing.

### Frozen hypothesis
When dollar funding liquidity expands, the currencies whose borrowers are most dependent on
dollar funding appreciate more against the dollar than the currencies whose borrowers are least
dependent, conditional on the interest differential, and the relation appears from the
publication date of the funding statistics and not before it.

### Frozen conceptual rules
- State: the published change in dollar-denominated cross-border liabilities of intermediaries
  (S-054), used exactly as published on its published calendar, with the publication lag respected.
- Dependence measure: each currency's share of its cross-border borrowing that is dollar-
  denominated, from the same published tables.
- Cross-section: the prediction is an ordering across currencies within a publication date, not a
  time-series forecast of the dollar.
- Sign discipline: the funding-liquidity channel has the **opposite** sign to the carry-crash
  channel; periods in which the two point in opposite directions must be either excluded or
  analysed separately, and the rule must state which channel it is trading.

### Ambiguities the validator must resolve and record
1. The exact published aggregate to use, and whether to use the locational or the consolidated view
   (S-054) — a choice that must be made on the training window and reported.
2. The dependence measure's construction and its coverage across currencies.
3. The publication *time* of day, which must be pinned down before any same-day effect is claimed.
4. The treatment of the 2007–09 structural shift noted by the authors (S-052) and of data revisions.
5. The carry control: which interest differential (policy rates or forward-implied) and at what
   tenor.

### Target universe, time frame, sampling frequency
- Universe: a pre-specified set of liquid currencies with materially different dollar-funding
  dependence, including at least one dollar-funding-dependent emerging-market group and one
  insulated group; the choice of which currencies enter the cross-section must be made ex ante.
- Time frame: all publication dates available in the chosen statistics, with a mandatory split
  around 2008–2010 and around the 2020 and 2022 episodes.
- Sampling frequency: event-driven at each publication date; the position is held until the next
  publication.

### Data fields required
Published cross-border and dollar-denominated liability aggregates by residence, currency and
counterparty sector; the dependence measure per currency; policy and forward-implied rate
differentials; a volatility series; and the FX spot series.

### Timing, execution and survivorship
- Data must be used as published; revised vintages must be handled explicitly, and the validator
  must state whether a real-time vintage or the latest vintage is used (and if the latter, that
  revisions may create a look-ahead).
- Currency selection must not use post-publication outcomes; the currency set must be point-in-time
  (a currency that becomes untradeable or is redenominated must be handled explicitly).

### Cost and execution assumptions the validator must justify independently
Bid-ask spread, the funding/carry cost of the position (which is the dominant cost at this
horizon), the transaction cost of the rebalance at each publication date, and the impact of the
size taken in the less liquid currencies, which are the ones with the highest funding dependence.
The validator must state whether the slow edge survives these costs.

### Pre-specified primary outcome and guardrails
- Primary: the cross-sectional spread between the predicted return of the most dependent currency
  group and the least dependent group, per publication date, net of the interest differential.
- Guardrails: maximum drawdown; per-currency concentration; gross and net exposure; the loss in
  the worst funding-contraction episode; turnover and carry cost as a share of gross return; and
  the exposure to the funding currency.

### Baselines, separation and controls
- Baselines: (a) the interest differential alone (the carry trade — the decisive comparison, and
  the candidate must beat it); (b) the **published aggregate results, which are baselines and not
  discoveries**: the funding-constraint state → carry-return relation (S-055) and the
  funding-liquidity → dollar-forecast relation (S-052), both of which must be reproduced and
  reported as reproductions, with the candidate's claim confined to what is added on top of them;
  (c) a time-only forecast of the dollar (S-052, duplicated baseline in substance); (d) a random
  currency grouping with the same sizes; and (e) an equal-weight cross-section of the same
  currencies.
- Separation: training, selection and holdout publication dates fixed in advance; all thresholds
  frozen on the training window; the holdout opened once.
- Controls against peeking: an explicit count of configurations examined; a pre-registered
  stopping rule; no re-specification of the dependence measure after seeing holdout results.

### Stress cases, regime slices, ablations
- Regime slices: funding expansion vs contraction; crisis vs calm; periods where the carry channel
  and the funding channel agree vs disagree; the 2007–09 structural shift.
- Ablations: (a) drop the dependence measure and use the funding state alone (this is the
  published result, and if nothing is added the candidate is a restatement of S-052); (b) replace
  the dependence measure with trade-weighted dollar invoicing share, to test whether trade
  invoicing rather than funding is doing the work; (c) add a risk-off control; (d) use the
  consolidated rather than the locational statistics.

### Pass / fail / uncertain
- **Pass:** the cross-sectional ordering holds out of sample, survives the interest-differential
  control, appears from the publication date and not before it, and exceeds costs.
- **Fail:** the effect is explained by the interest differential; the relation is present before
  the data were public (meaning the state is not the cause); the effect is a single-episode
  artefact; or the edge is below costs.
- **Uncertain:** the published series cannot support the cross-section (insufficient currency
  coverage) — report the time-series reproduction of S-052 and state that the cross-sectional
  candidate is untested.

### Kill criteria and follow-up justification
Kill if the candidate cannot beat the carry baseline, or if the publication-timing test fails.
Justify follow-up research if the cross-section works but the time-series version does not — that
would point to a cross-sectional rather than a level effect and to a different candidate.

---

## V-006 — FIXCLOCK (IDEA-006) — **WITHDRAWN in Cycle 5 — do not execute**

**Status: withdrawn.** The candidate was **rejected (R-009)** in Cycle 5, and its dedicated vehicle
IDEA-012 was **rejected (R-010)**, when the G-11 closure pass established that a settlement deadline
cluster is a published price determinant (S-112), that the securities settlement cycle is a published
price-impact determinant (S-113, S-114, S-115), and that the post-US-close FX window is documented
as a cost rather than an edge (S-117, S-118, S-119, S-120). Both candidates set the rule themselves —
"if a published paper already shows a settlement-side or T+1-window price effect, the candidate is
rejected, not narrowed" — and that condition is now met. The specification below is retained **only**
so that the reasoning is not re-derived; **no validator should execute it**, and any execution must
be reported as a reproduction of published work, never as a discovery.

**Blocking conditions (updated after the G-09 closure).** (a) **G-09 is now MOSTLY CLOSED**: the
intraday FX literature around the 4pm fix has been read and registered (S-074 … S-081), and the
consequence is a **scope restriction, not a release**. The fix-window price effect is **published**:
the temporary, end-of-month-concentrated impact of passive hedging demand at the fix (S-075), the
negative serial correlation around the fix (S-076), the negative pre/post-fixing autocorrelation
(S-077), the elevated volatility and movement size around 4pm (S-074) and the W-shaped dollar
pattern around global fixings (S-081). The aggregate version of this candidate was therefore
rejected as a known baseline (R-007), and the validator must execute **only the residual below** —
the settlement-side deadlines and the post-2015 persistence of the published fix effect. Reporting
"the fix moves prices in the evening" reproduces the literature and tests nothing.
(b) **G-11 must be closed first**: the settlement-side deadline cluster (the CLS currency-close and
pay-in cut-offs and the post-US-close window created by T+1) has not been searched at all, and if a
published paper already tests it as a price determinant, the candidate is rejected rather than
narrowed. (c) The validator must confirm access to intraday order-book data for the pairs in
scope; the dataset used in the peer-reviewed work was provided by the benchmark administrator and
is not public (S-047), and the fix literature itself used a decade of tick-by-tick data for 21
currency pairs (S-076) and administrator-provided high-frequency data (S-074, S-080). If (c) fails,
this specification is not executable and the candidate is a structural description only.

### Frozen hypothesis
*Residual only.* On days with no scheduled macro release, the settlement-side deadline windows —
between the US equity close and the CLS initial-pay-in deadline, and around the CLS currency-close
deadline (S-048, S-049) — show a systematic directional move in the direction of the funding
requirement, **after the published fix-window effect has been removed and the fix window itself
excluded from the sample**; and the published fix effect (S-075, S-076) is materially smaller after
the 2015 widening of the calculation window from one minute to five and after the post-2013
enforcement regime than before it.

### Frozen conceptual rules
- Windows: the 16:00 London fix window (five minutes, per the published methodology, S-045) is the
  **control to be reproduced, not traded**; the residual windows are the post-US-close settlement
  window between the US equity close and the CLS initial-pay-in deadline (S-048, S-049).
- Days with any scheduled macro release inside either window are excluded, and the exclusion is
  applied before any result is read.
- The state variable is the fix window's share of daily volume for the pair; the benchmark
  administrator's published notices (including holiday and service-alteration notices) define the
  days on which the fix does not exist.
- The position supplies liquidity to the deadline-driven flow, on the opposite side of the
  deadline-constrained demand, and is exited on a pre-specified schedule after the window.

### Ambiguities the validator must resolve and record
1. The data source and its coverage (which pairs, which platform, what depth of book).
2. How the "net deadline-constrained demand" is measured from order-book or print data, and how it
   is signed.
3. The exact window boundaries, given the five-minute calculation window and the different
   platform cut-offs.
4. The macro-release exclusion list and its data source.
5. Whether the post-US-close window and the fix window should be analysed jointly or separately
   (they overlap in time for some pairs).

### Target universe, time frame, sampling frequency
- Universe: the most liquid currency pairs, restricted to those with adequate fix-window volume.
- Time frame: the full period for which the chosen data exist, with a **mandatory pre- and
  post-May-2024 split**, because the T+1 transition changed the settlement calendar (S-048).
- Sampling frequency: intraday, tick or order-book level, with the aggregation into windows
  pre-specified.

### Data fields required
Order-book or print data for the pairs in scope, including timestamps, sizes and the fix window
boundaries; the published benchmark calendar and holiday notices; the CLS settlement timeline; a
macro-release calendar; and quoted spreads and depth.

### Timing, execution and survivorship
- No data may be used that is timestamped after the decision point; the exit rule must be
  executable with data available at the time.
- The benchmark administrator's methodology revisions (notably the 2015 widening of the window)
  must be handled as a regime break, not smoothed.

### Cost and execution assumptions the validator must justify independently
Bid-ask spread crossed twice, slippage in a concentrated window, the cost of trading *around* the
fix rather than at it, and the possibility that liquidity providers are already stationed in the
window (in which case the concession is competed away before the validator can measure it). The
validator must state whether the gross concession exceeds the round-trip cost.

### Pre-specified primary outcome and guardrails
- Primary: the mean signed price move into the fix window on no-release days, and the mean
  reversion after it, as a function of the fix-window volume share and the calendar position.
- Guardrails: maximum drawdown; the loss in the worst window; concentration; gross and net
  exposure; the cost floor test; and the effect of any benchmark suspension or service-alteration
  day.

### Baselines, separation and controls
- Baselines: (a) **the published fix results, which are baselines and not discoveries** — the
  temporary end-of-month impact of passive hedging demand (S-075), the negative serial correlation
  (S-076) and the negative pre/post-fixing autocorrelation (S-077) must be reproduced and reported
  as reproductions, and the candidate's claim is confined to what is added on top of them;
  (b) the same windows on days *with* macro releases; (c) the same calendar position on a placebo
  time of day with no institutional deadline; (d) the unconditional intraday drift; (e) the
  fix window itself, estimated on the same sample as the settlement window, as the quantity the
  settlement window must be separated from.
- Separation: training, selection and holdout *days* fixed in advance; thresholds frozen on the
  training window only.
- Controls against peeking: an explicit count of window/measure/calendar combinations examined; no
  re-selection of the exclusion list after seeing results.

### Stress cases, regime slices, ablations
- Regime slices: pre- vs post-T+1; month-end vs mid-month; high- vs low-fix-volume-share pairs;
  days around benchmark methodology changes and holidays.
- Ablations: (a) drop the no-release exclusion and show what the macro confound does; (b) replace
  the fix window with a placebo window of the same length; (c) replace the volume-share state
  with a simple liquidity measure; (d) analyse the settlement window alone.

### Pass / fail / uncertain
- **Pass:** the settlement-side window shows a signed, non-zero move in the funding direction
  after the fix effect is removed and the fix window excluded; the effect is absent in the
  pre-T+1 sample; the published fix effect is measurably smaller after the 2015 methodology
  revision; and the gross concession exceeds the justified round-trip cost.
- **Fail:** the settlement window is indistinguishable from the unconditional intraday drift or
  from a placebo window; the macro exclusion removes the entire effect (which would mean the
  candidate was a news-timestamp artefact); the effect vanishes once the fix effect is controlled
  for; the concession is below cost; or the published fix effect is unchanged across the
  post-2015 break, in which case there is no new state condition to trade.
- **Uncertain:** intraday data of adequate quality are unavailable — report the descriptive
  intraday periodicity, report the reproduction of the published fix result, and state that the
  candidate is untested.

### Kill criteria and follow-up justification
Kill if the placebo window performs the same, if the effect vanishes net of costs, or if the
settlement-side effect disappears once the fix effect is controlled for. Justify follow-up research
if the effect survives costs but is concentrated in one or two pairs, which would point to a
venue-specific rather than a general closing-clock phenomenon. **If G-11 closes against the
candidate, kill it rather than re-scoping it**: the aggregate version is already published, and a
narrower re-scope around an unsearched literature is how a known baseline returns wearing a
different label.

---

## V-007 — SECURITY-LEND (IDEA-008) — **WITHDRAWN in Cycle 6 — do not execute**

**Status: withdrawn.** The candidate was **parked (P-010)** in Cycle 6 after the G-13 screen was
applied to it, and the failure is a **publication calendar**, not a judgement. The specification
below assumes that "short interest and lending fees are public"; the second half of that
assumption is false on the present regulatory calendar. The Commission granted a temporary
exemption "from compliance with Rule 10c-1a **with respect to the reporting date until September
28, 2028, and with respect to the dissemination date until March 29, 2029**" (S-126), so the
earliest date on which a borrow-cost state can be public is **29 March 2029**. The short-interest
file is twice monthly and is published roughly seven to eight business days after its settlement
date (S-127), which makes it a *stale* state rather than a decision-time one, and the recall event
itself is not published at all. The specification below is retained **only** so that the reasoning
is not re-derived. **No validator should execute it as a candidate test** — there is no published
borrow-cost series to execute it on. The unblocking condition is **dated**: on or after 29 March
2029, re-read the Rule 10c-1a dissemination data and test whether a public, dated, security-level
borrow-cost series exists whose publication date precedes a decision date (gap **G-14**). The
related aggregate short-position regime (Rule 13f-2 / Form SHO) begins no earlier than 2 January
2028 (S-126) but measures positions, not borrow cost, and must not be substituted for it.

### Frozen hypothesis
When a stock's borrow becomes expensive or scarce and lenders recall loaned shares, short sellers
are forced to cover involuntarily; the resulting buying pressure creates a temporary price spike
that decays as the covering is completed. A rule that buys into borrow-constraint and recall
events and exits on a pre-scheduled basis captures a liquidity-provision premium paid by the
forced coverers.

### Frozen conceptual rules
- **Event universe:** US equities with publicly reported short interest and active
  securities-lending markets. Exclude names with scheduled fundamental news (earnings, M&A, FDA
  decisions) inside the event window; exclude names under a Reg SHO short-sale restriction
  (threshold securities).
- **State variable:** securities-lending fee ("specialness") relative to the name's own trailing
  distribution, and the change in short interest (biweekly, exchange-published). A borrow-fee
  spike into the top decile of the name's own distribution is the entry signal.
- **Position:** long the name, sized as a small fraction of its daily volume, entered when the
  fee spikes or short interest rises sharply with a simultaneous fee increase.
- **Exit:** pre-scheduled after T+1 to T+5 sessions, exit rule fixed in advance of the trade.
- **No look-ahead:** short interest is biweekly and lagged; a decision on day T may use only
  reports published on or before day T. The recall event itself is not published; it is inferred
  from fee spikes and volume anomalies, and this inference must be pre-specified.

### Ambiguities the validator must resolve and record
1. How "fee spike" is defined (top decile of trailing distribution, z-score, or threshold) —
   pre-specified on the training window.
2. How the recall event is inferred (fee spike, volume anomaly, or both), and the false-positive
   rate of the inference.
3. Whether the exit is T+1, T+3, or T+5, and whether it is time-based or condition-based
   (e.g. exit when the fee returns to median).
4. The treatment of names on the Reg SHO threshold list.
5. The treatment of delivery months, corporate actions, and price limits.

### Target universe, time frame, sampling frequency
- Universe: US-listed common stocks with exchange-published short interest and active
  securities-lending markets; liquidity filter (top quintile by dollar volume).
- Time frame: the validator must choose and justify a start date; a pre-2010 / post-2010 split
  should be reported because market structure changed.
- Sampling frequency: event-driven at daily resolution; the state is evaluated daily and the
  position is held for 1–5 sessions.

### Data fields required
Short interest (biweekly, exchange-published); securities-lending fees and availability (from
lending agents or data vendors — commercial); daily OHLCV; Reg SHO threshold list (exchange /
FINRA-published); fundamental-news calendar (earnings, M&A); borrow cost; a flag set for halts
and corporate actions.

### Timing, execution and survivorship
- All state variables must be used with their true publication lag; short interest is biweekly
  and lagged, so the state is stale by design and this must be handled explicitly.
- Universe construction must be point-in-time (no survivors, no backfilled borrow availability).
- The recall inference must itself be validated against an independent measure if one exists.

### Cost and execution assumptions the validator must justify independently
Bid-ask spread crossed twice, commission, slippage in the concentrated covering window, and
market impact relative to the name's typical depth. The validator must show the gross spike
exceeds round-trip cost at the pre-specified size.

### Pre-specified primary outcome and guardrails
- Primary: the average abnormal (market- and industry-adjusted) return over T+1 to T+5 after the
  fee-spike event, as a function of the fee-spike magnitude and the short-interest change.
- Guardrails: maximum drawdown; per-name and per-sector concentration; gross and net exposure;
  turnover; the worst single event; and the loss in calendar windows containing market-wide
  stress.
- Tail guardrail: the loss distribution in windows containing fundamental news that was not
  excluded (the news confounder).

### Baselines, separation and controls
- Baselines: (a) no-event days; (b) fee spikes on days with fundamental news (the confounder
  baseline); (c) a placebo window at a random time of day with no institutional event; (d) the
  unconditional long return of the selected names.
- Separation: training, selection and holdout windows fixed in advance; all thresholds frozen on
  the training window; the holdout opened once.
- Controls against peeking: an explicit count of every (state definition × event window ×
  sub-sample) combination examined; every rule change logged with a date and a reason.

### Stress cases, regime slices, ablations
- Regime slices: crisis vs calm; high vs low market-wide volatility; pre- vs post-2010; sectors
  with high recall rates.
- Ablations: (a) drop the state conditioning and take unconditional long positions on the
  selected names (if the state adds nothing, the candidate is dead); (b) use short interest alone
  without the fee spike; (c) remove the no-news exclusion to quantify the confounder; (d) use
  the Reg SHO threshold list as the sole entry signal.

### Pass / fail / uncertain
- **Pass:** the post-event abnormal return is positive, scales with the fee-spike magnitude,
  decays within 1–5 sessions, survives justified costs, and is not explained by the news
  confounder baseline.
- **Fail:** no post-event return, or no decay, or the effect is fully explained by fundamental
  news, or the gross spike is below cost in every selected name.
- **Uncertain:** the recall inference cannot be validated, or the event rate (~2% of loans per
  month) is too small for clean inference — report the descriptive event behaviour and state that
  the candidate is untested rather than concluding.

### Kill criteria and follow-up justification
Kill if the news confounder explains the entire event spike, or if the state conditioning adds
nothing after costs. Justify follow-up research if the effect survives costs but is concentrated
in a handful of names — that points to a capacity-and-selection problem and a more specialised
candidate rather than a general edge.

---

## V-008 — PERP-FUND (IDEA-009)

### Frozen hypothesis
The perpetual-futures funding rate is settled every few hours and published by the exchange; it
measures the crowded-leverage state directly. A rule that takes the side opposite to the
funding-rate crowd — short when the funding rate is high and positive (longs paying shorts),
long when it is low or negative (shorts paying longs) — captures a mean-reversion premium in the
futures-spot basis that decays as the crowd unwinds.

### Frozen conceptual rules
- **Event universe:** crypto perpetual futures on major exchanges for liquid underlyings (BTC,
  ETH and a small set of large altcoins). Exclude underlyings with thin perpetual order books;
  exclude periods of exchange outage or severe congestion.
- **State variable:** the published funding rate relative to its own trailing distribution (top /
  bottom decile), with zero lag. The funding rate is published by the exchange every funding
  period (typically every 8 hours).
- **Position:** short the perpetual when the funding rate is in the top decile (longs paying,
  crowded long side); long the perpetual when it is in the bottom decile (shorts paying, crowded
  short side). Sized as a small fraction of open interest.
- **Exit:** after a pre-specified number of funding periods (e.g. 1–3) or when the funding rate
  crosses zero, whichever comes first; exit rule fixed in advance.
- **No look-ahead:** the funding rate is published at the start of each funding period and is
  known before the position is entered.

### Ambiguities the validator must resolve and record
1. Which exchange(s) and which underlyings are in scope — pre-specified on the training window;
   results are not transferable across venues without restatement.
2. How "top/bottom decile" is defined (trailing window length, decile boundaries) — pre-specified.
3. The exit rule: fixed number of funding periods vs. funding-rate zero-crossing vs. a hybrid.
4. The clamp region: funding rates below the exchange clamp (e.g. 0.01% per period) are not
   informative and must be excluded.
5. The treatment of the position's own funding cost (which moves with the same state variable).

### Target universe, time frame, sampling frequency
- Universe: perpetual futures on at least two exchanges for BTC and ETH (and optionally large
  altcoins); liquidity filter (minimum open interest and depth).
- Time frame: the full period for which exchange-published funding rates are available.
- Sampling frequency: event-driven at each funding settlement (typically every 8 hours); the
  position is held for 1–3 funding periods.

### Data fields required
Exchange-published funding rates (every funding period); perpetual and spot prices; open
interest and volume; exchange clamp rules and calculation methods; a flag set for exchange
outages and congestion.

### Timing, execution and survivorship
- No data may be used that is timestamped after the decision point; the funding rate at the start
  of each funding period is the decision input.
- Exchange-specific funding implementations differ (clamp regions, calculation methods); results
  must be reported per exchange and not pooled without restatement.
- Crypto markets trade 24/7; the "session" concept does not apply, and the exit rule must be
  defined in funding periods, not sessions.

### Cost and execution assumptions the validator must justify independently
Bid-ask spread crossed twice, slippage, funding paid while holding the position (which moves with
the state variable), and market impact relative to the perpetual's depth. The validator must show
the gross reversal plus funding received exceeds round-trip cost at the pre-specified size.

### Pre-specified primary outcome and guardrails
- Primary: the average futures-spot basis change over 1–3 funding periods after the funding-rate
  extreme, as a function of the funding-rate decile; plus the funding payments received while
  holding.
- Guardrails: maximum drawdown; per-underlying concentration; gross and net exposure; turnover;
  the worst single funding period; and the loss in windows containing market-wide crypto stress.
- Tail guardrail: the loss distribution in windows containing a crypto deleveraging spike that
  gaps through the pre-scheduled exit.

### Baselines, separation and controls
- Baselines: (a) no-extreme funding periods; (b) a placebo window at a random time with no
  funding-rate extreme; (c) the unconditional basis return; (d) the documented funding-rate
  arbitrage (long spot, short expensive perpetual) as a baseline to compare against — the
  candidate must show it adds something the arbitrage does not capture.
- Separation: training, selection and holdout funding periods fixed in advance; all thresholds
  frozen on the training window; the holdout opened once.
- Controls against peeking: an explicit count of every (decile definition × exit rule ×
  underlying × exchange) combination examined; every rule change logged with a date and a reason.

### Stress cases, regime slices, ablations
- Regime slices: high vs low crypto volatility; bull vs bear markets; pre- vs post-2024 market
  structure; exchange-specific regimes.
- Ablations: (a) drop the state conditioning and take unconditional positions (if the state adds
  nothing, the candidate is dead); (b) use the basis alone without the funding-rate level; (c)
  test on a single exchange only, to quantify venue specificity; (d) replace the funding-rate
  level with a simple momentum measure (past returns) to separate reversal from momentum.

### Pass / fail / uncertain
- **Pass:** the basis mean-reverts after a funding-rate extreme (negative after a top-decile
  rate, positive after a bottom-decile rate), the reversal scales with the funding-rate extreme,
  the funding payments received contribute materially to the return, the effect holds on at least
  two exchanges, and the gross return exceeds justified costs.
- **Fail:** no mean reversion, or the basis moves in the same direction as the funding rate
  (momentum, not reversal), or the effect is exchange-specific, or the gross return is below cost
  in every selected underlying.
- **Uncertain:** momentum feedback explains the apparent reversal (past returns predict basis
  deviations in S-086), or venue risk makes the trade unexecutable at scale — report the
  descriptive behaviour and state that the candidate is untested rather than concluding.

### Kill criteria and follow-up justification
Kill if momentum explains the effect, or if the effect is exchange-specific, or if the gross
return is below cost. Justify follow-up research if the effect survives costs but is concentrated
in BTC/ETH only — that points to a liquidity-constrained candidate rather than a general crypto
edge.

---

## V-009 — ACCTCLOCK (IDEA-011) — *required by the Cycle-4 top-three rule*

### Frozen hypothesis
When a jurisdiction adopts a new accounting standard, the adoption date is regulator-published
years in advance and the affected firms are knowable ex ante. The market incorporates the
standards-driven improvement in information quality slowly — there is a drift in affected firms'
returns from the adoption announcement to the first full post-adoption reporting period — and the
drift partially reverses in the quarter after the first full report. The drift is larger for
firms with low pre-adoption information quality and for countries with weaker enforcement regimes,
and it is conditional on no concurrent macro shock dominating the event window.

### Frozen conceptual rules
- **Event universe:** adoption events of new accounting standards (IFRS or national GAAP changes)
  with a public announcement date and a published effective date, covering affected firms in the
  adopting jurisdiction. Exclude firms with scheduled fundamental news (earnings, M&A, regulatory
  decisions) inside the event window.
- **State variable:** pre-adoption information quality (e.g. analyst following, forecast dispersion,
  accruals quality) measured from public filings as of the announcement date; country enforcement
  regime (e.g. World Bank / regulatory quality indices) as of the announcement date. The adoption
  calendar itself is public years in advance and is the dated clock.
- **Position:** long affected firms with low pre-adoption information quality and/or weak-enforcement
  countries, from the announcement date to the first full post-adoption reporting date; exit on a
  pre-scheduled schedule (e.g. exit at the first full report, or hold 1–4 quarters). Sized as a
  small fraction of the firm's typical daily volume.
- **Exit:** pre-scheduled after the first full post-adoption report or after 1–4 quarters,
  whichever comes first; exit rule fixed in advance of the trade.
- **No look-ahead:** the adoption calendar and the affected-firm list are public before the decision;
  information quality is measured from filings available at the decision timestamp.

### Ambiguities the validator must resolve and record
1. Which standards count as "adoption events" (IFRS issuances, national GAAP changes, both) —
   pre-specified on the training window; results are not transferable across standard types without
   restatement.
2. The information-quality measure and its trailing window — pre-specified.
3. The enforcement-regime index and its source — pre-specified.
4. The exit rule: first full report vs. 1–4 quarters vs. hybrid — pre-specified.
5. The treatment of concurrent macro shocks around the event window — these must be excluded or
   analysed separately, and the rule must state which is done.
6. Whether the affected-firm list is knowable ex ante (regulator publications vs. inferred from
   filings) — this is the binding data constraint.

### Target universe, time frame, sampling frequency
- Universe: listed firms in adopting jurisdictions, restricted to liquid names (top quintile by
  dollar volume) and to jurisdictions with verifiable adoption calendars and enforcement data.
- Time frame: the full period for which adoption calendars, firm-level returns and accounting
  quality data exist, with a mandatory pre- vs post-2010 split because disclosure regimes changed.
- Sampling frequency: event-driven at each adoption announcement; the position is held from
  announcement to the first full post-adoption report or up to 4 quarters.

### Data fields required
Regulator adoption calendar (announcement date, effective date, affected firms/jurisdictions);
firm-level daily returns; accounting-quality proxies (analyst following, forecast dispersion,
accruals quality); country enforcement indices; fundamental-news calendar (earnings, M&A); borrow
series for any short leg; macro-release calendar; and a flag set for halts and corporate actions.

### Timing, execution and survivorship
- All state variables must be used with their true publication lag; accounting data is quarterly
  and lagged, so the state is stale by design and this must be handled explicitly.
- Universe construction must be point-in-time (no survivors, no backfilled enforcement data or
  firm membership).
- The adoption calendar must be treated as published at its true publication date; a decision rule
  that uses a date announced after the decision is a look-ahead and must be reported as such.

### Cost and execution assumptions the validator must justify independently
Bid-ask spread crossed twice, commission, slippage, financing/carry drag over the holding horizon
(which is quarters), borrow cost and availability for any short leg (which can be scarce in
small-cap names), and market impact relative to the firm's typical depth. The validator must show
the gross drift exceeds round-trip cost at the pre-specified size.

### Pre-specified primary outcome and guardrails
- Primary: the average abnormal (market- and industry-adjusted) return from announcement to the
  first full post-adoption report, as a function of the information-quality state and the
  enforcement-regime state; plus the average abnormal return in the post-report reversal window.
- Guardrails: maximum drawdown; per-name, per-sector and per-country concentration; gross and net
  exposure; turnover; the worst single event; and the loss in calendar windows containing market-wide
  stress.
- Tail guardrail: the loss distribution in windows containing a macro shock that dominates the
  event window (the concurrent-shock confounder).

### Baselines, separation and controls
- Baselines: (a) non-adoption firms in the same jurisdiction and period (placebo); (b) affected
  firms with high pre-adoption information quality (the state-conditioning control); (c) the
  unconditional drift of affected firms; (d) affected firms in jurisdictions with strong enforcement
  (the regime control); (e) a random date calendar matched by jurisdiction and sector.
- Separation: training, selection and holdout event windows fixed in advance; all thresholds frozen
  on the training window only; the holdout opened once.
- Controls against peeking: an explicit count of every (state definition × exit rule ×
  jurisdiction × sub-sample) combination examined; every rule change logged with a date and a
  reason.

### Stress cases, regime slices, ablations
- Regime slices: crisis vs calm; high vs low market-wide volatility; pre- vs post-2010; strong vs
  weak enforcement countries; quarters containing macro shocks.
- Ablations: (a) drop the state conditioning and take unconditional long positions on affected
  firms (if the state adds nothing, the candidate is dead); (b) use information quality alone
  without the enforcement regime; (c) remove the macro-shock exclusion to quantify the confounder;
  (d) replace the enforcement regime with trade invoicing share or another country characteristic,
  to test whether enforcement is doing the work.

### Pass / fail / uncertain
- **Pass:** the drift is positive for low-information-quality / weak-enforcement firms, scales with
  the state variables, partially reverses after the first full report, survives justified costs,
  and is not explained by the concurrent-shock confounder or the high-information-quality baseline.
- **Fail:** no drift, or no reversal, or the drift is fully explained by concurrent macro shocks,
  or the high-information-quality firms perform identically, or the gross drift is below cost in
  every selected firm.
- **Uncertain:** the adoption-event sample is too small for clean inference, or the affected-firm
  list cannot be constructed ex ante — report the descriptive event behaviour and state that the
  candidate is untested rather than concluding.

### Kill criteria and follow-up justification
Kill if the concurrent-shock confounder explains the entire drift, or if the state conditioning
adds nothing after costs. Justify follow-up research if the effect survives costs but is
concentrated in a handful of events — that points to a capacity-and-selection problem and a more
specialised candidate rather than a general edge.

---

## V-010 — CREDIT-ETF (IDEA-010) — *required by the Cycle-32 top-three rule* — specification only, never executed here

**Why this specification exists.** IDEA-010 entered the top three for the first time in Cycle 32 (68.0,
rank 3), and **G-16 — the precondition that blocked every specification for this candidate since
Cycle 6 — is now closed in the candidate's favour**. The validation is therefore no longer required
against the register's original target (disclosed dealer funding value adjustments), which Cycle 32
showed to be unusable: a dealer's FVA is an OTC-derivatives-specific, annual/quarterly and frequently
immaterial disclosure, and no continuous public FVA series exists (S-155). Independent published work
has performed the validation the register wanted, on a better target and on exactly the link the
candidate claims: Raddatz (S-194) constructs the authorized-participant set for each US corporate-bond
ETF from SEC regulatory filings, measures **APs' regulatory capital ratios**, and shows that the ratio
— not equity/assets, cash/assets, total assets or activity concentration — governs ETF arbitrage
intensity and ETF premia, materially so during the March 2020 dash-for-cash. The mechanism is published
(S-195), and three published rival explanations now stand against the candidate's interpretation
(S-196 fractional baskets, S-197 funding segmentation, S-199 client-sourced liquidity discounts).
**What remains open is registered as gap G-23** (cadence, and signedness of the state). This document
is a *specification*: no data were acquired, no test was run, and no result is reported or implied.

### Frozen hypothesis
When corporate-bond ETF redemptions meet an authorized-participant set whose regulatory capital ratios
are weak, the APs cannot absorb the delivered bonds onto their balance sheets at the speed the flow
requires; the ETF therefore trades at a wider discount to its NAV, and the underlying bonds cheapen
relative to the ETF. A participant who supplies the liquidity the AP cannot — long the discounted ETF
against the underlying basket — earns the concession when the AP set's capacity recovers and the discount
narrows. The *joint* conditioning (weak AP capital ratios **and** net redemption flow) is the claim;
neither leg alone is.

### Frozen conceptual rules
- **State (the AP-set regulatory capital ratio), constructed exactly as in S-194 and fixed ex ante.**
  For each ETF, the AP set is identified from the sponsor's public disclosures; for each AP, the
  regulatory capital ratio is taken from its SEC filings (Form 10-K/10-Q capital disclosures, and the
  equivalent for bank holding companies) at the most recent filing date; the ETF-level state is a
  pre-registered aggregate of that set (e.g. a cap-weighted median of the set's ratios, or the set's
  minimum — the validator must pre-register one aggregation and report the others as ablations).
  The state enters the rule **only from the filing date forward**; no filing is used before its public
  date.
- **Flow leg: net creations/redemptions, from the sponsor's published daily shares outstanding.** The
  signal is the change in shares outstanding over a pre-registered window, and its sign is defined
  ex ante (a decrease in shares outstanding = net redemption = the adverse flow). No other flow
  measure is allowed in the trigger.
- **Trigger: the joint condition.** The trade is opened only when the AP-set capital ratio is in the
  bottom tercile of its own trailing history *as of the last filing date* **and** the flow leg is
  adverse (net redemptions). The tercile is computed on the training window only and then frozen.
- **Leg 1 (the long leg): long the ETF.** Sized at a pre-registered fraction of the discount, or at a
  pre-registered fixed notional; the sizing rule must be fixed on the training window.
- **Leg 2 (the short leg): the underlying basket.** The ETF's published holdings (or its published
  creation-basket composition) define the basket; the short must be implemented in the way the
  validator pre-registers, and the validator must report the **shortability of the basket** as a first
  class result, because a basket that cannot be borrowed is a *cost* result and not a *kill* of the
  candidate — the register distinguishes the two.
- **Exit: pre-scheduled, not state-dependent.** The position is exited at a pre-registered horizon of
  1 to 10 sessions after entry (fixed at the training window, or a fixed grid reported separately),
  because the candidate's claim is a *reversion within 1–10 sessions*. No discretionary exit.
- **No look-ahead.** The ETF–NAV discount is *measured* at and after entry, never used as an input to
  the trigger. The discount may be used for sizing only if the sizing rule is frozen in advance.

### Ambiguities the validator must resolve and record
1. The ETF universe and its AP set per ETF, with the disclosure used for each mapping, and the
   treatment of ETFs whose AP set cannot be reconstructed (they must be dropped and the drop reported,
   not silently imputed).
2. The regulatory-capital-ratio definition used per AP type (broker-dealer, bank holding company,
   asset manager) and how non-comparable capital regimes are handled.
3. Whether the state is a level, a change, or a percentile of its own history, and how the tercile is
   set without peeking.
4. The NAV used for the discount (official end-of-day NAV, intraday indicative value, or a
   reconstructed basket mark) and the resulting measurement error, including stale-bond pricing inside
   the NAV.
5. The short-leg implementation and its borrow cost, including the possibility that the basket cannot
   be shorted.
6. The treatment of corporate-action and index-rebalance days inside the holding window.

### Target universe, time frame, sampling frequency
- Universe: US-listed corporate-bond ETFs (investment-grade and high-yield) whose AP set can be
  reconstructed from public filings, and their published underlying baskets.
- Time frame: the full history for which the ETF's AP set, the APs' filings and daily shares
  outstanding are all available — with the **March 2020 dash-for-cash window mandatory** in the
  sample, because that is the episode in which the state was published to bind (S-194), and with a
  pre- vs post-2020 split reported, because the RFS-style regulatory regimes and the ETF market have
  both changed.
- Sampling frequency: the **state is quarterly** (it changes only when an AP files); the **flow leg is
  daily**; the **position is daily**. This is a real constraint and the validator must state, in the
  results, how much of the sample is covered by a single filing.

### Data fields required
ETF daily market price, official NAV and intraday indicative value; daily shares outstanding and the
published creation/redemption basket composition; the ETF's holdings file; AP identifiers and their SEC
filings; TRACE bond prices and volumes for the basket and for the financing of the short leg; borrow
availability and cost for the short leg; and ETF bid-ask spreads.

### Timing, execution and survivorship
- AP capital ratios enter only on their filing dates; the state is then held constant until the next
  filing, which must be modelled explicitly (no retrospective revision).
- ETF survivorship: an ETF that merges, closes or changes its index must be handled explicitly, and
  the effect of dropping the pre-merger history must be reported.
- AP-set survivorship: an AP that leaves the AP set must be handled, and the rule for a set that
  changes between filings must be pre-registered.
- Parameter and threshold choices are made on the training window only; the holdout opens once.

### Cost and execution assumptions the validator must justify independently
ETF bid-ask spreads and market impact on the long leg; the cost and feasibility of shorting the
basket, including the financing and recall risk of a corporate-bond short; the ETF's own creation and
redemption mechanics as an alternative implementation of leg 2 (and their costs); financing on the long
leg; and the effect of the position size relative to the ETF's daily volume and to the basket's TRACE
depth. The validator must state whether the trade survives these assumptions at the pre-specified size,
and must report the **cost floor** explicitly, because a gross discount below the round-trip cost is a
kill condition in the candidate's own terms.

### Pre-specified primary outcome and guardrails
- **Primary:** the average net return of the **joint-conditioned** trade, and its difference against
  the **unconditioned** ETF-versus-basket basis trade over the same dates, on a pre-specified
  risk-adjusted measure. The joint conditioning is the claim; the unconditional basis trade is the
  baseline that the trade must beat.
- **Mandatory ablations that are part of the primary result (not extras):** (a) the state leg alone;
  (b) the flow leg alone; (c) the joint condition. If the joint condition does not add to the single
  legs, the candidate is dead, and the validator must say so rather than reporting only the best leg.
- **Rival-exclusion results, mandatory:** (i) *fractional baskets* (S-196) — does the discount persist
  after controlling for the ETF's basket composition; (ii) *funding segmentation* (S-197) — is the
  discount explained by a funding-segregation shock rather than by AP capacity; (iii) *client liquidity
  discounts* (S-199) — is the bond-side cheapening a dealer relationship-discount phenomenon rather
  than an ETF-arbiter phenomenon; and (iv) the **monthly-frequency** published dispersion proxy
  (S-200) as a robustness check on the state.
- Guardrails: maximum drawdown, worst single event, worst calendar window, worst single-day loss,
  loss attributable to the worst three events as a share of cumulative profit, turnover and round-trip
  cost, borrow recall events, and the gross-versus-net decomposition of every reported return.

### Stress cases, regime slices, ablations
- Regime slices: the March 2020 dash-for-cash window; other credit-stress episodes; high vs low
  aggregate ETF redemption flow; periods of wide vs narrow ETF spreads; pre- vs post-2020.
- Ablations: (a) the state replaced by the published interdealer dispersion proxy (S-200), acknowledging
  its monthly frequency; (b) the state replaced by an aggregate dealer financial-weakness proxy, which
  S-200 documents to be inferior — reported to show the difference, not as a candidate; (c) the flow leg
  replaced by a market-wide ETF-flow proxy to separate ETF-specific from market-wide redemption; and
  (d) an explicit count of every (state definition × aggregation × exit rule × universe) combination
  examined, with every rule change logged with a date and a reason.

### Pass / fail / uncertain
- **Pass:** the joint-conditioned trade beats the unconditional basis trade on the pre-specified
  risk-adjusted measure after justified costs; the discount widens in the conditioned state relative to
  its own history; the discount mean-reverts within the pre-registered horizon; and the result survives
  the three mandatory rival-exclusion controls and the monthly-proxy robustness check.
- **Fail:** no joint conditioning (the single legs do all the work); no mean-reversion inside the
  horizon; the gross discount below the round-trip cost in every ETF; or the effect explained by
  fractional baskets, funding segmentation or client liquidity discounts.
- **Uncertain:** the AP set cannot be reconstructed for enough of the sample, or the sample contains
  too few quarters with a bottom-tercile state for inference — report the descriptive behaviour and
  state that the candidate is untested rather than concluding.

### Kill criteria and follow-up justification
Kill if the joint conditioning adds nothing to the single legs after costs, or if the round-trip cost
exceeds the gross discount in every selected ETF, or if the rival-exclusion controls absorb the
effect. Justify follow-up research if the effect survives costs but is concentrated in one episode
(2020) or in one ETF type — that points to a capacity-and-selection problem, and would motivate a
narrower, more specialised candidate rather than a general edge.

### Register notes carried into execution
- The state is **public in principle and lagged**: quarterly filings, with a filing lag, against a
  1–10 session holding horizon (gap **G-23**). The validator must report how many *trading days* of
  the sample are covered by a single state reading, because that is the binding limitation of the
  rule as specified.
- The register's rule that "no specification is to be written until G-16 is closed" is now satisfied;
  **G-16 is closed in the candidate's favour** and **V-010 is executable as specified**, subject to the
  validator's own data and implementation checks.
- The candidate is **not** a discovery of the state-to-premium relation: that relation is published
  (S-194, S-195). What is untested is the **trade specification and the cost floor**, and the
  validator's report must be framed accordingly.
