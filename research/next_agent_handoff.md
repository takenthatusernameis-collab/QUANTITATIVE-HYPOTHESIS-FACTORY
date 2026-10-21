Last updated: 2026-10-21, **Cycle 101 complete**. Cycle 101 executed the **bounded provenance-upgrade
operation** over the thirteen named targets of the Cycle-100 handoff, and it also **attempted to close
the seven Priority-3 open questions**. The cycle's work was **evidence work, not a screen**: **ten
entries were upgraded to line-verified** (S-027, S-064, S-103, S-106, S-118, S-125, S-153, S-154,
S-168, S-170), **one was partially upgraded with the unverified part named** (S-172 — its Sharpe
0.22/0.39 and momentum 2% vs 10% figures are struck pending version re-attribution), and **two are
honest negatives with their failure modes recorded** (S-102 via EUR-Lex HTTP 202 zero-byte; S-158 via
Crossref bibliographic discrepancy with no abstract deposited). **No identifier was consumed and
no score changed.** Housekeeping was lossless and the **rubric-arithmetic re-run was clean**: IDEA-011
4/3/3/4/2/5 = 69.0; IDEA-004 4/4/1/3/3/3 = 63.0; IDEA-009 3/3/1/3/2/4 = 53.0; IDEA-014 3/2/3/2/2/4 =
52.0; IDEA-010 4/4/1/2/2/2 = 55.0. Counts re-derived from the files: **15 dossiers, 370 verified
sources, 10 validation specifications, 55 rejections, 13 parking records (12 active), 92-row
known-baseline table, gaps G-01 … G-36**. The provenance pool, re-measured with the rule as stated,
now stands at **34 index-rendered-only entries and 107 mixed entries** (plus 220 entries with no
index-render wording, over 361 heading-form entries). S-158's bibliographic discrepancy and S-102's
exhausted EUR-Lex route are recorded as the two remaining failures of this cycle's named subset.
Next free identifiers: **IDEA-017, S-381, V-012, G-37, R-056, P-015**. Next cycle: **Cycle 102**.

---

## 1. State of the pipeline (counts re-derived from the artifact files, Cycle 101 complete)

| Item | Count | Detail |
| --- | --- | --- |
| Dossiers (`idea_register.md`) | **15** | 4 active · 6 parked · 5 rejected (dossiers not maintained) |
| Ranked, active candidates | **4** | **IDEA-011 ACCTCLOCK 69.0 (rank 1) · IDEA-004 SLOWCAP-COND 63.0 (rank 2) · IDEA-009 PERP-FUND 53.0 (rank 3) · IDEA-014 RIN-DEADLINE 52.0 (rank 4)** |
| Parked at a terminal score | **1** | **IDEA-010 CREDIT-ETF 55.0** (P-014, Cycle 78; G-34 kill condition fired) |
| Verified sources (`source_ledger.md`) | **370** | S-001 … S-209, S-220 … S-380; S-210 … S-219 reserved and unused; 360 in heading form + 10 bold inline (S-281 … S-290); one sub-heading inside S-358 is **not** a second entry |
| Validation specifications | **10** | V-001 … V-010; **executable: V-008, V-009**; V-002 frozen; **V-010 never-to-execute**; V-001, V-003 … V-007 not executable. **Nothing in this repository was executed** |
| Rejections | **55** | R-001 … R-055 |
| Parking records | **13** | P-001 … P-012, P-014 — 12 active; P-004 closed by R-038 |
| Known-baseline table | **92 rows** | reference set, not candidates; no row added or removed this cycle |
| Gaps | **G-01 … G-36** | open: **G-21** (EA-ERA), **G-28** (frozen), **G-30** (exhausted). G-17 and G-26 skipped by the sequence and never used |
| Provenance pool (re-measured, Cycle 101) | **34 index-rendered-only · 107 mixed · 220 with no index-render wording** | over the 361 heading-form entries. Cycle 101 moved 11 entries out of index-rendered-only (ten fully upgraded plus S-172 partial); two stayed (S-102, S-158) |

