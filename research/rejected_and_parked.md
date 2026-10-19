# REJECTED AND PARKED LOG

Purpose: prevent rediscovery, and preserve the negative reasoning that killed each candidate. A
candidate rejected here is not deleted from the project's memory; it is not a top opportunity and
must not be presented as one. Items are re-openable only with a **new mechanism**, not with better
wording or a new parameter.

Last updated: Cycle 2, 2026-10-19. 5 rejections (R-001 … R-005), 7 parkings (P-001 … P-007),
15-row known-baseline table.

---

## Rejected

### R-001 — "Buy the dip when VIX spikes"
- **Rejection reason:** no participant mechanism. The only stated logic is that volatility is high,
  which says nothing about who is mispricing the asset or why the price should rise. The prompt's
  disqualifying pattern "markets overreact" without a defined mechanism applies directly. It also
  requires an ex-post trigger (a spike is only observed after it happened) with no look-ahead-safe
  state definition, and its outcome is dominated by whatever crash is in progress.
- **Could it be re-opened?** Only with a specified participant and constraint (e.g. a defined
  liquidity-provision balance sheet with a funding constraint) and an ex-ante state variable.

### R-002 — Options "IV crush" calendar trade (sell the front, buy the back around known expiries)
- **Rejection reason:** the effect is a mechanical consequence of the volatility smile's term
  structure rather than a behavioural or structural premium; the implementation is highly dependent
  on fills in a specific, often illiquid strike; and the "edge" is competed away by professional
  calendar-spread execution. No independent, durable mechanism was identified that would leave a
  residual after those participants.
- **Could it be re-opened?** Only with a mechanism that explains *why* the term structure should be
  mispriced for a persistent reason (for example a specific institutional flow constraint that
  pins the front end), which was not found in this cycle.

### R-003 — Sector-ETF pairs trading (simple mean reversion of sector ratios)
- **Rejection reason:** a known baseline without a differentiated participant mechanism beyond
  "arbitrageurs converge", which is the same claim that underwrites IDEA-004 and is only worth
  pursuing in the crowd-conditioned form developed there. Capacity is limited to the most liquid
  ETFs, where the residual is smallest; borrow and financing costs eat a large share of a typical
  convergence payoff; and the failure mode (a genuine sector-level re-rating) is not observable in
  advance.
- **Could it be re-opened?** Only as the low-crowding arm of IDEA-004, where the crowd state is
  the object of study rather than an assumption.

### R-004 — "Front-run the Goldman roll" (unconditioned commodity index-roll front-running)
- **Proposed:** exploit the S&P GSCI's monthly roll (5th to 9th business day, S-029) by taking
  the passive's direction before and during the roll window, as described in the practitioner
  literature and in Mou (2011) (S-035).
- **Rejection reason:** the effect is documented as *decayed*, and the closest supporting work is
  not peer reviewed. Four independent peer-reviewed lines point the other way: the roll's impact
  on the nearby-versus-deferred spread **disappears in 2012–2019** (S-033); in the deepest
  contract the order imbalance "is almost entirely reversed within one minute in the expiring
  contract and within three minutes in the second nearest-to-expiration contract on roll days"
  while the passive's own roll execution costs average about three percent per year (S-032); the
  impact of predictable index flows is "modest and temporary", consistent with liquidity
  *provision* rather than exploitation (S-034); and commodity index rolls are found to have
  "little futures price impact" (S-036) while index-trader positions do not predict near-contract
  excess returns (S-037). The supporting study (S-035) is a doctoral dissertation / working
  paper whose sample ends in March 2010 — entirely inside the window in which the effect existed —
  and whose reported statistics are the author's own.
- **What was learned:** the *mechanism* is real and is documented by the regulator itself
  (S-030: index traders replicate an index and roll "from future to future using a fixed
  methodology"). What does not survive is the unconditioned trade. The correct response is not to
  drop the family but to condition it on a state that is publicly observable and that changes the
  sign of the prediction — which is what IDEA-005 does.
- **Could it be re-opened?** Only as the *state-conditioned* question inside IDEA-005: does the
  concession survive in the thin, high-passive-share contracts after 2012? If the cross-section
  is flat, the whole family is dead and no re-parameterisation of the roll trade is worthwhile.
- **Kill condition met:** yes — published aggregate null post-2012 (S-033), documented transience
  and cost floor in the deep contract (S-032), and no supporting peer-reviewed evidence.

### R-005 — Corporate buyback / insider-purchase effect as a new candidate
- **Rejection reason:** the effect that a buyback or an insider purchase predicts subsequent
  returns is a widely documented published effect. Re-deriving it here would add a known baseline
  to the register without a differentiated participant-and-constraint mechanism, and the
  "issuer buys when cheap" channel is a momentum-adjacent mechanism that the register's momentum
  baseline already covers. **No external claim is asserted here**: the supporting literature for
  this family was not retrieved or verified in this cycle, so this rejection rests on the
  family's status as a known baseline, not on a citation.
- **Could it be re-opened?** Only with a *structural* refinement that is not the "issuer buys when
  cheap" channel — for example a dated, capacity-constrained rule (a regulatory safe-harbour
  volume cap) whose bindingness is observable — and only after the supporting literature has been
  read and registered in the source ledger.

