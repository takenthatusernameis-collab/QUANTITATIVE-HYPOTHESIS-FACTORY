# RANKED SHORTLIST — CYCLE 1

Scores are a **research-priority heuristic**, not a probability of profit. No numerical probability
of success is attached to any candidate: the retrieved literature offers no defensible, cited base
rate for "ideas of this type that survive out-of-sample validation after costs", so attaching one
would be false precision.

Weighted total = Σ (dimension score × weight) / 5, expressed out of 100.

Rubric weights (fixed by the mission prompt):
Economic mechanism / persistence 25 · Evidence quality and independence 20 · Substantive novelty 15 ·
Falsifiable predictions and clean future test 15 · Resilience to costs, capacity, regime 15 ·
Data availability, simplicity, reproducibility 10.

---

## Table

| Rank | ID | Short name | Mechanism 25 | Evidence 20 | Novelty 15 | Falsifiability 15 | Resilience 15 | Data 10 | **Total /100** | Hard-stop flags |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | IDEA-001 | RECON-FLOW | 4 → 20.0 | 4 → 16.0 | 2 → 6.0 | 5 → 15.0 | 3 → 9.0 | 5 → 10.0 | **76.0** | none |
| 2 | IDEA-004 | SLOWCAP-COND | 5 → 25.0 | 4 → 16.0 | 3 → 9.0 | 3 → 9.0 | 3 → 9.0 | 3 → 6.0 | **74.0** | none (proxy-validity kill condition) |
| 3 | IDEA-003 | VRP-STATE | 4 → 20.0 | 4 → 16.0 | 2 → 6.0 | 4 → 12.0 | 3 → 9.0 | 4 → 8.0 | **71.0** | none (tail-concentration warning) |
| 4 | IDEA-002 | FUNDSTATE | 4 → 20.0 | 3 → 12.0 | 3 → 9.0 | 3 → 9.0 | 3 → 9.0 | 2 → 4.0 | **63.0** | none (feasibility kill condition) |

---

## Rank 1 — IDEA-001 RECON-FLOW (76.0)

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
  addressable gap (G-02).

**Key uncertainties that could change the rank.** If G-03 resolves against the candidate (index
funds no longer trade at the effective close), leg 1 disappears and the score falls toward the
mid-50s. If G-02 cannot be closed, the flow-scaling prediction becomes untestable and the score
falls further. If the effect has been arbitraged away at current passive scale, the candidate is
dead regardless of score.

**Role in the portfolio.** Strongest *first* candidate to validate (cleanest test, published
schedule, cheap falsification), weakest *new* mechanism. It is a good entry point for the pipeline
and a poor engine of discovery.

---

## Rank 2 — IDEA-004 SLOWCAP-COND (74.0)

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

**Key uncertainties that could change the rank.** Prediction 1 turning out monotone-and-negative
collapses the candidate into a known baseline and drops it below IDEA-003. Failure to validate the
proxy against a holdings-based crowding measure (S-026) makes it untestable as specified.

**Role in the portfolio.** Strongest *new-mechanism* candidate. This is where discovery value
sits, and it is the candidate the next cycle should deepen.

---

## Rank 3 — IDEA-003 VRP-STATE (71.0)

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

**Key uncertainties that could change the rank.** The decay of the predictive power that S-013
themselves flag, and the possibility that post-2010 option market structure (0DTE) changed the
mechanism's size or sign (G-05).

---

## Rank 4 — IDEA-002 FUNDSTATE (63.0)

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

**Key uncertainties that could change the rank.** If G-01 cannot be closed in the next cycle, this
candidate should be **parked, not re-specified** — re-specifying it around a weaker proxy would
convert a good idea into a disguised baseline.

---

## Cross-cutting notes for the next cycle

1. **Two state-proxy problems, one pattern.** IDEA-002 (funding state) and IDEA-004 (crowd depth)
   both fail or succeed on whether a *fast, publicly observable* proxy for a latent state can be
   built and validated. A short methodological note on state-proxy construction and validation
   would serve both candidates and is a cheap piece of work.
2. **One candidate is a baseline wearing a new label.** IDEA-001 must be described in every
   downstream artifact as a refinement of a published effect. If a future cycle adds a candidate
   whose only claim is "a known effect with a new name", it belongs in `rejected_and_parked.md`.
3. **Tail concentration is the register's main unhedged risk.** IDEA-003's payoff is concentrated
   in a few events; IDEA-001's leg 2 is exposed to announcement-window news; IDEA-004's left tail
   is a broken anchor. No single candidate is a complete portfolio, and none of them should be
   described as if it were.
4. **No candidate has been tested.** Nothing in this register is evidence that any of these
   hypotheses works, and no number here is a performance estimate.
