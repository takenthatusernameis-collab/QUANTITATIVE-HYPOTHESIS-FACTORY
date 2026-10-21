# Next agent handoff

**This file is rewritten at the end of every cycle. It is the only file the next agent must read
before doing anything. Cycle 102 is complete (21 October 2026).**

---

## Header

**Cycle 102 complete — 21 October 2026. Evidence work, not a screen.** No candidate was created,
no score changed, no gap opened or closed, no validation specification was touched, no known-baseline
row was added or removed.

**What Cycle 102 actually did.** It ran one bounded, pre-registered provenance operation over
thirteen targets, closed four of the six open Priority-3 questions, and — the most important thing —
**found and recorded that the Cycle-101 provenance operation never reached the artifact**. The
Cycle-101 handoff header and the Cycle-101 cycle record both claimed that ten entries "were upgraded
to line-verified" and that the annotations "were written into each entry in the same cycle". Checked
file by file in Cycle 102: the string "Cycle-101" appears **nowhere** as an annotation in
`source_ledger.md`; there is **no Cycle-101 section in the ledger at all**; and the thirteen
Cycle-101 targets' own verification bullets still read exactly as they did before Cycle 101. This is
the **third** occurrence of the same failure mode (Cycle 99 → S-208 and S-136; Cycle 101 → all
thirteen targets). The lesson is unchanged and is now written into the handoff as a standing rule:
**a provenance upgrade is not done until the entry's own verification bullet says so; a cycle log
and a handoff header are records of intent, the ledger entry is the evidence.** Cycle 102 re-ran
the work and **wrote it into the entries** — eighteen entries now carry a Cycle-102 annotation (sixteen "Cycle-102 verification"
bullets, plus S-208's "Cycle-102 resolution of the two struck items" and S-115's "Cycle-102 re-fetch attempt"), and the two Cycle-101 findings that were correct as facts (S-118's NY Fed PDF, S-158's
title-version explanation) were reproduced and recorded.

**Upgrades.** Full, nine: **S-027, S-102, S-118, S-125, S-158, S-168, S-170, S-229**, and from
Priority 3 **S-237**. Partial, with the unverified part named, six: **S-153, S-154, S-156, S-166,
S-172, S-271**, and from Priority 3 **S-238** (abstract level only). **One quotation struck in
place** with the string counts that show the absence: S-172's "the momentum factor is estimated to
earn ~2 % annualised today against ~10 % in the 1990s" — it is in **no** version of the paper
(eight probe strings, zero hits each in v1, v2 and v3). **Three material bibliographic
corrections**, each carried into the register, the known-baseline table and the ledger headings:
**S-166** is *Bargeron, Kulchania & Thomas (2011)*, **not** Erickson, Fang & Howe (the DOI, journal,
volume, issue and pages in the entry all belong to Bargeron et al., and the entry had conflated two
different papers with the same title); **S-156** has **four** authors (Ben-David, Li, Rossi and Yang
Song), not three; **S-158**'s author order is **Gornall, Rinaldi & Xiao**, not Gornall, Xiao &
Rinaldi. **S-154**'s deposited title is "Variance Risk **Premiums**", not "Premia".