### R-006 — "Trade carry conditioned on the public funding-constraint state" (aggregate version)
- **Proposed:** take the FX carry trade only in the states where dollar funding constraints are
  tight, using covered interest parity deviations as the state — i.e. the aggregate version of
  IDEA-007, and the same mechanism IDEA-002 was reaching for in equities.
- **Rejection reason:** it is **published, peer-reviewed and positive**. Filipe, Nissinen and
  Suominen (2023) measure funding constraints by covered interest parity deviations, define
  funding risk from them, and show that funding risk explains carry trading activity, carry trade
  returns and carry-long/short correlations, with a model in which the investment and funding
  currencies crash together relative to a safe asset when the constraints bind (S-055). The state
  variable's determinants are themselves established: covered interest parity has been
  systematically violated since the crisis because dollar hedging demand meets balance-sheet-
  constrained arbitrage (S-056, S-057), and dollar strength moves with both the deviation and
  cross-border dollar lending contraction (S-059).
- **What was learned:** the aggregate relation is a **known baseline**, and any candidate in this
  family must be stated as a refinement of it or rejected. The part that is *not* published — and
  therefore the only defensible residual — is the **cross-sectional** structure (which currencies
  respond most to a given dollar funding expansion) and the publication-timing test. That residual
  is retained in IDEA-007 (v1.1) and nothing more.
- **Could it be re-opened?** Only as the cross-sectional version, with a clear demonstration that
  it adds to S-055 rather than restating it.
- **Kill condition met:** yes — the aggregate claim is published with a positive result, so
  presenting it as a candidate would be presenting a known baseline as a discovery.

### R-007 — "The end-of-day deadline clock rents a concession" (the aggregate version of IDEA-006)
- **Proposed:** trade the price concession that the end-of-day deadline cluster creates — the
  16:00 London benchmark fix, the CLS currency-close and pay-in deadlines, and the post-US-close
  window — i.e. supply liquidity into a price-insensitive, deadline-driven demand shock and
  capture the temporary reversal.
- **Rejection reason:** it is **published, and the mechanism is exactly as proposed.** Melvin and
  Prins (2015) show that passive equity-hedging flows executed at the fix "predict the direction of
  temporary exchange rate movements at this time of day" and that "hedging demand has a strong,
  but temporary, impact on exchange rates", concentrated at end of month (S-075); Evans (2018)
  documents negative serial correlation in price changes around the WMR fix and models the fix
  order as an optimal-execution problem (S-076); Ito and Yamada (2015) document the negative
  autocorrelation between the pre- and post-fixing periods, "particularly at the end-of-month
  trading day" (S-077); Michelberger and Witte (2016) document the increased volatility and
  size of movements around 4pm (S-074); and He (2026) reports the W-shaped pre-fix rise and
  post-fix fall in the dollar across the nine most traded currencies over 21 years (S-081).
- **What was learned:** the deadline-driven concession, its temporary character, its end-of-month
  concentration and the reversal are **established results, not discoveries** — and the *fix* is
  therefore a known baseline. The part that is not published, and is the only defensible residual,
  is (i) the **settlement-side** deadlines beyond the fix (the CLS cut-offs and the post-US-close
  window that T+1 created), which no located paper tests, and (ii) whether the published fix
  effect survives the 2015 methodology revision and the post-2013 enforcement regime. Both are
  retained narrowly in IDEA-006 (v1.1); the first is blocked on **G-11**.
- **Could it be re-opened?** Only as the settlement-side extension, and only after G-11 is closed
  with the same rigour that was applied to the fix literature.
- **Kill condition met:** yes — the aggregate claim is published with a positive result, so
  presenting it as a candidate would be presenting a known baseline as a discovery.

---

## Parked (not rejected; blocked on a specific question)