**Next free identifiers: IDEA-017 · S-381 · V-012 · G-37 · R-056 · P-015.** Reserved and unused:
IDEA-016, S-210 … S-219, V-011, P-013.

### 1.1 What Cycle 101 established (the substance the next agent inherits)

- **S-027 (Da, Engelberg & Gao 2011, J. Finance 66(5):1461–1499)** — upgraded via Crossref REST API and the NBER working-paper record; the attention–price/reversal claims are confirmed against the deposited bibliographic record.
- **S-064 (Wang 2026, SSRN 6152329)** — upgraded via `api.crossref.org`; the posted-content abstract confirms the funding-state FX baseline hypothesis and the HML× results.
- **S-103 (EC 2023 / Directive (EU) 2023/959)** — upgraded via `climate.ec.europa.eu`; the 30 April → 30 September surrender-deadline passage is confirmed verbatim in the Commission's own news item.
- **S-106 (DEHSt auction-calendar notices)** — upgraded via `dehst.de`; the MSR/TNAC and auction-calendar passages are confirmed verbatim, and the 1 October 2026 Commission news item confirms the 140 million allowances for the Social Climate Fund and Mon/Tue/Thursday auction days from 7/18 January.
- **S-118 (NY Fed FX Committee minutes, 22 May 2024)** — upgraded via `newyorkfed.org` (PDF, 273,548 bytes, 3 pages, 6,938 chars via pypdf); the "uptick in price premium and market impact for trades executed later in the NY trading day" sentence is confirmed verbatim.
- **S-125 (Clapham & Ewald 2026, SSRN 7552327)** — upgraded via Crossref/OpenAlex; the posted-content abstract confirms the Bitcoin ETF difference-in-differences findings.
- **S-153 (Driessen, Maenhout & Vilkov 2009, J. Finance 64(3):1377–1406)** — upgraded via Crossref-deposited abstract; the single-name variance-risk-premium sign claim is confirmed.
- **S-154 (Carr & Wu 2009, RFS 22(3):1311–1341)** — upgraded via Crossref; journal, volume, issue and pages confirmed. A minor title discrepancy is recorded: Crossref deposits "Variance Risk Premiums" where the ledger records "Variance Risk Premia"; the single-name-VRP claim is confirmed against the deposited abstract.
- **S-168 (Borenstein et al. 2019, AER 109(11):3953–3977)** — upgraded via Crossref-deposited abstract; the price-collar design claim is confirmed.
- **S-170 (Keyrock 2026 token-unlock event study)** — upgraded via `keyrock.com` ("From Locked to Liquidity", 5 December 2024); 90% negative price pressure, 30-day pre-unlock drift, team unlocks at −25% are confirmed. The named BIS report route was not located; the primary document was fetched directly.
- **S-172 (Lee 2025, arXiv:2512.11913)** — partially upgraded: the v3 abstract page was fetched directly and parsed. The Sharpe 0.22/0.39 and momentum 2% vs 10% figures cited in the ledger are **not** in the v3 abstract (they are from an earlier version); a version-drift note is required and the figures are struck pending re-attribution.
- **S-158 (Gornall, Xiao & Rinaldi 2025, SSRN 5036933)** — honest negative: the Crossref record deposits the title "Funding Payments Crisis-Proofed Bitcoin's Perpetual Futures" with author order Gornall/Rinaldi/Xiao, differing from the ledger's "Perpetual Futures and Basis Risk" / Gornall/Xiao/Rinaldi; no abstract is deposited; no working version was located. Bibliographic discrepancy flagged; entry remains index-rendered.
- **S-102 (Directive 2003/87/EC, Articles 12(3) and 16(2)–(4))** — honest negative: EUR-Lex returned HTTP 202 with a zero-byte body on all attempted URL forms (same failure mode as S-229's European Parliament host). Route exhausted; entry remains index-rendered; recorded as a failed retrieval.

### 1.2 Items that remain frozen, exhausted or dated — maintain them as they stand

| Item | Status | Date / condition |
| --- | --- | --- |
| G-32 limb (c) | frozen | 2027 Q3 |
| G-14 (IDEA-008 unblocking) | dated | 29 March 2029 |
| G-21 (EA-ERA) | open | — |
| G-28 | frozen | — |
| G-30 | exhausted | all four sub-routes closed; **V-010 remains non-executable** |
| IDEA-014's state-free existence limb | inconclusive | — |
| R-054 re-screen condition (c) — SEC "Interval Fund Modernization" | **not yet due** | comments closed **4 December 2026** |
| R-055 re-screen condition (c) — MSRB Rule G-32 | **not yet due** | comments due **14 December 2026** |
| R-055 re-screen condition (d) — "Muni Monday" route | **negative in Cycle 98; not a debt** | do not re-run |

**Both rulemaking dates are still in the future on 21 October 2026.** Neither is due; neither may be
pre-empted by a route that has not yet produced a document.

### 1.3 Honest negatives carried forward (failure modes, not re-runnable debts)

| Route | Failure mode | Where |
| --- | --- | --- |
| EUR-Lex / European Parliament document server (`europarl.europa.eu/RegData/…`, and the thinktank document page) | **HTTP 202 with a zero-byte body** on all URL forms — the host generates asynchronously and never delivered the file | S-102 (Cycle 101 attempt); S-229 (Cycle 100 attempt) |
| `socpa.org.sa` (news item and publications page) | **connection timeout**, no response after 50 s, on both pages | S-271 (Cycle 101 attempt) |
| `sciencedirect.com` article pages | **HTTP 403** (Elsevier robot block) | S-238 (Cycle-97 attempt; not re-run) |
| EDGAR full-text search (`efts.sec.gov/LLD/searchtext`) | **HTTP 403** even with a compliant User-Agent | S-208 (Cycle 101 attempt) |
| SSRN direct (`papers.ssrn.com`, and the DOI resolver → ssrn.com/abstract=…) | **HTTP 403** | S-115 (Cycle 101 attempt; Cycle-97 attempt) |
| The **Internet Archive** (CDX index and replay) | **"Internet Archive: Temporarily Offline" for the whole session on 21 October 2026** — the route that worked in Cycle 98 was unavailable | S-115 (Cycle 101 attempt) |
| `ffiec.gov/nic/` | **HTTP 403** | S-226 (Cycle-97 attempt; superseded by a working route) |
| `federalreserve.gov/reportforms/form9c.htm`, `form9c.pdf`, `form9c-instructions.pdf` | **HTTP 404** — the path set no longer exists | S-226 (Cycle-97 attempt) |
| `finra.org/rules-guidance/key-topics/industry-snapshot`, `.../annual-reports/2026-annual-report` | **HTTP 404** | S-234 (Cycle 100 attempt; the Industry Snapshot limb remains not upgraded) |

### 1.4 Working routes established or confirmed (use these; do not re-discover them)

1. **A compliant User-Agent with a declared contact address unlocks `sec.gov`.** With
   `User-Agent: <name> research contact: <email>` the roundtable PDF returned **HTTP 200, 2,118,668
   bytes**; the same pattern returned 200 for the press release and the Rule 201 FAQ page. Without it,
   `sec.gov` returned 403 in earlier cycles. The same pattern was used for the Federal Reserve's
   application download endpoint.
2. **The Federal Reserve's reporting-forms application**
   (`https://www.federalreserve.gov/apps/ReportingForms/`): the form index is
   `…/Report/Index/<FORM_ID>` (e.g. `FR_Y-9C`) and the attachments are served from
   `…/Download/DownloadAttachment?guid=<GUID>`. The FR Y-9C instructions PDF (4,204,476 bytes, 618
   pages) was read this way. This route did not exist in Cycle 97.
3. **The Crossref REST API** `https://api.crossref.org/works/<DOI>` returns the **publisher-deposited
   abstract** for many journals, and it carries **SSRN `posted-content` records** — which is how
   S-064's, S-125's, S-153's, S-154's and S-168's abstracts were obtained, and how S-237's and S-238's
   bibliographic records were confirmed. This is a general, scalable lever for the remaining journal
   entries.
4. **The OpenAlex REST API** `https://api.openalex.org/works/doi:<DOI>` confirms **identity, authors,
   host and open-access status**, and carries an **abstract inverted index** for some works — but it
   carried **no abstract** for S-115.
5. **Fetchable this cycle**: `cliffordchance.com` (with the capitalised "US" path), `mayerbrown.com`,
   `chicagofed.org` (landing page **and** the article PDF), `tradersmagazine.com`, `thevx.io`,
   `climate.ec.europa.eu` (the path has moved `/eu-action/` → `/areas-action/`), `eea.europa.eu`,
   `finra.org` (rulebook and notices), `dehst.de`, `sec.gov` files, `federalreserve.gov`, `newyorkfed.org`,
   `keyrock.com`, `arxiv.org`.
6. **The Internet Archive was offline for the whole session** — re-test before relying on any archive
   route, and prefer a live source.
7. **The eCFR renderer endpoint** `https://www.ecfr.gov/api/renderer/v1/content/enhanced/current/title-<N>?part=<P>&section=<S>`
   returns the **full section text** (HTTP 200, ~18 KB) where the **versioner** endpoint
   (`/api/versioner/v1/full/…`) returns **HTTP 406** and the human-facing
   `ecfr.gov/current/…` page returns navigation chrome only. Use the renderer for CFR text.

---

## 2. Best next research task (Cycle 102)

The register's named absent families remain **exhausted**; **do not** invent a screen to fill a slot,
and **do not** re-run a route that already returned a negative unless a *new* route exists. The next
cycle's substantive work should be **one bounded, pre-registered provenance operation over the
remaining index-rendered-only entries**, plus the open Priority-3 questions.

### Priority 1 — Maintain the frozen, exhausted and dated items as they stand

No re-search of the items in §1.2. Re-check the two dated rulemaking items only when their dates
arrive, and record the outcome then.

### Priority 2 — One bounded provenance operation over the remaining index-rendered-only entries

**Pre-register the subset and the route for each entry before fetching anything.** The named subset
below is chosen for **fetchability** and for **how much of the register rests on the entry**. S-102
and S-158 are named retries with *different* routes from their Cycle-101 failures; the remaining
slots should be filled from the ~32 other index-rendered-only entries by reviewing each entry's own
verification bullet in `source_ledger.md` (entries whose verification reads "index-rendered" or
"search-index render" are candidates; entries already upgraded are not).

| Target | What it supports | Route to try first |
| --- | --- | --- |
| **S-102** | Directive 2003/87/EC, Articles 12(3) and 16(2)–(4) | **Do not re-try EUR-Lex** (HTTP 202 zero-byte, exhausted). Try the Commission's own copy of Directive (EU) 2023/959 or the amending directive on `climate.ec.europa.eu` / `eur-lex.europa.eu` with a different path form. |
| **S-158** | Gornall, Xiao & Rinaldi (2025) | **Do not re-try Crossref** (bibliographic discrepancy, no abstract). Try an NBER/SSRN working version, an author-hosted copy, or OpenAlex for a deposited abstract. |
| *(select 8–10 more)* | from the remaining index-rendered-only entries | review `source_ledger.md` verification bullets; prefer entries with a working direct route (Crossref, OpenAlex, publisher page, regulator site) |

**Rules for the operation.** (a) Record for every entry: the URL fetched, the **HTTP status**, the
**byte count**, the **page or character count**, and the extraction method. (b) A quotation that cannot
be re-checked in the fetched document's text layer is **not a quotation** — extract the text layer or
record the entry as index-rendered and unattributed. (c) **Strike in place** any quotation the fetched
document does not contain, with the reason and the string counts that show the absence; **do not
silently keep it**. (d) Record a **negative** as a negative: the route tried, the status, the failure
mode. (e) An upgrade **may only strengthen an existing reason or record**; it may not re-score, add a
sixth reason, re-screen a family, or consume an identifier. (f) Write the annotation **into the entry
in the same cycle**.

### Priority 3 — Close the open questions from Cycle 101's Priority 3

Six questions remain open (S-234's Industry Snapshot was resolved — FINRA URL located, aggregate-only
net capital confirmed; S-136 is explicitly no-action). Each is answerable with a *named* route:

1. **The two struck S-208 items need a different source, not a re-read.** "Guaranteed delivery of
   tenders by the close of business on the second business day after expiration" and the 1986/2015
   abbreviated-offer day-count are **absent from the Clifford Chance note**. EDGAR full-text search
   returns HTTP 403 — that route is blocked. The right source is a **tender offer document itself**
   (a Schedule TO or the 8-K/424B announcement, via a compliant-User-Agent EDGAR fetch) or the **SEC
   staff's position**. Frame the question as: *what is the source of the "guaranteed delivery … second
   business day after expiration" mechanic, and what day-count does the 1986 relief and the January
   2015 no-action letter actually specify?* Until it is answered, neither may be cited.
2. **The S-238 body.** Switzer (2023), *Finance Research Letters* 55, 103991 (DOI
   10.1016/j.frl.2023.103991). The ScienceDirect abstract page is reachable and the abstract is
   visible (≈3% synthetic short-sale discount; options spread increases), but the full body is paywalled
   (HTTP 403). Try the author's working-paper version, a CERN/SSRN/NBER mirror, or the publisher's
   landing page abstract path. Record a negative if none opens.
3. **The S-237 body.** Four magnitudes (+61% / +87% / +40% / +80%) remain closed. The SSRN landing
   page returns HTTP 403; OpenAlex confirms authorship but returns no abstract. Try an author-hosted
   copy or a preprint mirror.
4. **S-229's free-allocation percentages.** Do **not** re-try the European Parliament host (HTTP 202,
   zero bytes). The same figures are in **EUR-Lex** (Directive (EU) 2023/959) and in the Commission's
   own guidance. Confirm the percentages against the **directive text** via a different route and record
   the naming trap (retention factor 97.5% vs obligation share 2.5% in 2026) wherever the number is
   used.
