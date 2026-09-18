---
title: "Source: 2025 ASEE — GPThermo"
type: source
visibility: public
pillars: [accessibility, self-sufficiency]
threads: [educational-tools, accessibility, ai-pedagogy, scholarship-and-dissemination]
status: draft
created: 2026-09-18
updated: 2026-09-18
---

# Source: 2025 ASEE — "GPThermo"

**Citation:** an undergraduate co-author & R. Ebadi, "GPThermo: An In-House Generative
Artificial Intelligence Tutor for Thermodynamics," *2025 ASEE Annual Conference &
Exposition*, Montreal, QC (Paper ID #46855). Peer-reviewed. *(Co-author in [[glossary]].)*

## Motivation
[CLAIM] Thermodynamics is a high-cognitive-load **"gateway course"** whose analysis
depends on constant lookups from large property tables. As students increasingly skip
textbooks and lack commercial software (EES, REFPROP, CoolProp), those property values —
the building blocks of any analysis — become inaccessible, especially after the course
ends. General-purpose LLMs (ChatGPT, Claude, Gemini, Copilot) answer technical thermo
prompts **inaccurately** but with convincing language, so students may trust wrong
answers. GPThermo targets this gap. Serves [[accessibility]].

## Architecture
[VALIDATED — as designed] Built on the **GPT-4o** foundation model with two augmentations
rather than costly retraining:
1. **Tool augmentation** — runs custom code (property functions, a calculator) for exact
   thermodynamic calculations.
2. **Retrieval augmentation** — accesses supervised/private property data (property
   tables, fluid identifiers).

A **multi-agent** design routes each query from a **Main Conversation Agent** (GPT-4o) to
two secondary agents — a **Retrieval Agent** (property lookups) and a **Calculation
Agent** (Python-based math) — iterating until a synthesized answer is produced.
*(The candidate statement notes PyroMat as the property backend.)*

## Validation result
[VALIDATED] A benchmark of **20 thermodynamics questions** with clear numerical answers
(correct = within **1%** of the analytical solution), tested against GPThermo and four
public models:

> **GPThermo answered 95% correctly, vs. 15–25% for ChatGPT, Gemini, Claude, and Copilot.**

The questions deliberately included mistyped units and grammatical errors to mimic real
student submissions. See the evidence page [[gpthermo-accuracy]].

## Broader impacts & honest caveats
[CLAIM] A subject-specific model **plus a companion validation tool** — demonstrating the
feasibility of customizing LLMs for STEM and a framework for validating them; potential
benefit for under-resourced learners (instant domain-specific feedback, lightweight to
deploy). The authors also state real caveats: adoption depends on curriculum fit, faculty
acceptance and training, and — notably — **giving students access too early risks
overreliance**, preventing them from developing foundational skills. This overreliance
concern is the same judgment issue at the center of [[self-sufficiency]] and the
[[ai-verification-cycle]].

## Related
- [[gpthermo]] · [[gpthermo-accuracy]] · [[educational-tools]] · [[ai-pedagogy]] · [[scholarship-and-dissemination]]
