---
title: Ingest / Query / Lint Log
type: log
visibility: public
status: draft
created: 2026-09-18
updated: 2026-09-18
---

# Log

Append-only record of ingests, queries, and lints.

## 2026-09-18 — INGEST: Candidate Statement (`raw/my-portfolio/RE_Candidate_Statement.pdf`, 7 pp)
First source ingested; the spine document. Discussed takeaways with Reza; settled three
standing publication-policy calls (student quotes allowed anonymized & sparingly;
external/pending grant dollar amounts omitted; collaborator names in glossary only, roles in
prose).

**Pages created**
- Spine: `teaching-philosophy.md`
- Source: `sources/candidate-statement.md`
- Threads: `stress-reduction`, `accessibility`, `self-sufficiency`, `ai-pedagogy`,
  `educational-tools`, `scholarship-and-dissemination`
- Practices: `weekly-group-quizzes`, `midterm-makeup-exams`, `two-part-final-exams`,
  `ai-verification-cycle`, `note-templates`
- Tools: `gpthermo`, `studyguideai`
- Evidence: `morgan-worcester-instructorship`, `stress-reduction-survey-results`,
  `mtlc-external-evaluation`, `teaching-evaluations`
- Updated: `index.md`, `glossary.md`

**Stripped per publication rules**: external evaluator's name; all external/pending grant
dollar amounts; tenure-case framing; individual-attributable student detail (kept only
short anonymized quotes).

**Open items / to reconcile on later ingests**
- Detailed practice pages (mechanics, iteration history, survey charts) to be enriched
  from the **Teaching Portfolio**.
- Confirm the make-up-exam SD (29.4%, per glossary) and the evaluation scale (5-pt).
- Create source pages for each paper as `raw/my-work/` is ingested; the thread pages
  already link to placeholder source slugs (`2023-ebadi-asee`, `2024-ebadi-iec`,
  `2025-brown-asee`, `2026-ebadi-asee`).
- Citation metrics (h-index etc.) pending the CV ingest.

**⚠ Safety flag (raised to Reza, not yet resolved):** the ignore file is named
`gitignore`, not `.gitignore`, so it will NOT protect `raw/` on first `git add`. Must be
renamed before the repo is initialized/committed.

## 2026-09-18 — FIX: renamed `gitignore` → `.gitignore`
Done at Reza's instruction. `raw/`, `.obsidian/`, `.DS_Store` etc. will now be ignored on
first `git add`. (Agent still never runs git; Reza controls all git operations.)

## 2026-09-18 — INGEST: Teaching Portfolio (`raw/my-portfolio/RE_Teaching_Portfolio.pdf`, 41 pp)
Reflective growth narrative (pp 1–6) + appendices A.1–A.10 (image/scanned). Extracted
narrative text with pypdf; installed poppler and rendered A.1 to verify survey figures.
Discussed takeaways; Reza chose to (a) generalize the stress-reduction motivation to
"mental-health challenges" — no deaths/anecdote, softened wording — and (b) tell the
Advanced CAD iteration story qualitatively, keeping only the improved 4.67/4.86 endpoint
(no low starting scores).

**Key finding:** Appendix A.1 is a scanned reprint of the **2023 ASEE paper** (Ebadi &
Sabuncu). Survey figures confirmed: n = 26 (~90% response); 77% / 65.4% / 65.4% / 48% /
38.6% / 65.3% / 76.9%; make-up improvement 40.8% (SD 29.4% now confirmed).

**Pages created**
- Source: `sources/teaching-portfolio.md` (incl. appendix-handling table)
- Practices: `iterative-course-development`, `project-advising` (new)
- Evidence: `stem-peer-academy` (new)

**Pages enriched**
- Practices: `weekly-group-quizzes`, `midterm-makeup-exams`, `two-part-final-exams`,
  `note-templates`, `ai-verification-cycle` (Summer Sandbox / "AI dissection")
- Threads: `stress-reduction` (motivation + terms), `accessibility` (flow-viz gap;
  access+self-sufficiency treated together), `self-sufficiency` (Eng. Exp. detail;
  advising), `ai-pedagogy` (specialist activities, AI Pedagogy Lab, ethics objection),
  `scholarship-and-dissemination` (stEm PEER Academy)