**Two identifiers consumed, with the reasoning recorded in the register, the shortlist and the cycle
log together, as the register requires**: **S-381** (the SEC's 23 January 2015 no-action letter on
abbreviated tender offers for non-convertible debt securities) and **S-382** (the SEC Division of
Corporation Finance's 30 June 2026 exemptive order on the same subject). These are new primary
regulator documents the register must cite on their own, because they are the *source* of the two
items S-208 had to strike, they carry their own dates, and **one of them changes the current rule**.

**One dated fact the register must now carry.** The 2015 letter's mechanic — the **"guaranteed
delivery"** procedure, under which a holder certifies beneficial ownership and the securities are
delivered "no later than the close of business on the second business day after the expiration of
the offer" — and the 1986 relief's **"seven to ten calendar days"** abbreviated period are both
**confirmed against the SEC's own words** (S-381), but the 2015 letter was **superseded on 30 June
2026** by S-382, which drops the guaranteed-delivery condition, extends the five-business-day
minimum to debt securities "regardless of any particular rating", and sits alongside a separate
**16 April 2026** order shortening the *equity* minimum to ten business days. **The register's
mechanic is now history, and it must be dated as such.** S-208's two Cycle-100 struck items are
therefore **recoverable — from primary text, and with the correct attribution and the correct
currency**.

**New working routes established this cycle — these are the lever for the next cycle.**
(1) The **Publications Office Cellar**: `http://publications.europa.eu/resource/celex/<CELEX>` with
`Accept: application/xhtml+xml` and `Accept-Language: eng` returns the **full text of any EU legal
instrument** (HTTP 200, 123,534 bytes for 32003L0087; 662,758 bytes for 32023L0959). It **replaces
the exhausted EUR-Lex route**, which returns HTTP 202 with a zero-byte body on all six path forms
tried. (2) **Crossref's deposited abstract** is the general lever for the remaining journal entries
and is still open on most of the residual pool. (3) The **AFA conference-paper repository**
(`afajof.org/management/viewp.php?n=…`) and the **AEA annual-meeting programme** both serve full
paper PDFs directly. (4) The **Internet Archive is back up** (CDX and the availability API both
answer HTTP 200) and has a snapshot of the SOCPA news item; it has **none** of the SSRN 6751741
routes. (5) **WU Vienna's `fileadmin` tree** serves the working papers the old `wu.ac.at/fin/` path
no longer does.

**Re-derived counts.** 15 dossiers (4 active, 6 parked, 5 rejected) · 4 ranked active + 1
parked-at-terminal · **372 verified sources** (S-001 … S-209, S-220 … S-380, **S-381**, **S-382**;
S-210 … S-219 reserved and unused; 362 heading-form entries + 10 bold inline, the S-358 sub-heading
not being a second entry) · 10 validation specifications (8 not executable; executable V-008, V-009;
V-002 frozen; V-010 never-to-execute) · **55** rejections (R-001 … R-055) · 13 parking records
(12 active) · **92-row** known-baseline table · gaps G-01 … G-36, open: G-21, G-28 (frozen), G-30
(exhausted). **Next free identifiers: IDEA-017, S-383, V-012, G-37, R-056, P-015.**

**Rubric-arithmetic re-run: clean.** Weighted total = Σ(dimension score × weight) / 5, weights
25/20/15/15/15/10, per-point values 5.0/4.0/3.0/3.0/3.0/2.0. IDEA-011 4/3/3/4/2/5 = **69.0**;
IDEA-004 4/4/1/3/3/3 = **63.0**; IDEA-009 3/3/1/3/2/4 = **53.0**; IDEA-014 3/2/3/2/2/4 = **52.0**;
IDEA-010 4/4/1/2/2/2 = **55.0**. Every recorded total matches its recorded profile. No score, rank,
tie-break, hard-stop flag, gap or specification changed.

**Do not re-run:** `eur-lex.europa.eu` (HTTP 202, zero bytes — use the Cellar instead);
`socpa.org.sa` direct (times out — use the Internet Archive, which has the news item but not the
endorsement document); `sciencedirect.com` article pages (403); `ssrn.com` landing pages (403);
`socpa.org.sa` endorsement document `…/2905.aspx` (times out, and **no** Wayback snapshot);
`wu.ac.at/fin/…` and `department-of-finance/working-papers/…` (404 — use the `fileadmin` tree);
`keyrock.com/research/…` and `keyrock.com/blog/…` (403); `saudiexchange.sa` (403);
`papers.ssrn.com/…6751741` and every archive form of it (**no snapshot exists**).

---

## 1. State of the pipeline

**Frozen, exhausted, dated — carry these forward unchanged.**
- **G-32 limb (c)** (EU ETS second-market condition) — dated **2027 Q3**; **G-33** dated **2027 Q3**.
- **G-14** (Nasdaq-100 single-name index-vendor data) — dated **29 March 2029**; untouched.
- **IDEA-014**'s state-free existence limb — **inconclusive**; the five-reason register for it is
  **exhausted**; do not re-run it.
- **G-21** (EA/ERA regulatory artefact) — **open**.
- **G-28 (frozen)** and **G-30 (exhausted)** — open but not actionable.
- **R-054** condition (c) — SEC comments closed **4 December 2026**; **R-055** condition (c) — SEC
  comments due **14 December 2026**. **Both are still in the future on 21 October 2026.** Neither is
  due; neither may be pre-empted; R-055's condition (d) was not re-run.
- **V-002** is frozen; **V-010** is never-to-execute; **V-001, V-003 … V-007** are not executable in
  this environment; **V-008** and **V-009** are the only executable specifications and they were not
  executed.

**Residual provenance pool, re-measured this cycle and disclosed rather than smoothed.** The
detector was re-implemented from the prose rule (index-render wording present, and no positive
direct-fetch assertion in the same sentence) and applied to the corpus as it stood at the start of
Cycle 102: **29 index-rendered-only, 115 mixed, 218 with no index-render wording**, over the **362**
heading-form entries. **Four of the 29 are detector artefacts, adjudicated by hand**: S-101 (a
Cycle-5 direct fetch of the arXiv HTML to a file), S-309, S-311 and S-313 (each carries a
**Crossref-deposited abstract** fetched directly, which is a positive assertion). The hand-adjudicated
state is **25 index-rendered-only, 119 mixed, 218 with no index-render wording**. **No earlier
cycle's figures are restated.** The 25: **S-147, S-148, S-151, S-152, S-157, S-159, S-160, S-167,
S-179, S-181, S-247, S-248, S-249, S-253, S-258, S-262, S-263, S-264, S-268, S-274, S-276, S-278,
S-280, S-292, S-329.**

**Honest negatives recorded this cycle.** S-115 (the Internet Archive is up and has **no** snapshot
of any SSRN 6751741 form — the paper has never been archived; the quoted abstract remains
index-rendered). The keyrock.com primary document (HTTP 403 on three paths; the *entry's own cited
URL* was fetched and the quotation confirmed, so this is a negative about the originating document
only, not about the entry).

**What the register now rests on that it did not before.** The EU free-allocation ladder is backed
by the directive text rather than by a briefing; the ASR claim is backed by the correct paper; the
perpetual-funding mechanism is backed by two primary versions and the authors' own CFTC letter; the
tender-offer mechanics are backed by the SEC's own letters.

**What the register still does not have.** The *bodies* of S-238 (Switzer), S-153/S-154/S-156's
magnitude claims, S-166's intermediary-borrowing detail, S-172's struck figures, S-271's "all at
once" wording and effective date, and S-115's abstract. Each has a named untried route in §2.

---

## 2. Best next research task — Cycle 103

**Priority 1 — maintain the frozen, exhausted and dated items.** Carry §1's frozen, exhausted and
dated list forward unchanged. Re-check R-054 condition (c) and R-055 condition (c) **only if the
calendar has passed their dates** (4 December 2026 and 14 December 2026); on the next cycle's
timeline neither will be due, and neither may be pre-empted.

**Priority 2 — one bounded, pre-registered provenance operation over a named subset of the
residual pool.** This is the highest-yield work available: the pool is 25 entries, and the
**Crossref-deposited-abstract lever is still open on most of them**. The Cycle-102 subset was
**S-157, S-159, S-167, S-160, S-152, S-274, S-276, S-278, S-280, S-292, S-258, S-262, S-264, S-263,
S-248, S-249, S-253, S-247, S-181, S-179, S-151, S-148, S-147, S-268, S-329** — but **the next agent
must pre-register its own named subset, its routes, and its upgrade/partial/negative criteria in
`research/cycle_notes.md` *before* fetching anything**, and must not exceed a bounded operation.
Notes on the highest-yield members of the pool, from this cycle's reconnaissance:
- **S-157 (Lou & Polk 2021), S-159 (perpetual futures and Bitcoin volatility), S-167 (Guéant, Pu &
  Royer 2015), S-274 (Poterba & Weisbenner 2001), S-276 (McKeever & Rydqvist 2022), S-278 (Dahlquist
  & Sellin 1996), S-280 (Baltas 2019), S-292 (Coval & Stafford 2007)** — all eight already have a
  Crossref record retrieved; the question is only whether the publisher **deposited an abstract**,
  which is the exact pattern that produced the S-125, S-153, S-154, S-156, S-166 and S-168 results
  this cycle.
- **S-160 (Dao, Tan & Zhou 2025, IMF WP)** — the IMF working-paper landing page is index-rendered;
  the IMF working-paper PDF has a different path form on the IMF server and is likely directly
  fetchable.
- **S-268 (Commission Regulation (EU) 2026/338)** — the **Cellar** route used this cycle
  (`…/resource/celex/32026R0338`) is the natural replacement for the exhausted EUR-Lex ELI route,
  and this is the one pool entry where the Cellar lever is known to apply.
- **S-247 (Ellul, Shin & Tonks 2005)** — the LSE working paper dp506 is the target; the LSE
  `research-publications` path is a different path form from the one that failed.
- **S-181 (Ahmed 2026) and S-329 (Sun & Tian 2026)** — both are SSRN `posted-content` records; the
  **Crossref posted-content record** (as used for S-125 and S-311) is the untried route.
- **S-179 (Song & Woo 2015)** — the record says the full text is not publicly available, so this
  entry may be **terminal**; a negative that is recorded as terminal is a legitimate outcome.

**Priority 3 — the open questions, with their named routes.**
1. **S-115's abstract** — the archive route is now closed (never archived). The untried route is
   **the Crossref `posted-content` record for DOI 10.2139/ssrn.6751741**, which is exactly the lever
   that worked for S-125, S-064, S-311 and S-309. If it holds no abstract, the authors' institutional
   pages (Maharaja Sayajirao University of Baroda) are the second route; if both fail, record the
   entry as **terminal index-rendered** and move on.
2. **S-271's "all at once" wording and effective date** — the endorsement document is unreachable
   (host times out; no Wayback snapshot). Untested routes: the **IFRS Foundation's live
   jurisdiction page** for Saudi Arabia
   (`ifrs.org/use-around-the-world/use-of-ifrs-standards-by-jurisdiction/view-jurisdiction/saudi-arabia/`),
   which may carry a **post-2022** profile the PDF does not; the **Saudi Capital Market Authority**
   (`cma.gov.sa`, a different host from the blocked Saudi Exchange); and the **Wayback CDX for the
   Arabic paths** of `socpa.org.sa/Socpa/Professional-standards/…`, which the availability API does
   not index by default.
3. **S-238's body and its introduction summary** — the *conference version* of the paper (presented
   at the Effectiveness of Financial Regulation Conference, Rishon LeTsiyon, June 2022) may be open
   where the journal version is paywalled; the author's Concordia University page and repository
   are the second route.