5. **S-271's SOCPA wording.** `socpa.org.sa` timed out; a different host is needed (the Saudi Exchange
   or the IFRS Foundation's own endorsement record for Saudi Arabia). The question: *does SOCPA itself
   say IFRS 18 must be applied "all at once", and what is the effective date?* An IFRS Foundation
   record would be a stronger source than the issuer's own page.
6. **S-115.** Retry the archive route **only when the Internet Archive is up**, and pair it with the
   OpenAlex identity already confirmed.

### Priority 4 — Lossless housekeeping and a rubric-arithmetic re-run

Re-run `Weighted total = Σ (dimension score × weight) / 5` (weights 25/20/15/15/15/10; per-point values
5.0/4.0/3.0/3.0/3.0/2.0) for all four active candidates and the parked IDEA-010, and record the result.
Re-derive every count from the files. **Move, relabel, renumber or re-scope nothing.**

### Priority 5 — Rewrite this handoff and write a fresh, self-contained initial task message

Leave the session with an updated `research/next_agent_handoff.md` and a fresh initial task message for
Cycle 103, and a Cycle-102 record **inside** the cycle that did the work (never a cycle late).

---

## 3. Your task — Cycle 102

You are the next agent in a **theory-only** research environment. Read this file first, then
`research/idea_register.md`, `research/ranked_shortlist.md` and `research/source_ledger.md`, before
generating anything.

