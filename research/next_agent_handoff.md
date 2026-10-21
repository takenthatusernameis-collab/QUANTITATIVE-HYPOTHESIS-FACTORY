Last updated: 2026-10-21, **Cycle 100 complete**. Cycle 100 executed the **bounded provenance-upgrade
operation** the Cycle-99 handoff had specified, and it also **repaired a state-integrity defect in the
prior cycle**: the Cycle-99 handoff header and cycle log recorded two provenance upgrades (S-208 and
S-136) and a rewritten handoff, but **the ledger carried no Cycle-99 annotation at all** — the S-208
upgrade never reached the artifact, and S-136 has been line-verified since it was minted, so it was never
an index-rendered entry. Cycle 100 therefore performed the S-208 upgrade itself and wrote the
annotation the prior session recorded but did not write, and it rewrote the handoff in full, body and
header. The cycle's work was **evidence work, not a screen**: **sixteen entries were upgraded to
line-verified** (S-208, S-209, S-226, S-234, S-235, S-236, S-237, S-202, S-108, S-110, S-116, S-119,
S-120, S-169, S-230, and S-238 at bibliographic level only), **two are partially upgraded with the unverified
parts named** (S-187 — a live tracker whose 16 October 2026 figures are not reproducible and are struck
in place; and S-238's quotations, which Crossref does not carry), and **three are honest negatives with
their failure modes recorded** (S-115, S-229, S-271). The operation consumed **no identifier** and
**no score**. Housekeeping was lossless and the **rubric-arithmetic re-run was clean**: IDEA-011
4/3/3/4/2/5 = 69.0; IDEA-004 4/4/1/3/3/3 = 63.0; IDEA-009 3/3/1/3/2/4 = 53.0; IDEA-014 3/2/3/2/2/4 =
52.0; IDEA-010 4/4/1/2/2/2 = 55.0. Counts re-derived from the files: **15 dossiers, 370 verified
sources, 10 validation specifications, 55 rejections, 13 parking records (12 active), 92-row
known-baseline table, gaps G-01 … G-36**. The provenance pool, re-measured with the rule as stated
below, now stands at **45 index-rendered-only entries and 96 mixed entries**. Next free identifiers:
**IDEA-017, S-381, V-012, G-37, R-056, P-015**. Next cycle: **Cycle 101**.

---

## 1. State of the pipeline (counts re-derived from the artifact files, Cycle 100 complete)

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
| Provenance pool (re-measured, Cycle 100) | **45 index-rendered-only · 96 mixed · 220 with no index-render wording** | over the 361 heading-form entries. The inherited figure was 57 / 85; the **+5 / −6** residual is a **detector** difference, disclosed in the ledger's Cycle-100 record, and **no earlier cycle's figures are restated** |

**Next free identifiers: IDEA-017 · S-381 · V-012 · G-37 · R-056 · P-015.** Reserved and unused:
IDEA-016, S-210 … S-219, V-011, P-013.

### 1.1 What Cycle 100 established (the substance the next agent inherits)

- **The FR Y-9C submission deadlines are line-verified** (S-226), from the Federal Reserve's **own
  instructions** (June 2026 edition, 618 pages), reached through a route that did not exist when the
  entry was written: the Board has **restructured its reporting-forms material into an application**,
  and every previously documented path still 404s and the FFIEC National Information Center still 403s.
  The verbatim text: "The submission date for holding companies is **40 calendar days** after the March
  31, June 30, and September 30 as-of dates unless that day falls on a weekend or holiday … The
  submission date for holding companies is **45 calendar days** after the December 31 as of date." This
  **strengthens G-23's cadence limb** for IDEA-010.
- **The public-availability half of that entry is corrected** (S-226): the form's own index page names
  the Federal Reserve Bulletin, the BHCPR and the Board's **Freedom of Information Office** — **not** the
  National Information Center — and the strings "National Information Center" and "made available as
  received" return **zero** hits in the 618-page instructions. The release-lag sub-claim is now marked
  unverified rather than silently carried.
- **FINRA Rule 8312's enumerated BrokerCheck release set is line-verified** (S-234) and contains **no
  firm-level net capital** — which **strengthens G-27 limb 1's route selection** for IDEA-010 — and
  **no IAPD**, so the entry's IAPD element is struck. The *Industry Snapshot* limb is **not** upgraded:
  both implied FINRA paths return **HTTP 404**.
- **The Rule 201 facts are line-verified against the regulator's own text** (S-235): the 10 % trigger,
  the restriction lasting "for the remainder of the day and the following day", the intra-day
  re-trigger, the "short exempt" marking under Rule 201(c), and the 28 February 2011 compliance date.
- **The RFS regulation's own text is now line-verified, and it corrects the register's arithmetic
  source** (S-202): 40 CFR 80.1405 was read through the **eCFR renderer endpoint**, which returns the
  section's full text where the versioner endpoint (406) and the human-facing page (navigation chrome
  only) do not. Table 1 (annual percentage standards, 2010 → 2027), the percentage-standard equations,
  the **GEi/DEi** exemption terms and the small-refinery-exemption reallocation volumes are all
  confirmed verbatim. **Correction**: the regulation does **not** state the volumes in "billion RINs"
  (zero hits) — it states **percentages** in Table 1 and **gallon-RINs** in the formula terms; the
  billion-RIN figures are the **agency's summary presentation (S-203)**. **A dated observation that
  bears on G-20 and on IDEA-014's state**: the current text carries standards through **2027** and the
  string "2028" returns **zero** hits, so the 2028 standards are not yet in the section.
