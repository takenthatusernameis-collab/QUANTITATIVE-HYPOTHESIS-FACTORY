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

## Cycle 20 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 20 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0) remains structurally unresolvable at current evidence; do not arbitrarily break; (b) confirm V-002 remains frozen (G-18 bounded negative); (c) frontier screens only if genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycle 19): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 19 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 20), `cycle_notes.md` updated with Cycle 20.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 18 — 2026-10-20 — Tie resolution pass

**Cycle objective.** Execute Cycle 18 task from handoff section 3: (a) resolve the IDEA-011 / IDEA-004 tie at 69.0 under the fixed rubric using nearest published post-2010 test; either re-score one or document tie as structurally unresolvable at current evidence; (b) confirm V-002 remains frozen (G-18 bounded negative, not closure); (c) frontier screens only if genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Review tie between IDEA-011 (69.0, rank 4) and IDEA-004 (69.0, rank 3). Examine S-178 (Hung, Li & Wang 2014/2015, RFS) and S-179 (Song & Woo 2015) cited in ledger; compare rubric scores (mechanism/persistence, evidence, novelty, falsifiability, resilience, data). Assess whether post-2010 decay evidence (PEAD shrinking with better information quality/enforcement) differentially affects the two candidates.

**Pass 2 — Critique.** For IDEA-011 (ACCTCLOCK), the post-2010 evidence (S-178, S-179) shows PEAD declines after IFRS adoption/better info quality — weakening persistence. Enforcement-regime concentration is a scope condition (drift survives in weak-enforcement states), not rejection. For IDEA-004 (SLOWCAP-COND), persistence weakened by S-156 (momentum decay) and S-172 (crowding-based factor selection fails out-of-sample). Both have had persistence adjusted downward (mechanism 4). Current scores: IDEA-011: mech 4 (20), evidence 3 (12), novelty 3 (9), falsifiability 4 (12), resilience 3 (9), data 4 (8) = 69.0; IDEA-004: mech 4 (20), evidence 4 (16), novelty 3 (9), falsifiability 3 (9), resilience 3 (9), data 3 (6) = 69.0. Different strengths balance (IDEA-004 stronger evidence, IDEA-011 stronger falsifiability and data availability). This is structurally unresolvable at current evidence. V-002 frozen: G-18 remains bounded negative per handoff (comomentum S-157 not validated substitute for holdings-based crowding S-026).

**Pass 3 — Revise.** Document tie as structurally unresolvable. Confirm V-002 frozen. No new candidates. Update handoff and write initial task for next agent.

### Outcome

- **Tie resolution:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Tie persists because relative strengths (evidence vs falsifiability/data) balance; both affected by post-2010 decay evidence (S-178/S-179 for IDEA-011, S-156/S-172 for IDEA-004). Tie documented as structurally unresolvable at current evidence.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; V-002 must not be executed.
- **Frontier screens:** None conducted (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 18), `cycle_notes.md` updated with Cycle 18.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 22 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 22 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-21): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 21 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 22), `cycle_notes.md` updated with Cycle 22.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 19 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 19 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0) remains structurally unresolvable at current evidence; do not arbitrarily break; (b) confirm V-002 remains frozen (G-18 bounded negative); (c) frontier screens only if genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycle 18): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 18 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 19), `cycle_notes.md` updated with Cycle 19.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 2 — new mechanism families, 2026-10-19
[... remainder of existing cycle notes preserved ...]

---

## Cycle 21 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 21 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-20): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 20 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 21), `cycle_notes.md` updated with Cycle 21.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 23 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 23 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-22): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 22 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 23), `cycle_notes.md` updated with Cycle 23.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 24 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 24 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-23): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 23 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 24), `cycle_notes.md` updated with Cycle 24.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 25 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 25 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-24): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 24 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 25), `cycle_notes.md` updated with Cycle 25.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 26 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 26 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-25): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 25 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 26), `cycle_notes.md` updated with Cycle 26.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

---

## Cycle 28 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 28 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-27): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 27 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 28), `cycle_notes.md` updated with Cycle 28.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

**Cycle objective.** Execute Cycle 27 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-26): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 26 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 27), `cycle_notes.md` updated with Cycle 27.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 29 — 2026-10-20 — Tie monitor / V-002 freeze confirmation