### P-001 — Crypto breakout momentum
- **Why parked:** the operator's own prior family. It is a documented strategy family with a
  well-understood mechanism (trend following over crypto's high-volatility, thin, 24/7 regime) and
  it is not new to this project. Re-deriving it here would add a variant, not a mechanism. It is
  also the family most exposed to the exact failure modes the operator has already documented:
  small samples, concentrated winners, and holdout erosion.
- **Unblocking question:** is there a *distinct* crypto-specific structural feature (e.g. venue
  structure, funding-mechanics at a specific venue, or a listing/listing-exit mechanism) that
  generates a return the classic breakout rule does not already capture? If yes, that is a new
  candidate; the breakout rule itself is not.

### P-002 — Machine-learned cross-sectional momentum
- **Why parked:** the mechanism is a repackaging of a known factor family with a non-transparent
  estimator, and the discovery process it proposes (feature search against a return target) is
  exactly the data-mining route the mission prompt rules out as a substitute for mechanism. It also
  cannot be honestly assessed without running it, which is out of scope here.
- **Unblocking question:** a specific structural feature with a named participant and a pre-specified
  estimator, where the machine-learning component is incidental rather than the point.

### P-003 — Index-reconstitution pressure in *non-US* benchmark families
- **Why parked:** the mechanism in IDEA-001 should generalise, but the event dataset (provider
  announcements, weight changes, effective dates) is not yet assembled for any non-US family, and
  several providers changed their announcement conventions in ways that would break the rule
  assumptions. Parked as an extension of IDEA-001, not a separate candidate, to avoid double
  counting the same mechanism.
- **Unblocking question:** a provider whose announcement and effective-date conventions are stable
  and publicly documented, plus a passive-asset series for that benchmark.

### P-004 — FUNDSTATE (IDEA-002) — *parked pending feasibility evidence*
- **Why parked:** the mechanism is credible and the components are well evidenced, but the
  candidate depends on a public, defensible funding-state proxy (source gap G-01) that has not
  been established. Proceeding without it would mean silently substituting a weaker proxy, which
  would convert the candidate into a disguised baseline.
- **Unblocking question:** can a proxy be constructed that demonstrably predicts disclosed dealer
  funding value adjustments over a multi-year sample? If not, this candidate should be rejected
  rather than re-specified.

### P-005 — CFTC "Index Traders" (CIT) positions as a standalone positioning signal
- **Why parked:** the CFTC publishes, for free and weekly, a contract-level measure of the
  passive complex in commodity futures (S-030, S-031), and it is tempting to treat the change in
  that measure as a timing signal. Three things block it as a candidate in its own right: the
  published evidence finds that index-trader positions do **not** predict near-contract excess
  returns (S-037); the category is contaminated in both directions by the regulator's own
  caveats (it includes some non-index traders and excludes some index traders) and is reported
  with a weekly, five-day lag (S-030, S-037); and a position measure is not a mechanism — it says
  who is long, not why someone else is mispriced.
- **Unblocking question:** the state is retained only as a *conditioning variable* inside
  IDEA-005, where it enters a dated, price-insensitive flow with a published schedule. If a
  candidate were wanted here, it would need a mechanism in which the *passive's own roll
  constraint* binds — which is the IDEA-005 question, not a new one.

### P-006 — Retail 0DTE flow as a driver of intraday index moves (the "gamma squeeze" channel)
- **Why parked:** the structural change is real and well documented by the exchange itself
  (S-043): same-day expiries went from about 5% of SPX options volume in 2016 to 59–62% in
  2025, the flow is roughly half retail and about 98% electronically traded, and most of it is in
  limited-risk formats. But the *magnitude* of the presumed channel is what the candidate needs,
  and the exchange's own estimate is that net market-maker gamma hedging is de minimis — "at best,
  just 0.2% of the SPX daily liquidity" (S-043). A channel that small is not a candidate without
  independent measurement, and the single-name version of the question is still open (G-05).
- **Unblocking question:** an independent, peer-reviewed measurement of the single-name option
  market's post-2010 structure, and a specification of *which* participant's constraint binds
  (retail's cash-secured constraint, or the dealer's gamma constraint) — not a narrative about
  "gamma squeezes".

### P-007 — "Scheduled-flow liquidity premium" as a general, venue-free template
- **Why parked:** Cycle 2's clearest generalisation is that a dated, price-insensitive, scheduled
  institutional flow creates a liquidity-provision premium that a *scheduled* provider can earn,
  and that the premium is a function of the flow's size relative to liquidity. That is a
  **template**, not a candidate: a candidate must specify a venue, a participant, a constraint, a
  rule, and falsifiable predictions. Treating the template as a candidate would be the same
  category error as listing "the momentum family" as an opportunity.
- **Unblocking question:** which venue, which published calendar, and which observable
  flow-to-liquidity ratio? The commodity roll (IDEA-005) is the first instantiation; the
  end-of-day fixing clock and the funding-currency state are the other two Cycle-2 instantiations
  and each must be specified separately.

---

## Known baselines (reference set, not candidates)

These are recorded so that future sessions do not re-present them as discoveries and so that new
candidates can be compared against them. Listed without scores; the ranking rubric is not applied
to baselines.

| Baseline family | Why it is a baseline (not a discovery) |
| --- | --- |
| Cross-sectional momentum / reversal | Long-established factor family; well understood mechanisms; the interesting questions are about implementation, crowding and decay, not about the existence of the effect. |
| Value and quality-minus-junk | Established premia with well-known explanations (cash-flow duration, risk, mispricing); the operator's own caution about small samples and concentrated winners applies directly. |
| Time-series momentum / trend following | Established; the mechanism (underreaction to persistent trends, limits to arbitrage) is documented, including in this register via S-024 and S-021. |
| Carry / basis / convenience yield | Established risk-premium family; the interesting boundary is financing and funding structure, which is where IDEA-002 and the next cycle's frontier live. |
| Short-term reversal and liquidity provision | Established; the interesting boundary is the *state* in which the provision is profitable, which IDEA-002 and IDEA-004 address. |
| Variance risk premium harvesting (short volatility) | Established baseline; IDEA-003 is a state-conditioned refinement of it, and must always be described that way. |
| Overnight vs intraday decomposition | Established decomposition with an identified clientele mechanism (S-028); useful as a *control* for other candidates, not as a candidate itself. |
| Index inclusion / reconstitution effect | Established effect (S-001 … S-004); IDEA-001 is a flow-scaled, two-leg refinement and must always be described that way. |
| Crowding as a risk factor | Established (S-026); IDEA-004 is a trade specification built on it, not a discovery of crowding itself. |
| Commodity index roll: order-flow impact and the "financialisation" of commodity futures | Established and heavily studied, with contested results (S-035 supporting; S-032, S-033, S-034, S-036, S-037 contesting). IDEA-005 is a state-conditioned refinement of a *documented and contested* family and must always be described that way; the unconditioned trade is logged as R-004. |
| Liquidity provision around predictable large trades ("sunshine trading") | Established mechanism and evidence (S-032, S-034). Any candidate built on supplying liquidity to a scheduled flow must cite and differentiate from this, not present it as new. |
| Hedging pressure and the inventory state in commodity futures | Established (S-039, S-038); these are the rival explanations for any futures-spread move and the state against which a convenience-yield bound must be measured. |
| Retail / same-day-expiry options flow and market-maker gamma | Established as a market-structure fact and as a narrative (S-043, exchange-published); the size of the index-level channel is estimated by the exchange to be de minimis, and the single-name question is open (G-05). P-006 records the parked candidate. |
| FX end-of-day fixing and closing-clock effects | **Literature read in the G-09 closure pass** (S-074 … S-081). The *fix* is a published, documented effect: the temporary, end-of-month-concentrated price impact of passive hedging demand at the 16:00 London fix (S-075), negative serial correlation around the fix (S-076), negative pre/post-fixing autocorrelation (S-077), elevated volatility and movement size around 4pm (S-074), and the W-shaped dollar pattern around global fixings (S-081). The benchmark's post-2015-revision quality is separately documented (S-080). **The fix is a baseline, not a candidate**: the aggregate version of IDEA-006 was rejected as R-007. The only residual not covered by the located literature is the *settlement-side* half of the deadline cluster — the CLS currency-close and pay-in deadlines and the post-US-close window created by T+1 (S-048, S-049) — which is unsearched (**G-11**) and must be described as an expectation until it is checked. Any candidate in this family must name the published fixing/session rules it depends on and must not present the fix's price impact as a discovery. |
| Funding-currency / global-liquidity channel and FX carry crashes | **Literature read in Cycle 2** (S-052 … S-073). The *aggregate* funding-constraint-state → carry-return relation is a published, peer-reviewed, positive baseline (S-055); the dollar-funding-liquidity → dollar-forecast relation is published in working-paper form (S-052) and peer-reviewed form (S-053); the crash mechanism, CIP deviations, hedging demand and the global-liquidity driver are documented in the central-bank and peer-reviewed literature (S-056 … S-060, S-069, S-072). **The aggregate versions are baselines, not candidates**: they were rejected as R-006. The only residual that is not published is the *cross-sectional* structure — which currencies respond most to a given dollar funding expansion — and the publication-timing test, which is retained as IDEA-007's narrow residual (v1.1) and must always be described that way. |

---

## Rediscovery guard

Before adding any candidate, check it against (a) the seven dossiers in `idea_register.md`,
(b) the baseline table above, and (c) the six specified validation hand-offs. If the candidate
differs from a baseline only in parameterisation, in label, or in the time frame, it is a variant
and belongs in this log with the baseline named, not in the register. A candidate that differs
from a baseline only in the *state variable* it is conditioned on must still show that the state
variable is observable at decision time — and must show that the conditioning changes the
*sign* or the *existence* of the effect, not merely its size.