- **S-208's two unsupported items are struck** (see §2, Priority 3): "guaranteed delivery of tenders by
  the close of business on the second business day after expiration" and the "(7–10 calendar days)"
  day-count for the abbreviated investment-grade cash tender are **not in the fetched document**; the
  document's own words are "an abbreviated **five-day** offer period" for the 2015 no-action letter, and
  the 1986 relief is described with no day count at all.
- **S-237 has three authors, not one** (Rainer Brand, Matthias Molnar, Angel Tengulov), and the entry's
  quoted fragment is aligned to the deposited abstract's wording. The four magnitudes (+61 % / +87 % /
  +40 % / +80 %) and the paper body **remain closed**.
- **S-209's document is a slide deck**, not a note, and its "Dutch/modified-Dutch auctions for non-US
  holders" phrase is narrowed to what the document supports ("Modified Dutch" and "reverse Dutch" return
  **zero** hits).
- **S-187 is a live tracker**: the entry's 16 October 2026 figures (389 filings; 78 of 101 dispositions)
  and the "1,792 remaining shares" footnote are **not reproducible** from the fetched page and are
  struck; the page's structure and its per-filing 10b5-1 flags are confirmed at the fetch date
  (20 October 2026: 58 % of dispositions pre-arranged). A live page is a moving target and must always
  be cited with its fetch date.

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
| SSRN direct (papers.ssrn.com, and the DOI resolver → ssrn.com/abstract=…) | **HTTP 403** | S-115 (Cycle-100 attempt; Cycle-97 attempt) |
| The **Internet Archive** (CDX index and replay) | **"Internet Archive: Temporarily Offline" for the whole session on 21 October 2026** — the route that worked in Cycle 98 was unavailable this cycle | S-115 (Cycle-100 attempt) |
| European Parliament document server (`europarl.europa.eu/RegData/…`, and the thinktank document page) | **HTTP 202 with a zero-byte body** on all four URL forms — the host generates asynchronously and never delivered the file | S-229 (Cycle-100 attempt) |
| `socpa.org.sa` (news item and publications page) | **connection timeout**, no response after 50 s, on both pages | S-271 (Cycle-100 attempt) |
| `sciencedirect.com` article pages | **HTTP 403** (Elsevier robot block) | S-238 (Cycle-97 attempt; not re-run) |
| `ffiec.gov/nic/` | **HTTP 403** | S-226 (Cycle-97 attempt; superseded by a working route) |
| `federalreserve.gov/reportforms/form9c.htm`, `form9c.pdf`, `form9c-instructions.pdf` | **HTTP 404** — the path set no longer exists | S-226 (Cycle-97 attempt) |
| WU Vienna working-paper page | **404 / 403**; superseded in Cycle 100 by the Crossref posted-content record for the SSRN DOI | S-237 |
| SEC direct fetch **without** a declared contact User-Agent | **HTTP 403** — with a compliant User-Agent the same URL returned **200** | S-169 (Cycle-97 attempt) |
| `finra.org/rules-guidance/key-topics/industry-snapshot`, `.../annual-reports/2026-annual-report` | **HTTP 404** | S-234 (Cycle-100 attempt) |

