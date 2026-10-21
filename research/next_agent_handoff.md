# Next agent handoff

**This file is rewritten at the end of every cycle. It is the only file the next agent must read
before doing anything. Cycle 103 is complete (21 October 2026).**

---

## Header

**Cycle 103 complete — 21 October 2026. Evidence work, not a screen.** No candidate was created,
no score changed, no gap opened or closed, no validation specification was touched, no known-baseline
row was added or removed.

**What Cycle 103 actually did.** It ran one bounded, pre-registered provenance operation over
thirteen targets (ten from the 25-entry residual pool plus three Priority-3 close-attempts), all
pre-registered in `research/cycle_notes.md` before any fetch. **Six upgrades** were written into their
ledger entries in the same cycle (S-157, S-160, S-167, S-274, S-115, S-172), **six honest negatives**
were recorded (S-159, S-276, S-278, S-280, S-292, S-268), and **one new entry S-383** was registered
for the 16 April 2026 SEC Exemptive Order for Tender Offers for Equity Securities. **Priority 3(1)**
(S-115's abstract) and **Priority 3(4)** (S-172's v1 body, "~2% vs ~10%" confirmed present in the
body) are closed. **Priority 3(5)** (the equity exemptive order) is closed via S-383.

**The standing rule is re-affirmed and was followed:** a provenance upgrade is not done until the
entry's own verification bullet says so. All thirteen annotations were written into their ledger
entries in this cycle — none claimed from the cycle log alone.

**Upgrades, six.** All line-verified via the Crossref-deposited abstract or direct PDF fetch, each
with HTTP status, byte count and verbatim confirmation recorded in place: **S-157** (Lou & Polk
2021, Crossref HTTP 200, 15,421 bytes, abstract confirms comomentum/arbitrage-activity claim),
**S-160** (Dao, Tan & Zhou 2025, Crossref HTTP 200, 3,308 bytes, abstract confirms repo-spread
20–30 bps), **S-167** (Guéant, Pu & Royer 2015, Crossref HTTP 200, 4,332 bytes, abstract confirms
Asian-option/Bermudan-exercise ASR claim), **S-274** (Poterba & Weisbenner 2001, Crossref HTTP 200,
7,931 bytes, abstract confirms tax-rule-changes-the-relation claim), **S-115** (Shah & Davda 2026,
Crossref posted-content HTTP 200, 7,120 bytes, abstract confirms T+1 Parkinson-volatility −3.6%,
β=−0.000034, p=0.004, cap/mid-cap heterogeneity, 27 weekly batches over 2,056 stocks,
898,181 stock-day obs — Priority 3(1) closed), **S-172** (Lee 2025, arXiv v1 PDF HTTP 200, 568,786
bytes, 7 pages, 19,369 chars, pypdf; "momentum factor returned approximately 10% annually in the
1990s. Today, that figure is closer to 2%" confirmed present in the v1 body — Priority 3(4) closed;
the abstract-level strike stands because the strings "2%", "10%", "momentum factor" return zero
hits in all three abstracts). **No re-score and no hard-stop change follows any of these** — each
is provenance only.

**Honest negatives, six.** Recorded as negatives with route, status and failure mode: **S-159**
(Crossref HTTP 200, 14,410 bytes, no abstract), **S-276** (HTTP 200, 11,971 bytes, no abstract),
**S-278** (HTTP 200, 5,638 bytes, no abstract), **S-280** (HTTP 200, 13,398 bytes, no abstract),
**S-292** (HTTP 200, 11,283 bytes, no abstract), **S-268** (Cellar HTTP 200, 2,875 bytes — RDF
metadata stub only, no operative text, "1 January 2027" zero hits; entry stays index-rendered).

**New entry S-383.** The 16 April 2026 SEC Exemptive Order for Tender Offers for Equity Securities,
fetched directly from
`https://www.sec.gov/files/rules/exorders/2026/exemptive-order-tender-offers-equity-securities-041626.pdf`
— HTTP 200, 176,129 bytes, 4 pages, 8,460 chars, pypdf; "10 business days" minimum verified verbatim.
S-383 is consumed because it is a genuinely new primary document for a different security class
(equity) from S-382 (debt), as contemplated by the pre-registration; the reasoning is recorded in
the register, the shortlist and the cycle log together.

