---
title: GPThermo
type: tool
visibility: public
pillars: [accessibility, self-sufficiency]
threads: [educational-tools, accessibility, ai-pedagogy]
status: draft
created: 2026-09-18
updated: 2026-09-18
---

# GPThermo

**URL:** gpthermo.wpi.edu · Serves [[accessibility]]; a platform for [[ai-pedagogy]].

## Purpose
[CLAIM] An AI-powered educational assistant for **thermodynamics**, built to make robust
thermodynamics help accessible outside the classroom (the [[accessibility]] pillar) and
to keep students from relying on unverified free resources.

## What it does
- Interactive, step-by-step problem solving with guidance.
- Real-time property calculations for **20+ working fluids**, backed by **PyroMat** for
  numerical accuracy (LLM for reasoning, PyroMat for the numbers).
- Visual thermodynamic diagrams.

## How it was built
[VALIDATED — as designed] Built on the **GPT-4o** foundation model with two augmentations
(rather than costly retraining): **tool augmentation** (runs code for exact property
calculations) and **retrieval augmentation** (supervised/private property tables). A
**multi-agent** design routes each query from a Main Conversation Agent to a **Retrieval
Agent** and a **Calculation Agent** (Python-based). PyroMat provides the property backend.
See [[2025-brown-asee]].

[CLAIM] It grew out of two **unfunded** external NSF proposals on accessible
thermodynamics education (see [[scholarship-and-dissemination]]); rather than shelve the
idea, Reza secured a **$16.5k MTLC grant** and built the platform himself, and has
**maintained it after the grant ended**.

## Accuracy
[VALIDATED] On a 20-question benchmark (correct = within 1% of the analytical answer),
GPThermo scored **95%** vs. **15–25%** for four leading public LLMs. See
[[gpthermo-accuracy]].

## Adoption
[VALIDATED] **19 verified users** at educational institutions beyond WPI (as of the
[[candidate-statement]]) — early adoption outside his own courses. *Keep this figure
dated; update from tool docs when ingested.*

## Role as a research platform
[ASPIRATIONAL] Intended as a research platform for the future [[ai-pedagogy]] program on
how engineering students interact with AI in domain-specific contexts. It also directly
informed the design of [[studyguideai]].

## Noted caveat
[CLAIM] The 2025 paper flags a real risk: giving students the tool **too early** could
foster **overreliance** and stunt foundational skills — the same judgment concern behind
[[self-sufficiency]] and the [[ai-verification-cycle]].

## Dissemination
[VALIDATED] Presented at **ASEE 2025**. → [[2025-brown-asee]].

## To enrich
Dated usage metrics and any newer adoption numbers from tool docs (architecture and the
accuracy benchmark are now captured from [[2025-brown-asee]]).

## Related
- [[educational-tools]] · [[studyguideai]] · [[accessibility]] · [[ai-pedagogy]]
