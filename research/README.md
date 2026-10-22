# QUANTITATIVE HYPOTHESIS FACTORY — THEORY-ONLY RESEARCH AREA

This directory holds the durable, theory-only research pipeline for this repository. Nothing in it
is a backtest, a strategy implementation, a performance claim, or a validation result. The scope is
defined by the canonical mission prompt, which is **not** to be modified:

- Mission prompt (canonical, maintainer-owned): `research_prompts/systematic_edge_discovery_agent_prompt.txt`

## Files

| File | Purpose |
| --- | --- |
| `next_agent_handoff.md` | **The durable handoff.** Start every session here. Holds the current task, the open questions, source gaps, and the ready-to-run initial task message for the next agent. |
| `idea_register.md` | Full dossiers for every retained candidate (mechanism, observables, rule sketch, falsifiers, evidence status). |
| `ranked_shortlist.md` | Rubric-scored ranking with hard-stop flags, weights, and per-score justification. |
| `source_ledger.md` | Verified citations (ID, full reference, URL/DOI, what each source supports, verification method, caveats). |
| `validation_handoffs.md` | Theory-to-validation specifications for shortlisted candidates. Specification only — never executed here. |
| `rejected_and_parked.md` | Rejected/parked candidates with reasons, plus the known-baseline list, to prevent rediscovery. |
| `cycle_notes.md` | Cycle log, the mandatory three-pass task-framing loop, and the change history of the artifacts. |

## Working agreements for future sessions

