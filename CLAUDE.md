# CLAUDE.md — Engineering Education & Pedagogy Knowledge Wiki

This file tells the LLM agent how to build and maintain this wiki. Claude Code reads
it automatically at the start of a session; read it in full before touching any file.
This wiki follows the "LLM Wiki" pattern: the agent reads immutable sources and
incrementally builds a persistent, interlinked set of markdown pages. Reza curates
sources and supplies all judgments about the quality or significance of his own work;
the agent organizes, cross-references, and surfaces evidence.

## Who this is for

Reza Ebadi — Assistant Professor of Teaching in Mechanical & Materials Engineering at
WPI, on the tenure track, and WPI's inaugural AI Pedagogy Specialist. This wiki covers
his engineering-education and pedagogy work: scholarship, teaching practices, the AI
tools he built, his specialist role, and his grant/dissemination record. 

## What this wiki is for

This wiki is primarily a **public showcase** of Reza's engineering-education work,
published to the open web via GitHub Pages. It also serves as organized knowledge for
him and a feeder for future papers and grants. Because the primary audience is the
public web, the publication discipline below (git-ignored private sources, public-by-
construction wiki pages, and the stripping checklist) is the most important rule in
this file — a leak of a name, a letter, or student data is the failure that matters
most here.

## The three layers — and the public/private boundary