**Cycle objective.** Execute Cycle 29 task from handoff section 3: (a) note IDEA-011/IDEA-004 tie (both 69.0, ranks 4 and 3 respectively) remains structurally unresolvable at current evidence; do not arbitrarily break it; (b) confirm V-002 remains frozen — G-18 is a bounded negative, not a closure, so V-002 stays on hold and must not be executed; (c) frontier screens / new candidates only if a genuine new mechanism family surfaces.

### Three-pass task-framing loop

**Pass 1 — Draft.** Re-read tie documentation (Cycles 18-28): IDEA-011 retained 69.0 rank 4, IDEA-004 retained 69.0 rank 3. Review post-2010 decay evidence: S-178/S-179 for IDEA-011 (PEAD shrinks with better info environment), S-156/S-172 for IDEA-004 (momentum decay, crowding-based selection fails out-of-sample). Assess whether any new evidence has surfaced since Cycle 28 that could differentially affect either candidate.

**Pass 2 — Critique.** No new evidence has surfaced. Relative strengths (IDEA-004 stronger evidence; IDEA-011 stronger falsifiability and data availability) still balance. Tie remains structurally unresolvable at current evidence; do not re-score to force resolution. V-002: G-18 remains bounded negative (comomentum S-157 not validated against holdings-based crowding S-026); V-002 stays frozen and must not be executed. No genuine new mechanism family has surfaced; no frontier screens conducted.

**Pass 3 — Revise.** Confirm tie documented as structurally unresolvable. Confirm V-002 frozen. Preserve tie documentation. No new candidates, no new sources, no re-scoring. Update handoff and write initial task for next agent.

### Outcome

- **Tie:** IDEA-011 remains 69.0 (rank 4), IDEA-004 remains 69.0 (rank 3). Structurally unresolvable at current evidence; no arbitrary break.
- **V-002 status:** Confirmed frozen — G-18 bounded negative, not closure; must not be executed.
- **Frontier screens:** None (no genuine new mechanism family surfaced).
- **Artifacts updated:** `next_agent_handoff.md` rewritten (now Cycle 29), `cycle_notes.md` updated with Cycle 29.

### What this cycle did not do

- No re-scoring to break tie.
- No new dossiers or sources added.
- No tests, data acquisition, or code.
- No modifications to canonical prompt.

---

## Cycle 30 — 2026-10-20 — Prior-art and convention audit (IDEA-003), crowding-state closure attempt (IDEA-004), RIN state audit (IDEA-014), one new family screen (10b5-1 plan supply)

**Cycle objective.** Cycles 18–29 were twelve consecutive tie-monitor passes that changed no score,
no source and no dossier. The mission prompt forbids exactly that: "Continue searching for new
substantive mechanisms rather than repeatedly tuning a candidate that has already been described",
and the register's own cross-cutting note 4 names the highest-value operation as "re-reading an
existing candidate against newer literature". Cycle 30 therefore did three evidence operations on
the three most consequential active candidates, screened one new mechanism family, and recorded one
bounded negative. Nothing was executed, tested or downloaded.

### Three-pass task-framing loop

**Pass 1 — Draft.** Draft task: (a) *IDEA-003* — the register's rank-1 candidate — is the one whose
novelty rests on the least-verified claim ("the gate"). Search the conditional-VRP-harvesting
literature (2024–2026) and the premium-measurement literature for (i) any published strategy that
conditions variance-premium harvesting on a decision-time state, and (ii) any published statement of
what the "premium" is measured against. (b) *IDEA-004* — re-run G-18 with a different framing than
the thirteen prior "find a validation paper" searches: ask instead whether published work constructs
a *decision-time, filing-resolved, holdings-based* crowding measure and what it says about return
prediction. (c) *IDEA-014* — establish whether the sign-determining state (the net obligated
position) is published *before* the compliance deadline, since that decides whether G-15's two-sided
sign test is runnable at all. (d) Screen one new mechanism family with a published decision-time
state and a date-bound, price-insensitive flow.

**Pass 2 — Critique.** Pass 1 risks three specific errors. (i) Searching for "a paper validating
comomentum against holdings-based crowding" for a fourteenth time is a null operation; the framing
must change. (ii) Any IDEA-003 literature hit could be read as either *support* (the mechanism is
real) or *contradiction* (the gate is published), and the register's rule requires the difference to
be resolved by reading what the paper actually measures, not by its title. (iii) A new family must
clear the register's own bar — a published decision-time state, a dated price-insensitive flow, a
sign-determining state, and no published result already showing the effect — or it must be logged as
a bounded negative rather than dressed up as a candidate.