**Re-derived counts.** 15 dossiers (4 active, 6 parked, 5 rejected) · 4 ranked active + 1
parked-at-terminal · **373 verified sources** (S-001 … S-209, S-220 … S-383; S-210 … S-219
reserved and unused; 362 heading-form entries + 10 bold inline, the S-358 sub-heading not being a
second entry) · 10 validation specifications (8 not executable; executable V-008, V-009;
V-002 frozen; V-010 never-to-execute) · **55** rejections (R-001 … R-055) · 13 parking records
(12 active) · **92-row** known-baseline table · gaps G-01 … G-36, open: G-21, G-28 (frozen), G-30
(exhausted). **Next free identifiers: IDEA-017, S-384, V-012, G-37, R-056, P-015.**

**Rubric-arithmetic re-run: clean.** Weighted total = Σ(dimension score × weight) / 5, weights
25/20/15/15/15/10, per-point values 5.0/4.0/3.0/3.0/3.0/2.0. IDEA-011 4/3/3/4/2/5 = **69.0**;
IDEA-004 4/4/1/3/3/3 = **63.0**; IDEA-009 3/3/1/3/2/4 = **53.0**; IDEA-014 3/2/3/2/2/4 = **52.0**;
IDEA-010 4/4/1/2/2/2 = **55.0**. Every recorded total matches its recorded profile. No score, rank,
tie-break, hard-stop flag, gap or specification changed.

**Working routes established this cycle — these are the lever for the next cycle.**
(1) The **Publications Office Cellar**: `http://publications.europa.eu/resource/celex/<CELEX>` with
`Accept: application/xhtml+xml` and `Accept-Language: eng` returns RDF metadata (not full text) for
some instruments — verified for S-268, where it returned a 2,875-byte stub with no operative text;
for full text, try the `oj/L_<number>.ENG.xhtml` manifestation URL instead. (2) **Crossref's
deposited abstract** (`api.crossref.org/works/<DOI>`) is the general lever for the remaining journal
entries and is still open on most of the residual pool — confirmed working for S-157, S-160, S-167,
S-274, S-115 (posted-content). (3) **arXiv v1 PDF** (`arxiv.org/pdf/<id>v1`) serves full text —
confirmed working for S-172. (4) The **Internet Archive is back up** (CDX and the availability API
both answer HTTP 200). (5) **WU Vienna's `fileadmin` tree** serves working papers the old path no
longer does.

**Do not re-run:** `eur-lex.europa.eu` (HTTP 202, zero bytes — use the Cellar or the oj/L_
manifestation URL instead); `socpa.org.sa` direct (times out — use the Internet Archive, which has
the news item but not the endorsement document); `sciencedirect.com` article pages (403);
`ssrn.com` landing pages (403); `socpa.org.sa` endorsement document `…/2905.aspx` (times out, and
**no** Wayback snapshot); `wu.ac.at/fin/…` and `department-of-finance/working-papers/…` (404 — use
the `fileadmin` tree); `keyrock.com/research/…` and `keyrock.com/blog/…` (403); `saudiexchange.sa`
(403); `papers.ssrn.com/…6751741` and every archive form of it (**no snapshot exists**);
`sec.gov/files/rules/exorders/2026/` directory listing (404 — use the direct PDF path form instead).

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

**Residual provenance pool, re-measured this cycle.** Ten of the 25 index-rendered-only entries were
touched in Cycle 103 (S-157, S-159, S-160, S-167, S-274, S-276, S-278, S-280, S-292, S-268). The
residual pool is **15 entries**:
**S-147, S-148, S-151, S-152, S-179, S-181, S-247, S-248, S-249, S-253, S-258, S-262, S-263, S-264,
S-329.**
The **Crossref-deposited-abstract lever is still open on most of them**. Highest-yield members, from
this cycle's reconnaissance:
- **S-181 (Ahmed 2026)** and **S-329 (Sun & Tian 2026)** — both are SSRN `posted-content` records; the
  **Crossref posted-content record** (as used for S-115 and S-125) is the untried route.
- **S-247 (Ellul, Shin & Tonks 2005)** — the LSE working paper dp506 is the target; the LSE
  `research-publications` path is a different path form from the one that failed.
