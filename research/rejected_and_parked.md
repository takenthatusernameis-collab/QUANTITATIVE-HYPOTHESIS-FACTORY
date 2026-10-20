# REJECTED AND PARKED LOG

Purpose: prevent rediscovery, and preserve the negative reasoning that killed each candidate. A
candidate rejected here is not deleted from the project's memory; it is not a top opportunity and
must not be presented as one. Items are re-openable only with a **new mechanism**, not with better
wording or a new parameter.

Last updated: Cycle 43 complete, 2026-10-20. **23 rejections (R-001 … R-023), 12 parkings
(P-001 … P-012), 62-row known-baseline table.** Cycle 40 added **R-020** (the eligibility-switch family
screen — bounded negative). Cycle 41 added **R-021** (the disclosure-mandate switch family — bounded negative).
Cycle 42 added **R-022** (the benchmark-methodology-change family — bounded negative). Cycle 43 added **R-023**
(the margin-schedule switch family — bounded negative: changes are published in advance but affect all participants broadly as cost/risk controls, no third-party concession flow, small effective sample). Cycle 40 also
**merged the duplicate R-019**. The log's own counts are re-derived from the file on every cycle.

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

### R-008 — "The cross-section of who feels the dollar funding constraint" (IDEA-007 v1.1 → v1.2)
- **Proposed:** the cross-sectional version of the funding-state channel — that the currencies whose
  own borrowers depend most on dollar funding respond most to a given dollar funding expansion,
  conditional on the interest differential — measured *ex ante* from the published BIS locational
  banking statistics (S-054) on their quarterly publication calendar, and identified by a
  publication-timing test (the effect must appear from the publication date and not before it).
- **Rejection reason:** it is **published, with a positive result**, and the publication is
  *precisely* the residual the dossier claimed. Wang (2026), "Deviations from Covered Interest
  Parity, Dollar Funding Pressure, and Currency Risk Premia" (S-064), states the hypothesis in the
  register's own words — "Currencies with higher dollar funding pressure (higher unconditional level
  of basis) earn higher expected excess returns" — and reports that a global high-minus-low basis
  factor earns a 4–4.5% annual risk premium, explains a large share of the cross-sectional
  variation in currency excess returns, and subsumes carry and several other factors (G10
  currencies, January 1999 – January 2025). The mechanism's own literature closed in the same
  direction during the same cycle: Moskowitz, Ross, Ross and Vasudevan are now peer-reviewed as
  "Risk, Specialization, and Covered-Interest Parity" (*Journal of Finance*, S-095) and document the
  cross-section of CIP bases and its pass-through to prices; Cenedese, Della Corte and Wang (2021,
  S-096) show that a binding regulatory balance-sheet constraint prices currency funding at the
  dealer level (about 20 basis points per annum for affected dealers); and Adrian, Etula and Muir
  (2014, S-097) establish the general intermediary-state → cross-section-of-returns mechanism that
  the candidate's family sits inside.
- **What was learned (and it is the transferable lesson of this cycle).** The only surviving
  difference between the candidate and the published result was **the choice of state variable**:
  the published work conditions on the *market-quote* cross-currency basis, the candidate would
  condition on the *published* BIS banking statistics. Two consequences, both general:
  1. A **published state on a known calendar is a feasibility property, not a source of novelty.**
     It makes an effect implementable without look-ahead or vendor data; it does not make the
     effect a discovery. The register's rediscovery guard already required a state-only difference
     to change the *sign or existence* of the effect; this case shows why, and the requirement is
     now generalised and logged as **G-12**.
  2. A **published, slow, point-in-time proxy for a market-quote state is not a better candidate
     than the market-quote state** — it is a re-specification around a weaker proxy, which the
     register's own state-proxy note forbids. This is the second time this register has produced a
     candidate whose only claim was a proxy swap; the rule now bites hard.
- **Caveats recorded for honesty.** S-064 is a **preprint / job-market paper, not peer reviewed**;
  its results are the author's own and are not reproduced here. The rejection rests on the
  *existence and positive sign* of the published result, not on its peer-review status — a
  positive working-paper result is enough to stop a candidate being presented as a discovery, and
  the peer-reviewed neighbours (S-095, S-096, S-097) independently establish the mechanism.
- **Could it be re-opened?** Only with a **new mechanism** — a new venue, participant or
  constraint — and only with a demonstration that it adds to S-055, S-064, S-095, S-096 and S-097.
  A new state variable on the same channel is explicitly not sufficient (G-12). One *unrelated*
  lead from the same closure pass is carried forward and is **not** a re-opening: "does the level of
  forward points predict the future level of forward points, on a state constructed from public
  data?" — a different mechanism, which would need its own dossier and its own originality check.
- **Kill condition met:** yes — the cross-sectional claim is published with a positive result, so
  presenting it as a candidate would be presenting a known baseline as a discovery.
- **Consequence for the register:** the register now holds **no FX candidate**. The shortlist had
  pre-registered this consequence explicitly. The funding-state *family* survives as a published
  baseline and moves into the known-baseline table.


### R-020 — The eligibility switch (*who may hold*): a regulatory or provider switch in who may hold or must trade a security, with a published compliance date and published thresholds (Cycle 40 family screen — bounded negative)

- **The family screened.** A switch that changes the *eligible holder set* of a security: a regulator
  changes who may hold a restricted security, or a market/index provider changes who qualifies for
  inclusion, and the switch has a published compliance or effective date and published thresholds. The
  template was chosen because it is *different in kind* from the compliance-deadline family the register
  has been exhausting — nothing here is an obligation converging on a date — and because it satisfies the
  register's G-13 test by construction: the thresholds and the date are published in advance.
- **The two instances run.**
  1. **The SEC's accredited-investor and qualified-institutional-buyer definition amendment** (S-244:
     Release 33-10824, 85 FR 64234, 9 October 2020, effective **8 December 2020**), which keeps the
     $1 million net-worth and $200,000 income tests and the $100 million QIB threshold and adds
     categories. This is the cleanest instance of "who may hold, published compliance date, published
     thresholds".
  2. **Index-provider eligibility and float screens** (minimum float, multi-class treatment), which are
     the nearest *observable* analogue, with published criteria, published transition periods and
     published constituent lists.
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale — four independent reasons, any one of which is sufficient.**
  1. **There is no published decision-time *binding* state.** The thresholds are published, but each
     holder's distance to its own limit is private. The state a candidate would condition on — "which
     securities have an eligible holder near the threshold" — is a **construction**, not a published
     series, and the register's rule (G-13) is about *published* decision-time states. A construction
     that must be built from non-public holder-level data is the same failure the register has already
     recorded against the 13F holdings-matching route.
  2. **The switch is published in advance, so the flow is anticipated.** Any effect of the switch is
     known before the effective date, and the nearest published analogue says what happens then: the
     index-reconstitution effect has collapsed to approximately zero in the modern sample, with
     additions below 1 % over the past decade and an average inclusion effect of about −3 basis points
     in 2020 (S-146), and the front-running around announced reconstitution is published as *competitive
     anticipatory liquidity provision* that shifts price pressure **away** from the effective date
     (S-147). A rule that buys an announced switch is buying a published anticipation.
  3. **The constrained flow is the obligor's own.** In instance 1 the constrained party is the holder
     whose eligibility changes; in instance 2 it is the index fund that must sell. In neither case is a
     third-party arbitrageur the party who is forced to trade, and the register's template requires a
     *third-party* flow creating a concession that another participant can harvest. The counterparty to
     a passive forced sale is the issuing firm and the active managers, not an arbitrageur paying a
     concession (S-151).
  4. **The effective sample is the number of switches.** A switch is a dated, discrete event: the
     number of episodes is the number of rule changes (a handful), not securities × dates, so a
     positive rule would have almost no degrees of freedom, and the cross-sectional variation the
     register would need (which securities are near the threshold) is exactly what is not published.
- **What is *not* the reason.** G-13 passes for this family: the state is public, dated and in advance
  of the event. The screen failed on the *binding-state* test, on prior publication of the nearest
  analogue, on the identity of the constrained party, and on the effective sample — and the screen was
  run against the literature before any conclusion was reached.
- **Dated re-screen condition.** Re-screen only if (i) a rule or provider methodology change is
  announced that creates a *large*, *dated*, *third-party* forced-flow obligation with a **published
  list of affected securities** and a **published distance-to-limit measure** for each affected
  holder — for example a published index-provider float screen that publishes each constituent's
  distance to the threshold; or (ii) a published study identifies a residual that survives the
  anticipation objection for a *regulatory* eligibility change.
- **Decision:** bounded negative (R-020). The eligibility-switch family is recorded in the
  known-baseline set; no dossier was created; no `IDEA-` identifier was consumed; no score changed.

### R-021 — The disclosure-mandate switch (*what must be published*): a regulator starts or stops a required public disclosure, changing the information set rather than the flow (Cycle 41 family screen — bounded negative)

- **The family screened.** A switch that changes the *information set* rather than the flow: a regulator starts or stops a required public disclosure, or changes what must be disclosed, and the switch has a published effective date. The nearest instance is the SEC's 2022 amendments to Rule 10b5-1 under the Exchange Act (87 FR 80362 final rule; 87 FR 8686 proposed release), which added Item 408(a) quarterly disclosure of 10b5-1 plan adoption, termination and modification, a mandatory cooling-off period, a Form 4 plan checkbox, and a ban on overlapping plans (S-182, S-183). The template was chosen because it is *different in kind* from the compliance-deadline family — nothing here is an obligation converging on a date — and because it satisfies the register's G-13 test by construction: the effective date is published in advance.
- **The instance run.** The SEC's 2022 Rule 10b5-1 amendments, effective for filings made on or after the compliance dates in the adopting release, changing what issuers and insiders must disclose about trading plans.
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale — four independent reasons, any one of which is sufficient.**
  1. **The sign a candidate would claim is already published.** The nearest published literature on the 10b5-1 amendments (as characterised in S-183) documents that plan **adoption** around earnings announcements carries abnormal returns of roughly −2% to −3%, while sales after the announcement do not, and no effect attaches where the cooling-off period exceeded 60 days. The sign and the window are claimed; there is no unclaimed residual for a disclosure-mandate switch candidate to harvest.
  2. **The switch is published in advance, so any reaction is anticipatory.** The rule and its compliance dates were published before they took effect, so any price response to the disclosure change is known before the effective date and is priced in anticipation. A rule that trades an announced disclosure change is trading a published anticipation, not an unclaimed concession.
  3. **The disclosure change is the obligor's own obligation.** The party whose disclosure changes is the issuer or the insider; there is no third-party arbitrageur who is forced to trade and who pays a concession to a counterparty. The register's template requires a *third-party* flow creating a concession; a change in what the obligor must publish does not create one.
  4. **The effective sample is the number of amendments.** A disclosure-mandate switch is a dated, discrete event: the number of episodes is the number of rule changes (a handful), not securities × dates. A positive rule would have almost no degrees of freedom, and any cross-sectional variation (which securities are most affected by the new disclosure) is exactly what is not published at decision time.
- **What is *not* the reason.** G-13 passes for this family: the effective date is public and dated in advance. The screen failed on prior publication of the nearest analogue's sign, on the identity of the constrained party (the obligor, not a third party), and on the effective sample — and the screen was run against the literature before any conclusion was reached.
- **Dated re-screen condition.** Re-screen only if (i) a regulator announces a disclosure mandate whose *scope or threshold* creates a dated, third-party forced-flow obligation with a **published list of affected securities**; or (ii) a published study identifies a residual price effect attached to the *execution* of a disclosed schedule rather than to its adoption, for a regulatory disclosure change.
- **Decision:** bounded negative (R-021). The disclosure-mandate-switch family is recorded in the known-baseline set; no dossier was created; no `IDEA-` identifier was consumed; no score changed.

### R-022 — Benchmark-methodology change with a published effective date (Cycle 42 family screen — bounded negative)