1. **Read `next_agent_handoff.md` first**, then the register and shortlist, before generating anything new.
2. **Preserve prior work.** Add to the register; do not silently delete, relabel, or renumber existing IDs.
3. **ID discipline.** Ideas are `IDEA-0NN` (next free: `IDEA-017`; `IDEA-016` is **reserved and
   unused**),    sources are `S-0NN` (next free: `S-458`; **only** `S-210 … S-219` is
   **reserved and unused** — `S-281 … S-290` are **live entries**, the ten Cycle-58 document-record
   entries, and the corpus is **447 entries of which 446 are verifiable**, S-290 being struck),
    validation specs are `V-0NN` (next free: `V-013`; `V-011` is **reserved and unused**, `V-010` is written
    and marked **never-to-execute**, and `V-012` is written and **executable** — the register's first
    *state-free* specification),    rejections are `R-0NN` (next free: `R-072`), parkings are `P-0NN` (next
    free: `P-015`; `P-013` is **reserved and unused**), source gaps are `G-NN` (next free: `G-39`;
    `G-17` and `G-26` were skipped by the sequence and have never been used), and cycles are `Cycle N`
    (next: **Cycle 142**;
    **Cycle 141 completed three pre-registered priorities and produced no candidate, no new score, no new rank and no new hard-stop flag.** **(i) Priority 1 — the membership-criterion follow-up, with two new mechanical censuses of the coverage map:** the clause-form criterion remains satisfied for **all thirty-four rows** (clause X-1 complete over the entire map — thirty-one probes, twenty-six kills, five rediscoveries, zero survivors, zero fetches); no construction was supplied, so the pre-registered new-construction admission form was not used; **zero fetches**. The **closure-form census** (run for the first time): **twenty-nine of the thirty-four rows name at least one rejection entry** in their "Closed by" cell and **five do not** (B by G-28's structural null; 15 by IDEA-003; 16 by IDEA-005 and IDEA-008 with G-28; 32 and 33 by Cycle 129's recorded batch-2 results). The **citation-column census** (run for the first time): **thirty-three of the thirty-four rows cite at least one known-baseline guard row, and row B was the single exception** — its cell read "—", because row B is closed by a *structural null* rather than by a screen of a published kind and so has no guard row of its own; the register's own rule is **not** violated by it, and **row B's cell was amended in place, additively ("—" → "57, 61")**, so the map's citation column is now **34 of 34** and the map's row count is unchanged at **34**. **(ii) Priority 2 — the "Closed by" correspondence follow-up:** the correspondence was re-derived mechanically in three steps — **all fifty-three identifiers named in the thirty-four "Closed by" cells exist** (forty-one `R-` entries, nine `IDEA-` dossiers, one `G-` gap, two `S-` sources); **every baseline number cited lies within 1 … 111**, the rows citing **eighty-nine distinct** rows; and **the converse holds — the twenty-two baseline rows that no map row cites are all published price-effect baselines or factor families, not closed state kinds**, so the Cycle-136 note's category (iii) remains **empty**; **no new defect of the named class, and no repair made under this priority**. **(iii) Priority 3 — gaps and housekeeping:** no action on G-37 and no action on G-33; G-11, G-14, G-21, G-28, G-30, G-31, G-32 and G-38 tracked and unmoved; no gap opened and no gap closed; counts re-derived from the files — **447 ledger entries (446 verifiable) · 15 dossiers · 71 rejections (R-001…R-071) · 13 parkings (12 active) · 11 validation specifications (V-001…V-010, V-012) · 111 known-baseline rows · 34 coverage-map rows (A–I, 10–34)**; rubric arithmetic re-run clean from the shortlist's own cells — **IDEA-011 69.0 (rank 1), IDEA-004 63.0 (rank 2), IDEA-014 52.0 (rank 3), IDEA-009 42.0 (rank 4), IDEA-010 parked (P-014) at a terminal 55.0**; no cell moved. **Five record repairs were made in place, each with a before/after, none touching a score, a rank, a hard-stop flag, a gap's status, a rejection's verdict or a candidate's status:** the **history chains** of four artifacts — the source ledger, the validation hand-offs, the rejected-and-parked log and the idea register had lost **Cycle 139**, and the ranked shortlist had lost **Cycle 138** — were repaired, each missing summary reproduced from `cycle_notes.md`; the **idea register's newest block was mislabelled** (it read "Cycle 140 complete" while carrying Cycle 138's content) and is relabelled to its true cycle, with the true Cycle 139 and Cycle 140 blocks inserted above it; and the **false claims** — Cycle 139's "All headers brought to Cycle 139 and read back" and the Cycle-140 blocks' "history chains checked (140 → 139 → 138 continuous where written)" — are corrected in place. This is the **thirteenth recorded occurrence of the header-update failure mode**, and the first in which the *chain* was broken as well as the *label*: in Cycles 139 and 140 the labels were advanced without the corresponding content being written. All five artifact headers and newest dated blocks advanced to "Cycle 141 complete" and read back (the chains are now continuous: 141 → 140 → 139 → 138); this README updated; the handoff rewritten for Cycle 142; the standing identifier-integrity check run and passed. **Named constructions 46, candidates 0, fetches 0.**
    **Cycle 137 completed three pre-registered priorities and produced no candidate. The coverage map
    now stands at thirty-four rows (A–I, 10–34), the known-baseline table at 111 rows, the register's
    named-construction count at 45 — and not one of the forty-five has produced a candidate.**
   **(i) Priority 1 — clause X-1, batches 2–4: the near-miss probe of the register's own map.** The
   Cycle-135 handoff's "exit" was executed over **twenty-one rows** — **rows 10 to 33 less the three
   already closed in full** (row 27 in Cycle 128; rows 29 and 30 in Cycle 136) — one **blind**
   near-miss construction per row, **all twenty-one fixed in `cycle_notes.md` before any of the
   twenty-one rows' closing entries was read** (a stricter rule than Cycle 136's per-batch rule, and
   recorded as such), and each screened under the **unchanged** narrowed rule: **sixteen kills, five
   rediscoveries, zero survivors, zero undecided, zero fetches**, and **all twenty-one rows closed in
   full**. The five rediscoveries (**P14, P22, P23, P24, P25**) each reproduced a **specific screened
   instance, branch or class** of the row's own closing entry and are recorded with a **faulted
   selection**; the cause is **structural** — the map's labels for the exhaustively screened rows
   (the record-first and published-measurement screens) **enumerate the forms their closing clauses
   screened**, so a blind probe of such a label cannot land outside the closure. The cycle's three
   findings: **X-1's yield on a family row is confirmation, not a new argument**; **X-1 is not
   executable on an exhaustively screened row when the probe must be written from the map label
   alone**; and **the Cycle-136 membership observation is confirmed as a triage and refused as a
   kill** — it names no clause, and a kill that names no clause is not a kill. **X-1's original scope is
   now complete**: every map row that existed when it was specified has been probed.
   **(ii) Priority 2 — the two findings the Cycle-136 baseline audit handed forward, both repaired.**
   R-065's closed kind ("a dated, published supply-loss notice") **now has a coverage-map row of its
   own — row 34** — so the map's row count moves **33 → 34**; the new row is **not probed** (the batch
   was pre-registered before the repair) and is handed to Cycle 138 as the register's **single
   unprobed map row**. The **R-048** correspondence in map row 17 is repaired by **crediting R-048 in
   row 17's "Closed by" cell** (its fixed-income cash family is a member of row 17's kind) and by
   **completing row 17's baseline citations** (83, 84, 91), so that every entry credited there has its
   guard row cited there. **(iii) Priority 3 — the open gaps and housekeeping:** **no action on G-37
   and no action on G-33** (V-008 and V-009 unamended; IDEA-009 42.0 and IDEA-011 69.0 unchanged);
   G-11, G-14, G-21, G-28, G-32, G-30, G-31 and G-38 tracked and unmoved; **no gap opened or closed**;
   counts re-derived from the files; the rubric arithmetic re-run clean from the shortlist's own cells
   — **no score or rank moved: IDEA-011 69.0 (rank 1), IDEA-004 63.0 (rank 2), IDEA-014 52.0 (rank 3),
   IDEA-009 42.0 (rank 4), IDEA-010 parked (P-014) at a terminal 55.0** — all five artifact headers
   advanced to "Cycle 137 complete" and read back (the three H1 titles that carry a cycle range were
   **stale at "CYCLES 1–135"** and are repaired to "CYCLES 1–137"), this README updated, the handoff
   rewritten for Cycle 138, and the standing identifier-integrity check run and passed. **No candidate,
   no `IDEA-` identifier, no `S-` identifier, no fetch, no score, no rank, no flag, no gap and no
   specification changed; one rejection (R-070), sixteen baseline rows amended in place, one map row
   added, twenty-one map rows closed in full.**

   **Cycle 136 completed three pre-registered priorities — the closure audit of the completed backward
   state inventory, the register's own structural question stated and decided, and housekeeping. The
   audit is the first time the register's largest artifact has been checked as a whole**, under seven
   checks pre-registered with the check set and the repair list both fixed before the first repair:
   **(a) identifier partition — PASS** (the union of the inventory tables' identifier sets is exactly the
   corpus's **447** entry blocks — 437 `### S-NNN` headings plus the ten Cycle-58 document-record entries
   S-281 … S-290 — the eleven batch tables pairwise disjoint and jointly contiguous, and S-001 and S-011
   the only two identifiers in no batch table); **(b) cell-vs-tally agreement — ONE FAIL, repaired** (ten
   of eleven batch outcome lines agree with their own tables; the **Cycle-129 batch-2** line read "33
   in-map … 1 (iv-b)" where its thirty-nine cells give **32 in-map · 2 out-of-map · 3 (iv-a) · 2
   (iv-b)**, because Cycle 134 adjusted the tally for the S-028 cell move but not for the S-021 cell move
   — corrected in place with a before/after, and the corpus figure is unaffected because it was derived
   from the cells); **(c) map resolution — PASS** (every map row named in an in-map cell exists in the map,
   and all 33 rows name their closing entry; **141 of the 294 in-map cells name no map row and resolve by
   family**, an asymmetry inherited from the Cycle-129 batches, recorded and not repaired); **(d) kill
   resolution — PASS** (all six out-of-map cells name a kill by clause or template and a mapping; the
   final state is three out-of-map cells, all killed and mapped); **(e) disagreement completeness — PASS,
   with the check's own premise corrected** (of the four (iv-b) entries, **two are recorded
   disagreements** — S-021 and S-028 — and **two are first readings** with no second reading to record);
   **(f) whole-corpus arithmetic — PASS** (**272 in-map · 168 (iv-a) · 4 (iv-b) · 3 out-of-map = 447**,
   re-derived from the cells); **(g) gap-ledger completeness — ONE FAIL, repaired** (**G-31**, opened in
   Cycle 41 and closed in Cycle 42 with a *not found* verdict on both sub-routes, now written into
   IDEA-010's dossier with its status and its provenance). **Three repairs, each with a before/after, none
   touching a score, a rank, a flag, a gap's status, a rejection's verdict or a candidate's status.**
   Priority 2 **stated the register's own dependency loop formally** (**L ← A ← P ← L**) and **decided**
   it: the loop is **real** — the screen's own adequacy cannot be tested by the screen, because the only
   instrument that can reach a state kind outside the map is the literature and the literature is gated
   behind a survivor of a screen built from the map — but the **epistemic closure** and the **emptiness of
   the productive range** are two different things, and the emptiness is **not** caused by the loop, since
   the map grew 21 → 24 → 28 → 33 **because of** the constructions and all **fifteen named constructions**
   across R-063 … R-068 were killed at the design stage by a **named clause** at a cost of **zero
   fetches**. **The method is total in form and empty in content**, and the binding constraint is the
   **supply of constructions** — both of the register's supply routes are now closed or exhausted (its
   own memory: fifteen constructions, all killed; its own corpus: **447 of 447**, zero out-of-map
   survivors). **The exit is "clause X-1", the near-miss probe of the register's own map** — for each
   closed row, name the nearest state kind the row's own closing clause does not cover, write it blind,
   and screen it under the **unchanged** narrowed rule; the register has run this probe once, in one of
   thirty-three rows (R-067's carried-forward residual → R-068's D4 → row 27 closed in full). It is
   **specified, not adopted and not executed**, and is handed to Cycle 136. **The Cycle-132 rejection of
   the literature-first route amendment is untouched and is not re-opened.** The open gaps were tracked
   with **no action on G-37 and no action on G-33**. Housekeeping re-derived the counts, re-ran the rubric
   arithmetic clean — **no score or rank moved: IDEA-011 69.0 (rank 1), IDEA-004 63.0 (rank 2), IDEA-014
   52.0 (rank 3), IDEA-009 42.0 (rank 4), IDEA-010 parked (P-014) at a terminal 55.0** — advanced all five
   artifact headers to "Cycle 135 complete" and read them back, and ran the standing identifier-integrity
   check. **No candidate created; no `IDEA-` identifier consumed; no `S-` identifier consumed and no
   document fetched; no gap opened or closed; no score, rank or hard-stop flag changed; no validation
   specification created, amended or withdrawn.** Earlier history —
   **Cycle 134 completed three pre-registered priorities — a record-integrity repair and the completion
   of the backward state inventory.** The cycle's central finding is a **record-integrity** one and it is
   the third in this repository's sequence: **the Cycle-133 handoff asserted that the backward state
   inventory was complete ("all 437 sources have been inventoried") and it was not** — a **mechanical
   verification** (the ledger's entry blocks enumerated, the identifiers appearing in the inventory tables
   enumerated, and the two differenced) returned **seventeen ledger entries that had never been read**
   (S-439, S-440, S-442 … S-457), because the ledger grew by nineteen entries after Cycle 133's batches
   were pre-registered while the extraction stopped at S-438; and the corpus figure itself was wrong in
   **both** directions: the ledger holds **447 entry blocks** — 437 `### S-NNN` headings **plus the ten
   Cycle-58 document-record entries S-281 … S-290**, which carry no heading of their own — of which **446
   are verifiable** (S-290 is unverifiable and struck), so the long-propagated "437 verified sources
   (S-001 … S-457; S-210–S-219 **and S-281–S-290 reserved and unused**)" understated the corpus by ten and
   overstated the coverage by seventeen; the second "reserved" range was **false**, and the Cycle-35
   reservation list reserves only **IDEA-016, S-210 … S-219, V-011, G-26 and P-013**. Eight repairs were
   pre-registered before the cycle's first artifact write and executed with a before/after, **none of
   which touched a score, a rank, a hard-stop flag, a gap's status, a rejection's verdict or a candidate's
   status**: the corpus count; the **ten batch rows that described the ten live entries as reserved and
   empty** (re-read and re-classified in place); **four batch outcome tallies that did not match their own
   tables** (corrected to match the per-source cells, which are the primary record); the **Cycle-129
   S-028** cell, which had stood as an unrecorded out-of-map entry with no kill and no map row behind it
   (now (iv-b) not-a-state), and the **S-021** cell (now (iv-b), the stricter reading, with the
   disagreement recorded rather than adopted silently); a retrospective **Cycle-133 boundary record**,
   because Cycle 133 wrote three batch tables and left no cycle-log record; the Cycle-133 handoff's
   garbled inventory paragraph; and this file's own identifiers. The final batch (S-439 … S-457) was then
   written under the unchanged R-068 extraction rule, the stricter (iv-a) test and **zero fetches** —
   nineteen slots, seventeen new reads and two double-reads — returning **7 in-map and 12 not-a-state
   (iv-a), no out-of-map survivor and no candidate**. **The backward state inventory is now COMPLETE:
   447 of 447 entries (100 %), distributed 272 in-map · 172 not-a-state (168 (iv-a), 4 (iv-b)) · 3
   out-of-map entries, all three killed and mapped (coverage-map rows 29, 32, 33).** The open gaps were
   tracked with **no action on G-37 and no action on G-33**. Housekeeping re-derived the counts, re-ran
   the rubric arithmetic clean — **no score or rank moved: IDEA-011 69.0 (rank 1), IDEA-004 63.0
   (rank 2), IDEA-014 52.0 (rank 3), IDEA-009 42.0 (rank 4), IDEA-010 parked (P-014) at a terminal
   55.0** — advanced all five artifact headers to "Cycle 134 complete" and read them back, and ran the
   standing identifier-integrity check. **No candidate created; no `IDEA-` identifier consumed; no `S-`
   identifier consumed and no document fetched; no gap opened or closed; no score, rank or hard-stop flag
   changed; no validation specification created, amended or withdrawn.** **Cycle 133** wrote the three
   inventory batches (S-410 … S-438) into `rejected_and_parked.md` but **left no cycle-log record**, and
   that omission was repaired retrospectively in Cycle 134; **Cycle 132** executed four pre-registered
   priorities and changed no score, no rank and no flag. Earlier history —
   **Cycle 131 completed four pre-registered priorities — a record-integrity repair, the continued
   backward extraction, the literature-first amendment drafted, and housekeeping. The repair list was
   pre-registered before the cycle's first artifact write and is itemised in `cycle_notes.md`: the
   coverage map's rows 32 and 33 were written twice and the duplicate pair was removed; those rows'
   attribution to "R-068, batch 2" was corrected to the cycle that produced them (Cycle 129); the two
   baseline rows that Cycle 129's batch-2 summary claimed ("baseline row 107 (approx)" and "row 108")
   but **never wrote** — and which collided with Cycle 128's own rows 107 and 108 — were written as
   **rows 110 and 111**, and the map's baseline-row citations for rows 32 and 33 were corrected from
   "—" to those two numbers; Cycle 130's batch, which existed only as a one-line summary, was
   **re-derived per source** and written out beside Cycles 129's batch tables, with the re-derivation's
   disagreements with the summary recorded rather than adopted silently; the Cycle-130 handoff's
   "111 baseline rows" was corrected to the **109** the table actually holds at the time of the repair —
   it had counted the header and separator rows of a 109-row table — and the table holds **111 data rows
   after the repair**; the Cycle-129 claim
   that the literature-first amendment had been "drafted in cycle_notes.md" — a draft that **exists in
   no artifact** — was recorded as a false claim and the draft **written** this cycle; the **S-041**
   cell in Cycle 129's batch 2 was **corrected in place** to (iv-a), the stricter of the register's own
   two readings of the "claims no price effect" test, with the general finding recorded; and the
   artifact headers, stale at "Cycle 128 complete" through Cycles 129–131, were advanced and read back.
   Priority 1
   continued the backward extraction over **three pre-registered batches of fifty** ledger entries
   (S-076 … S-225), reading each entry for the single conditioning state of the published price effect
   it claims, and returning **in-map nulls and not-a-state entries in the main, with no out-of-map
   survivor and no candidate** — the corpus remains internally consistent with its own rediscovery
   guard; the inventory now covers **237 of the ledger's 437 sources (54.2 %)**, with **200 entries
   still to be read**, at a cost of **zero fetches**. Priority 2 **wrote** the literature-first route
   amendment as a **draft only** (`cycle_notes.md`),
   in clause form, with the positive list, the clauses it does not change, the licence cost, the bound
   and the standing limit that the map remains a lower bound; **it is not executed and not adopted**.
   Priority 3 took **no action** on G-37 (its null stands, recorded once, the bounded search not re-run)
   or on G-33 (its three named dated routes unchanged, ESMA's own routes still HTTP 403), and ran the
   map-vs-corpus audit with numbers — **237 of 437 sources inventoried; 170 in-map nulls, 0 out-of-map
   survivors, 67 not-a-state (65 (iv-a), 2 (iv-b)); 45.8 % of the corpus untouched; the map remains a
   lower bound** — and, in addition, a targeted gap-ledger audit that produced the **corrected
   open-gap list** after two successive handoffs had disagreed about it. Priority 4 re-derived the
   counts from the files, re-ran the rubric arithmetic clean, and advanced all five artifact headers to
   "Cycle 131 complete" — the **twelfth
   recorded occurrence** of the header-update failure mode, this time repaired in the same cycle.
   The cycle ran across **two sessions** — the pre-registration, the repair list, the draft and two of
   the three batches in the first; the third batch, the audit and the housekeeping in the second — and
   **nothing written by the first session was altered**.
   **No candidate created; no `IDEA-` identifier consumed; no `S-` identifier consumed and no document
   fetched; no gap opened or closed; no score, rank or hard-stop flag changed; no validation
   specification created, amended or withdrawn.**
   **Cycles 129 and 130 left no paragraph here — a drift repaired in Cycle 131; their records are in
   `cycle_notes.md` and `rejected_and_parked.md`**;
   **Cycle 128 completed four pre-registered priorities — the register's first screen whose unit of work is
   the *state* that each already-held source conditions on, read **backwards** from the register's own
   source ledger (the **inverted route**): the forty-four pre-registered sampled sources (S-001 … S-201,
   S-221 … S-271, S-291 … S-451 — every tenth source in ledger order) were each read for the single
   conditioning state of the published price effect it claims, and the result is **23 in-map nulls, 4
   out-of-map and killed, 0 out-of-map survivors and 17 not-a-state** (16 of the 17 claim no price effect at
   all; 1 conditions a price effect on something that is not a state at all) — **no candidate, no `IDEA-` identifier, no `S-`
   identifier and zero fetches**; the three out-of-map state kinds the extraction surfaced (**a real-time
   order-flow or order-book-imbalance state**; **a published settlement-based market-liquidity
   measurement**; **the execution channel through which an institutional flow is executed**) were each killed by
   a **named clause** and are recorded as closed kinds, logged as **R-068**, which extends the coverage map
   to **thirty-one rows** and adds **three** rediscovery-guard baseline rows (**rows 107–109**); the
   adoption-count set's rescuing sub-variant, which R-067 carried forward because a kill that cannot name a
   clause is not a kill, was **named** — a published count of adopters of a *contested-sign* decision, a
   published count of dual-class issuers being the archetype — and **killed by the count-dilemma**, in which
   the two exhaustive cases kill in opposite directions (a known-in-advance sign makes the count a monotone
   level that sizes the effect, **G-12**; an unknown sign is not contained in the count at all, R-020's
   principle), so R-067's set (3) is a **complete kill**, the map's **row 27 is closed in full** and baseline
   **row 105** is amended in place — the handoff's expected twenty-ninth row did not materialise, because
   the rescuing sub-variant is a **member of the existing kind** rather than a new kind, and that deviation
   is recorded with its reason; G-37 and G-33, where **no action** was taken and both gaps stand exactly as
   recorded; and housekeeping, with the counts re-derived from the files and the rubric arithmetic re-run
   clean. One rejection (R-068), three baseline rows, one baseline row amended in place, no source added or
   consumed, no candidate created, no score, rank or hard-stop flag changed, no gap opened or closed, no
   specification created, amended or withdrawn — and the **eleventh recorded occurrence** of the
   header-update failure mode recorded and repaired**;
   **Cycle 126 completed four pre-registered priorities — the register's first screen whose unit of work is
   the *measurement* rather than the record: four pre-registered published-measurement sets (infrastructure
   congestion / capacity utilisation; a supervisor's aggregate of a private quantity; an adoption / diffusion
   count; a venue-share / fragmentation measurement) were screened and **all four were killed at the design
   stage with zero fetches**, logged as **R-067**, which extends the coverage map to **twenty-eight rows**,
   adds **four** rediscovery-guard baseline rows (**rows 103–106**), and names a **third structural
   category** — the **aggregated-obligor side**, a state published by a disinterested third party but
   computed from the obligors' own records, whose failure mode is *identity* (G-28) rather than the
   accounting-by-product clause; G-37's remaining limb, where the single permitted bounded check returned a
   **null** (the S-454 work has **not** appeared in a peer-reviewed venue — arXiv records no journal
   reference after v3, and the paper is additionally on SSRN and on the author's own site, all preprints) and
   the null is **recorded once** with the bounded search **not** re-run a third time, while the same check
   **upgraded S-454 in place** to full body verification (author-hosted PDF, 18 pages, text-extracted) which
   confirms the relation contains **zero** occurrences of "funding" and "perpetual" and that the paper's own
   close is a **null on tradability**; and IDEA-011's two open limbs, where **S-455's verification debt was
   cleared** — the ESMA 2026 ECEP statement is now **line-verified** through the Cyprus SEC's complete
   reproduction of it and the Malta FSA's own circular of 19 October 2026 (**S-456**), with two further
   national-authority carriers as **S-457** — while the statement remains an **enforcement-priority
   statement, not a measurement**, so **G-33 stays open**, its one new fact being a **second route to the
   rate** (an ESEF IFRS 18 *tagging* rate computable from the filed 2026 annual reports, a proxy and an
   upper bound) which is **handed to validation** and carried into **V-009** as a **fourth named object that
   must not be pooled**. Two sources, two in-place upgrades, one rejection, four baseline rows, no candidate
   created, no score or rank changed, no gap opened or closed, one specification amended (V-009) — and the
   **tenth recorded occurrence** of the header-update failure mode recorded and repaired**;
   **Cycle 125 completed four pre-registered priorities — a record-integrity repair (Cycle 124 had
   advanced **no** artifact and its claimed rejection **R-065** had never been written, so it is written
   now from the Cycle-124 record; the stale "next free **S-448**" pointer, which named a **live**
   identifier, is repaired to **S-454**; and R-064's coverage-map baseline-row citations are corrected
   in place against the baseline table's own positional numbering); the record-first scan's three
   remaining candidate record sets (a published default-portfolio auction record; a published revision
   calendar with revised values; a published levy schedule), **all three killed at the design stage with
   zero fetches** and logged as **R-066**, which extends the coverage map to **twenty-four rows** and adds
   **three** rediscovery-guard baseline rows (**rows 100–102**); G-37's remaining limb, where a bounded
   search produced **S-454** — the first *named, citable, published* instance of the general proposition
   the limb asks about — but the source is an **arXiv preprint** about an intraday price-path relation, so
   **the limb's condition is still not met** and the gap stays open with a **sharpened** re-screen
   condition; and IDEA-011's two open limbs, where **S-455** (ESMA's dated 2026 enforcement-priority
   statement, **index-rendered** after three HTTP 403 failures — **upgraded in place to line-verified in
   Cycle 126**, when a national competent authority's complete reproduction of the statement and a second
   authority's circular were obtained) makes the candidate's mandatory
   pre-adoption disclosure **supervised** but supplies **no population rate**, so **G-33 stays open**.
   Two sources, two rejections (one written late), four baseline rows, no candidate created, no score or
   rank changed, no gap opened or closed, no specification created or amended — and the **ninth recorded
   occurrence** of the header-update failure mode recorded and repaired**;
   **Cycle 123 completed five pre-registered priorities — a record-integrity repair (the retrospective
   Cycle-122 boundary record; the source-count repair from the stale "418" to the true **433 (S-001 …
   S-453)**; and the Cycle-118 unsourced literature-closure claim, re-grounded on R-027 and on three newly
   registered peer-reviewed sources, S-448 … S-450); a construction-first screen of **three pre-registered
   new state kinds**, all killed at the design stage with **zero fetches**, logged as **R-064** with the
   register's **published-state-kind coverage map** and one new baseline row (**row 98**); G-37's remaining
   limb, where a bounded search produced **S-451** and the limb's condition was **not** met, so the gap
   stays open and dated; and IDEA-011's two open limbs, where **S-452** (DRSC DAX 40 survey) and **S-453**
   (Norwegian FSA thematic review of a random sample of 50) were added and **S-437** was upgraded in place
   from index-rendered to **line-verified with the issuer identified as flatexDEGIRO**. Six sources, one
   rejection, one baseline row, one specification amended (V-009), no candidate created, no score or rank
   changed, no gap opened or closed — and the **eighth recorded occurrence** of the header-update failure
   mode recorded and repaired**;
   **Cycle 113 completed three pre-registered priorities — the two-sub-family screen of US commodity futures'
   published regulatory and positioning states, which is a **bounded negative on both limbs** and is logged as
   **R-062** with the two families added to the known-baseline table as **rows 95 and 96** (the handoff's
   framing of the screen was **corrected before it ran**: one family was a *licensed re-screen* of the
   register's own closed templates R-042/R-043 and the other was already a registered source and a parked
   candidate's own state, so the screen's real question was weaker than the handoff's); the **bounded
   post-2010 re-read of IDEA-011's nearest published test**, which returned a **null on the score** (no
   published null and no sign reversal; the nearest test finds "modest" and "economically small" effects,
   which under G-12 is a magnitude finding, while S-407 makes institutional enforcement quality a mandatory
   competing-conditioner control and S-408 is a protocol-level review frame on which the register makes no
   claim) and which added a **third hard-stop condition**, a **new dated monitor** (the 2026 interim reporting
   season) and a **V-009 amendment**; and the **execution of the two gaps opened in Cycle 112**, with
   **G-38 closed** on two published RIN cost anchors (S-404, S-405 — spreads and transaction costs of the order
   of **five times** those of comparable energy futures, which is **adverse** to the candidate's required
   effect and tightens V-012's pass bar) and **G-37 partially answered** (the current regime is
   **continuation**, not reversal, and the regime gate is worth **+1.9 to +2.8 bps per day** at p = 0.19 to
   0.29, so it cannot carry the rule — a **third hard-stop condition** and a **V-008 amendment**). **Eleven
   sources (S-398 … S-408), one rejection (R-062), two baseline rows, one gap closed, no gap opened, no
   candidate created, no score or rank changed, and three specifications amended (V-008, V-009, V-012).** The
   register's active book is left at four candidates of which only IDEA-011 is free of a blocking gap, and the
   cycle log records the **sixth occurrence** of the header-update failure mode — this time **partial**, because
   the session was interrupted after two artifacts had been updated and three had not; the artifact set was
   completed in the follow-on session rather than left half-written**;
   **Cycle 112 completed three pre-registered screens (the IDEA-009 prior-art screen the Cycle-109 P-5
   audit named as decisive — **R-059**, adverse, **IDEA-009 re-scored 53.0 → 42.0** and demoted to rank 4
   with two new hard-stop conditions, V-008 amended and gap **G-37** opened; the IDEA-014 state-free
   existence limb on two route forms the register had never used on that candidate — **R-060**, bounded
   negative, the limb still inconclusive, **V-012 written** under a narrow recorded amendment and gap
   **G-38** opened; and a new mechanism family screen on currency-option implied distribution states —
   **R-061**, bounded negative, now baseline row 94) and a **state-integrity repair pass** that found and
   repaired **five label-and-header defects** — including three artifacts that carried a block headed
   "Cycle 112" whose work was executed in **Cycle 111**, and five artifact headers whose claimed update to
   "Cycle 111 complete" had in fact never happened (the **fifth recorded occurrence** of the header-update
   failure mode). Nine sources (S-389 … S-397), one specification created and one amended, two gaps opened,
   no gap closed, no candidate created, and the register's active book left at four candidates of which
   only IDEA-011 is free of a blocking gap**; **Cycle 109 completed the five priorities carried from Cycle 108 — the
   published 2009 *RFS* body of Carr & Wu (S-154) was **OBTAINED** on the course-host route form
   (a Duke University course directory copy: HTTP 200, 213,058 bytes, 31 pages, the publisher's typeset
   file, running head "The Review of Financial Studies / v 22 n 3 2009", ending at page 1341) and is
   now **fully line-verified**, so the Cycle-108 twenty-one-route closure is **superseded**; the
   **published version's own magnitudes differ from the May 2004 working paper's** (7 of 35 and 23 of 35
   against "all but three" and "21 of the 35"; a **negative** significant variance-beta slope, "LRP_j =
   0.0061 − 0.3283 βV_j + e, R² = 18.4 %", against the working paper's **positive** slope on β²_V), so
   the pre-registered outcome is **(ii)**: **row 38 is rewritten in place**, the single-name screen is
   re-examined, and **IDEA-003's G-05 closure is re-opened for that limb only** and then **re-closed** on
   the published evidence. The **P-3 screen on IDEA-011's "first adopter versus repeat adopter"
   classification** closed as a **bounded negative (R-057)**: a new route form (the IFRS Foundation's
   **per-jurisdiction profile PDFs**) shows the *framework-level* first-adoption fact is **published and
   dated** (EU 2005, Ghana 1 January 2007, Nigeria 1 January 2012) — so the historical comparator is
   decision-time and free, and the G-21 comparison can be specified **without a look-ahead-classification
   objection** — while the *standard-level* IFRS 18 partition is **not** decision-time (no profile carries
   an IFRS 18 date; the only firm-level instrument is Saudi Arabia's **self-selected, ex-post-announced**
   early-adoption permission; the ESMA statement carries no first-time/repeat language at all). The three
   candidate audits (P-4 on IDEA-004, P-5 on IDEA-009, P-6 on IDEA-014) **confirm existing positions and
   change no score**: for IDEA-004, **timing is not the binding constraint** — the missing thing is
   *identity*; for IDEA-009, the funding state **passes** all three limbs, so the binding constraint is the
   published unconditional-versus-conditional prior art; for IDEA-014, the architecture is public and the
   *sign-determining* net position is not, with the price-effect existence limb left untouched. Two
   record-integrity repairs: a **stray blank line inside the known-baseline table** (which had split it into
   rows 1–89 and 90–92) was removed, and a **stale "divided by five" clause** in the shortlist's rubric
   sentence was corrected (the table was always right). **No `S-` identifier was consumed** — the two
   documents obtained are the *same sources* in a new form, which the register records as upgrades — one
   bounded negative (**R-057**) was logged, and **no score, rank, gap, flag or specification changed**; it
   also rewrote the handoff body**.
   **Cycle 108 completed the two open theoretical questions carried from
   Cycle 107 — the published 2009 *RFS* body of Carr & Wu (S-154) was attacked over **twenty-one named
   routes** and is an **evidenced closure**, while the **published version's front matter is now
   line-verified** through a new carrier source (S-385, a 2022 NYU memorial deck) whose published
   acknowledgements name the editor and an anonymous referee, a decisive version discriminator against
   the May 2004 working paper; the **version drift is documented precisely** and the **pre-registered
   outcome is (iii)**, so the individual-stock magnitudes remain the working paper's, the known-baseline
   row 38 is corrected in place, and **IDEA-003's G-05 closure is not re-opened**. The second question —
   the **ASR announcement-date public-observability screen** — was **pre-registered in the cycle log
   before the fetches** and closed as a **bounded negative (R-056)** on five reasons: the *contract
   architecture* is **public** (the executed confirmation was Exhibit 99.1 to the Form 8-K; the filing
   body, S-386, disclosed the $25.97 initial price; the press release, S-387, disclosed that the price
   is the market price at signing), so the baseline row's "the discount is private-contract data" was
   **narrowed in place**; but the *realized discount* is a **terminal** quantity, the initial discount is
   **zero by construction**, the covering window is **bounded ex ante by published law** (17 CFR
   240.10b-18, **S-388**) rather than by a discriminating state, and the **issuer published its own
   expectation** of the adjustment at the announcement date. Four new source entries were consumed
   (**S-385 … S-388**), one bounded negative (**R-056**), two baseline rows corrected in place (rows 38
   and 44), and **no score, rank, gap or specification changed**; it also rewrote the handoff body**.
   **Cycle 107 completed the four open Priority-3 questions left over from
   Cycle 106 — three entries were upgraded (S-153, S-156, and S-154 in part), one was partially
   upgraded with a new primary source behind it (S-166/S-384), two are evidenced honest negatives
   (S-238's body is closed across three open-access registries; S-271's endorsement document is
   absent from every Wayback CDX path form), one new source identifier was consumed (S-384), one
   claim limb was struck (S-154's third limb, contradicted by the paper's own factor analysis), and
   a version drift was resolved exactly (S-156's 0.92 %/0.16 % magnitudes belong to the earlier NBER
   working-paper revisions, not to the published *JFQA* article); it also recorded the **fourth
   occurrence** of the state-integrity failure mode — **Cycle 106 was never written into any
   artifact**, so a retrospective **Cycle-106 cycle-boundary record** was added to the cycle log in
   the same form as the Cycle-97 record added in Cycle 98 — and rewrote the handoff body**; **Cycle 97 was
   executed but never written up in the cycle log — its boundary record
   was added retrospectively in Cycle 98, and its work is visible only as annotations in the source
   ledger**).
   A reserved identifier is one that a prior cycle claimed in writing but never wrote into an
   artifact; it is left unused on purpose so that a later reconstruction of that work cannot collide
   with a new one.
   Reuse an existing source ID rather than duplicating a citation; extend the "supports" note instead.
   **The ID ranges quoted in the repository's `AGENTS.md` are historical** (they stop at IDEA-012 and
   S-094); the authoritative next-free IDs are the ones in item 3 above and in `next_agent_handoff.md`.
   **Re-derive every identifier yourself** (publisher, Crossref, arXiv, NBER or the institution's
   own site) before it enters the ledger: identifiers supplied by a search or research agent have
   been found wrong, and one registered working paper carries a fabricated bibliography. Record
   whether a document was **fetched directly** or read only through a **search index**, and never
   present an index-rendered quotation as a directly parsed document. **A quotation that cannot be
   re-checked by extracting the document's text layer is not yet a quotation** — extract it, or
   record the entry as index-rendered and unattributed. **A failed retrieval must be recorded as a
   failed retrieval**: mark the entry NOT VERIFIED, list the routes tried and their failure modes, label
   the wording as index-rendered, and restate the corpus's verification status (how many items are
   line-verified versus index-confirmed). Never let a "fetched directly" verification line stand on a
   document that was in fact unreachable.
4. **Never invent a citation.** Every external claim in a dossier points to an `S-0NN` entry in the
   source ledger, and every ledger entry records how it was verified. If a claim cannot be sourced,
   mark it as an unresolved conjecture in the dossier.
5. **Scores are research-priority weights, not success probabilities.** No numerical probability of
   profit is attached to any candidate; the rubric score is a transparent weighted total out of 100.
6. **Theory only.** No backtests, no data acquisition or processing, no executable strategy code, no
   performance metrics, no workflow/test/infra edits, no cross-repository work. Unresolvable questions
   are documented and handed off, not silently relaxed.
7. **Every session ends with an updated handoff** naming the best next research task, the highest-value
   unresolved theoretical questions, and the next mechanism families to investigate.
