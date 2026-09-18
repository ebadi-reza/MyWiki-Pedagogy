---
title: "Source: 2024 ASEE — Lab on Cart (Low-Cost Flow Visualization)"
type: source
visibility: public
pillars: [accessibility, self-sufficiency]
threads: [accessibility, scholarship-and-dissemination]
status: draft
created: 2026-09-18
updated: 2026-09-18
---

# Source: 2024 ASEE — "Lab on Cart"

**Citation:** R. Ebadi (as A. Ebadi) & a WPI colleague, "Work In Progress: Lab on Cart:
Developing a Low-Cost Fluid Visualization Setup for Experiential Learning, Class
Demonstration and Outreach," *2024 ASEE Annual Conference & Exposition*, Portland, OR
(Paper ID #41213). Peer-reviewed. *(Co-author in [[glossary]]; built with undergraduate
students.)*

## Motivation
[CLAIM] Fluid dynamics is hard to teach — common fluids are transparent and the governing
equations are complex — and **flow visualization**, though effective, is rare in
undergraduate courses because wind/water tunnels cost tens of thousands of dollars, occupy
a room, and take time to set up. This addresses a gap Reza identified (no flow-viz in
Fluids, Eng. Exp., or MME/Aerospace MQPs for 2022–23). Serves [[accessibility]].

## What was built
[VALIDATED — built] A low-cost, safe, **portable Particle Image Velocimetry (PIV)** setup
— "Lab on Cart" — designed to be **replicated in quantity** so each small student team
gets its own, enabling simultaneous or customizable experiments.

**Cost — total ≈ $251 per unit** (vs. tens of thousands for a tunnel):

| Component | Cost |
|---|---|
| 10-gallon fish tank | $25 |
| Small cart | $81 |
| USB camera | $77 |
| Hunting laser diode + mounts | $25 |
| Cylindrical lens | $43 |

A companion **MATLAB app** (built on the open-source **PIVlab** library) runs the
workflow in four stages — Calibration, Image Pre-processing, PIV Settings,
Post-processing — with in-app troubleshooting tips (instruction manual in the paper's
Appendix A).

## Status & assessment
[ASPIRATIONAL] Work in Progress: a single proof-of-concept unit is built and
**qualitatively** validated; the team is fine-tuning repeatability, building out the array,
and designing student experiments (sample Fluids and Experimentation activities in
Appendix B — e.g. an L-shaped-pipe jet, and a bluff-body surface-texture drag study).
**Learning-gains assessment is planned via the SALG survey** — no efficacy data reported
yet, so the accessibility benefit is a design goal, not a measured outcome.

## Intended use
Fluid Mechanics (ES 3004), Engineering Experimentation (ME 3902), MQPs, and outreach.
Funded by a **$13,040** MTLC Teaching Innovation Grant (see [[scholarship-and-dissemination]]).

## Threads & pillars
[[accessibility]] (low-cost lab hardware), [[self-sufficiency]] (students run and
customize their own experiments), [[scholarship-and-dissemination]].

## Related
- [[accessibility]] · [[scholarship-and-dissemination]] · [[cv]]