- **The family screened.** An index provider changes its benchmark methodology — constituent rules, weighting scheme, rebalancing schedule, or effective date — and publishes the change and its effective date in advance. This is the index-provider analogue of the eligibility switch (R-020): the *who* changes in R-020; here the *rule* changes. The template was chosen because it is genuinely different from the compliance-deadline family — nothing here is an obligation converging on a date — and because it satisfies G-13 by construction: the methodology change and its effective date are published before they take effect.
- **The instances run.**
  1. **S&P Dow Jones Indices methodology changes published 2026-04-26 with published effective dates**, covering index maintenance, timing of changes and rebalancing conventions across the S&P U.S. indices family.
  2. **FTSE Russell index notices**, including gilt-index changes announced 2026-05-12 effective 2026-05-20 and FCA-driven changes effective 2024-07-29, each with a published announcement date and effective date.
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale — four independent reasons, any one of which is sufficient.**
  1. **The change is published in advance, so any flow is anticipated.** The methodology change, its effective date and (for rebalancing) the share-freeze window are all published before the event, so any index-tracker flow responding to the change is known before it happens. The nearest published analogue — index reconstitution — finds the effect collapsed to approximately zero in the modern sample (additions below 1% over the past decade, average inclusion effect about −3 basis points in 2020; S-146) and modelled as anticipatory liquidity provision that shifts price pressure *away* from the effective date (S-147). A rule that trades an announced methodology change is trading a published anticipation.
  2. **The flow effect is a published baseline.** Index reconstitution and rebalancing flows are a documented institutional pattern (S-001 … S-004, S-146), and the published literature already explains the structure: anticipatory pre-positioning before the event and covering after it (S-147), with the counterparty to passive demand being the issuing firm (S-151). A methodology change is a variation on reconstitution, not a new mechanism.
  3. **The constrained flow is the index fund's own.** The party that must trade is the index fund or ETF tracking the benchmark — the obligor whose mandate changes — not a third-party arbitrageur forced to trade at a concession. The counterparty to the passive flow is the issuing firm and other institutions trading in the same direction (S-151), so there is no arbitrageur paying a concession to harvest.
  4. **The effective sample is the number of methodology changes.** A methodology change is a dated, discrete provider-level event: the number of episodes is the number of provider rule changes (a handful per provider), not securities × dates. A positive rule would have almost no degrees of freedom, and the cross-sectional variation (which constituents are near a weighting threshold) is not published at decision time.
- **What is *not* the reason.** G-13 passes for this family: the effective date is public, dated and in advance of the event. The screen failed on prior publication of the reconstitution analogue, on the identity of the constrained party (the index fund, not a third party), and on the effective sample — and the screen was run against the literature before any conclusion was reached.
- **Dated re-screen condition.** Re-screen only if (i) a provider announces a methodology change that creates a *large*, *dated*, *third-party* forced-flow obligation with a **published list of affected securities** and a **published effective date**; or (ii) a published study identifies a residual that survives the anticipation objection for a *benchmark methodology* change (as distinct from the published reconstitution literature).
- **Decision:** bounded negative (R-022). The benchmark-methodology-change family is recorded in the known-baseline set; no dossier was created; no `IDEA-` identifier was consumed; no score changed.


### R-023 — Margin-schedule switch (venue rule changes margin requirements on a published calendar) (Cycle 43 family screen — bounded negative)

- **The family screened.** A switch where a venue/clearinghouse changes margin requirements (initial/maintenance, SPAN parameters) on a published calendar/effective date.
- **Instances run.** CME SPAN 2 framework parameter changes (energy/equity pods, Feb-Mar 2026 notices with effective dates), CME precious metals margin setting changes (Jan 2026 shift to percentage-of-notional).
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale — four independent reasons, any one of which is sufficient:**
  1. **Published in advance** — changes are announced via notices with effective dates, satisfying G-13.
  2. **No third-party concession flow** — margin changes affect all participants with positions; the constrained response is typically margin calls/liquidation by participants themselves or their clearing firms, not a forced flow by one party creating a concession to another third-party arbitrageur.
  3. **Broad-based cost change, not targeted opportunity** — affects entire product classes/risk profiles; no published list of affected securities with exploitable cross-section creating an unclaimed sign.
  4. **Effective sample is small** — discrete rule changes with limited degrees of freedom; margin effects are known as costs/risk controls.
- **Decision:** bounded negative (R-023). No dossier created; no `IDEA-` identifier was consumed; no score changed.


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

### R-009 — IDEA-006 FIXCLOCK: the end-of-day deadline cluster (settlement-side residual) — *Cycle 5, G-11 closure*
- **What was claimed:** the FX day ends with a cluster of hard, published deadlines, and the flows
  those deadlines force are not price-sensitive; the *fix* half of the cluster is published (rejected
  as R-007), and the candidate's residual claim was that the **settlement-side** deadlines impose a
  separable, additional price-insensitive demand in a window that is not a benchmark — the CLS
  currency-close and pay-in cut-offs and the post-US-close window created by the May 2024 T+1
  transition (S-048, S-049) — and that the published fix effect survives the 2015 methodology
  revision and the post-2013 enforcement regime.
- **Why rejected:** the candidate set its own gate — "G-11 must be closed before any of the above is
  treated as a candidate rather than a hypothesis. **If a published paper already shows a
  settlement-side or T+1-window price effect, the candidate is rejected, not narrowed**" — and the
  Cycle-5 G-11 closure met it in both limbs. **(i) A settlement deadline cluster is a published
  price determinant:** Kraenzlin and Nellen (2010, S-112) show that after the introduction of CLS
  "the value of intraday liquidity has increased during the hours of the CLS settlement cycle", with
  a structural break at the pay-in schedule and an estimated mark-up of "approximately 0.50bp per
  hour, leading to a total of roughly 1.5bp for the CLS settlement cycle"; the mechanism is stated
  explicitly — "CLS members have to meet a pay-in schedule set by CLS in due time. This requires
  large amounts of reserve balances to be transferred during specific time slots." **(ii) A
  T+1-window price effect is also published**, and with the *opposite* sign to a harvestable
  concession: shortening the securities settlement cycle *improved* liquidity (S-113: US securities
  "become more liquid, relative to similarly matched securities listed on the London Stock
  Exchange" after T+3 → T+2; S-114: T+1 "significantly improved liquidity, measured by bid-ask
  spreads, Amihud illiquidity and price impact measures"; S-115, preprint: T+1 "significantly
  reduces Parkinson volatility by 3.6% relative to its mean"). **(iii) The residual's own
  kill condition on post-2015 persistence was answered earlier** by the published, pre-registered
  reassessment of the 4pm fix using 2015–2023 data (S-047, S-080). **(iv) The remaining sliver —
  the post-US-close window's own market quality — is documented as a cost, not an edge:** the
  New York Fed's FX Committee material names "NY 4-6pm currency liquidity" as the transition's
  priority FX risk (S-117) and records the market's expectation of "an uptick in price premium and
  market impact for trades executed later in the NY trading day" (S-118); the market record is that
  "less than 1% of trades in the $7 trillion OTC FX market are carried out in this window", that at
  5pm ET "most of the large investment banks shutdown their market making pricing engines for
  anywhere up to 30 minutes", and that "bid/ask spreads widen and liquidity shrinks" (S-119); the
  market's own solution was custodian cut-off extensions and pre-funding (S-120).
- **What would have rescued it:** nothing in the literature — the candidate's own rule forecloses
  narrowing when a published paper already shows the effect. A *different* mechanism in the same
  window (for example, a flow whose size is published and dated rather than a price premium) would
  be a new candidate with its own originality check, not a revival of this one.
- **Residual open for the register (not for this candidate):** no located paper measures an
  **FX-spot** price effect specific to the post-US-close window with the published fix effect
  removed. That gap is now recorded as a *baseline boundary* in the table below, not as an
  opportunity: the window is documented as too illiquid to harvest, and the data required are
  commercial.

### R-010 — IDEA-012 CLS-CLOSE: the settlement-side deadline cluster as a price determinant — *Cycle 5, G-11 closure*
- **What was claimed:** a dedicated vehicle for the settlement-side residual of IDEA-006: the CLS
  settlement deadline cluster (the CLS midnight CET currency close and pay-in schedule) and the
  post-US-close T+1 window impose a price-insensitive funding demand in a window that is not a
  benchmark, and the resulting concession has not been tested.
- **Why rejected:** the candidate existed to *be* a literature check, and it recorded its own
  consequence in advance: "If G-11 closes against the candidate (a published paper tests the
  settlement-side deadline cluster as a price determinant), the candidate is rejected, not
  re-scored." The check was run and returned "tested and found priced" — S-112 (settlement deadlines
  priced), S-113/S-114/S-115 (the securities settlement cycle is a published price-impact and
  market-quality determinant), S-082 and S-071 (the FX settlement-risk premium is published) — and
  the residual window is documented as structurally illiquid and costly rather than concession-rich
  (S-117 … S-120). A pip-level concession measured inside minutes in a window carrying under 1% of
  daily volume cannot survive a round trip, which was the candidate's acknowledged weakest point
  even before the closure.
- **What would have rescued it:** a materially different specification with public intraday data
  and a cost estimate that survives the documented market structure — which is precisely what the
  market-structure evidence denies.
- **Note on scope:** this rejection is about the *price-determinant* claim. The market-structure
  facts established here (the window's illiquidity, the pricing-engine outage, the custodian
  cut-off extensions) are recorded as baselines and may be useful as *costs* in the design of
  unrelated candidates that must trade in or around that window.

### R-011 — IDEA-001 RECON-FLOW: announcement-timed, flow-scaled reconstitution pressure with a post-effective reversal leg — *Cycle 13, evidence closure*

- **What was claimed:** that an index provider's reconstitution creates a scheduled, deadline-driven,
  price-insensitive demand shock; that the price concession paid to the counterparty is partly
  reversed after the passive flow has been executed; that the announcement-to-effective drift
  *scales with the required passive flow*; and that the asymmetry between additions and deletions is
  a flow-and-capacity effect rather than an awareness effect. The candidate entered the register as
  the rank-1 item at 76.0 and had a validation specification (V-001) for six cycles.
- **Why rejected:** three published results close it, and they close different limbs.
  1. **The base effect has disappeared.** Greenwood & Sammon (S-146, *Journal of Finance* 2025)
     document that the abnormal return associated with an S&P 500 addition has fallen from an
     average of **7.4% in the 1990s to less than 1% over the past decade**, that deletions average
     **0.1% between 2010 and 2020**, and that the average inclusion effect in 2020 was **−3 basis
     points**. A concession of approximately zero is not a concession that can be harvested; the
     candidate's leg 1 has no effect left to trade, and its side-asymmetry claim has no economic
     content in the modern sample.
  2. **The differentiator has a published null.** The same paper finds "no apparent relationship
     between net purchases [by index trackers] and the index inclusion effect, for either additions
     or deletions". The candidate's stated differentiator — that the drift scales with the required
     passive flow — is not merely unclaimed; it is contradicted.
  3. **The mechanism is published, and it points at a different window.** Pegoraro, Sammon & Shim
     (S-147) model speculators as *anticipatory liquidity providers* whose pre-positioning "shifts
     price pressure away from the reconstitution date"; they report that short interest **rises on
     implementation dates and falls afterwards** as speculators cover, that trading costs decline as
     speculator competition rises, and that "apparent front-running reflects competitive liquidity
     provision and benefits index investors". The candidate's chain required the concession to be
     paid *between the announcement and the effective close* and to persist until the arbitrageur
     unwound; the published structure is anticipation *before* the event and unwinding *after* it.
     Sammon & Shim (S-151) supply the reason: the counterparty to a passive fund's demand is **the
     issuing firm itself**, and most demand-side institutions trade in the same direction as index
     funds, so there is no arbitrageur paying a concession to capture.
- **The rejection is *not* a data or premise failure.** Two gaps closed **in the candidate's
  favour** in the same cycle, and the register records them because they are reusable research
  assets: **G-03** — the index funds' effective-close convention is now documented by the index
  manager itself (S-149: index funds and ETFs are "structurally incentivized to execute trades at
  the closing auction" because official NAVs are struck on closing prices, with Market-on-Close
  orders "the dominant mechanism for end-of-day execution") and by peer-reviewed work (S-150 on
  closing-auction volume share, price impact and passive attribution; S-148 on execution at the
  closing price on reconstitution day); and **G-02/G-07** — a **published construction method** for
  benchmark-specific tracked assets now exists (S-148 infers the AUM tracking each of five named
  indices from reconstitution-day closing volume, 2000–2021), so the flow-scaling limb no longer
  rests on an industry estimate. The candidate died on evidence, not on an unresolved technicality.
