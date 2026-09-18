# Engineering Education & Pedagogy — Knowledge Wiki

A public, interlinked knowledge base of Reza Ebadi's engineering-education and pedagogy work — teaching practices, scholarship, the AI tools he built, and his role as WPI's first AI Pedagogy Specialist — built with the "LLM Wiki" pattern (immutable sources in, a maintained set of interlinked Markdown pages out). The wiki is organized around three pillars: **accessibility**, **stress reduction**, and **self-sufficiency**.

## Layout

- **`wiki/`** — the knowledge base, and the only part published to the web. Markdown with Obsidian-style `[[wikilinks]]`.
  Start at [`wiki/overview.md`](wiki/overview.md) (the philosophy spine and how the threads connect) and
  [`wiki/index.md`](wiki/index.md) (catalog of every page).
- **`raw/`** — immutable private source documents (papers, portfolio, notes, data). **Not tracked in git**
  (see `.gitignore`): reference material only, kept local, never published.
- **`CLAUDE.md`** — the schema and operating instructions for how the wiki is built and maintained.

Everything in `wiki/` is **public by construction**: pages are written already cleared for public view —
no third-party names or letters, no student data, no dossier framing. The private/public boundary is the
`.gitignore` on `raw/`, not a setting that can be toggled per page.

## Inside `wiki/`

| Path | What |
|---|---|
| `overview.md` | The three-pillar spine and how the threads connect |
| `index.md` | Catalog of every page, by category |
| `teaching-philosophy.md` | The three pillars — the spine page |
| `glossary.md` | WPI shorthand, term codes, acronyms, entities |
| `log.md` | Append-only ingest / query / lint history |
| `threads/` | One page per thread (the 3 pillars + 3 cross-cutting threads) |
| `practices/` | Individual teaching / assessment practices |
| `tools/` | Built artifacts (GPThermo, StudyGuideAI, …) |
| `sources/` | One page per ingested paper / poster / document |
| `evidence/` | Reusable, publishable evidence items (aggregate results, metrics, awards) |
| `analyses/` | Comparisons and syntheses filed back from questions |

## Viewing

Open the folder as an **Obsidian vault** for graph view and backlinks.

## Publishing (GitHub Pages via Quartz)

The `wiki/` folder is published as a static site with [Quartz](https://quartz.jzhao.xyz/)
through `.github/workflows/deploy.yml`. On each push to `main`, a GitHub Action fetches
Quartz on the runner, builds **only** `wiki/` into a site (preserving `[[wikilinks]]` and
regular `[text](url)` links), and deploys it to GitHub Pages. Quartz itself is not
committed here — the workflow pulls it fresh each build.

`raw/` is git-ignored, so it never reaches the repository and can never be published.
To enable: in the repo, **Settings → Pages → Source: GitHub Actions**. Live site:
`https://ebadi-reza.github.io/MyWiki-Pedagogy/`.