### 1.4 Working routes established or confirmed in Cycle 100 (use these; do not re-discover them)

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
   abstract** for many journals, and it carries **SSRN `posted-content` records** — which is how S-237's
   deposited abstract and S-236's abstract were obtained, and how S-238's bibliographic record was
   confirmed. This is a general, scalable lever for the remaining journal entries.
4. **The OpenAlex REST API** `https://api.openalex.org/works/doi:<DOI>` confirms **identity, authors,
   host and open-access status**, and carries an **abstract inverted index** for some works — but it
   carried **no abstract** for S-115.
5. **Fetchable this cycle**: `cliffordchance.com` (with the capitalised "US" path), `mayerbrown.com`,
   `chicagofed.org` (landing page **and** the article PDF), `tradersmagazine.com`, `thevx.io`,
   `climate.ec.europa.eu` (the path has moved `/eu-action/` → `/areas-action/`), `eea.europa.eu`,
   `finra.org` (rulebook and notices), `dehst.de`, `sec.gov` files, `federalreserve.gov`.
6. **The Internet Archive was offline for the whole session** — re-test before relying on any archive
   route, and prefer a live source.
7. **The eCFR renderer endpoint** `https://www.ecfr.gov/api/renderer/v1/content/enhanced/current/title-<N>?part=<P>&section=<S>`
   returns the **full section text** (HTTP 200, ~18 KB) where the **versioner** endpoint
   (`/api/versioner/v1/full/…`) returns **HTTP 406** and the human-facing
   `ecfr.gov/current/…` page returns navigation chrome only. Use the renderer for CFR text, and
   remember that a CFR section states **percentages and gallon-RINs**, not billion-RINs.

---

## 2. Best next research task (Cycle 101)

The register's named absent families remain **exhausted**; **do not** invent a screen to fill a slot, and
**do not** re-run a route that already returned a negative unless a *new* route exists. The next cycle's
substantive work should be **one bounded, pre-registered provenance operation over the remaining
index-rendered entries**, plus the specific questions Cycle 100 left open.

### Priority 1 — Maintain the frozen, exhausted and dated items as they stand
No re-search of the items in §1.2. Re-check the two dated rulemaking items only when their dates
arrive, and record the outcome then.

### Priority 2 — One bounded provenance operation over the remaining 45 index-rendered-only entries
**Pre-register the subset and the route for each entry before fetching anything** (the Cycle-99 failure
mode was fetching without a written route and then not writing the annotation back). The named subset
below is chosen for **fetchability** and for **how much of the register rests on the entry**:

| Target | What it supports | Route to try first |
| --- | --- | --- |
| **S-102** | Directive 2003/87/EC, Articles 12(3) and 16(2)–(4) | **EUR-Lex** consolidated text (HTML and PDF) |
| **S-103** | European Commission (2023) and Directive (EU) 2023/959 — the move of the surrender deadline | **EUR-Lex** (the 2023 amending directive) and the Commission's own note |
| **S-106** | DEHSt auction-calendar notices | **dehst.de** (fetchable this cycle) |
| **S-118** | NY Fed FX Committee minutes, 22 May 2024 | **newyorkfed.org** |
| **S-027** | Da, Engelberg & Gao (2011) | the **NBER working-paper PDF**, else the Crossref abstract |
| **S-064** | Wang (2026) — the funding-state FX baseline | **Crossref** / SSRN record via `api.crossref.org` |
| **S-153** | Driessen, Maenhout & Vilkov (2009) | **Crossref** abstract + the publisher's abstract page |
| **S-158** | Gornall, Xiao & Rinaldi (2025) | **Crossref** abstract, or the NBER/SSRN working version |
| **S-170** | Keyrock (2026) token-unlock event study, quoted in a public document | the **BIS** report PDF that quotes it |
| **S-172** | Lee (2025) — arXiv record | the **arXiv** abstract page and the PDF (`arxiv.org/abs/<id>`) — the entry already has the API metadata; what is missing is the **v3 abstract text** |
| **S-125** | Clapham & Ewald (2026) | **Crossref** / **OpenAlex** / the SSRN record |
| **S-154** | Carr & Wu (2009) | **Crossref** abstract (the *Journal of Finance* record) |
| **S-168** | Borenstein, Bushnell, Wolak & Zaragoza-Watkins (2019) | **Crossref** abstract; the working-paper version on the authors' or the regulator's site |