- **What would have rescued it (and is now foreclosed):** a specification whose timing is the
  *announcement-to-implementation* window rather than the announcement-to-effective-close window, and
  which trades *against* the anticipatory flow rather than with it. That structure is exactly what
  S-147 publishes, and a second 2026 preprint (S-171) models it again as a differential game. It is
  therefore a **published baseline**, not an unclaimed candidate.
- **Standing:** priority score **76.0 withdrawn**; V-001 **withdrawn**; the dossier is retained in
  `idea_register.md` (v2.0, terminal) for the audit trail; the reusable outputs are filed as
  baselines ("the disappearing index effect", "anticipatory liquidity provision at reconstitution",
  "benchmark-specific passive-asset estimation from reconstitution-day volume").

### P-008 — IDEA-013 EU-ETSCOMP: the surrender-deadline concession in the EU ETS — *parked, not rejected*
- **Why parked rather than retained or rejected:** the required full-text check on the published work
  (S-101) was performed in Cycle 5 and came out *against* the candidate in three specific ways.
  (i) The published paper does **not** condition the surrender-month premium on the aggregate
  allowance surplus, so the candidate is **not** a re-description of published work; but the paper's
  *model* already makes the equilibrium price affine in the aggregate bank of allowances, so the
  state-conditional structure is an implication of the published model rather than an unclaimed
  idea; and the paper's own robustness construction works from **operator-level, bank-adjusted**
  shortfalls, which implies the aggregate balance is not the object that determines residual demand.
  (ii) The published sample contains a **high-surplus year in which the effect persisted** — "This
  delayed and frictional trading pattern persists into the most recent phase of the EU ETS" (Phase
  IV, 2021; TNAC 1 134 794 738 for 2022 and 1 111 736 535 for 2023, S-121) — which does not support
  the candidate's existence-flipping hypothesis. (iii) The **decision-time availability** of the
  state is the binding constraint: the Commission publishes TNAC for emissions year Y in late May or
  June of year Y+1 (S-121), so under the pre-2023 regime the aggregate state for the compliance
  year was published **after** the 30 April deadline it was meant to inform. Decision-time
  availability begins only with the 2023 compliance year, leaving **three observations, none in a
  deficit year** (new gap **G-13**). Re-specifying around a weaker state — operator-level
  bank-adjusted shortfalls, public only *ex post* in the Union Registry — would convert the idea
  into a disguised baseline, which the register's own method forbids.
- **Unblocking question (dated):** the unblocking event is the accumulation of enough post-2023
  compliance years for the aggregate balance to cross a sign change with at least one observation on
  each side. The next TNAC (emissions year 2026) is expected in late May or June 2027, with the
  corresponding surrender deadline on 30 September 2027. **Before 2029 the candidate cannot be
  validated in decision-time form, and no further effort should be spent on it.** A cheaper
  secondary check, worth at most one search: whether a replication of the surrender-month premium in
  the post-2023 September regime has appeared in the literature — if it has, the *regime* residual is
  closed too and the candidate should be rejected rather than parked.
- **Score and standing:** priority score **58/100** (down from 70 in v1.0), below every retained
  candidate. The dossier remains in `idea_register.md` because the reasoning is worth preserving;
  the candidate is not in the active ranking and has no validation specification.

### P-009 — IDEA-005 ROLLCOND: the scheduled commodity-index roll as a size-conditional liquidity demand — *parked in Cycle 6 on G-12, not rejected*
- **Why parked rather than retained or rejected:** the candidate was **retained through five cycles**
  on the strength of one idea — that the published aggregate null is a *composition effect*, and
  that the concession survives only where the passive share of open interest is high and contract
  depth is thin. The Cycle-6 G-12 screen was applied to it and the screen **failed**. The
  candidate's own formulation is an *existence* claim, which is what G-12 asks for, but G-12 asks
  what the candidate *demonstrates*, and the demonstration runs the other way on three independent
  counts. (i) The **closest published test of the candidate's own state variable** — the CFTC
  Index Traders' share of open interest, conditioned on *commodity returns during roll periods* —
  reports **no significant effect** (S-099); the published work on the trader-type channel
  conditions *rate of convergence* rather than the nearby-to-deferred spread concession (S-098).
  (ii) The **aggregate effect the joint claim would rescue is documented as decayed**: the roll's
  impact on the nearby-versus-deferred spread "disappears in the 2012–2019 subperiod" (S-033), with
  index-trader positions not predicting near-contract excess returns (S-037) and commodity index
  rolls found to have "little futures price impact" (S-036). (iii) G-06 closed as a **bounded
  negative finding**: no located paper conditions the joint state on the concession, so the
  differentiator is untested rather than supported.
- **Why this is a parking and not a rejection:** the register's rule is to reject when a published
  result **shows the candidate's effect** (R-007, R-009, R-010). S-099 shows a **null**; nothing
  published claims what IDEA-005 claims. The joint state is untested, not refuted, and the
  reconciling composition argument is a legitimate hypothesis. So the candidate is parked with its
  reasoning intact, and its falsifiable question preserved.
- **Unblocking questions (both required, and neither is a search):** (i) a published or constructible
  test of the **joint** state — passive share **×** contract depth — against the nearby-to-deferred
  spread concession; and (ii) evidence that the concession **survives 2012–present** in the thin,
  high-passive-share contracts. Until both are met, IDEA-005 must not be presented as a candidate,
  must not be given a validation specification (**V-004 is withdrawn**), and must not be
  re-specified around a weaker proxy — the joint state already requires an input (contract depth)
  that is real-time observable but is not a published downloadable series, which is why the data
  dimension was cut from 5 to 4.
- **Score and standing:** priority score **60/100** (down from 72) — evidence 3 → 2, novelty 3 → 2,
  falsifiability 4 → 3, data 5 → 4; mechanism 4 and resilience 3 unchanged. Below every retained
  candidate. The dossier remains in `idea_register.md`; the candidate is not in the active ranking.

### P-010 — IDEA-008 SECURITY-LEND: borrow constraints, recall-driven forced covering — *parked in Cycle 6 on G-13, with a dated unblocking condition*
- **Why parked rather than retained or rejected:** this is a **calendar** failure, not an evidence
  failure, and the distinction matters. The candidate's mechanism is documented (borrow constraints
  as limits to arbitrage, S-083; recall risk as a real cost of shorting, S-084) and its core
  specification is not a re-description of published work, so it is not a rejection. But the state
  the candidate names — **securities-lending fees and borrow availability** — is not published to
  the public on any usable calendar. The Commission granted a temporary exemption "from compliance
  with Rule 10c-1a **with respect to the reporting date until September 28, 2028, and with respect
  to the dissemination date until March 29, 2029**" (S-126), so the earliest date on which a
  borrow-cost state can be public is **29 March 2029**; the July 2025 order had set the
  corresponding dates two years earlier, so the public-availability date has already been pushed
  back once. The fallback state does not rescue the candidate: the short-interest file is **twice a
  month**, must be reported "by 6 p.m. Eastern Time on the second business day after the reporting
  settlement date", and is published on the later date in FINRA's own schedule — in the worked
  examples on that page a 14 November settlement is published on 25 November, and a 2 December
  settlement on 15 December (S-127) — so it is a *stale* state rather than a decision-time one, and
  it measures positions rather than borrow cost. The event itself, the recall, is not published at
  all and must be inferred.
- **G-12 note:** the screen would have passed — the forced-covering spike exists only when the
  borrow constraint binds, so the state conditions the *existence* of the effect rather than its
  size. The failure is G-13 alone, and it is recorded as such so that a future session does not
  re-litigate the mechanism.
- **Unblocking question (dated):** **on or after 29 March 2029**, re-read the Rule 10c-1a
  dissemination data — the RNSA's public reporting of Rule 10c-1a information, including loan-rate
  terms — and test whether a public, dated, security-level borrow-cost series exists whose
  *publication date precedes a decision date*. Only then re-open the candidate (new gap **G-14**).
  The related aggregate short-position regime (Rule 13f-2 / Form SHO) has its own dated start —
  "until January 2, 2028" (S-126) — but it measures **positions**, not borrow cost, and must not be
  substituted for it: re-specifying around a different measure is exactly what the state-proxy note
  forbids.
- **Score and standing:** priority score **63/100** (down from 65) — data 3 → 2 only; mechanism 4,
  evidence 3, novelty 3, falsifiability 3 and resilience 3 unchanged. **V-007 (IDEA-008) is
  withdrawn.** The dossier remains in `idea_register.md`; the candidate is not in the active ranking.

---

### R-012 — "Statutory payment-date liquidity drains" as a dated, price-insensitive cross-asset flow (Cycle 30 family screen — bounded negative)

- **The family screened.** Recurring statutory payment dates that move cash from the private sector
  into the Treasury on a known calendar: US corporate estimated income-tax payments (the four
  instalment dates set by statute for calendar-year large corporations), payroll-tax deposit dates,
  and the EU/UK provisional-tax dates. The template is the register's own "dated, price-insensitive
  institutional flow" template with the *state* being the size of the payment due.
- **Why no candidate.**
  1. *The funding-market manifestation is published.* Treasury cash drains are an identified driver of
     short-term funding-market stress: an IMF working paper quantifies repo-spread swings around
     debt-ceiling episodes (S-160), and the Federal Reserve's own notes model repo-rate sensitivity
     to Treasury issuance through the SOMA, the ON RRP facility and the TGA, using the public
     **TGCR − IORB** spread as the decision-time stress measure (S-161, S-162). A candidate in this
     family would therefore be re-presenting a published channel, and the register already files the
     TGA channel as both a baseline and a **cost model**.
  2. *There is no surprise to price.* The payment dates are fixed by statute years in advance, so the
     flow is known rather than anticipated; the register's own note on sovereign issuance calendars
     makes the same point — the announcement is a *news* event whose surprise component requires
     expectations that are not published (S-142, S-144). A known-date flow can still carry a
     concession, but only if the *size* or the *timing* of the flow is uncertain, and here both are
     published.
  3. *No published decision-time state isolates the payment due.* Aggregate corporate tax receipts
     are published monthly with a lag, the corporate sector's cash position is published quarterly,
     and neither identifies the payment that is *due* at a given decision date, nor separates the
     non-withheld corporate tax (which drains the banking system) from withheld tax (which does not).
     A candidate built on this family would have to construct that state rather than read it, which
     is the state-proxy problem the register has already learned to treat as a blocking condition.
  4. *Confounders of the first order.* Corporate earnings seasons sit near the same calendar dates,
     and the flow is second-order relative to daily turnover in every asset class the register
     covers.
- **Verdict: bounded negative — no candidate.** The family's funding-market channel is published
  (S-160, S-161, S-162); the cross-asset extension fails on state construction and on surprise. **No
  external claim is asserted beyond the ledger entries cited above**: the tax-date magnitudes reported
  in trade press during 2026 were *not* verified in this cycle and are therefore deliberately not
  recorded here.
- **Rediscovery guard.** Any future candidate in this family must (i) name the published TGA → repo
  channel as the funding-market manifestation rather than as a discovery, (ii) construct a
  decision-time state that isolates the payment due at the decision date and separates non-withheld
  from withheld tax, and (iii) show a concession that survives the earnings-season and macro-release
  confounders. Until then the family is a baseline.

### R-013 — "Debt tender offers and liability-management exercises" as a dated, price-insensitive deadline flow (Cycle 32 family screen — bounded negative)

- **The family screened.** Corporate-debt tender offers and liability-management exercises: an issuer
  offers to buy its own bonds for cash at a fixed price (or a fixed spread, or a Dutch auction) before a
  published expiration date, with the offer document publishing the price, the amount sought and the
  deadline. It looked like the register's best remaining template fit — a *dated*, *price-insensitive*
  flow into a *published* deadline, with a decision-time state literally inside the offer document.