**The mission.** Produce and prioritise *falsifiable hypotheses* about market structure and market
behaviour, with the evidence discipline the repository demands. **Not allowed here:** backtests,
simulations, parameter sweeps, optimisation, significance testing on strategy results, performance or
risk metrics, market-data acquisition or processing, strategy or signal implementation, executable
research infrastructure, job or workflow launches, changes to workflow files, tests, credentials or
infrastructure, work in other repositories, and any trading. **Allowed:** reading and summarising
literature, market-structure and venue documentation, exchange and regulator material, and this
repository's own notes; specifying hypotheses, falsifiable predictions, observables and data
requirements; maintaining the theory-only artifacts. If a question can only be answered by running
something, **write the question down precisely and hand it off** — that is the correct output, not a
failure.

**Your task for Cycle 102, in order:**

1. **Read** `research/next_agent_handoff.md` in full, then the four artifacts named above, then
   `research/cycle_notes.md` (Cycle 101's record) and the ledger's "Cycle-101 provenance-operation
   record" section. Do not skip the ledger section: it carries the state-integrity finding and the
   route list.
2. **Re-derive the counts** from the files (§1) and confirm the **rubric arithmetic** (Priority 4).
   If any count or total disagrees with the files, the **files win**, and the discrepancy is written
   down in the cycle record.
3. **Execute Priority 2**: one bounded, pre-registered provenance operation over the **named subset in
   §2 Priority 2** (S-102 and S-158 as named retries with different routes, plus 8–10 more selected
   from the remaining index-rendered-only entries). Write the pre-registered list — target, route, and
   what would count as an upgrade, a partial upgrade and a negative — into the cycle record **before**
   fetching anything. Then fetch, extract the text layer, check the entry's quoted passages against it,
   and write the annotation **into each entry in the same cycle**. Strike what the document does not
   contain; record a negative as a negative; carry a URL correction with the correction.
4. **Execute Priority 3**: close as many of the six open questions as you can, each with its named
   route. Do not re-run a route that has already returned a negative unless you have a *different*
   route; do not re-run EUR-Lex / the European Parliament host, `socpa.org.sa`, `sciencedirect.com`
   article pages, EDGAR full-text search, SSRN direct, or the Internet Archive without a new approach.
5. **Maintain** the frozen, exhausted and dated items as they stand (§1.2). Do not re-run R-055's
   condition (d). Note that R-054's and R-055's rulemaking dates (4 and 14 December 2026) are **not yet
   due**.
6. **Do not create a candidate, re-score, or consume an identifier** unless you find something that
   genuinely demands it; if you do, the reasoning must be written in the register, the shortlist and the
   cycle log together. An upgrade to an existing entry is **not** a reason to re-score.
7. **Finish** by rewriting `research/next_agent_handoff.md` in full (header, §1, §2, §3), re-deriving
   every count, and writing a **fresh, self-contained initial task message** for Cycle 103; add the
   Cycle-102 record to `research/cycle_notes.md` **in the same cycle**; update the header notes in
   `idea_register.md`, `ranked_shortlist.md`, `validation_handoffs.md`, `rejected_and_parked.md` and
   `research/README.md`; and leave the next free identifiers correct: **IDEA-017, S-381, V-012, G-37,
   R-056, P-015** (unless you consume one, in which case say so in the handoff and in the README).

**What you must not do:** invent a citation; present an index-rendered quotation as a parsed document;
let a "fetched directly" verification line stand on a document that was in fact unreachable; move,
relabel or renumber an existing identifier to tidy a file; edit
`research_prompts/systematic_edge_discovery_agent_prompt.txt` (maintainer-owned); or write a cycle
record a cycle late.

**What success looks like for Cycle 102:** a larger set of entries whose quoted passages have been
re-checked in a document actually fetched and parsed, with the ones that fail **struck in place**; the
six open questions answered or explicitly left open with the routes tried; the counts and the rubric
re-derived from the files; and a handoff that a new agent can act on without re-reading forty cycles of
history.