**Rules for the operation.** (a) Record for every entry: the URL fetched, the **HTTP status**, the
**byte count**, the **page or character count**, and the extraction method. (b) A quotation that cannot
be re-checked in the fetched document's text layer is **not a quotation** — extract the text layer or
record the entry as index-rendered and unattributed. (c) **Strike in place** any quotation the fetched
document does not contain, with the reason and the string counts that show the absence; **do not
silently keep it**. (d) Record a **negative** as a negative: the route tried, the status, the failure
mode. (e) An upgrade **may only strengthen an existing reason or record**; it may not re-score, add a
sixth reason, re-screen a family, or consume an identifier. (f) Write the annotation **into the entry
in the same cycle** — a cycle log is a record of intent, the ledger entry is the evidence.

### Priority 3 — Close the specific open questions Cycle 100 created
Each of these is answerable with a *named* route and is a precise, small piece of work:

1. **The two struck S-208 items need a different source, not a re-read.** "Guaranteed delivery of tenders
   by the close of business on the second business day after expiration" and the 1986/2015 abbreviated
   offer-period day-count are **absent from the Clifford Chance note**. The right source is a **tender
   offer document itself** (a Schedule TO or the 8-K/424B announcement, via EDGAR full-text search) or
   the **SEC staff's position**. Frame the question as: *what is the source of the "guaranteed delivery
   … second business day after expiration" mechanic, and what day-count does the 1986 relief and the
   January 2015 no-action letter actually specify?* Until it is answered, neither may be cited.
2. **The two S-238/S-237 bodies.** S-238's two quotations and S-237's four magnitudes are still closed.
   A **Scopus/DOI abstract via the publisher's landing page** (Elsevier blocks, but the *abstract* is
   often served on the `sciencedirect.com/science/article/abs/pii/...` path) or the author's own
   working-paper version is the route; a **CERN/SSRN/NBER mirror** is the alternative. Record a negative
   if neither opens.
3. **S-234's Industry Snapshot.** Find the current FINRA URL for the firm-level statistics pages (the
   two implied paths 404). The question: *does FINRA publish firm-level net capital or only
   aggregate-by-size-bucket tables, and at what URL?* If only aggregate tables exist, say so and record
   it — it is the same negative the register already relies on.
4. **S-229's free-allocation percentages.** Do **not** re-try the European Parliament host (HTTP 202,
   zero bytes). The same figures are in **EUR-Lex** (Directive (EU) 2023/959) and in the Commission's
   own guidance. Confirm the percentages against the **directive text** and record the naming trap
   (retention factor 97.5 % vs obligation share 2.5 % in 2026) wherever the number is used.
5. **S-271's SOCPA wording.** The host timed out; a different host is needed (the site's alternate
   language paths, or the Saudi Exchange / the IFRS Foundation's own endorsement record for Saudi
   Arabia). The question: *does SOCPA itself say IFRS 18 must be applied "all at once", and what is the
   effective date?* An IFRS Foundation or IFRS Advisable Council record would be a stronger source
   than the issuer's own page.
6. **S-115** — retry the archive route **only when the Internet Archive is up**, and pair it with the
   OpenAlex identity already confirmed.
7. **S-136** — take no action. It is line-verified and must not be counted in any pool measurement
   again.

### Priority 4 — Lossless housekeeping and a rubric-arithmetic re-run
Re-run `Weighted total = Σ (dimension score × weight) / 5` (weights 25/20/15/15/15/10; per-point values
5.0/4.0/3.0/3.0/3.0/2.0) for all four active candidates and the parked IDEA-010, and record the result.
Re-derive every count from the files. **Move, relabel, renumber or re-scope nothing.**

### Priority 5 — Rewrite this handoff and write a fresh, self-contained initial task message
Leave the session with an updated `research/next_agent_handoff.md` and a fresh initial task message for
Cycle 102, and a Cycle-101 record **inside** the cycle that did the work (never a cycle late).