- **Why no candidate.**
  1. *The flow is published and quantified.* The tender price averages a **4.75%** premium (median
     3.40%) to the pre-tender market price and **82.3%** of the issue (median 94.6%) tenders; a 1% rise
     in the tender premium raises the tendering rate by as much as 10% (S-204). The price-insensitive
     flow at a published deadline is a documented object, not an unclaimed mechanism.
  2. *The deadline-cluster behaviour is published too.* **72%** of exercised-clawback issues underwent
     renegotiation by tender, and **73.9%** of them did so *before* the clawback's published expiration
     date (S-206). The "obligations converge on a published deadline" structure is documented.
  3. *The price-insensitive flow is the issuer's, and it supports the price.* The issuer commits to buy
     at a fixed premium, so price-insensitive *demand* at a published price puts a floor under the bond
     and pulls it *toward* the offer price as expiry approaches — the opposite shape to the register's
     cap-and-trade and compliance-deadline template (IDEA-013, IDEA-014), which requires the flow to push
     the price *below* fair value into the deadline and revert afterwards. The structural contrast is
     explicit: the tender is the price-known-to-the-seller repurchase route, open-market repurchase is
     not (S-205).
  4. *The one tradeable implication is a mechanical arbitrage, not an edge.* Buying a bond below a
     *published* offer price and tendering it is a trade against a known price, subject only to
     completion risk, proration and the "early bird" priority (S-208) and the guaranteed-delivery
     mechanic (S-207). The residual after the deadline is the re-pricing of the *remaining* bonds as the
     capital structure changes — a **credit event**, not a mechanical reversion, and therefore not the
     register's object.
  5. *There is no cross-issuer deadline cluster.* The tender deadline is **issuer-set**, subject to
     regulatory minimum offering periods (S-207, S-208) rather than a single statutory date shared by a
     population of obligors. The register's deadline-cluster template works because a *regulator* fixes
     one date for everyone; in credit the deadlines are staggered by construction.
- **Verdict: bounded negative — no candidate.** The family is filed as a **baseline** in the table below.
  **One item is flagged as not independently verified:** the specific Rule 14e-1 periods and disclosure
  duties used in this screen are index-rendered from practitioner notes (S-208, S-209); the rule text
  itself was located at the eCFR (S-207) but the relevant paragraphs were not read in this cycle. A
  future cycle that relies on those provisions must read the rule.
- **Rediscovery guard.** Any future candidate in this family must (i) explain why the *issuer's* demand
  does not simply support the bond price, (ii) identify a state that is published *before* the deadline
  and determines the *sign* of any price effect, (iii) show that the effect is not the mechanical
  arbitrage against the published offer price, and (iv) show that it survives the capital-structure
  re-pricing that occurs after the deadline. Until then the family is a baseline.

### P-011 — IDEA-015 PLAN-SUPPLY: pre-announced, non-discretionary insider supply — *parked in Cycle 30 on evidence (G-21), not rejected*

