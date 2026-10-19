# CYCLE NOTES

## Cycle 1 — 2026-10-19 — first cycle, empty register

**Starting state.** The research area did not exist. The repository contained only the canonical
mission prompt (`research_prompts/systematic_edge_discovery_agent_prompt.txt`), the maintainer
workflow, and the diagnostics ledger. No idea register, no source ledger, no handoff. The prior
worker session produced no repository changes (it terminated on a network timeout with no commits
and no artifacts), so Cycle 1 also established the durable handoff mechanism described in
`next_agent_handoff.md`.

**Scope compliance.** This cycle was theory-only. No backtest, simulation, parameter sweep,
performance calculation, market data download, strategy code, workflow edit, test edit, or job
launch was performed. No external system was modified. The only external action was reading public
web pages to verify citations, which is explicitly permitted ("Read and summarize relevant
literature, market-structure documentation, exchange specifications, public research").

---

## Mandatory task-framing loop (three passes)

The mission prompt requires three deliberate passes before each meaningful research cycle. The
canonical prompt file was **not** modified (mission prompt, continuous-loop step 8).

### Pass 1 — Draft
- **Objective.** Build the first ranked pipeline of candidate systematic trading edges for this
  repository, from an empty register.
- **Key uncertainty.** Whether the pipeline can be made genuinely useful — i.e. whether the first
  cycle can produce candidates that are (a) mechanistically grounded, (b) honestly differentiated
  from published baselines, and (c) specified well enough that an independent validation agent
  could execute them without guessing.
- **Research frontier.** Chosen after inspection: the *institutional intermediation* frontier —
  participants whose balance sheets, mandates, or deadlines create predictable, state-dependent
  demand or supply pressure. Chosen over a momentum/reversal/breakout frontier because the
  operator's stated experience is already in that family, and because a first cycle needs
  mechanisms with published institutional rules attached (provable timing constraints) rather than
  mechanisms inferred from price patterns.
- **Deliverables.** Idea register with complete dossiers; ranked shortlist with the rubric;
  source ledger with verified citations; rejected/parked log; validation hand-off specifications;
  durable handoff for the next session.
- **Scope boundaries.** As per the canonical prompt; the additional self-imposed constraint for
  this cycle was to make every citation verifiable by URL/DOI and to mark every unverified claim as
  an explicit conjecture or source gap.

### Pass 2 — Critique
- **Ambiguity:** "systematic trading edge" could pull the cycle toward either (i) asset-class
  breadth (equities, FX, crypto, futures) or (ii) mechanism breadth. Resolved in favour of
  mechanism breadth in a single market, with asset-class breadth deferred to Cycle 2.
- **Confirmation bias risk:** picking well-trodden literature because it is easy to cite, then
  dressing it as discovery. Mitigation: every dossier carries an explicit "honest classification"
  line, and two of the four candidates were deliberately scored 2/5 on novelty.
- **Novelty inflation:** the index-inclusion effect (IDEA-001) is a 40-year-old published effect.
  Mitigation: it is classified as a documented effect with a conditional refinement, its novelty
  score is the lowest in the register, and the shortlist states explicitly that it is the best
  *test* but the weakest *discovery*.
- **Duplication:** three of the four candidates (IDEA-002, IDEA-004, IDEA-003) risk being
  re-descriptions of known baselines. Mitigation: the baseline table in `rejected_and_parked.md`
  and the "closest known work / what is already known / differentiator" structure in each dossier.
- **Hidden implementation assumptions:** the candidates were checked against the disqualifying
  patterns — no look-ahead, no impossible fills, no zero costs, no survivorship-blind universes.
  IDEA-001's announcement-after-close and effective-close-auction issues and IDEA-004's stale
  crowd proxy were both surfaced rather than assumed away.
- **Data-mining temptation:** IDEA-003's gate and IDEA-004's terciles are exactly the places where
  a validation agent could peek. Mitigation: the validation specifications mandate training/
  selection/holdout separation, frozen thresholds, and an explicit count of variants searched.
- **Wording that could encourage practical validation:** all rule sketches are descriptive and
  non-executable, and every file states the theory-only boundary.

### Pass 3 — Revise and red-team
Final task used for this cycle:
> *Produce the first ranked, theory-only candidate pipeline for the institutional-intermediation
> mechanism family, where each candidate must (i) name a participant and a constraint, (ii) state a
> state variable observable at decision time, (iii) survive an explicit comparison against the
> published baseline it resembles, (iv) carry pre-specified falsification conditions, and (v) be
> accompanied by a validation specification that a separate authorised agent could execute without
> guessing. Every citation must be verifiable; every unverified claim must be labelled as a
> conjecture or a source gap. Rank by the fixed rubric, and hand off the best next theory-only
> task, naming the highest-value unresolved questions, the next mechanism families to investigate,
> and the source gaps to close.*

Red-team of the final task against the forbidden-action list: it does not authorise data acquisition,
backtests, code, metrics, workflow changes, cross-repository work, or any claim that a candidate
has been tested. It explicitly requires source-gap labelling rather than gap-filling by assumption.

---

## What this cycle changed

- Created the `research/` area and the five canonical artifacts plus this file.
- Added 4 dossiers: IDEA-001, IDEA-002, IDEA-003, IDEA-004.
- Added 28 verified sources (S-001 … S-028) and 5 explicit source gaps (G-01 … G-05).
- Added 3 validation hand-off specifications (V-001 … V-003).
- Logged 3 rejections, 4 parkings, and a 9-row known-baseline reference table.
- Established `research/next_agent_handoff.md` as the durable handoff and pointed at it from
  `AGENTS.md` and `research/README.md`.

## What this cycle did **not** do

- It did not test anything. No candidate has any evidence of working, and no number in the
  register is a performance estimate.
- It did not establish the size of passive assets tracking any benchmark (G-02), the current
  index-fund trading convention (G-03), a public funding-state proxy (G-01), a timely crowd-depth
  proxy (G-04), or the post-2010 single-name option structure (G-05).
- It did not touch the workflow, the tests, or the diagnostics ledger.