- Evidence: `stress-reduction-survey-results` (full Q-by-Q figures, n/response, SD
  confirmed), `mtlc-external-evaluation` (letter provenance, still de-identified)
- Updated: `glossary.md`, `index.md`

**Stripped/handled per publication rules**: student deaths & individual anecdote
(generalized & softened); low early CAD scores (omitted, endpoint kept); external
evaluator's letter (A.2) and name (de-identified aggregate only); IQP cover pages (A.5)
and appointment letter (A.10) not reproduced; team/member/sponsor names omitted from
[[project-advising]]; PMKS+ developer named in glossary only, not prose.

**Open items**
- Confirm CMSC full name (glossary [REVIEW]); confirm stEm PEER Academy year.
- The 2023 ASEE paper (A.1) will get its own source page when `raw/my-work/2023_Ebadi_ASEE.pdf`
  is ingested; reconcile with [[stress-reduction-survey-results]] then.
- Live problem-solving / CAD live-demo practices still to be written from later sources.

## 2026-09-18 — INGEST: Curriculum Vitae (`raw/my-portfolio/RE_CV.pdf`, 18 pp)
The authoritative record. Extracted with pypdf (all pages had text). Discussed takeaways;
Reza confirmed **keep the external evaluator unnamed even as a published co-author**, and
(on my recommendation) chose **Option 3 for evaluations** — representative strong scores +
an honest note that some courses started lower and improved through iteration, without
printing the specific low term-by-term numbers.

**Confirmations resolved:** evals are a 5-pt scale (Q1 course / Q2 instructor); **CMSC =
Consortium of Multiple Sclerosis Centers**; **stEm PEER Academy = 2025–2026** (Silevitch/
Duggan Center); several funded internal grants; funded external = none. *(Grant dollar
amounts later removed from the wiki by policy — 2026-09-18.)*

**Pages created**
- Sources: `sources/cv.md`; paper stubs `2023-ebadi-asee`, `2024-ebadi-asee` (flow-viz),
  `2025-brown-asee` (GPThermo), `2026-ebadi-asee` (AI-pedagogy; ASEE **Finalist**).

**Pages enriched**
- `threads/scholarship-and-dissemination` — full rewrite: de-identified publication/talk/
  workshop list, funded-internal grant ledger (with amounts), pending & not-funded
  proposals (amounts omitted), recognitions, press, service/reviewing, memberships.
- `evidence/teaching-evaluations` (Option 3; scale + Q defs), `evidence/stem-peer-academy`
  (year/host), `threads/accessibility` (flow-viz link → 2024-ebadi-asee), glossary, index.
- Removed remaining "(to be created)" placeholders now that the four stubs exist.

**Stripped/handled**: all MQP/IQP student names + provisional-patent numbers; co-PI/
co-author names (glossary only, roles in prose); the evaluator kept unnamed even as
co-author (2024 "Capstone Projects" cited by title, "led by a WPI colleague"); pending/
unfunded amounts omitted (incl. unfunded internal CQP/Summer-Sandbox proposals); **fluids/
turbulence journal articles & APS-DFD talks NOT reproduced or cross-linked** (separate
research vault).

**Open items**
- **Citation metrics unsourced:** the glossary's "h-index 5" has no source in the ingested
  docs and the CV states none. Flagged [REVIEW] on the glossary and scholarship thread —
  needs a citation report to validate.
- Title/wording variance recorded: 2026 ASEE Best Overall Paper = "Finalist" (CV) vs
  "nominated" (candidate statement); paper title "...AI Pedagogy Role" (CV) vs
  "...Specialist Initiative" (statement).
- Remaining `raw/my-work` PDFs/PPTX will enrich the paper stubs and add the capstone,
  IMECE, IEC, PBL, AI-Summit, and workshop sources.

## 2026-09-18 — INGEST: COVID Statement (`raw/my-portfolio/RE_COVID_Statement.pdf`, 1 p)
Short one-paragraph document; least sensitive so far (no names, student data, or figures).
No new decisions needed — applied established policy.