- **What the candidate is.** A trade keyed to a security's *remaining scheduled insider supply* under
  Rule 10b5-1 plans: the plan's adoption date, duration and maximum aggregate size are disclosed
  quarterly in the issuer's Form 10-Q/10-K under Item 408(a), and individual plan sales are reported
  on Form 4 within two business days with the plan's adoption date and, sometimes, the plan's
  remaining capacity (S-182, S-187). The supply is scheduled, non-discretionary and price-insensitive
  because the insider cannot accelerate out of a plan without restarting the regulatory cooling-off
  period, so the state is a *legal*, statutorily cadenced, published object — the register's first
  instance of that class (see the shortlist's cross-cutting note 11).
- **Why it is parked and not rejected.** The register rejects only when a published result *shows* the
  candidate's effect, and nothing published shows it: the nearest published price evidence attaches to
  plan **adoption** around earnings announcements — abnormal returns of roughly −2% to −3% for plans
  executing a sale in the window between adoption and that quarter's earnings announcement, no price
  drop after the announcement, and no effect where the cooling-off period exceeded 60 days (S-183, as
  characterised by the SEC) — not to the **execution** of a disclosed schedule. The candidate is
  therefore parked on an *evidence* question, with the register's IDEA-005-style treatment.
- **Unblocking condition — G-21.** Is there published work that (a) constructs a security-level
  *remaining scheduled supply* state from Item 408(a) and Form 4 filings, and (b) documents a price
  effect attached to the *execution* window rather than the adoption window? A positive published
  result → re-score and admit to the active ranking (it would enter between IDEA-010 at 65.0 and
  IDEA-009 at 60.0). A published null on execution-window price pressure → reject. Nothing published
  → the candidate stays parked with an evidence-first condition.
- **What it must not do.** It must not be re-specified around an easier state (plan *existence*
  rather than remaining capacity), must not use sell-to-cover sales tied to vesting and tax
  withholding, and must not be given a validation specification while parked. **V-010 is not opened.**

### P-012 — IDEA-003 VRP-STATE: an option-surface crash state layered on a variance harvest — *parked in Cycle 35 on evidence (G-22), not rejected*

- **What the candidate is.** A variance-risk-premium harvest — selling options, or its delta-hedged
  equivalent — whose *state* is an imminent-crash measure read off the option surface, on the claim that
  the harvest's risk-adjusted value improves, or its tail improves, when the state says a crash is
  imminent. After the Cycle-32 re-specification it survived only as a *tail-management* claim: the
  realised harvest is catastrophically left-tailed in crash states, and the candidate's residual
  content is the **state construction**.
- **Why it is parked and not rejected.** The register rejects only when a published result *shows* the
  candidate's effect, and nothing published shows it. G-22 was registered in Cycle 32 with an explicit
  rule: *does any published work establish that an option-surface-implied imminent-crash measure adds
  risk-adjusted value to a variance harvest beyond the published state-conditioned volatility-trading
  family (S-180)? If not, the candidate is a known baseline and must be parked.* The Cycle-35 search
  (executed, not assumed) found that the published option-implied crash literature does three different
  things — it **forecasts crash events**, it **predicts the expected market return** from a crash measure
  with a markedly different marginal effect in crisis and non-crisis periods (S-223), and it **prices
  crash risk** — and none of it asks whether a crash state improves the risk-adjusted value of
  harvesting variance. By the registered rule, the candidate is a known baseline with an unvalidated
  state overlay and **must be parked**. It is parked, not rejected: the candidate is unsupported and
  unranked, not falsified.
- **Prior art now also in the way.** Cycle 32 closed G-19 against the candidate's sign claim: the
  expected variance premium is stated by three independent peer-reviewed sources (S-190, S-191, S-192)
  and its sign in bad states has been tested — the premium is **positive and higher in turmoil**
  (S-190), while the negative stress readings belong to the naive ex-post estimator. So the candidate's
  "the harvest pays more in crash states" framing is contradicted at the premium level, and the
  *newest* literature prices a crash measure's own return-predictive content (S-223) rather than its
  usefulness as a harvest conditioner.
- **Unblocking condition — a new G-22 restatement, to be registered if pursued.** The candidate could
  be re-admitted only if published work exists that (a) constructs a **purely option-surface-implied**
  imminent-crash measure (no realised-moment component, as in S-223) and (b) demonstrates that
  conditioning a variance harvest on it **improves the harvest's risk-adjusted value**, as opposed to
  improving crash-event forecasting or expected-return prediction. Nothing published in the Cycle-35
  search does both.
- **What it must not do.** It must not be re-specified around an easier state (a realised-volatility
  or VIX-level state, which would be a published baseline), must not be presented as a new premium
  edge, and must not be given a validation specification while parked. **V-003 is marked
  never-to-execute.**
- **Cycle-35 note on the record-keeping.** The Cycle-33 source-ledger header and the Cycle-34 handoff
  both asserted that this parking ("P-012, G-22 closed against") had already been executed. It had not:
  no source, verdict or parking existed in any artifact. Cycle 35 executed the search, wrote the
  parking and the verdict, and the handoff's standing condition is now true rather than claimed.

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
| Funding-currency / global-liquidity channel and FX carry crashes | **Literature read in Cycle 2 and closed in Cycle 5** (S-052 … S-073, S-095 … S-097). The *aggregate* funding-constraint-state → carry-return relation is a published, peer-reviewed, positive baseline (S-055); the dollar-funding-liquidity → dollar-forecast relation is published in working-paper form (S-052) and peer-reviewed form (S-053); the crash mechanism, CIP deviations, hedging demand and the global-liquidity driver are documented in the central-bank and peer-reviewed literature (S-056 … S-060, S-069, S-072). **The aggregate versions were rejected as R-006, and the cross-sectional version was rejected as R-008 in Cycle 5.** The whole family — aggregate, cross-sectional, and the publication-timing variant — is now a baseline, not a candidate. |
| Cross-currency basis as a priced cross-section of currency risk premia | **Published and positive** (S-064, a preprint; G10 currencies 1999–2025). "Currencies with higher dollar funding pressure (higher unconditional level of basis) earn higher expected excess returns"; a high-minus-low basis factor is reported to earn 4–4.5% annually and to subsume carry and other factors. Any FX candidate in this family must be a **new mechanism**, not a new state variable (R-008, G-12). |
| Intermediary specialization, safe-asset scarcity and the cross-section of CIP bases | **Published, peer-reviewed** (S-095, *Journal of Finance* 2026; NBER WP 32707; FEDS 2024-061). Three forces are documented — foreign safe asset scarcity, market power and segmentation of banks by market, and concentration of demand — and their pass-through to prices is quantified (of the order of 7–18 basis points per standard deviation). The state is **confidential supervisory data**, so it is not reproducible from public sources; this is the strongest argument that the family needs a new mechanism rather than a new proxy. |
| **Sovereign bond index inclusion and exclusion** | **Published, peer-reviewed — screened in Cycle 6 as frontier family 4.** Inclusion-driven flows into local-currency sovereign debt indices are a published causal object: sovereign yields fall and the domestic currency appreciates (S-137, *Journal of International Economics* 2021), and rebalancing flows move prices, deepen the market and appreciate the currency with placebo tests around the event (S-138, *Journal of Financial Economics* 2019). The institutional scale and the correlated-yield consequences are documented by the IMF (S-139). The equity-reconstitution analogue is IDEA-001's territory. **No candidate in this family is available without a new mechanism.** |
| **Sovereign issuance calendars (US Treasury quarterly refunding)** | **Published — screened in Cycle 6 as frontier family 2.** The refunding announcement is an issuer-run, published, recurring event (S-143), and its price consequences are already the subject of published work: a paper decomposing "debt supply shocks using Treasury auction announcements" (S-142) and a paper on "pre-refunding announcement gains" in Treasuries (S-144). The announcement is also a *news* event whose surprise component requires expectations that are not published, so the residual is not a state-conditioned concession at all. **No candidate in this family.** |
| **Fast-payment rails and the liquidity-demand channel** | **Published mechanism, no candidate structure — screened in Cycle 6 as frontier family 3.** Instant payments raise banks' liquidity demand because they remove the ability to delay and net payment flows (S-140), and 24/7 settlement is modelled as inducing a precautionary demand for central bank balances with upward pressure on the overnight rate (S-141). The family's decision-time object is a rail's *adoption curve*, not a dated obligation: there is no date-bound, price-insensitive flow to capture, and the effect is a level shift in reserve demand that is repriced as it is learned. **No candidate in this family.** |
| **Physical-delivery calendars and the inventory channel in commodity futures** | **Published mechanics — screened in Cycle 6 as frontier family 5.** The inventory-and-convenience-yield channel that makes a delivery calendar a price determinant is already in this ledger (S-038, S-039); the roll mechanics that generate the delivery-month pattern are peer reviewed (S-145, alongside S-032, S-033, S-034, S-036); and the *published* state the family would need — exchange warehouse stocks and delivery calendars — is the same published-inventory channel already in this table. **No candidate in this family.** |
| **Statutory compliance-deadline concessions: the EU ETS instance** | **Published — the template's baseline, and the reason the US RFS instance is a separate candidate.** The EU ETS surrender-month premium is documented: April returns "averaging more than 10% in Aprils" (S-101). Any candidate in this family must be a **different market with a different regulator and a different obligor population**, and must state how its state decides the *sign* of the effect — the published EU ETS instance has no such state. That is exactly what IDEA-014 does in the US Renewable Fuel Standard. |
| **RIN price formation and pass-through (US biofuel credits)** | **Published — the market object, not the candidate.** The RIN price and its pass-through into wholesale and retail fuels are studied in the peer-reviewed literature (S-134, S-135), and the market's quality, liquidity and transaction costs are documented (S-133). A candidate in this family must be about something the published price literature does not state — the *compliance-deadline* effect, and the state that decides its sign. |
| Dealer balance-sheet constraints as a priced currency-funding spread | **Published, peer-reviewed** (S-096): dealers affected by the U.K. leverage-ratio framework charge about 20 basis points per annum more for synthetic dollar funding. Dealer-level and counterparty-identified, so the state is proprietary. |
| Intermediary leverage as a stochastic discount factor for the cross-section of returns | **Published, peer-reviewed** (S-097). The canonical intermediary-state asset-pricing baseline (R² of 77% on size, book-to-market, momentum and bond portfolios). Any funding-state candidate in any asset class must be measured against it. |
| Trader type and the rate of spot–futures convergence in commodity futures | **Published, peer-reviewed** (S-098): "There is strong evidence that speculators (commodity index traders) increase (reduce) the rate of convergence between spot and futures markets." This is a *component* of IDEA-005's differentiator, not the differentiator itself. |
| Commodity index-trader market share and roll-period returns | **Published, peer-reviewed, and largely null** (S-099): the CIT market share (CIT ÷ open interest) is tested directly as a contributor to commodity returns in roll periods, with risk adjustments, and the reported effect is not significant. This is the closest published test of IDEA-005's state variable and is recorded as **contradicting evidence** against it. |
| Payment-system / CLS settlement deadlines as a price determinant | **Published, peer-reviewed** (S-112): after the introduction of CLS "the value of intraday liquidity has increased during the hours of the CLS settlement cycle", with a structural break at the pay-in schedule and an estimated mark-up of "roughly 1.5bp for the CLS settlement cycle"; the mechanism is "large amounts of reserve balances … transferred during specific time slots". Settlement risk in currency markets is also published (S-082, S-071). **This is a baseline**: any candidate whose mechanism is "settlement deadlines are priced" is re-presenting published work. |
| Securities settlement cycle length as a price-impact and market-quality determinant | **Published, peer-reviewed** (S-113, S-114; plus a preprint in S-115): shortening the cycle *improved* liquidity — US securities became more liquid relative to matched London-listed ones after T+3 → T+2, and T+1 "significantly improved liquidity, measured by bid-ask spreads, Amihud illiquidity and price impact measures". The published sign is the opposite of a harvestable concession, and any candidate in this family must explain that sign. |
| The post-US-close FX window (the T+1 funding window) as a market-quality object | **Documented, institutionally** (S-117, S-118, S-119, S-120): the New York Fed's FX Committee names "NY 4-6pm currency liquidity" as the transition's priority FX risk and records the market's expectation of "an uptick in price premium and market impact for trades executed later in the NY trading day"; the market record is "less than 1% of trades in the $7 trillion OTC FX market" in that window, a half-hour pricing-engine outage at 5pm ET, and "bid/ask spreads widen and liquidity shrinks". **This is a baseline and a cost model, not an opportunity**: a concession that exists only in a sub-1%-of-volume window with widening spreads cannot survive a round trip. |
| EU ETS surrender-month premium (compliance-deadline concession) | **Published** (S-101): purchases concentrate in April, April returns average about 10%, the implied premium is of the order of €5 billion, and operator flow predicts future returns. The *state-conditioned* version is unclaimed but currently untestable (P-008): the aggregate balance is published **after** the pre-2023 deadline it would inform (S-121, G-13), so the decision-time rule has three observations and none in a deficit year. Any future candidate in this family must not present the surrender-month premium as a discovery. |
| Exchange-published maintenance-margin schedules as a liquidity and volatility determinant | **Published** (S-122): margin increases cause hedgers and speculators to reduce open positions and produce "funding liquidity spillovers that affect price impact for all contracts", but "I do not find a significant effect of margin changes on the futures price level", while "realized variance increases by 50% on average on the day of a margin increase". The margin schedule is published by the venue and its setting rule is published too ("2.5 times the daily standard deviation of returns"). **This is a baseline**: the family is studied, and its published effect is on liquidity and volatility, not on the price level. |
| ETF primary-market arbitrage and AP inventory as a driver of ETF mispricing | **Published, institutionally** (S-123): with a regulatory dataset covering the primary and secondary market transactions of 128 ETFs from 2018 to 2022, the FCA finds "a connection between mispricing … and AP's inventory", with "excess AP inventory … widen[ing] discounts". **This is a baseline**, and its dataset is proprietary — the same AP-level data constraint that blocks IDEA-010. |
| Spot-crypto-ETF flow as a channel into the underlying market | **Published, institutionally and as a preprint** (S-124, S-125): the Fed finds crypto ETPs "track NAV less-closely than other ETPs and ETFs" and that the premium reflects segmentation and arbitrage difficulty; the preprint finds that the ETF channels large, uninformed demand into the spot market, "making it busier but shallower", with volume rising "only within U.S. trading hours, when ETF and Authorized Participant activity is concentrated". **This is a baseline**: the creation-flow channel is published, with a *liquidity-deterioration* sign and a published intraday timing pattern. |
| **The disappearing index effect (added in Cycle 13)** | **Published, peer-reviewed** (S-146, *Journal of Finance* 2025). The S&P 500 inclusion effect has collapsed: additions below 1% over the past decade (7.4% in the 1990s), deletions 0.1% between 2010 and 2020, an average inclusion effect of −3 basis points in 2020, and "no apparent relationship between net purchases [by index trackers] and the index inclusion effect, for either additions or deletions". **Any future candidate in the index-reconstitution family must start from this paper and must explain what is left**; the magnitudes are version-dependent between the working-paper and journal versions, so the version must be cited. |
| **Anticipatory liquidity provision at reconstitution (added in Cycle 13)** | **Published as a model and as a documented structure** (S-147, working paper; S-171, preprint; S-151, peer-reviewed). Speculators pre-position, which shifts price pressure away from the effective date; short interest rises on implementation dates and falls afterwards; "apparent front-running reflects competitive liquidity provision and benefits index investors"; and the counterparty to passive demand is the issuing firm. **This is a baseline**: a candidate that trades the pre-announcement anticipation or the post-implementation unwind of reconstitution is presenting published work. |
| **Benchmark-specific passive-asset estimation from reconstitution-day volume (added in Cycle 13)** | **Published, peer-reviewed** (S-148, *Journal of Financial Economics* 2024): the passive ownership share was 33.3% in 2021, roughly double the index-fund-only figure, and the AUM tracking each of the Russell 1000, Russell 2000, S&P 500, S&P MidCap 400 and Nasdaq 100 is inferred from reconstitution-day closing volume for 2000–2021. **This is a method note, not a candidate**: it closes G-02/G-07 as construction questions. |
| **Single-name variance risk premia are frequently zero or positive (added in Cycle 13)** | **Published, peer-reviewed** (S-153, Driessen, Maenhout & Vilkov, *JF* 2009; S-154, Carr & Wu, *RFS* 2009): individual equity options do not embed a negative variance risk premium, single-stock variance swap returns are insignificant, and the negative premium is a large-index phenomenon with correlation risk doing the pricing work. **This forecloses the single-name extension of IDEA-003**; the aggregate version is a baseline (S-014, S-093, S-094) and IDEA-003 must always be described as a state-conditioned refinement of it. |
| **Factor-profitability decay and the crowding/alpha relation (added in Cycle 13)** | **Published, peer-reviewed for the decay** (S-156, *JFQA* 2023: the momentum factor's returns fell from 0.92% to 0.16% per month after mid-2002, with an identified mechanism) and **preprint for the crowding result** (S-172: crowding-based factor selection fails out-of-sample; crowding predicts tail risk rather than average returns). **This is a baseline for any crowding-conditioned candidate**: the base effect must be shown to survive, and the preprint's title has already changed between versions, so the version must be cited. |
| **Crowding inferred from return correlations — "comomentum" (added in Cycle 13)** | **Published, peer-reviewed** (S-157, Lou & Polk, *RFS* 2021): arbitrage-activity intensity is inferable from return correlations, so it is computable from public prices at decision time. **This is a baseline and the object of the new gap G-18**: it is a *different construct* from the holdings-based position-concentration measure (S-026), and the two have never been validated against each other. |
| **Perpetual-futures funding, drawdown mean reversion and the unwind channel (added in Cycle 13)** | **Published** (S-158, working paper: perpetual drawdowns quickly mean-revert while quarterly drawdowns persist, and a higher funding rate attenuates price sensitivity to demand shocks; S-159, *Journal of Empirical Finance* 2026: funding rates have incremental forecasting power for spot volatility because they capture imbalanced leveraged positions vulnerable to subsequent unwinding). **This is a baseline**: IDEA-009's mechanism and mean-reversion are published, and its residual is a dated, signed, exit-specified rule keyed to the funding *level*. |
| **Treasury General Account flows and repo-market stress (added in Cycle 13)** | **Published** (S-160, IMF working paper: TGA flows can create large swings in the repo spread; S-161, S-162, Federal Reserve FEDS Notes: repo-rate sensitivity to Treasury issuance through the SOMA, the ON RRP facility and the TGA, with the public **TGCR − IORB** spread as the decision-time stress measure). **This is a baseline and a cost model**: the funding-state family is published, and what remains open in G-01 is specifically a *dealer-level* funding-value-adjustment series (construct: S-155). |
| **California cap-and-trade price collars, reserve sales and surrender obligations (added in Cycle 13)** | **Published and institutionally documented** (S-163, Bushnell on the price-collar design and the reserve's never having been used; S-164, CARB's Reserve Sale Notice and Annual APCR Notice, including the codified 60%-of-tier trigger, the published tier prices and quantities, the ~30-day notices and the Appendix C schedule; S-174, 17 CCR §§ 95856/95857/95913 — the 1 November, 5:00 p.m. Pacific surrender deadline and the four-times untimely-surrender penalty; S-165, CRS R48314 on prices and compliance; S-168, *AER* 2019 on the collar's design; S-173, CBO 2010 on reserve mechanics). **This is a baseline and a template**: the state is published, the obligation is punitive, and yet the price-insensitive demand is satisfied in advance and the reserve never opens — which is why no candidate emerged from the screen and why the register's own cap-and-trade candidates must state how their state makes the deadline demand *tight*. |
| **Accelerated share repurchases (added in Cycle 13)** | **Published, peer-reviewed** (S-166, Erickson, Fang & Howe, *JFE* 2011; S-167, Guéant, Pu & Royer, *IJTAF* 2015: the ASR is an Asian option with Bermudan exercise dates and the intermediary's problem is optimal execution with market impact). **This is a baseline**: the mechanism, the pricing and the announcement effects are published, and the discount is private-contract data. |
| **Crypto token unlock schedules and their price effects (added in Cycle 13)** | **Published by an interested party, not peer-reviewed** (S-170: a market maker's study of more than 16,000 unlock events reports roughly 90% followed by negative price pressure, with the decline typically starting about 30 days before the unlock and stabilising within about two weeks after, and team unlocks the most disruptive). **This is a baseline and a rediscovery guard**: the schedule is published and the sign and window are already stated publicly, and there is no published state that says whether recipients will sell. |
| **The closing-auction passive execution convention (added in Cycle 13)** | **Documented institutionally and published** (S-149, the index manager's own statement that index funds and ETFs are structurally incentivised to execute in the closing auction because NAVs are struck on closing prices, with Market-on-Close orders dominant; S-150, closing-auction volume at roughly 4–10% of ADV, lower price impact than in the continuous market, and a significant association with passive creation/redemption activity; S-148, passive rebalancing executed at the closing price on reconstitution day). **This is a baseline and a cost note**: the convention is settled, so any candidate that needs a *different* execution convention must justify why the passive does not trade at the close. |
| **State-conditioned variance risk premium harvesting (added in Cycle 30)** | **Published, peer-reviewed** (S-180, Konstantinidi & Skiadopoulos, *Journal of Banking & Finance* 2016): the variance risk premium's time variation is predictable from decision-time state variables, and volatility-trading strategies that condition on those states **outperform buy-and-hold and the naive short-volatility strategy even after transaction costs**. **This is a baseline**: IDEA-003 must always be described as an incremental variant of published conditional-VRP work whose residual is the *state construction* and the *sign* claim, never as a discovery of state-conditioned harvesting. |
| **The variance risk premium as a crash-conditional tail premium, and the premium's measurement convention (added in Cycle 30)** | **Published as a preprint, author-reported** (S-181): the premium is characterised as "a downside, crash-conditional risk premium, compensation for a systematic tail rather than harvestable carry", with the regime-average premium positive in every crisis and widening in high-stress and high-credit-spread states, and an "irreducible left tail" even voltargeted and overlaid. **This is a baseline and a convention warning**: that paper measures the premium as implied minus *subsequently realized* variance, while the candidate's claim is about the *expected* premium, and the two can move in opposite directions in the same state. Any future candidate or specification that conditions on a measured premium must name its convention ex ante. |
| **10b5-1 plans: the rule, the disclosure regime and the plan-timing price effects (added in Cycle 30)** | **Published law plus a regulator's own literature review** (S-182, the SEC's 2022 final rule, 87 FR 80362 — Item 408(a) quarterly disclosure, the mandatory cooling-off period, the Form 4 plan checkbox and the ban on overlapping plans; S-183, the SEC's 2022 proposed release, 87 FR 8686 — the agency's account of the academic evidence that plan **adoption** around earnings announcements carries abnormal returns of roughly −2% to −3% while sales after the announcement do not). **This is a baseline and a rediscovery guard for IDEA-015**: the rule and the state are published law, and the nearest published price effect is attached to the adoption window, not to the execution of a disclosed schedule. |
| **Statutory payment-date Treasury cash drains in the funding market (added in Cycle 30)** | **Published** (S-160, S-161, S-162 — the TGA → repo-spread channel, with the public **TGCR − IORB** spread as the decision-time stress measure). **This is a baseline and a cost model**; the register's family screen in Cycle 30 produced the bounded negative **R-012** on the cross-asset extension, because the payment dates are known by statute and no published state isolates the payment due at the decision date. |
| **The expected variance risk premium, its conventions, and its sign in bad states (added in Cycle 32)** | **Published, peer-reviewed, and now the register's binding constraint on IDEA-003** (S-190, *Journal of Econometrics* 2020; S-191, *Annual Review of Financial Economics* 2018; S-192, *Review of Finance* 2023; S-193, *Management Science* 2021). The expected premium (risk-neutral minus physical conditional expectation) is **positive**, and it is **higher** in bad states: "the continuous component of the VRP … is systematically positive and is higher in periods of market turmoil" (S-190); "the variance risk premium is positive … high variance risk premiums coincide with the left tail of the consumption growth distribution shifting down" (S-192). The *negative* readings of the premium in stress belong to the **naive ex-post** estimator, which "systematically becomes negative, rather than largely positive, in periods of market distress" because it ignores the latent conditional structure (S-190). The only published sign-flip in a variance-premium quantity in distress is in the **term** premium (the term structure turns upward-sloping, S-193). **This is a baseline and a rediscovery guard:** any future candidate that claims an expected-premium sign flip in a crash state must explain S-190 and S-192, and any specification must name its convention ex ante. |
| **Authorized-participant regulatory capital ratios as the operative ETF-arbitrage state (added in Cycle 32)** | **Published, peer-reviewed** (S-194, *Journal of Banking & Finance* 2025). APs' **regulatory capital ratios, disclosed in SEC regulatory filings**, govern ETF arbitrage intensity and ETF premia; the effect is material (0.69pp vs 0.39pp decline in arbitrage intensity between 25th- and 75th-percentile APs in the March 2020 dash-for-cash) and other AP characteristics do not matter. The mechanism is S-195 (working paper, **proprietary datasets**) and the published rivals are S-196 (fractional baskets), S-197 (funding segmentation) and S-199 (client-sourced liquidity discounts). **This is a baseline and a state note:** the AP capital ratio is a *public* state that is already validated against the ETF-premium relation, so IDEA-010 must be described as a trade specification and cost-floor test on a published relation, never as a discovery of the relation. |
| **The RFS volume requirement is calibrated to the agency's own supply projection, and projected shortfalls are waived rather than bought (added in Cycle 32)** | **Primary regulator material** (S-201, the Set 2 final rule, 91 FR 16388; S-202, 40 CFR 80.1405; S-203, the agency's 2026–2027 standards summary). The annual volume requirement is set so that the agency's **projected** supply meets it, so the projected net obligated position is near zero by construction; where the projection fell short (2025 cellulosic: 1.21 billion gallons projected against a 1.38 billion RIN requirement, "a shortfall of approximately 13 percent") the agency's response was the **waiver** of the volume requirement, not a market purchase. **This is a baseline and a state note:** the projected net obligated position is not a sign-determining state, and the realised one is published only after the deadline. Any future candidate in the RFS family must name a different pre-deadline state. |
| **Debt tender offers and liability-management exercises: the price-insensitive flow at a published deadline (added in Cycle 32)** | **Published, peer-reviewed, plus the rule itself** (S-204, Mann & Powers, *Journal of Banking & Finance* 2006: the tender price averages a 4.75% premium to the pre-tender market price and 82.3% of the issue tenders; S-205, Levy & Shalev, *Journal of Accounting and Economics* 2016: the tender is the price-insensitive, dated repurchase route; S-206, Daniels, Díaz & Ramírez, *Journal of Corporate Finance* 2012: renegotiations cluster before a published clawback deadline; S-207, 17 CFR 240.14e-1, and S-208/S-209 for the offer mechanics). **This is a baseline and a bounded-negative family screen (Cycle 32):** the deadline-clustered, price-insensitive flow is a documented institutional pattern, and the one tradeable implication — buying a bond below a published offer price and tendering it — is a mechanical, published arbitrage rather than an edge, with the residual (the post-deadline capital-structure jump) being a credit event rather than a mechanical reversion. |
| **The EU CBAM certificate purchase obligation (added in Cycle 35)** | **Primary regulator material** (S-227, the Commission's published certificate prices — the weighted average of EUA auction clearing prices, quarterly for 2026 and weekly from 2027; S-228, the definitive-regime guidance, the Q&A and the certificate factsheet — the 50 %-of-embedded-emissions quarter-end holding requirement from 2027, the 30 September annual surrender, sales from 1 February 2027 and the deadline's one revision from 31 May; S-229, the free-allocation phase-out — 97.5 % free allocation in 2026 falling to 0 % in 2034, so the obligation share is 2.5 % in 2026 and 100 % only from 2034; S-230, the loss of authorised-declarant status for non-compliance). **This is a baseline and a bounded-negative family screen (Cycle 35, R-016):** the obligation is a genuine, punitive, dated purchase obligation, but the certificate price is a published deterministic formula off EUA auction prices and the certificate is neither tradable by a third party nor usable for anything but the obligation, so no concession is harvestable; the obligation is near zero by construction in the near term; the obligor is the beneficiary; and CBAM's effect on EU carbon prices is itself published. **Dated re-screen condition:** re-screen when the obligation share is materially larger (the 2029–2030 step to 48.5 % of embedded emissions) **and** the weekly pricing regime has run long enough for authorised declarants' pre-deadline **hedging behaviour in the EUA market** to be observable. |
| **Option-implied crash measures as return predictors and crash forecasters (added in Cycle 35)** | **Published, peer-reviewed** (S-223, Chen & Song, *Journal of Futures Markets* 2025: a hybrid option-implied-variance/realised-moment crash measure with significant predictive power for the expected market return, a markedly different marginal effect in crisis and non-crisis periods, and superior out-of-sample crash-event forecasting when combined with variance risk), alongside the option-implied crash-index and crash-risk-pricing literature. **This is a baseline and the reason IDEA-003 was parked (P-012, G-22):** the published work forecasts crash events, predicts the expected market return and prices crash risk — it does not condition a variance harvest on a crash state, and the measure it uses is not a pure option-surface construct. Any future candidate that layers a crash state on a variance harvest must engage S-223 explicitly. |
| **Crowding as a published first-order conditioning variable (added in Cycle 35)** | **Published, peer-reviewed** (S-222, Chincarini, Lazo-Paz & Moneta, *Journal of Banking & Finance* 2025: crowding measured on Days-ADV over 13F holdings 1980–2021 is positively related to subsequent abnormal returns on well-known anomalies, with anomaly risk-adjusted returns "primarily generated by most (least) crowded stocks for the long-leg (short-leg) portfolio", surviving publication-date controls, and with a published crash-risk channel in which crowding "adds new considerations to limits to arbitrage"), on top of S-026's holdings-based construction and S-157's comomentum. **This is a baseline and a rediscovery guard for IDEA-004:** crowding is no longer a discovery, the published relation is *monotone* where the candidate claims a two-sided gate, and the published crowd is all 13F institutional investors (directional positioning) rather than the candidate's convergence-arbitrage capital — which is why G-04 was restated and G-28 opened. |
| **Ex-dividend date mechanics as a dated, mechanical supply event (added in Cycle 37)** | **A baseline and a rediscovery guard (bounded negative R-017, Cycle-36 screen written for real in Cycle 37).** The ex-dividend price adjustment is an accounting identity executed on a fully published date by the party obliged to execute it; there is no unpriced residual supply and no published state that makes an ex-date tight or loose. Any candidate built on the ex-date would be repackaging arithmetic. |
| **The Rule 201 short-sale price-test circuit breaker (added in Cycle 37)** | **Published, peer-reviewed — a baseline and a bounded-negative family screen (R-018).** The effect a candidate would claim is already published and quantified: comparing stocks on either side of the −10 % threshold in the same hour, the restriction leads to 8 % lower short-sale volume and 35 bps higher daily returns, and those price effects "do not reverse after the restriction is lifted" (S-236). The constraint is also defeasible: after a trigger, short sellers migrate to the options market (put open interest +61 %, put volume +87 %; S-237) at low cost (S-238). The rule's mechanics are published law (S-235). **Any future candidate in this family must start from S-236 and must explain what is left.** |

| **Authorised-participant naming in ETF statutory filings: a crypto- and commodity-trust practice (added in Cycle 40)** | **Primary statutory filings (S-239).** ETF prospectuses that name their authorised participants exist and were read directly: the iShares Bitcoin Trust ETF's Form 424B3 prospectuses name their APs verbatim (five APs in the 9 January 2024 prospectus, nine in April 2024, twelve in August 2024; twelve cash and four in-kind as of 31 July 2025), and the same practice appears in the iShares Ethereum and Staked Ethereum trusts, the Bitcoin Premium Income trust, the WisdomTree, Invesco Galaxy, 21Shares, Morgan Stanley, T. Rowe Price Active Crypto and Ark 21Shares digital-asset trusts, and — in older form — in the iShares commodity trusts, whose prospectuses name market makers and clearing counterparties. **This is a baseline and a state note:** the naming practice is real, dated and verifiable, and it is **confined to the commodity/crypto trust class**; a full-document search found **no corporate-bond ETF naming its APs**. Any candidate that needs an ETF → authorised-participant mapping must state which route it uses, and must not assume that a corporate-bond ETF discloses one. |
| **The short-interest branch of the crowding literature (added in Cycle 40)** | **Published, peer-reviewed (plus one working paper)** — S-241 (Mitchell, Pulvino & Stafford, *Journal of Finance* 2004: short interest is the published measure of merger-arb short selling, with its price-pressure effect), S-242 (Hanson & Sunderam, *Review of Financial Studies* 2014: short interest as a published crowding measure of arbitrage capital, whose limits bind when crowding is high) and S-243 (Chan & Tan, SSRN 2020, working paper: daily short interest infers near-real-time crowding of quantitative long-short strategies). **This is a baseline and a rediscovery guard for IDEA-004:** the register's published-neighbour inventory for the convergence-crowd candidate was incomplete without this branch, and the candidate may not present a short-interest-based convergence-activity measure as a discovery. These measures identify **style** arbitrage capital, not the pair/merger-spread convergence crowd, and their published relation is monotone where the candidate claims a two-sided gate. |
| **Eligibility switches: regulatory and provider changes in *who may hold* (added in Cycle 40)** | **Primary regulator material plus a bounded-negative family screen (R-020).** The instances are the SEC's accredited-investor and qualified-institutional-buyer definition amendment (S-244: Release 33-10824, 85 FR 64234, effective 8 December 2020; the $1 million net-worth, $200,000 income and $100 million QIB thresholds are published) and index-provider eligibility and float screens. **This is a baseline and a bounded-negative family screen (Cycle 40, R-020):** the switch is published in advance so any flow is anticipated (and the nearest published analogue finds the effect collapsed to approximately zero and shifted away from the effective date — S-146, S-147); the constrained flow is the obligor's own, so there is no third-party concession to harvest (S-151); each holder's distance to its own limit is private, so the state would be a construction; and the effective sample is the number of switches, not securities × dates. **Dated re-screen condition:** re-screen only if a change arrives with a published list of affected securities *and* a published distance-to-limit measure for each affected holder. |

---

## Rediscovery guard

Before adding any candidate, check it against (a) the fifteen dossiers in `idea_register.md`,
(b) the baseline table above, and (c) the validation hand-offs in `validation_handoffs.md` (**seven of the ten are not executable** — V-001,
V-004, V-005, V-006 and V-007 withdrawn because their candidates were rejected or parked, V-003
marked never-to-execute because IDEA-003 was parked in Cycle 35, and V-002 frozen pending G-28). If the candidate differs from
a baseline only in parameterisation, in label, or in the time frame, it is a variant and belongs in
this log with the baseline named, not in the register. A candidate that differs from a baseline only
in the *state variable* it is conditioned on must still show that the state variable is observable at
decision time — and must show that the conditioning changes the *sign* or the *existence* of the
effect, not merely its size.

**One standing condition added in Cycle 35 (state integrity), and it is a guard on the register's
own bookkeeping, not on candidates.** *No artifact may be described as written, executed, verified
or complete anywhere in this register until the agent has checked that it is present in the artifact
set, and every count and claim in the handoff must be re-derived from the files rather than carried
forward.* In Cycle 35 an audit found that a prior cycle's source-ledger header and handoff had
asserted a set of artifacts — the sources S-210 … S-218, the "Cycle 33 sources" and "Cycle 33 gap
verdicts" blocks, the candidate IDEA-016, the specification V-011, the bounded negative R-014, the
parkings P-012 and P-013 and a formal G-25 verdict — that had **never existed in any file and appear
in no commit in the repository's history**; a note in that same header asserted that the missing
blocks were "the executed record". The register's candidates were not damaged, but its *claims* were,
and a claim that cannot be checked is worse than no claim. The identifiers **IDEA-016, S-210 … S-219,
V-011, G-26 and P-013 are therefore reserved and unused**: they are left unused on purpose so that a
later reconstruction of that missing work cannot collide with new work. The standing practice that
follows: (i) re-derive the state of the register from the files at the **start** of every cycle,
before generating anything; (ii) where a prior claim turns out to be unwritten, either **execute** it
if it is a research question, or **record it as unwritten** — never reconstruct a document by
guessing; and (iii) a *bounded negative* is a legitimate outcome, and an *unwritten artifact* is not
a result.

**Cycle-37 record under the standing condition.** The Cycle-36 handoff asserted "one new family
screen logged as a bounded negative"; the screen existed in the cycle log but had **no entry, no
identifier and no verdict in this file**. Cycle 37 wrote it as **R-017** — a screen that had genuinely
been executed, so it was written for real rather than reconstructed — and corrected this log's own
stale header counts (which still read "Cycle 6 complete … 10 rejections, 10 parkings, 34-row
known-baseline table" while the file actually held 16 rejections, 12 parkings and 57 baseline rows;
it now reads 18, 12 and 59). A second, larger instance of the same failure was found and repaired in
the same cycle, in the *source ledger* and the *candidate dossier*: Cycle 36's central negative claim
about IDEA-010's state availability ("broker-dealer firm-level regulatory capital ratios are not
publicly available") was recorded without a check against EDGAR, and Cycle 37's check showed it to be
**false** — the state is public (S-231). The lesson generalises: **a negative recorded without an
executed check is a claim, not a result**, and a negative about *data availability* must be tested at
the level at which the data would actually be used — the filing, not the dataset.

**One standing condition added in Cycle 13 (after R-011), and it is the most important entry in
this guard.** *Before a candidate is written, its nearest published test must be re-read in the
post-2010 sample.* The register's rank-1 candidate survived six cycles of screening because its
literature had been read only up to 2023; the 2025 *Journal of Finance* paper (S-146) then showed
that the effect it trades had collapsed to approximately zero and that its stated differentiator
had a published null. The failure was not in the screening logic — G-13 and G-12 were applied
correctly — but in the *age of the evidence base*. Therefore: (i) every candidate must carry a
**dated evidence-currency check**, and (ii) a candidate whose base effect is documented as decayed
(S-146, S-156, S-033) must show that the *conditioned* effect survives where the base has not, or
be parked. The register also now keeps two version-drift warnings on file (S-152, whose published
and working-paper versions carry opposite signs, and S-172, whose title changed between versions):
**a number quoted from a working paper must be cited with its version.**

**Three standing screening conditions added in Cycle 5** (they are now part of the guard, not
advice):

1. **G-12 — the conditioning must change the sign or the existence of the effect.** A published
   effect conditioned on a published state is a baseline re-description unless the conditioning
   flips the sign or creates/destroys the effect. IDEA-007 and IDEA-013 both failed this test in
   different ways, and both are recorded so the failure is not repeated.
2. **G-13 — the state must be published *before* the decision.** An official state published on a
   calendar that runs after the decision it informs (the EU ETS aggregate balance before 2024,
   S-121) supports an explanatory decomposition but never a decision-time rule. Every candidate must
   record, per observation, the state's publication date relative to the decision date.
3. **The literature-closure rule, applied symmetrically.** If a published paper already shows the
   candidate's effect, the candidate is **rejected, not narrowed** — this is the rule IDEA-006 and
   IDEA-012 set for themselves and the rule that closed both of them (R-009, R-010). A residual
   survives only if it is (a) genuinely untested, (b) testable with the data that exist, and
   (c) large enough to survive the cost structure of the venue in which it would be traded.

**Cycle 6 — the two screens are now applied to every candidate, and a fourth condition was added.**

4. **G-13 and G-12 are run as a screen on every active candidate before it is ranked**, and their
   results are recorded per candidate in `idea_register.md` and summarised in the source ledger's
   "Cycle-6 verdicts" block. In Cycle 6 the screen **parked two candidates** (IDEA-005 on G-12,
   IDEA-008 on G-13) and re-scored one (IDEA-010, 68.0 → 65.0). A candidate that fails either
   screen is re-scored or parked; it is not left in the active ranking with the failure noted.
5. **New standing condition — a failed G-13 with a *dated* future publication calendar is a
   parking with an unblocking date, not a rejection** (IDEA-008: the lending-rate state is not
   publicly disseminated until 29 March 2029 — S-126 — so the candidate is parked as P-010 with the
   unblocking condition recorded as gap G-14). The complementary case is recorded too: a G-12
   failure where the *closest published test of the candidate's own state variable is null* is a
   parking, not a rejection, because nothing published shows the candidate's effect (IDEA-005:
   S-099). **A rejection still requires a published result that shows the effect** — that remains
   the rule that produced R-007, R-009 and R-010.
6. **New standing condition — a candidate that differs from a published baseline only by a state
   variable, and whose differentiating state is *commercial*, is retained only with an explicit
   validation precondition** (IDEA-010: the published substitutes for AP balance-sheet stress are
   different constructs and have not been validated against a dealer-balance-sheet measure, gap
   G-16). Re-specifying around an unvalidated proxy is not permitted, and no validation
   specification may be written for such a candidate until the validation is done.


### R-015 — New mechanism family screen (Cycle 34)
- **Screen conducted:** one new mechanism family screening per Cycle 34 priorities (Priority 5).
- **Outcome:** bounded negative. No new candidate met the register's bar (published decision-time state, dated price-insensitive flow, unclaimed sign, no published result showing the effect).
- **Rationale:** examined multiple potential families (e.g., treasury refunding announcements, CDS index roll dates, corporate bond maturity walls, SPAC combination deadlines, FTSE/index rebalancing effects beyond those already covered). None possessed a clear signed pre-decision state that differs meaningfully from existing known baselines. Most were either already covered by existing literature/baselines or failed the "price-insensitive flow with unclaimed sign" criterion.
- **Decision:** log bounded negative (R-015). No new dossier created. No score change.

### R-014 — Crypto token-unlock schedule as a dated, price-insensitive supply flow (Cycle 35 family screen — bounded negative; written for real)
- **Why this entry exists.** The Cycle-33 source-ledger header and the Cycle-34 handoff both asserted
  that a crypto-unlock family screen had been executed and logged as **R-014**. It had not: no entry,
  no verdict and no source existed in any artifact. Cycle 35 executed the screen and wrote the result.
- **Screen conducted.** Token unlock schedules — project, team, foundation and investor allocations
  whose vesting cliffs expire on published dates — as a **dated, pre-announced, price-insensitive supply
  flow** with an unclaimed sign and a state that is published before the event.
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale.**
  1. **The channel is already documented, not unclaimed.** The register's own corpus holds the
     Cycle-13 unlock event study (S-170): across more than 16,000 unlock events, roughly 90 % were
     followed by negative price pressure, prices typically begin declining about 30 days *before* the
     unlock, team unlocks were the most disruptive, and the move stabilises within roughly two weeks
     after. A dated supply whose price effect is already published, in a signed direction, with a
     published pre-event window, is a baseline by the register's rule ("a candidate that merely
     repackages a known idea is not a candidate"). Cycle 35's screen reproduced that verdict and added
     nothing that could un-claim it.
  2. **The state is commercial, not regulated.** Unlock schedules are compiled and distributed by
     third-party trackers, not by the issuer, an exchange or a regulator. The register's data rule
     requires a published, reproducible state from a primary source; a vendor's calendar is a
     commercial dataset whose coverage, revision policy and definitions are not auditable, and the
     register's own standing condition (added in Cycle 30 for IDEA-010) is that a candidate whose
     differentiating state is *commercial* is retained only with an explicit validation precondition
     and may not be re-specified around an unvalidated proxy.
  3. **The obligor population is anonymous and the flow cannot be sized in advance.** The recipients
     of an unlock are wallet addresses, and their intent to sell is not observable; no pre-event
     measure of "scheduled supply about to be absorbed" can be constructed that is not a restatement of
     the schedule itself.
  4. **Venue risk is inherited and unresolved.** The register's surviving crypto candidate
     (IDEA-009 PERP-FUND, 60.0) already carries an unresolved crypto-venue risk condition; a second
     crypto family would inherit that operational risk without adding a signed, published state.
- **Decision:** bounded negative (R-014). The token-unlock channel is recorded in the known-baseline
  set; no dossier was created; no IDEA identifier was consumed; no score changed.

### R-016 — The EU CBAM certificate purchase obligation as a dated, mandatory compliance flow (Cycle 35 family screen — bounded negative)
- **Screen conducted.** The EU Carbon Border Adjustment Mechanism's **mandatory certificate purchase
  obligation** — importers of CBAM goods (iron and steel, aluminium, cement, fertilisers, electricity
  and hydrogen) must hold certificates for a share of embedded emissions at each quarter end from 2027
  and must surrender them by 30 September each year, the annual deadline having been moved once, from
  31 May (Regulation (EU) 2025/2083, in force 20 October 2025) — as a dated, mandatory, price-insensitive
  flow with a published pre-deadline signed state. The family was screened because it is the closest
  thing the register has not yet covered to the register's own **compliance-deadline concession**
  template, and because IDEA-013 (EU ETS) and IDEA-014 (RIN) are both parked or retired — so the
  template needed a *third* market with a *different regulator* (the European Commission) and a
  *different obligor population* (importers rather than fuel producers) before the template could be
  declared exhausted.
- **Outcome: bounded negative. No new candidate; the family is a baseline with a dated re-screen
  condition.**
- **Rationale — five independent reasons, any one of which is sufficient.**
  1. **The flow is not into a tradable market and the concession is not harvestable.** The certificate
     price is a *published deterministic formula* — the weighted average of EUA auction clearing
     prices (S-227) — and the certificate is sold only by the Commission to authorised declarants on
     the common central platform and can be used only to discharge the CBAM obligation. A third party
     cannot buy the certificate, so no participant can capture a concession; and the declarant
     receives a certificate, not an allowance, so certificate sales do not consume EUAs and create no
     EUA demand.
  2. **The would-be sign-determining "state" is a definition, not a state.** Because the certificate
     price is a *lagged average* of EUA auction prices, any gap between the certificate price and the
     spot EUA price is an artefact of the formula. Declarants can time purchases within the window
     (weekly prices from 2027, sales from 1 February 2027), so the gap is arbitraged by the obligor
     rather than being a price. There is no state that decides the sign of a harvestable effect.
  3. **The obligation is near zero by construction in the near term.** The share of embedded emissions
     that generates a certificate obligation is the complement of the free-allocation factor: **2.5 % in
     2026**, 5 % in 2027, 10 % in 2028, 22.5 % in 2029, 48.5 % in 2030 and 100 % only from 2034
     (S-229; the Directive's "CBAM factor" is the *retention* factor — 97.5 % in 2026 — and the
     obligation share is its complement; the two conventions must not be confused). This is the same
     "near zero by construction" structure the register already closed against IDEA-014's RIN state
     (G-20), so the near-term flow is immaterial against EU allowance turnover.
  4. **The constraint is real but captive.** An authorised declarant that fails to hold the required
     certificates risks loss of its authorised-declarant status for serious or repeated infringement
     (S-230), so the family does pass the register's "participant and constraint" test. The party that
     would capture any concession is that obligor, not a participant the register could act as.
  5. **The macro channel is an already-published baseline.** CBAM's effect on EU carbon prices, on
     trade and on competitiveness is a large and growing published and policy literature, including the
     Commission's own materials and the European Parliament's briefing at S-229. A candidate claiming
     "CBAM moves EUA prices" would be presenting a published baseline.
- **Dated re-screen condition (so the negative is not permanent).** Re-screen the family when **both**
  hold: (i) the obligation share has grown materially — the 2029–2030 step to 48.5 % of embedded
  emissions (S-229); and (ii) the weekly pricing regime has been running long enough for the
  **pre-deadline hedging behaviour of authorised declarants in the EUA market** to be observable, i.e.
  published evidence of *how* declarants hedge a certificate obligation priced off EUAs and with what
  timing. That residue — obligor behaviour, not a regulatory-calendar fact — is the only part of the
  family that could carry a sign.
- **Decision:** bounded negative (R-016). The CBAM certificate family is recorded in the
  known-baseline set with the dated re-screen condition above; no dossier was created; no IDEA
  identifier was consumed; no score changed.

### R-017 — Ex-dividend date mechanics as a dated, mechanical supply event (Cycle 36 family screen — bounded negative; written for real in Cycle 37)
- **Why this entry exists.** Cycle 36 ran a family screen on **ex-dividend date mechanics** and recorded
  a bounded negative in the cycle log and in the Cycle-36 handoff ("one new family screen logged as a
  bounded negative"). No entry, no identifier and no verdict were ever written into this file, so the
  screen existed only as prose. That is the state-integrity failure this log's standing condition was
  written to stop: a negative that cannot be found cannot prevent rediscovery. Cycle 37 assigns the
  chronologically next free identifier, **R-017**, and writes the entry for real.
- **Screen conducted.** The **ex-dividend date** as a dated, pre-announced, price-insensitive supply
  event: on a published ex-date the entitlement to the dividend separates from the share, the
  reference price adjusts, and any index member or exchange-traded fund obliged to track that index
  must trade the adjustment through on the date.
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale.**
  1. **The event is an accounting identity, not a concession.** The ex-dividend price adjustment is
     mechanical: the entitlement transfers from the seller to the holder on a date whose every element
     is published in advance. A trade that buys the adjustment is buying arithmetic; any measured
     effect would be the reversion of a known, published adjustment rather than the compensation of
     an unpriced risk.
  2. **The flow is executed by the party that is obliged to execute it.** The adjusting trade is
     required of the index member or the fund, not offered by a participant the register could act
     as, so there is no residual supply to harvest — the same structural reason that closed the CBAM
     certificate family (R-016) and the EU ETS instance.
  3. **The state is fully published and fully anticipated.** The dividend amount and the ex-date are
     public before the decision, and the rule's published state is not a *signed* state: it says when
     the adjustment happens, not whether the adjusting buyer is unusually eager or unusually
     constrained on that date. No published state distinguishes a tight from a loose ex-date, so
     there is no state-conditioned claim to make.
  4. **The family is already inside the register's baseline set in substance.** The register's
     closing-auction and index-mechanics rows (S-149, S-150, S-148) and the index-inclusion row
     (S-001 … S-004) already record that passive execution and index mechanics are documented
     institutional facts rather than discoveries.
- **Sources.** None were added. This entry asserts no external claim beyond the mechanical character
  of the ex-dividend price adjustment and the structural fact that the adjusting trade is obligatory;
  it is filed as a baseline and a rediscovery guard, and it does not rest on a literature finding.
- **Decision:** bounded negative (R-017). The ex-dividend family is recorded in the known-baseline
  set; no dossier was created; no `IDEA-` identifier was consumed; no score changed.

### R-018 — The Rule 201 short-sale price-test circuit breaker as a regulatory seller-disabling switch (Cycle 37 family screen — bounded negative)
- **Screen conducted.** **SEC Rule 201 of Regulation SHO** — the "alternative uptick rule". The rule is
  a genuinely different template from the compliance-deadline family the register has been
  exhausting: it is **not** an obligation converging on a calendar date. It is a **regulatory switch
  that disables a seller**, triggered in real time by a published and observable threshold (a decline
  of 10 % or more from the prior day's closing price), and it stays in force for a published and
  bounded duration (the remainder of the trigger day and the following trading day), with the
  short-sale price test requiring short orders to be placed above the national best bid (S-235).
- **Outcome: bounded negative. No new candidate; the family is a baseline.**
- **Rationale — four independent reasons, any one of which is sufficient.**
  1. **The effect is published, peer-reviewed and positive — it is the claim a candidate would make.**
     Barardehi, Bird, Karolyi and Ruchti (2025, *Management Science*) test precisely the proposition
     that short-sale restrictions raise prices, using quasi-experimental variation from the −10 %
     threshold: the restriction "leads to 8% lower short-sale volume and 35 bps higher daily
     returns", and "these price effects do not reverse after the restriction is lifted" (S-236).
     A candidate trading the trigger would be trading a published, quantified result. The register's
     G-12 rule requires an **unclaimed** sign; here the sign is claimed, sized and peer-reviewed.
  2. **The constraint is defeasible by the seller it constrains.** After a trigger, short sellers
     migrate to the options market: put option open interest rises 61 % and put trading volume 87 %,
     with call open interest up 40 % and call volume up 80 % (S-237), and the circumvention is
     documented as low-cost (S-238). The mechanism a candidate would need — a binding constraint on
     the marginal seller's ability to press the price — is therefore only partly binding.
  3. **The trigger is an information event, and the identification has to be separated from it.** A
     10 % single-day decline is overwhelmingly news-driven. The published design compares stocks on
     either side of the threshold *in the same hour* (S-236); a tradeable form of the claim — buy
     after the trigger — is exposed to the news that produced the trigger, which dominates the risk
     in exactly those names. The 35 bp figure is a threshold-contrast estimate, not a captureable
     post-trigger return, and the working paper itself observes that the restricted short-selling
     opportunities "are transient in nature".
  4. **The cost floor is severe in the affected universe.** The affected names are those that moved
     10 % in a session: the widest spreads, the largest gaps, the highest borrow costs and the most
     borrow recalls. A 35 bp daily difference does not survive a round trip in that universe. (The
     published result finds *narrower* spreads under the restriction itself, so this objection is
     about entering at the trigger, not about the restriction.)
- **What is *not* the reason.** The state is public, real-time and published in the rule, so G-13
  (decision-time availability) **passes**; and the register's own discipline was applied: the screen
  was run against the literature before any conclusion, and the literature was found to be
  peer-reviewed, positive and directly on point.
- **Dated re-screen condition.** Re-screen only if (i) the SEC materially changes the trigger
  threshold or the scope of the restriction; or (ii) a published study identifies a residual that
  survives the threshold-contrast design — for example an asymmetry around the **expiry** of the
  restriction at the end of the following trading day that is not already covered by S-236's finding
  that the price effects do not reverse after the restriction is lifted.
- **Decision:** bounded negative (R-018). The Rule 201 family is recorded in the known-baseline set;
  no dossier was created; no `IDEA-` identifier was consumed; no score changed.

### R-019 — The Rule 10b-18 buyback repurchase cap (rate-limited price-insensitive demand) (Cycle 38 family screen — bounded negative)

> **Merge note (Cycle 40).** This file carried **two** entries under the identifier R-019 — a short one and a
> longer one, both describing the same screen. They are merged here into a single entry; the longer text is
> retained and the short text's distinctive points are folded into it. One identifier, one entry.

- **The family screened.** Rule 10b-18's safe harbour for issuer repurchases limits the volume of shares an issuer may repurchase in a single day to the greater of 25% of the average daily trading volume for the four calendar weeks preceding the week of the repurchase, or the issuer's average daily volume for the same four-week period — a **daily** capacity cap (not monthly) that makes an issuer's own buyback demand *rate-limited* and deferred across days.
- **Why no candidate.**
  1. **The constrained flow is the issuer's own flow, not a third-party's.** The template the register seeks is a deadline-driven constraint on *another participant* (arbitrageur/liquidity provider) that creates a harvestable concession. Rule 10b-18 constrains the issuer's repurchase volume; in the standard mechanism this is a limit on the issuer supplying liquidity to the market, not a deadline forcing a third party to trade at a concession.
  2. **Remaining capacity is not published with a clean decision-time granularity.** Issuers are not required to publish their remaining 10b-18 capacity intraday or even daily in a central public feed. The 10b-18 repurchase tables appear in periodic reports (10-Q/10-K) and typically disclose total repurchases over periods, not a continuous remaining capacity series. No 10b-18 source existed in the ledger and the state is not a decision-time published state suitable for the register's rule.
  3. **The mechanism is price-sensitive and literature-dense.** Buyback literature studies price impact and signaling; the safe-harbour cap is a legal/volume constraint, not a published deadline switch that disables a participant at a specific time with an unclaimed sign. Existing literature addresses whether buybacks push prices and the signaling channel rather than a rate-limited third-party concession template.
  4. **No unclaimed sign or clean separation.** Establishing that the cap binds on a given day and produces a concession to a third party requires identifying binding episodes from sparse public data and separating from price-sensitive execution. The bar (published decision-time state, dated price-insensitive flow, unclaimed sign) is not met.

- **Verdict: bounded negative — no candidate.** The family is a baseline of rate-limited supply, not the deadline-driven third-party constraint the register screens for. No 10b-18 source added in the main ledger in this cycle; the finding is recorded as a bounded negative. Two further points from the shorter duplicate entry, retained on merge: **no unclaimed sign or clean separation** — establishing that the cap binds on a given day and produces a concession to a third party requires identifying binding episodes from sparse public data and separating them from price-sensitive execution; and the **state is periodic, not decision-time** — issuers are not required to publish remaining 10b-18 capacity intraday or even daily in a central public feed, and the 10b-18 repurchase tables in periodic reports disclose total repurchases over periods rather than a continuous remaining-capacity series.