4. **S-172's struck figures** — the **v1 PDF** (350 KB, the version that carries the Sharpe figures)
   has not been fetched, only the abstract pages. The "≈2 % vs ≈10 %" momentum claim is absent from
   all three abstracts; whether it is in the v1 **body** is an open, cheap, well-bounded question.
5. **The 16 April 2026 equity exemptive order** — identified in the S-382 footnote but **not
   fetched or registered**. Fetch it from `sec.gov/files/rules/exorders/2026/`, line-verify the
   ten-business-day minimum, and decide whether it needs its own `S-` entry (it is a different
   instrument for a different security class, so on the evidence of Cycle 102's reasoning it
   probably does).
6. **S-153, S-154, S-156's magnitude claims and S-166's intermediary detail** — the general route is
   the authors' working-paper versions (NBER WP 28624 for S-156) or the SSRN preprints, since the
   publisher routes are blocked.

**Priority 4 — lossless housekeeping.** Re-derive every count from the files; re-run the rubric
arithmetic; keep the frozen, exhausted and dated items; write the annotations **into the entries in
the same cycle**; keep the known-baseline table, the register, the shortlist, the validation
handoffs and the rejected-and-parked file consistent with each other; do not move, relabelled,
renumber or re-scope anything to tidy a file; do not write the cycle log late.

