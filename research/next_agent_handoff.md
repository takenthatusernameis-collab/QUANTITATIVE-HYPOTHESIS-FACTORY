# DURABLE HANDOFF — NEXT AGENT

**This file is the durable handoff.** Every worker session in this repository must begin by reading
it, then `research/idea_register.md`, `research/ranked_shortlist.md`, and
`research/source_ledger.md`. It is rewritten (not appended to) at the end of each session; the
superseded text is summarised into `research/cycle_notes.md` so the pipeline history survives.

Last updated: 2026-10-19, end of Cycle 1 · Cycle 1 closed · Next cycle: Cycle 2

---

## 1. State of the pipeline

| Item | Status |
| --- | --- |
| Idea register | 4 dossiers (IDEA-001 … IDEA-004) |
| Ranked shortlist | 4 ranked, scored out of 100 (76 / 74 / 71 / 63) |
| Source ledger | 28 verified sources (S-001 … S-028), 5 open source gaps (G-01 … G-05) |
| Validation hand-offs | 3 specifications (V-001 … V-003); IDEA-002 deliberately not specified |
| Rejected / parked | 3 rejected (R-001 … R-003), 4 parked (P-001 … P-004), 9-row baseline table |
| Canonical mission prompt | `research_prompts/systematic_edge_discovery_agent_prompt.txt` — **unchanged, must stay unchanged** |
| Validation performed | **None.** No candidate has been tested; no number here is a performance estimate. |

Cycle 1 was the first cycle: the register was empty and the prior worker session had produced no
artifacts. Cycle 1 established the pipeline, produced the first four candidates, and left the
state described above.

### Candidates in one line each
- **IDEA-001 RECON-FLOW (rank 1, 76)** — announcement-timed, flow-scaled reconstitution pressure
  with a post-effective reversal leg. *Documented effect, conditional refinement.* Best first
  **test**, weakest **discovery**.
- **IDEA-004 SLOWCAP-COND (rank 2, 74)** — convergence trades conditioned on observable crowd
  depth, with a predicted non-monotone relation. Strongest **new mechanism**.
- **IDEA-003 VRP-STATE (rank 3, 71)** — the variance risk premium is crash-state compensation;
  harvest it only behind an ex-ante crash-state gate. *Known baseline, state-conditioned.*
- **IDEA-002 FUNDSTATE (rank 4, 63)** — funding cost as a state variable for flow-driven impact
  asymmetry. Blocked on a proxy (G-01); **park rather than re-specify** if the proxy fails.

---

## 2. Highest-priority unresolved theoretical questions

1. **Is the crowd-depth conditioning in IDEA-004 non-monotone?** Prediction: convergence returns
   are higher at moderate crowding than at low crowding (deviations persist because capital is
   slow) and lower at high crowding (the edge is competed shut), while tail severity rises with
   crowding. If the relation is monotone and negative, IDEA-004 collapses into the known
   "avoid crowded trades" baseline and must be reclassified. This is the single most valuable
   open question in the register.
2. **Does the announcement-to-effective drift in IDEA-001 scale with the size of the required
   passive flow**, rather than with "being in the index"? A quantitative, publicly checkable
   prediction that separates price pressure from anticipation and awareness.
3. **Is the variance risk premium only harvestable outside crash-imminent states**, and can the
   gate be computed from the option surface alone? The gate is the entire content of IDEA-003.
4. **What is a defensible public proxy for a latent state variable in general?** IDEA-002
   (funding state) and IDEA-004 (crowd depth) both live or die on this. A short methodological
   note would serve both, and the pattern of failure may generalise to future candidates.
5. **Does the single-name insurance-demand channel (S-014) still exist after the 2010s change in
   single-name option market structure (G-05)?** Relevant to IDEA-003 and to any future
   derivatives candidate.

---

## 3. Next distinct mechanism families to investigate (not yet in the register)

These are *not* covered by Cycle 1 and are the recommended search space for Cycle 2. They are
suggestions with reasons, not quotas — a cycle that produces one excellent candidate from an
unlisted family is better than four weak ones from these.

1. **Forced and inventory-driven flows in commodities** — participants with a *physical*
   constraint (inventory holders, producers, index funds) whose trades are dated or scheduled.
   The generic carry/premium literature is a baseline; the open boundary is a participant-and-
   constraint mechanism (for example roll-date inventory repositioning by index funds) that is
   distinct from "carry" as such. *Why now:* it leaves listed equities entirely and has a
   naturally dated flow structure to model.