- **S-147, S-148, S-151, S-152, S-179** — Song & Woo (S-179) records the full text as not publicly
  available, so this entry may be **terminal**; a negative recorded as terminal is a legitimate
  outcome. The others remain untried on Crossref.
- **S-253, S-258, S-262, S-263, S-264** — untried on Crossref; no reconnaissance yet.

**What the register now rests on that it did not before.** The EU free-allocation ladder is backed
by the directive text rather than by a briefing; the ASR claim is backed by the correct paper; the
perpetual-funding mechanism is backed by two primary versions and the authors' own CFTC letter; the
tender-offer mechanics are backed by the SEC's own letters; the T+1 India evidence is backed by the
authors' own deposited abstract.

**What the register still does not have.** The *bodies* of S-238 (Switzer), S-153/S-154/S-156's
magnitude claims, S-166's intermediary-borrowing detail, S-271's "all at once" wording and effective
date, and S-172's abstract-level figures (present in the v1 body but absent from all three abstracts).
Each has a named untried route in §2.

---

## 2. Best next research task — Cycle 104

**Priority 1 — maintain the frozen, exhausted and dated items.** Carry §1's frozen, exhausted and
dated list forward unchanged. Re-check R-054 condition (c) and R-055 condition (c) **only if the
calendar has passed their dates** (4 December 2026 and 14 December 2026); on the next cycle's
timeline neither will be due, and neither may be pre-empted.

**Priority 2 — one bounded, pre-registered provenance operation over a named subset of the
residual pool.** This is the highest-yield work available: the pool is 15 entries, and the
**Crossref-deposited-abstract lever is still open on most of them**. **The next agent must
pre-register its own named subset, its routes, and its upgrade/partial/negative criteria in
`research/cycle_notes.md` *before* fetching anything**, and must not exceed a bounded operation.

**Priority 3 — the open questions, with their named routes.**
1. **S-271's "all at once" wording and effective date** — the endorsement document is unreachable
   (host times out; no Wayback snapshot). Untested routes: the **IFRS Foundation's live
   jurisdiction page** for Saudi Arabia
   (`ifrs.org/use-around-the-world/use-of-ifrs-standards-by-jurisdiction/view-jurisdiction/saudi-arabia/`),
   which may carry a **post-2022** profile the PDF does not; the **Saudi Capital Market Authority**
   (`cma.gov.sa`, a different host from the blocked Saudi Exchange); and the **Wayback CDX for the
   Arabic paths** of `socpa.org.sa/Socpa/Professional-standards/…`, which the availability API does
   not index by default.
2. **S-238's body and its introduction summary** — the *conference version* of the paper (presented
   at the Effectiveness of Financial Regulation Conference, Rishon LeTsiyon, June 2022) may be open
   where the journal version is paywalled; the author's Concordia University page and repository
   are the second route.
3. **S-153, S-154, S-156's magnitude claims and S-166's intermediary detail** — the general route is
   the authors' working-paper versions (NBER WP 28624 for S-156) or the SSRN preprints, since the
   publisher routes are blocked.

**Priority 4 — lossless housekeeping.** Re-derive every count from the files; re-run the rubric
arithmetic; keep the frozen, exhausted and dated items; write the annotations **into the entries in
the same cycle**; keep the known-baseline table, the register, the shortlist, the validation
handoffs and the rejected-and-parked file consistent with each other; do not move, relabel,
renumber or re-scope anything to tidy a file; do not write the cycle log late.

**Priority 5 — rewrite the handoff** at the end of the session and write a fresh, self-contained
initial task message for Cycle 105.

**Out of scope, permanently:** backtests, simulations, parameter sweeps, optimisation, significance
testing on strategy results, performance or risk metrics, market-data acquisition or processing,
strategy or signal implementation, executable research infrastructure, job or workflow launches,
changes to workflow files, tests, credentials or infrastructure, work in other repositories, and any
trading. The canonical prompt `research_prompts/systematic_edge_discovery_agent_prompt.txt` is
maintainer-owned and must not be edited. If a question can only be answered by running something,
write the question down precisely and hand it off; that is the correct output, not a failure.

---

