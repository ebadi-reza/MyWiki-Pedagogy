---
title: "Evidence: GPThermo Accuracy Benchmark"
type: evidence
visibility: public
pillars: [accessibility]
threads: [educational-tools, ai-pedagogy]
status: draft
created: 2026-09-18
updated: 2026-09-18
sources: [2025-brown-asee]
---

# Evidence: GPThermo Accuracy Benchmark

**Provenance:** [VALIDATED] — peer-reviewed benchmark result (2025 ASEE).

## The figure
On a **20-question** thermodynamics benchmark with clear numerical answers — scored
**correct only if within 1%** of the analytical solution — **[[gpthermo]] answered 95%
correctly**, versus **15–25%** for four leading public models (OpenAI ChatGPT, Google
Gemini, Anthropic Claude, Microsoft Copilot).

The benchmark questions deliberately included mistyped units and grammatical errors to
mimic real student submissions. The authors report the gap has stayed roughly consistent
as public models improved and GPThermo was updated in response.

## Why it counts as evidence
It is a quantitative, peer-reviewed comparison showing the domain-specific tool
substantially outperforms general-purpose LLMs on the exact task students would use it
for — the core justification for building a subject-specific model.

## Source
[[2025-brown-asee]] (§ Validation and Results; benchmark in the paper's Appendix B).

## Claims it supports
- The [[accessibility]] value of [[gpthermo]] as a reliable thermodynamics tool; the
  "build domain-specific AI" argument in [[educational-tools]] and [[ai-pedagogy]].