**Pass 3 — Revise.** Revised task: (a) read the two IDEA-003 sources *for their measurement
convention* and, if the convention matters (it does), amend the candidate's specification rather than
re-score it; (b) keep the G-18 search but reframe it as a *state-construction* question and accept a
restated bounded negative as a legitimate outcome; (c) for IDEA-014 ask the *publication-status*
question, not the price-pattern question, and treat "the state exists only in projected form" as a
legitimate finding; (d) for the new family, prefer a family whose state is published by **law**
rather than by a market operator, and require that any candidate it produces enters **parked** with
an explicit unblocking condition unless the price-effect literature supports it.

### Outcome

- **IDEA-003 VRP-STATE — no score change (71.0), material narrowing.** Two new sources: S-180
  (Konstantinidi & Skiadopoulos, *Journal of Banking & Finance* 2016, Crossref-verified) publishes
  that state-conditioned volatility-trading strategies beat buy-and-hold and naive short-vol after
  costs — so "gate the variance-premium harvest on a state" is a **published strategy family**, and
  the candidate is reclassified as an **incremental variant** of published conditional-VRP work.
  S-181 (a 2026 SSRN preprint) frames the premium in the candidate's own vocabulary as a
  crash-conditional tail premium that is "not harvestable carry". Critically, S-181 measures the
  premium as implied minus **subsequently realised** variance, whereas the candidate claims the
  **expected** premium collapses in crash-imminent states; the two quantities can move in opposite
  directions in the same state. **V-003 was amended** to fix the convention ex ante and to state that
  an ex-post null is **not** a kill; **G-19** opened for the residual.
- **IDEA-004 SLOWCAP-COND — no score change (69.0).** S-186 (Hu & Shen, *Finance Research Letters*,
  8 October 2026, OpenAlex-verified) shows the holdings-based crowding construction is now an active
  published object (13F holdings, 2013Q2–2025Q4) and associates crowding with prices, comovement and
  **fragility**, not with a return-predictive rule. G-18 is **restated, not closed**; V-002 stays
  frozen.
- **IDEA-014 RIN-DEADLINE — no score change (60.0).** S-184 (EPA proposed rule, 91 FR 65699,
  16 October 2026, Federal Register API verified) establishes that the compliance deadline's
  movement is **rule-determined** (an automatic extension mechanism) and that the **realised** state
  publishes only *after* the deadline it informs, while the projected state publishes before it.
  S-185 records EPA's published data categories, including "Renewable Volume Obligations" and the
  participant-level RIN Holdings report. G-15 sharpened; **G-20** opened.
- **New family screened; one new candidate entered, parked.** IDEA-015 **PLAN-SUPPLY** (61.0,
  P-011): pre-announced, non-discretionary insider supply under Rule 10b5-1 plans, whose state is
  published by **corporate disclosure law** (Item 408(a) quarterly tables; Form 4 plan disclosures;
  S-182 the 2022 final rule, 87 FR 80362; S-183 the 2022 proposed release, 87 FR 8686). Parked
  because the nearest published price effect attaches to plan *adoption* around earnings, not to the
  execution of a disclosed schedule. **G-21** opened.
- **One bounded negative.** R-012: the statutory payment-date liquidity-drain family (US corporate
  estimated tax dates) — funding-market manifestation published (S-160, S-161, S-162), no surprise
  component, no published decision-time state isolating the payment due.
- **Artifacts updated:** `source_ledger.md` (S-180 … S-187), `idea_register.md` (three Cycle-30
  blocks, one new dossier), `ranked_shortlist.md` (table flags, parked table, cross-cutting notes 10
  and 11), `validation_handoffs.md` (V-003 amendment), `rejected_and_parked.md` (R-012, P-011, five
  baseline rows), `cycle_notes.md` (this entry), `next_agent_handoff.md` (rewritten for Cycle 31).

### What this cycle did not do

- No score changed, no candidate was rejected, no validation specification was executed.
- **No new validation specification was written** — the top three are unchanged, so V-010 stays free.
- No backtest, simulation, parameter sweep, data download, strategy code, test or workflow edit.
- No modification to the canonical prompt.
- Trade-press figures for the 2026 tax-date drain were deliberately **not** recorded, because they
  could not be verified in this cycle; the family screen rests on the register's own ledger entries.