2. **Corporate credit: index and ETF flow against dealer balance-sheet capacity** — the equity
   version of IDEA-002 applied to a market where dealer capacity and mutual-fund flow both
   matter, with the possibility that the credit premium and the flow premium are separable.
   *Why now:* it reuses the funding-state idea in a venue where it has not been tested, and credit
   markets have explicit, dated issuance calendars.
3. **The funding-currency channel in FX** — the *dollar as collateral and funding currency* as a
   mechanism that is distinct from the generic carry premium, with a state-dependent crisis
   behaviour. *Why now:* the operator's crypto/breakout experience does not cover FX, and the
   funding-currency mechanism has a different persistence argument (global dollar balance sheets)
   than the carry premium.
4. **Securities-lending, short-sale constraints and recall-driven forced selling** — a mechanism
   family in which a *borrow* constraint rather than a flow drives the price, and where the
   constraint is observable.
5. **Slow information diffusion with an identifiable event clock** — distinct from Cycle 1's
   attention baseline (S-027): e.g. accounting-recognition timing, index-provider methodology
   changes, or regulatory-implementation dates that produce dated underreaction.

---

## 4. Best next research task (Cycle 2)

> **Open a new mechanism family and produce 2–3 fully specified dossiers in it, at least one of
> which must sit outside listed US equities, in which every candidate names a participant, a binding
> constraint, a decision-time-observable state variable, and a dated or state-dependent flow.**

Concretely, Cycle 2 should:

1. **Choose the frontier** from section 3 (or a better one you can justify). State the choice and
   the reason in `cycle_notes.md` before generating candidates.
2. **Search primary sources** for the *participant and constraint*: venue and regulator
   documentation, index-provider and issuer methodology documents, and primary academic work on
   the mechanism. Verify every citation by URL/DOI exactly as Cycle 1 did (S-001 … S-028 set the
   standard: full reference, link, type, what it supports, caveat, how it was verified).
3. **Write 2–3 dossiers** in the same field structure as `idea_register.md` (the REQUIRED IDEA
   DOSSIER field list in the canonical prompt), each with an explicit **honest classification**
   against the Cycle-1 register and the known-baseline table in `rejected_and_parked.md`.
4. **Red-team and rank** with the fixed rubric, adding the new candidates to
   `ranked_shortlist.md` with per-score justification and hard-stop flags, and re-check the
   Cycle-1 ranks (the new candidates may legitimately displace them).
5. **Add validation hand-off specifications** (V-004 onward) for any new candidate that reaches
   the top three, in the same structure as `validation_handoffs.md`.
6. **Update this handoff** with the new state, the new best next task, and a fresh initial task
   message for the following agent.

**Bounded supporting tasks** (cheap, high value, each closes a named gap — do these *in addition*,
not instead of the new-mechanism work):

- **T1 (G-02):** find and cite a defensible time series of assets tracking the S&P 500 or another
  benchmark. This unblocks the flow-scaling test in IDEA-001 and V-001.
- **T2 (G-03):** determine the current index-fund trading convention at the effective close from
  provider methodology documents (S-008 points to the Index Mathematics Methodology) and fund
  disclosure. If the funds pre-position, IDEA-001's leg 1 must be re-specified or dropped.
- **T3 (G-01, G-04):** one short note each on the feasibility of a public funding-state proxy and
  of a timely crowd-depth proxy, each ending in an explicit verdict (viable / not viable / viable
  only with X). If G-01 is not viable, move IDEA-002 to the rejected log rather than re-specifying
  it on a weaker proxy.
- **T4 (G-05):** characterise the post-2010 change in single-name option market structure and
  whether it plausibly alters the single-name insurance channel.

---

## 5. Operating rules for the next session (unchanged from Cycle 1)

1. **Read this file first.** Then the register, the shortlist, the source ledger, and the rejected
   log before generating anything.
2. **Theory only, absolutely.** No backtests, no data acquisition or processing, no executable
   strategy code, no performance metrics, no parameter sweeps, no jobs, no workflow/test/infra
   edits, no cross-repository work, no trading. If a question can only be answered by running
   something, write the question down and hand it off — that is the correct output, not a failure.
   *Note: the mission prompt permits reading and summarising literature and market-structure
   documentation; that is what source verification is, and it is the only external action taken in
   Cycle 1.*
3. **Do not modify** `research_prompts/systematic_edge_discovery_agent_prompt.txt`.
4. **Preserve prior work.** Add, do not delete or renumber. New IDs: `IDEA-005`+, `S-029`+,
   `V-004`+, `G-06`+, `R-004`+, `P-005`+, and call the next cycle `Cycle 2`.
5. **Never invent a citation.** Every external claim points to a ledger entry; every ledger entry
   records how it was verified. Unverifiable claims are labelled conjectures and become source gaps.
