# REJECTED AND PARKED LOG

Purpose: prevent rediscovery, and preserve the negative reasoning that killed each candidate. A
candidate rejected here is not deleted from the project's memory; it is not a top opportunity and
must not be presented as one. Items are re-openable only with a **new mechanism**, not with better
wording or a new parameter.

Last updated: Cycle 1, 2026-10-19.

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

---

## Rediscovery guard

Before adding any candidate, check it against (a) the four dossiers in `idea_register.md`,
(b) the baseline table above, and (c) the three specified validation hand-offs. If the candidate
differs from a baseline only in parameterisation, in label, or in the time frame, it is a variant
and belongs in this log with the baseline named, not in the register.