### Highest-value unresolved theoretical questions (unchanged, and still unresolved)
1. Does an **accounting-standards adoption** (IFRS 18 / ASC 350) create a *measurable*, dated
   information-diffusion clock across filers, separable from a mechanical window-dressing explanation?
   (IDEA-011, rank 1; the sample-size condition is the binding constraint.)
2. Is a **crowding-conditioned** slow-capital decay (IDEA-004) sign-stable once the conditioning is
   estimated rather than assumed, and does it survive the cost-over-65 % gate?
3. Is the **perpetual-futures funding rate** a market-wide measure of speculative demand that transfers
   across venues, or a venue artefact with a momentum confound? (IDEA-009.)
4. Does the **EU ETS surrender deadline** concentrate flows enough to move prices, and is the concession
   visible ex ante? (IDEA-013, parked; G-13's decision-time sample.)
5. Does a **dealer balance-sheet constraint** bind corporate-bond ETF discounts, and is the state
   quarterly and lagged? (IDEA-010, parked: yes to the second, unproved on the first.)

---

## 3. Your task — Cycle 101

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

**Your task for Cycle 101, in order:**

1. **Read** `research/next_agent_handoff.md` in full, then the four artifacts named above, then
   `research/cycle_notes.md` (Cycle 100's record) and the ledger's "Cycle-100 provenance-operation
   record" section. Do not skip the ledger section: it carries the state-integrity finding and the
   route list.
2. **Re-derive the counts** from the files (§1) and confirm the **rubric arithmetic** (Priority 4).
   If any count or total disagrees with the files, the **files win**, and the discrepancy is written
   down in the cycle record.
3. **Execute Priority 2**: one bounded, pre-registered provenance operation over the **named subset in
   §2 Priority 2** (thirteen entries, each with a first route). Write the pre-registered list — target,
   route, and what would count as an upgrade, a partial upgrade and a negative — into the cycle record
   **before** fetching anything. Then fetch, extract the text layer, check the entry's quoted passages
   against it, and write the annotation **into each entry in the same cycle**. Strike what the document
   does not contain; record a negative as a negative; carry a URL correction with the correction.
4. **Execute Priority 3**: close as many of the seven specific open questions as you can, each with its
   named route. Do not re-run a route that has already returned a negative unless you have a *different*
   route; do not re-run the European Parliament host, `socpa.org.sa`, `sciencedirect.com` article pages
   or `ffiec.gov/nic/` without a new approach.
5. **Maintain** the frozen, exhausted and dated items as they stand (§1.2). Do not re-run R-055's
   condition (d). Note that R-054's and R-055's rulemaking dates (4 and 14 December 2026) are **not yet
   due**.
6. **Do not create a candidate, re-score, or consume an identifier** unless you find something that
   genuinely demands it; if you do, the reasoning must be written in the register, the shortlist and the
   cycle log together. An upgrade to an existing entry is **not** a reason to re-score.
7. **Finish** by rewriting `research/next_agent_handoff.md` in full (header, §1, §2, §3), re-deriving
   every count, and writing a **fresh, self-contained initial task message** for Cycle 102; add the
   Cycle-101 record to `research/cycle_notes.md` **in the same cycle**; update the header notes in
   `idea_register.md`, `ranked_shortlist.md`, `validation_handoffs.md`, `rejected_and_parked.md` and
   `research/README.md`; and leave the next free identifiers correct: **IDEA-017, S-381, V-012, G-37,
   R-056, P-015** (unless you consume one, in which case say so in the handoff and in the README).

**What you must not do:** invent a citation; present an index-rendered quotation as a parsed document;
let a "fetched directly" verification line stand on a document that was in fact unreachable; move,
relabel or renumber an existing identifier to tidy a file; edit
`research_prompts/systematic_edge_discovery_agent_prompt.txt` (maintainer-owned); or write a cycle
record a cycle late.

**What success looks like for Cycle 101:** a larger set of entries whose quoted passages have been
re-checked in a document actually fetched and parsed, with the ones that fail **struck in place**; the
seven open questions answered or explicitly left open with the routes tried; the counts and the rubric
re-derived from the files; and a handoff that a new agent can act on without re-reading forty cycles of
history.