6. **Scores are research priority, not success probability.** No numerical probability of profit.
7. **Update this handoff last**, and keep the initial task message below current and self-contained.

---

## 6. Environment observations (reported, not actioned — outside the agent's scope)

These are maintainer items. The mission prompt forbids the agent from changing workflow files,
tests, credentials or execution infrastructure, so they are recorded here for the operator and
were deliberately not acted on.

- The workflow `.github/workflows/main.yml` references `scripts/controller_progress.py` (used to
  decide whether a session produced meaningful repository progress) and four test modules under
  `tests/`. **None of these exist in the repository.** The most recent completed run recorded in
  `research_state/workflow_run_diagnostics.jsonl` (run id 39263963610, head sha `e3fa662`) failed
  with `file or directory not found: tests/test_controller_progress_accounting.py` and
  `TEST_OUTCOME: failure`.
- Consequence to be aware of: because `scripts/controller_progress.py` is missing, the
  controller's project-progress accounting cannot succeed even when a checkpoint is committed and
  pushed, so a run can report "no meaningful repository change" and exit non-zero despite the work
  being durably persisted. The work itself is still committed by the controller and pushed — check
  `git log` and the remote SHA rather than the job conclusion.
- A workflow-file push is a diagnostics-only activation; the worker loop runs on schedule and on
  `workflow_dispatch`.

---

## 7. Initial task message for the next agent (copy verbatim)

```
You are continuing the theory-only systematic edge discovery pipeline in the
QUANTITATIVE-HYPOTHESIS-FACTORY repository. This is a research-prioritisation
environment only.

1. Read the durable handoff at research/next_agent_handoff.md first, then
   research/idea_register.md, research/ranked_shortlist.md,
   research/source_ledger.md and research/rejected_and_parked.md. Do not
   regenerate what already exists and do not renumber or delete existing IDs.

2. Execute the best next research task stated in section 4 of the handoff:
   open a new mechanism family (section 3 lists the recommended, not yet
   covered families) and produce 2-3 fully specified candidate dossiers in it,
   at least one of them outside listed US equities. Each dossier must name the
   participant, the binding constraint, a decision-time-observable state
   variable, a dated or state-dependent flow, the expected return source, an
   honest originality comparison against the Cycle-1 register and the
   known-baseline table, falsifiable predictions with explicit rejection
   conditions, confounders, data requirements, a theory/evidence status, and
   verified sources. Also close the bounded supporting tasks T1-T4 if time
   allows, and record any gap you cannot close as a new source gap.

3. Apply the three-pass task-framing loop (draft, critique, revise and
   red-team) before the research cycle and record the final framing in
   research/cycle_notes.md. Do not modify the canonical prompt file at
   research_prompts/systematic_edge_discovery_agent_prompt.txt.

4. Rank the new candidates with the fixed rubric in
   research/ranked_shortlist.md, write validation hand-off specifications for
   any new candidate reaching the top three (V-004 onward, same structure as
   research/validation_handoffs.md), and log anything rejected or parked in
   research/rejected_and_parked.md with the reason.

5. Absolute scope boundary: theory and discovery only. Do not run or
   commission backtests, simulations, parameter sweeps, significance tests on
   strategy results or any performance calculation. Do not download or process
   market data, build a research notebook, implement a strategy, write a
   signal generator or any executable research infrastructure, or launch any
   job, workflow or CI run. Do not change workflow files, tests, credentials or
   infrastructure, and do not touch other repositories. You may read public
   literature, venue and regulator documentation, and market-structure
   documentation in order to verify citations. If a question can only be
   answered by running something, document the question precisely and hand it
   off instead of relaxing the boundary.

6. Cite every external claim with a verifiable URL or DOI, and never invent a
   citation. Distinguish authors' reported results from independently
   reproduced results, and label unresolved claims as conjectures. Scores are
   research-priority weights, not probabilities of profit; attach no numerical
   probability of success.

7. Finish by rewriting research/next_agent_handoff.md: current pipeline state,
   the highest-priority unresolved theoretical questions, the next mechanism
   families to investigate, the open source gaps, the best next research task,
   any environment observations for the maintainer, and a fresh, self-contained
   initial task message for the following agent. Summarise the superseded
   handoff into research/cycle_notes.md.
```

---

## 8. Handoff history

| Cycle | Date | Outcome | Handoff closed |
| --- | --- | --- | --- |
| 1 | 2026-10-19 | First cycle: pipeline created, 4 dossiers, 28 sources, 3 validation specs, 3 rejections, 4 parkings, baseline table, durable handoff established. | Yes — this file. |