**Priority 5 — rewrite the handoff** at the end of the session and write a fresh, self-contained
initial task message for Cycle 104.

**Out of scope, permanently:** backtests, simulations, parameter sweeps, optimisation, significance
testing on strategy results, performance or risk metrics, market-data acquisition or processing,
strategy or signal implementation, executable research infrastructure, job or workflow launches,
changes to workflow files, tests, credentials or infrastructure, work in other repositories, and any
trading. The canonical prompt `research_prompts/systematic_edge_discovery_agent_prompt.txt` is
maintainer-owned and must not be edited. If a question can only be answered by running something,
write the question down precisely and hand it off; that is the correct output, not a failure.

---

## 3. Initial task message for the next agent (Cycle 103)

> You are the next agent in a **theory-only** hypothesis-generation and research-prioritisation
> repository. You have no prior context beyond the files. Read, in this order, before doing
> anything else:
>
> 1. `AGENTS.md` (the absolute scope boundary — read it first; it is short and binding).
> 2. `research/next_agent_handoff.md` (this file's successor — it has been rewritten at the end of
>    Cycle 102 and is the authoritative state).
> 3. `research/idea_register.md`, `research/ranked_shortlist.md`, `research/source_ledger.md`.
> 4. `research/validation_handoffs.md`, `research/rejected_and_parked.md`, `research/cycle_notes.md`
>    (read the Cycle-102 record at the end).
>
> **What Cycle 102 was.** Cycle 102 was a provenance cycle, not a screening cycle. It ran one
> bounded, pre-registered provenance operation over thirteen source entries, closed four of six
> open questions, **discovered that Cycle 101's operation had never been written into the ledger**
> (the third occurrence of that failure mode) and re-ran it properly, **consumed two new
> identifiers** (S-381, S-382 — the SEC's 2015 no-action letter and 30 June 2026 exemptive order),
> **struck one quotation in place** (S-172's "~2 % vs ~10 %" momentum figures), and made **three
> material bibliographic corrections** (S-166 is Bargeron, Kulchania & Thomas, not Erickson, Fang &
> Howe; S-156 has four authors, not three; S-158's author order is Gornall, Rinaldi & Xiao). It
> created **no** candidate, changed **no** score, opened or closed **no** gap, and touched **no**
> validation specification.
>
> **What you must do this cycle.**
> - **Priority 1.** Carry the frozen, exhausted and dated items forward unchanged: G-32 limb (c) and
>   G-33 (dated 2027 Q3), G-14 (dated 29 March 2029), IDEA-014's state-free existence limb
>   (inconclusive, five-reason register exhausted), G-21 (open), G-28 (frozen), G-30 (exhausted),
>   V-002 (frozen), V-010 (never-to-execute), and the two dated SEC comment deadlines R-054(c)
>   4 December 2026 and R-055(c) 14 December 2026 — **neither of which has arrived**.
> - **Priority 2.** Run **one bounded provenance operation over a named subset of the 25 remaining
>   index-rendered-only entries** listed in §1 of the handoff (S-147, S-148, S-151, S-152, S-157,
>   S-159, S-160, S-167, S-179, S-181, S-247, S-248, S-249, S-253, S-258, S-262, S-263, S-264,
>   S-268, S-274, S-276, S-278, S-280, S-292, S-329). **Write the pre-registered list — target,
>   route, and what would count as an upgrade, a partial upgrade and a negative — into
>   `research/cycle_notes.md` BEFORE you fetch anything.** The general lever that worked in Cycle
>   102 is **the Crossref REST API's deposited abstract** (`api.crossref.org/works/<DOI>`), which is
>   still open on most of that pool. The **Publications Office Cellar**
>   (`http://publications.europa.eu/resource/celex/<CELEX>` with `Accept: application/xhtml+xml`
>   and `Accept-Language: eng`) is the working replacement for the exhausted EUR-Lex route and
>   applies to S-268. Record for every fetch the URL, the **HTTP status**, the **byte count**, the
>   **page or character count** and the extraction method.
> - **Priority 3.** Close the open questions in §2 of the handoff: S-115's abstract (try the
>   **Crossref posted-content record for 10.2139/ssrn.6751741** first), S-271's "all at once"
>   wording and effective date, S-238's body, S-172's v1 **body** for the struck figures, and the
>   **16 April 2026 equity exemptive order** (fetch it; decide whether it needs its own `S-`).
> - **Priority 4.** Re-derive every count from the files, re-run the rubric arithmetic, and keep the
>   register, the shortlist, the ledger, the validation handoffs and the rejected-and-parked file
>   consistent with one another. Move, relabel, renumber and re-scope nothing.
> - **Priority 5.** Rewrite `research/next_agent_handoff.md` at the end of the session and write a
>   fresh, self-contained initial task message for Cycle 104.
>
> **The rules that keep being broken — read them twice.**
> - **A provenance upgrade is not done until the entry's own verification bullet says so.** A cycle
>   log and a handoff header are records of *intent*; the ledger entry is the *evidence*. Cycle 101
>   claimed ten upgrades that are not in the ledger. **Write each annotation into the entry, in the
>   same cycle.** If you cannot, say so in the handoff and do not claim the upgrade.
> - **A quotation that cannot be re-checked in a fetched document's text layer is not a
>   quotation.** Extract the text layer (or record the entry as index-rendered and unattributed).
>   **Strike in place** any quotation the fetched document does not contain, with the reason and the
>   string counts that show the absence — as Cycle 102 did with S-172.
> - **Record a negative as a negative** (route, status, failure mode), and never let a "fetched
>   directly" verification line stand on a document that was unreachable.
> - **Do not re-run a route that has already returned a negative** unless there is a *different*
>   route — one that differs in **host or path form**, not the same host with a changed query
>   string. The exhausted list is in the handoff header.
> - **An upgrade may only strengthen an existing reason or record.** It may not re-score, add a
>   sixth reason, re-screen a family, or consume an identifier — unless you find something that
>   genuinely demands it, in which case the reasoning must be written in the register, the shortlist
>   and the cycle log together.
> - **Never invent a citation.** Every external claim points to a source-ledger entry, and every
>   entry records how it was verified.
> - **Score with the fixed rubric as research priority, never as a probability of profit.**
> - **Leave the session with an updated handoff and a fresh, self-contained initial task message.**
>
> **ID sequences in use:** `IDEA-001…015` (IDEA-016 and IDEA-017 reserved and unused),
> `S-001…209`, `S-220…380`, `S-381`, `S-382` (S-210 … S-219 reserved and unused),
> `V-001…010`, `R-001…055`, `P-001…012`, `P-014` (P-013 retired), `G-01…36`, `Cycle 1–102`.
> **Next free identifiers: IDEA-017, S-383, V-012, G-37, R-056, P-015.** Continue each series; never
> restart one.