**Value:** provides the **pandemic origin** of several accessibility practices (recorded/
broadcast lectures, posted notes, and optional virtual/hybrid office hours), built as a
UNH lecturer and retained post-pandemic; reinforces the stress-reduction motivation
timeline (first year at WPI, AY21-22), kept in softened/general terms.

**Pages created:** `sources/covid-statement.md`.
**Pages enriched:** `threads/accessibility` (virtual office hours + pandemic-origin
provenance), `teaching-philosophy` (source link), `index`.

**This completes the `raw/my-portfolio/` folder** (Candidate Statement, Teaching
Portfolio, CV, COVID Statement all ingested). Next folder: `raw/my-work/` (10 papers/
talks), then `raw/evidence/` (letters L1–L4 — mostly private; publish only de-identified
aggregate facts, if any).

## 2026-09-18 — INGEST: 2023 ASEE paper (`raw/my-work/2023_Ebadi_ASEE.pdf`, 8 pp)
Full standalone version (the portfolio's Appendix A.1 was a scan). All content public
(peer-reviewed); no stripping beyond dossier voice. Key nuance: the paper's own frame is
**"learning through teaching"** (comprehension), and its three modules are group quizzes,
a **group project**, and the midterm make-up — NOT the two-part final. The
stress-reduction framing is the portfolio/statement's later lens on the same work.

**Pages:** filled `sources/2023-ebadi-asee.md` (stub → full: design, grade + survey
results Q1–Q6, honest limitations); created `practices/kinematics-community-project.md`
(new); enriched `midterm-makeup-exams` (14/29 opted, all-but-one improved, 12→68 range),
`stress-reduction-survey-results` (source + make-up detail), `self-sufficiency` (link),
`index`.

**Confirmed figures:** 40.8% (SD 29.4%); survey n=26 (90%); Q1 77% / Q2 65.4% / Q3 65.4%
/ Q4 38.6% / Q5 65.3% / Q6 76.9%. Q4 low ≈ survey timing (pre-project).

## 2026-09-18 — INGEST: 2024 ASEE "Lab on Cart" (`raw/my-work/2024_Ebadi_ASEE.pdf`, 11 pp)
Low-cost flow-visualization (PIV) paper. Public/peer-reviewed. **Work in Progress** — the
rig is built & qualitatively validated but has **no efficacy data yet** (SALG assessment
planned), so I tagged the build [VALIDATED] and the learning benefit [ASPIRATIONAL] to
avoid overclaiming.

**Pages:** filled `sources/2024-ebadi-asee.md` (stub → full: motivation, the **\$251**
per-unit cost table, MATLAB/PIVlab app, WIP status, sample activities); enriched
`threads/accessibility` (portable PIV + \$251 + WIP caveat); glossary (PIV, PIVlab, SALG);
index.

**Stripped:** two undergraduate students acknowledged by name → credited generically.
**Discrepancy noted (not resolved):** candidate statement says "four undergraduates" on the
grant; the paper acknowledges two. **Chose not to create a separate evidence page** for the
\$251 figure (WIP, no efficacy yet) — it lives on the source + accessibility pages; promote
later if learning-gains data arrives.

## 2026-09-18 — INGEST: 2024 IEC "Combating Exam Stress" (`raw/my-work/2024_Ebadi_IEC.pdf`, 1-page poster)
Rendered the poster (charts are images). It's the invited Innovative Education Conference
(URI) presentation — and a **richer, separate survey** than the 2023 paper: Kinematics,
**n = 47, 100% participation**, with module helpfulness, learning gains, AND anxiety
prevalence. All aggregate; nothing to strip.

**Pages:** created `sources/2024-ebadi-iec.md`; added a distinct **"Survey B" section** to
`evidence/stress-reduction-survey-results.md` (kept separate from the n=26 survey, not
pooled); gave the previously number-less `two-part-final-exams` (38%) and `note-templates`
(47%) their first aggregate figures, and added IEC figures to `weekly-group-quizzes` (83%)
and `midterm-makeup-exams` (62%); linked from `stress-reduction` and
`scholarship-and-dissemination` threads; index.

**Transparency:** poster percentages combine the top two Likert categories (e.g. "highly or
extremely helpful", "good or great gain") — labeled as such on every page. Module figures:
quizzes 83% / make-up 62% / notes 47% / two-part final 38%. Gains: kinematics-confidence
68%, enthusiasm 66%, understanding 60%, interest 53%, exam-comfort 28%.

## 2026-09-18 — INGEST: 2024 ASEE Capstone study (24 pp; `raw/my-work/` capstone paper)
A large quantitative **alumni study** (~2,101 WPI grads) on capstone/MQP → professional
skills → self-efficacy → career preparedness. **Led by the external evaluator; Reza is one
of five co-authors (contributing, not lead).** Handled carefully: attributed as a
co-authored WPI study, findings credited to the study (not to Reza), lead author **kept
unnamed** per policy.

**Findings recorded:** capstones significantly build skills + self-efficacy; both predict
career preparedness; **self-efficacy largely mediates** (≈79% of professional-skills
variance also explained by self-efficacy).

**Pages:** created `sources/2024-capstone-asee.md` (topic-titled slug, not the lead
author's name); linked from `scholarship-and-dissemination` and added a "related
scholarship" note to `project-advising`; glossary (WPI Plan, self-efficacy, co-authors
F. Levey & J. McNeill added — evaluator still excluded); index.

**Handling notes:** connected self-efficacy ↔ the self-sufficiency pillar without
overstating Reza's role; no student/alumni identifiers reproduced (aggregate only).

## 2026-09-18 — INGEST: 2024 IMECE drag-reduction (7 pp; `raw/my-work/` IMECE MQP paper)
An **advised-MQP fluids-research paper** (bio-inspired riblets for drag reduction) Reza
co-advised. Treated as **project-advising dissemination**, NOT pedagogy scholarship, and
kept deliberately light on the fluids research (research-vault boundary). Read only p.1
for framing/authorship.

**Pages:** created `sources/2024-drag-reduction-imece.md` (**topic-based slug**, not a
student surname); linked from `scholarship-and-dissemination` and `project-advising` (as
the concrete IMECE-honorable-mention example); glossary (A. Gnanaskandan co-advisor, YEP
Contest); index.

**Stripped:** both undergraduate MQP student names (also kept out of the slug).
**Boundary respected:** the technical result (~5–13% drag reduction) noted only as the
project's finding; fluids methodology not reproduced here.

## 2026-09-18 — INGEST: 2025 ASEE GPThermo (`raw/my-work/` GPThermo paper, 14 pp)
Full, self-contained paper (undergraduate co-author + Reza). Public/peer-reviewed; only
role-in-prose for the co-author (already a sanctioned glossary co-author).

**New evidence:** GPThermo's architecture (**GPT-4o** + tool & retrieval augmentation,
multi-agent: Conversation → Retrieval + Calculation agents) and a **benchmark**: 20
thermo questions, correct within 1% → **GPThermo 95% vs 15–25%** for ChatGPT/Gemini/
Claude/Copilot. Honest caveat: overreliance risk if used too early (ties to
self-sufficiency).

**Pages:** filled `sources/2025-brown-asee.md` (stub → full); created
`evidence/gpthermo-accuracy.md`; enriched `tools/gpthermo` (architecture, accuracy,
caveat), `threads/educational-tools`, glossary; index.

## 2026-09-18 — INGEST: 2025 Global School Forum PBL talk (`raw/my-work/` PBL deck, 8 slides)
Extracted slide text from the `.pptx` (zip/XML — python-pptx absent; notes were just slide
numbers). A **position/framework talk**, no new data — mostly [CLAIM]/[ASPIRATIONAL].
All public.

**Value:** articulates Reza's AI-in-courses framework — AI removes PBL barriers so
instructors can raise project complexity; the **uneven-AI-readiness equity risk** (ties AI
to the accessibility pillar); a near-2029 / 2030+ timeline; and five faculty
recommendations ("teach AI as a tool, not a crutch"; redesign assessments around
verification). ME 3902 case study reinforces existing self-sufficiency material.

**Pages:** created `sources/2025-ebadi-pbl.md`; added a "Stated framework" section to
`threads/ai-pedagogy` and linked from its dissemination list; linked from
`self-sufficiency` and `scholarship-and-dissemination`; index. No new practice page (no new
discrete practice; the Eng. Exp. AI approach is already captured).

## 2026-09-18 — INGEST: 2026 AI Summit talk (`raw/my-work/` AI-Summit deck, 9 slides)
Extracted slide text from the `.pptx`. The **definitive documentation of the AI
verification cycle** — Reza's own framework (deck says so). All public; one anonymized
student opt-out quote (already in use).

**Big enrichment:** the previously-sketchy `ai-verification-cycle` practice page now has
the real **weekly cadence** (TA test Thu → TA report Mon → student quiz Tue → AI Lab Wed),
**participation-not-correctness grading** (stress-reduction crossover), the PMKS+ live-demo
mechanics, a worked coupler-curve "fluent-but-wrong" example, and the takeaways
(**confidence ≠ correctness**, **expertise can't be outsourced**, transferable).

**Pages:** created `sources/2026-ebadi-ai-summit.md`; substantially expanded
`practices/ai-verification-cycle`; sharpened the research-program thesis in
`threads/ai-pedagogy`; linked from `scholarship-and-dissemination`; index. Companion:
2026 Capital PKAL "A Weekly Cycle for AI Verification" (same topic; already listed).

## 2026-09-18 — INGEST: 2026 ASEE AI Pedagogy paper (`raw/my-work/` 2026 ASEE paper, 15 pp)
The flagship AI-Pedagogy-Specialist paper (**ASEE Best Overall Paper Finalist**). Reza is
**lead author**; co-authors incl. J. Hill (glossary) + the evaluator (**kept unnamed**;
her name IS in the paper's author bios — not reproduced). Turns much of the ai-pedagogy
thread from [CLAIM]/[ASPIRATIONAL] into [VALIDATED] institutional evidence.

**Key data:** POD-framework structure (sieve/incubator/hub); needs assessment — 155
faculty / 107 students (58% use AI for own work not teaching; ethics top faculty need 56%;
clear policies top student need 50%); inaugural-year reach 69 faculty/staff across 4
sessions; 43-policy survey (49% tiered; 60% no enforcement); 3 AI Pedagogy Labs; Food for
Thought; Assignment Redesign Worksheet; advisory circle + 2 ambassadors.

**Pages:** filled `sources/2026-ebadi-asee.md` (stub → full); created
`evidence/ai-pedagogy-inaugural-year.md`; substantially enriched `threads/ai-pedagogy`
(POD structure + first-year evidence; "nominated"→**Finalist**); glossary (POD/CTL, FFT,
AI Advisory Circle); index.

**Discrepancies flagged (not resolved):** consultations = 4 (abstract/§4.4) vs 7 (§4.3);
paper's own title varies (Role vs Specialist Initiative). Both noted on the source page.

## 2026-09-18 — INGEST: 2026 ASEE workshop deck (`raw/my-work/` workshop, 19 slides)
"Building AI-Enhanced Educational Websites" — a hands-on, no-code faculty-development
workshop (150 min, 4 phases). All public. **Completes the `raw/my-work/` folder** (10/10).

**Value:** operationalizes the specialist's sieve/incubator function — teaching faculty
"vibe coding" (Prompt→Generate→**Inspect**→Iterate), university branding (60-30-10 rule),
GitHub Pages publishing, and **responsible design** ("don't publish sensitive data"). Nice
thematic parallel: the Inspect/verify step applies the student AI-verification ethos to
faculty. His own sites used as examples.

**Pages:** created `sources/2026-ebadi-asee-workshop.md`; linked from `ai-pedagogy` and
`scholarship-and-dissemination` (dropped stale "will organize"/[ASPIRATIONAL] now that the
materials exist and the 2026 conference date has passed — but claimed NO attendance/outcome
data, since none is given); glossary (vibe coding, GitHub Pages); index.

## STATUS after `raw/my-work/`: 42 wiki pages. Remaining: `raw/evidence/` (L1.docx, L2–L4.pdf)
— letters; mostly PRIVATE. Plan: read for any publishable de-identified aggregate facts
only; never reproduce letter text or names.

## 2026-09-18 — INGEST: L1 (`raw/evidence/L1.docx`) — PRIVATE letter, LOG-ONLY
The external evaluator's support letter for Reza's **stEm PEER Academy** application (Apr
2025). It is the **private origin** of already-published de-identified facts: the C24
Kinematics stress/92% figure ([[mtlc-external-evaluation]]), the "real challenge" / "low
pressure, but really complex" descriptions, and the ">1 download/day" figure. Confirms the
sensitive context (a cluster of suicides at WPI) — reinforces keeping the motivation
softened; stays out.

**Decision (Reza):** log-only, **no source page** for letters (a public source page would
surface the letter/evaluator). Letter stays in `raw/`; evaluator unnamed everywhere.
**One addition made:** noted the stress level used a **"validated survey scale"** on
[[mtlc-external-evaluation]] (de-identified, aggregate; no name, no letter text). This
log-only handling applies to L2–L4 unless one holds a genuinely new publishable
de-identified fact.

## 2026-09-18 — INGEST: L2 (`raw/evidence/L2.pdf`) — PRIVATE, NOTHING PUBLISHED
Not an evaluation letter: a **personal student email** (an IQP-presentation invitation with
personal thanks). Contains a **named student, individual quotes, and personal/health
disclosures** — fully private under every publication rule. **Nothing publishable, nothing
extracted, no names.** Stays in `raw/` only. (Flagged to Reza that this is personal
correspondence, not portfolio evidence.)

## 2026-09-18 — INGEST: L3 (`raw/evidence/L3.pdf`) — PRIVATE, NOTHING PUBLISHED
A **promotion evaluation letter** (for Reza's promotion to Associate Teaching Professor)
from a **named senior WPI colleague**. Third-party evaluative statements about Reza +
promotion-case framing → private under CLAUDE.md rules 1 and 3. The only concrete items it
cites (Morgan-Worcester Instructorship 2026–2029, breadth of courses, "outstanding"
evaluations) are **already in the wiki from public sources**. **Nothing new published; no
names; letter not reproduced.** Stays in `raw/`.

## 2026-09-18 — INGEST: L4 (`raw/evidence/L4.pdf`) — PRIVATE, NOTHING PUBLISHED
A **tenure-support letter** from an external ed-tech partner (Collage AI) to Reza's
department head. Third-party evaluative statements + promotion-case framing → private
(rules 1, 3). Only confirms Reza's **Collage AI advisory/consulting** role, already noted
neutrally in [[scholarship-and-dissemination]] and [[glossary]]. **Nothing new published;
no names; letter not reproduced.** Stays in `raw/`.

## 2026-09-18 — CORPUS COMPLETE
All `raw/` ingested: `my-portfolio/` (4), `my-work/` (10), `evidence/` (4 letters,
log-only). Wiki = 42 public pages, all wikilinks resolve, zero third-party surnames in
`wiki/` (scanned). Standing publication policy captured in agent memory. Open [REVIEW]
items remain in the glossary/threads (e.g. unsourced h-index; consultations 4-vs-7).

## 2026-09-18 — LINT PASS + number cleanup + AI Pedagogy website
**Lint findings:** no banned superlatives; no problematic orphans (only `index`/`log`
stand alone, by design); all 8 evidence pages linked to ≥1 claim; `[VALIDATED]` tags are
backed by evidence links or qualified (`— funded`/`— built`/`— as designed`). Fixed:
`overview.md` and `glossary.md` were missing the required `visibility: public` tag (added);
refreshed the overview's stale "refine as sources are ingested" caveat and its date.

**Numbers removed (Reza's instruction — unreliable figures):** the unsourced **h-index**
(glossary + scholarship thread), the disputed **consultation count** (source + evidence
pages), and the contradicted **"four undergraduates"** on Lab-on-Cart (→ "undergraduate
students"). Well-sourced, dated figures (survey %, 95% benchmark, dollar amounts, adoption "as
of the candidate statement") were kept.

**AI Pedagogy website:** featured [aipedagogy.wpi.edu](https://aipedagogy.wpi.edu) as a
clickable **Companion site** callout atop `threads/ai-pedagogy`, and made the tool/site
URLs clickable in the glossary.

**Still-open [REVIEW] items for Reza:** glossary term-calendar (A–E) mapping; CTAF
meaning; confirm the co-author people-list is public-co-authorship only.