- **raw/** — immutable PRIVATE sources: Reza's papers, posters, presentations, candidate statement,
  teaching portfolio, CV, citation reports, tool docs, workshop materials, student
  survey data, letters. The agent READS these for reference and NEVER modifies them.
  **This folder is git-ignored (see `.gitignore`) and must NEVER be committed or
  pushed.** It exists only on Reza's disk as reference material for the agent.
  Subfolders in raw/ are for Reza's organization only — they don't define the structure.
- **wiki/** — everything the agent writes. **This is PUBLIC BY CONSTRUCTION**: every
  page here is committed and published to the open web. Therefore a page in `wiki/` may
  contain ONLY content already cleared for public view — the stripping (see the
  Publication rules below) happens when the page is WRITTEN, not later. There is no
  private area inside `wiki/`.
- **CLAUDE.md** (this file) — the schema, co-evolved over time. Committed and public.

**The boundary is physical, not a tag.** `raw/` being git-ignored is the real wall
that keeps source documents off the web. The `visibility:` frontmatter tag (below) is
a second, softer guard against a private *detail* (a name, a quote, a figure) leaking
into a public page's prose. Both matter; the .gitignore is the one that can't fail by
accident if set up correctly.

## Publication rules (public-by-construction)

Every page the agent writes in `wiki/` goes on the public web. Before writing ANY
content into a wiki page, the agent applies this stripping checklist — the cleanup is
part of authoring, never a later pass:

1. **No third-party names or evaluative statements about Reza.** Do not name
   Kimberly LeChasseur, colleagues, students, or reproduce their letters/quotes. An
   external validation may be stated in de-identified, aggregate form ONLY (e.g. "an
   external MTLC evaluation found 92% of highly-stressed students reported the
   strategies helped") — never the letter text, never the evaluator's name, unless
   Reza confirms explicit written permission.
2. **No student data or identifiers.** No student quotes attributable to an individual,
   no survey microdata, no MQP/IQP team names or member names, no course-section-level
   detail that could identify a cohort. Aggregate survey percentages are fine.
3. **No tenure-case framing.** Never write "why this meets the tenure criteria," never
   reproduce candidate-statement self-argument, never frame a page as a promotion case.
   Describe the work and its evidence; omit the dossier voice entirely.
4. **No sensitive figures.** No pending/unfunded grant dollar amounts, no internal
   appointment-letter content (e.g. the Provost letter), unless Reza clears them.
5. **Every `visibility` tag is `public`.** If content can't be made public even after
   stripping, it does not go in a wiki page at all — it stays in `raw/` as reference.

When the source material and the publishable page differ (they usually will), the
agent writes the clean public version and, if useful, notes to Reza what it left out
and why — in the chat, not in the file.

The agent NEVER commits, pushes, or runs git. Reza controls all git operations. The
agent's job is to ensure that what it writes into `wiki/` is already safe to publish.

## The organizing spine: three-pillar philosophy

Reza's teaching philosophy has three pillars, and nearly all his work is an expression
of one or more of them. The wiki is organized around this spine, NOT as a flat list of
projects. The three pillars:

1. **Accessibility** — making education more accessible (lecture videos, note
   templates, OER, low-cost equipment, AI tools as access instruments).
2. **Stress reduction** — reducing anxiety while maintaining rigor (group quizzes,
   midterm make-up exams, two-part finals).
3. **Self-sufficiency** — developing students who can solve unfamiliar problems
   (AI verification cycle, project advising, professional-tool exposure).

Every thread and source page should link back to the pillar(s) it serves via
[[teaching-philosophy]].

## Directory structure inside wiki/

```
wiki/
├── index.md                  # catalog of every page, by category
├── log.md                    # append-only record of ingests/queries/lints
├── overview.md               # the philosophy spine + how threads hang off it
├── glossary.md               # WPI shorthand, term codes, acronyms, entities
├── teaching-philosophy.md    # the three pillars — the spine page
├── threads/                  # the seven threads (below)
├── practices/                # individual teaching/assessment practices, one per page
├── tools/                    # GPThermo, StudyGuideAI, etc. — built artifacts
├── sources/                  # one page per paper/poster/document ingested
├── evidence/                 # reusable evidence items (survey results, metrics, quotes, letters)
└── analyses/                 # syntheses filed back from queries
```

## The seven threads

Three pillar threads, three cross-cutting threads, plus the spine:

- **[[teaching-philosophy]]** — the spine (the three pillars and their relationships)
- **[[stress-reduction]]** — pillar; strongest evidence base
- **[[accessibility]]** — pillar
- **[[self-sufficiency]]** — pillar
- **[[ai-pedagogy]]** — cross-cutting: the AI Pedagogy Specialist role, website,
  workshops, faculty development, and the future research program
- **[[educational-tools]]** — cross-cutting: GPThermo, StudyGuideAI as built artifacts
- **[[scholarship-and-dissemination]]** — cross-cutting: ASEE record, invited talks,
  grant history (funded and unfunded), citation metrics

## Evidence-first discipline (most important rule)

This wiki supports a tenure narrative, so claims must be anchored to evidence, not
adjectives. Rules:

- Every claim about impact or effectiveness must cite a specific evidence item: a
  number, a survey result, a quote, an external validation, an award, a metric. No
  bare superlatives ("transformative," "pioneering," "groundbreaking," "revolutionary").
  If the evidence is a 40.8% improvement, write the number and cite it — don't write
  "dramatic improvement."
- Evidence items live in `evidence/` as reusable pages (e.g. the 
  evaluation, the quiz-comprehension figure, GPThermo's user adoption, the
  ">1 download/day" figure). Claims elsewhere link to them.
- Numbers get sourced to the document they came from. A number with no source is
  flagged, not filed as fact.

## Provenance discipline (second most important rule)

Keep three kinds of statement visually distinct on every page, because a portfolio
reader (and Reza) needs to see at a glance what's backed:

- **[CLAIM]** — Reza's own assertion about his work (from the candidate statement,
  portfolio, etc.).
- **[VALIDATED]** — supported by external evidence: LeChasseur's letter, adoption
  numbers, download rates, awards, student votes (Morgan-Worcester), peer-reviewed
  acceptance, citation counts.
- **[ASPIRATIONAL]** — future plans, in-preparation work, pending grants, the intended
  research program. Real and worth tracking, but not yet accomplished.

Never silently promote [ASPIRATIONAL] to [VALIDATED], or [CLAIM] to [VALIDATED].
Pending grants are [ASPIRATIONAL]. Unfunded grants are part of the record but marked as
not funded — Reza treats them as growth and dissemination, not failures; file them
that way, neutrally.

## The self-assessment boundary (do not cross)

The agent NEVER writes Reza's self-assessment, reflection, or judgment of his own
quality. It does not draft "why this matters for tenure," rate his work, or generate
narrative claims of excellence. Those must be Reza's own words. The agent's job is to
organize evidence and surface connections so Reza can write his own narrative. When a
task would require judging the significance of his work, the agent assembles the
relevant evidence and stops there.

## Page conventions

- YAML frontmatter on every page:
  ```
  ---
  title:
  type: philosophy | thread | practice | tool | source | evidence | analysis | overview | index | glossary
  visibility: public          # every wiki/ page is public; this is a standing reminder
  pillars: [accessibility, stress-reduction, self-sufficiency]   # if relevant
  threads: [related thread slugs]
  status: draft | reviewed
  created: YYYY-MM-DD
  updated: YYYY-MM-DD
  ---
  ```
  The `visibility: public` line is always present and always `public` — it reminds the
  agent on every page that the audience is the open web. A page that cannot be `public`
  is not written to `wiki/` at all.
- Obsidian `[[wikilinks]]` for all cross-references.
- Practice pages (a specific teaching/assessment module): what it is, how it runs,
  which pillar it serves, the evidence for it (linked), iteration history, which
  courses/terms it ran in.
- Tool pages: purpose, what it does, how built, adoption/usage numbers (with dates),
  which pillar(s) it serves, its role as a future research platform, lessons.
- Source pages: full citation, one-paragraph summary, key results (each cited to a
  specific figure/number), which threads/pillars it supports, connections.
- Evidence pages: the publishable evidence item — a number, an aggregate survey
  result, an award, a public metric, a de-identified finding — with its source and
  date and the claims it supports. Evidence pages are PUBLIC, so they hold NO letters,
  NO named third parties, NO individual student quotes. The underlying letter or raw
  survey stays in `raw/` as reference; the evidence page states only the publishable,
  de-identified fact drawn from it.

## Operations

**Ingest.** When Reza adds a source to `raw/`:
1. Read it fully (from `raw/`, which is private reference). For documents with
   figures/tables (survey charts, citation tables, screenshots), read the numbers
   carefully — they are the evidence.
2. Discuss key takeaways with Reza before writing much.
3. **Apply the stripping checklist (Publication rules) to decide what is publishable.**
   Everything written in the next steps goes to the public web, so de-identify and
   drop dossier framing as you write — not afterward.
4. Write/update the source page in `sources/` — a public-safe summary, NOT a
   reproduction of the private document.
5. Extract discrete PUBLISHABLE evidence items into `evidence/` pages (aggregate
   figures, awards, public metrics — no letters, names, or individual quotes).
6. Update the relevant thread and practice/tool pages, linking to evidence.
7. Tag every statement [CLAIM] / [VALIDATED] / [ASPIRATIONAL].
8. Update glossary.md with any new WPI shorthand. NOTE: glossary.md is public too —
   keep the people list to public-professional facts only, no private detail.
9. Update index.md; append to log.md.

**Query.** Read index.md first, drill into relevant pages, answer with evidence links.
Keep good syntheses as `analyses/` pages. When asked anything that amounts to "how good
is my work" or "make my tenure case," assemble evidence and connections — do not write
the judgment.

**Lint.** Report: unsupported claims (impact language with no evidence link),
provenance errors ([VALIDATED] with no external source), stale numbers, orphan pages,
missing pillar links, glossary inconsistencies, and evidence items not yet linked to
any claim. Propose; don't auto-rewrite.

## What the agent must never do

- Never modify raw/, and never commit, push, or run git — Reza controls all git.
- Never write into `wiki/` anything not cleared for the public web: no third-party
  names or letters, no individual student quotes or survey microdata, no MQP/IQP team
  or member names, no tenure-case framing, no pending/unfunded grant dollar amounts,
  no internal appointment-letter content — unless Reza explicitly clears it.
- Never reproduce a private `raw/` document into a wiki page — summarize, de-identify,
  and publish only the public-safe version.
- Never write bare superlatives or unsourced impact claims.
- Never mislabel provenance or promote aspirational/claim to validated.
- Never write Reza's self-assessment or judge the quality/significance of his work.
- Never cross-link into or merge with the turbulence vault.
- Never treat an unfunded grant as a failure — file it neutrally as record.