## 3. Initial task message for the next agent (Cycle 104)

> You are the next agent in a **theory-only** hypothesis-generation and research-prioritisation
> repository. You have no prior context beyond the files. Read, in this order, before doing
> anything else:
>
> 1. `AGENTS.md` (the absolute scope boundary — read it first; it is short and binding).
> 2. `research/next_agent_handoff.md` (this file's successor — it has been rewritten at the end of
>    Cycle 103 and is the authoritative state).
> 3. `research/idea_register.md`, `research/ranked_shortlist.md`, `research/source_ledger.md`.
> 4. `research/validation_handoffs.md`, `research/rejected_and_parked.md`, `research/cycle_notes.md`
>    (read the Cycle-103 record at the end).
>
> **What Cycle 103 was.** Cycle 103 was a provenance cycle, not a screening cycle. It ran one
> bounded, pre-registered provenance operation over thirteen source entries (ten from the residual
> 25-entry pool plus three Priority-3 close-attempts), recorded **six upgrades** (S-157, S-160,
> S-167, S-274, S-115, S-172), **six honest negatives** (S-159, S-276, S-278, S-280, S-292, S-268),
> and **one new entry S-383** (the 16 April 2026 SEC equity exemptive order, a different instrument
> from S-382's debt order). It closed **Priority 3(1)** (S-115's SSRN abstract via Crossref
> posted-content), **Priority 3(4)** (S-172's v1 body — "~2% vs ~10%" confirmed present in the body)
> and **Priority 3(5)** (the equity exemptive order fetched and line-verified). It created **no**
> candidate, changed **no** score, opened or closed **no** gap, and touched **no** validation
> specification. All thirteen annotations were written into their ledger entries in the same cycle.
>
> **What you must do this cycle.**
> - **Priority 1.** Carry the frozen, exhausted and dated items forward unchanged: G-32 limb (c) and
>   G-33 (dated 2027 Q3), G-14 (dated 29 March 2029), IDEA-014's state-free existence limb
>   (inconclusive, five-reason register exhausted), G-21 (open), G-28 (frozen), G-30 (exhausted),
>   V-002 (frozen), V-010 (never-to-execute), and the two dated SEC comment deadlines R-054(c)
>   4 December 2026 and R-055(c) 14 December 2026 — **neither of which has arrived**.
> - **Priority 2.** Run **one bounded provenance operation over a named subset of the 15 remaining
>   index-rendered-only entries** listed in §1 of the handoff (S-147, S-148, S-151, S-152, S-179,
>   S-181, S-247, S-248, S-249, S-253, S-258, S-262, S-263, S-264, S-329). **Write the pre-registered
>   list — target, route, and what would count as an upgrade, a partial upgrade and a negative —
>   into `research/cycle_notes.md` BEFORE you fetch anything.** The general lever that worked in
>   Cycle 103 is **the Crossref REST API's deposited abstract** (`api.crossref.org/works/<DOI>`),
>   which is still open on most of that pool; for SSRN posted-content records (S-181, S-329) use
>   the Crossref `posted-content` form. Record for every fetch the URL, the **HTTP status**, the
>   **byte count**, the **page or character count** and the extraction method.
> - **Priority 3.** Close the open questions in §2 of the handoff: S-271's "all at once" wording
>   and effective date, S-238's body, S-153/S-154/S-156 magnitude claims, S-166 intermediary detail,
>   each with its named route.
> - **Priority 4.** Re-derive every count from the files, re-run the rubric arithmetic, and keep the
>   register, the shortlist, the ledger, the validation handoffs and the rejected-and-parked file
>   consistent with one another. Move, relabel, renumber and re-scope nothing.
> - **Priority 5.** Rewrite `research/next_agent_handoff.md` at the end of the session and write a
>   fresh, self-contained initial task message for Cycle 105.
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
> `S-001…209`, `S-220…383` (S-381, S-382, S-383 now exist; S-210 … S-219 reserved and unused),
> `V-001…010`, `R-001…055`, `P-001…012`, `P-014` (P-013 retired), `G-01…36`, `Cycle 1–103`.
> **Next free identifiers: IDEA-017, S-384, V-012, G-37, R-056, P-015.** Continue each series; never
> restart one.
