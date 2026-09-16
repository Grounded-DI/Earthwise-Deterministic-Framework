# EarthWise — Impact × Feasibility Conservation Framework

A documented deterministic framework for screening and ranking declining U.S. species under explicit 10-year, Endangered Species Act, and low-intensity distributed-intervention constraints.

## Overview

This repository contains EarthWise Report v1.0, dated February 21, 2026, and a companion image of its species table. The report defines a canonical prompt, eligibility screen, fixed criteria, scoring worksheets, composite calculation, ranking, and ecological-assumption disclosure.

EarthWise is described as an environmental logic layer connecting CleanAirWise DI², CleanWaterWise DI², HazardWise DI², and EndangeredSpeciesWise DI². Those modules are referenced as framework context; their implementations are not bundled in this repository.

The output is a transparent model artifact. It is not a field deployment, population survey, or regulatory determination.

## Why It Matters

Conservation choices often combine ecological leverage with implementation friction. EarthWise makes those dimensions explicit so a reviewer can inspect the assumptions, reproduce the arithmetic, and recalculate the ranking when a material input changes.

## Core Control Model

The report’s execution path is:

**canonical prompt and constraints → eligibility filter → criterion scoring → Impact and Effort averages → multiplicative composite → ranked outputs → assumption review**

The fixed model is:

- Impact = (I1 + I2 + I3 + I4) / 4
- Effort = (E1 + E2 + E3 + E4) / 4
- Composite = Impact × Effort

Each criterion uses a 1–5 ordinal scale with equal weighting. In the report’s convention, a higher Effort score means lower implementation friction. No probabilistic weighting, adaptive adjustment, or secondary sort is used.

## What the Repository Contains

| Artifact | Role |
|---|---|
| [Framework_for_Stabilizing_Declining_U.S._Species_10-Year_Horizon](Framework_for_Stabilizing_Declining_U.S._Species_10-Year_Horizon) | 2,225-line EarthWise Report v1.0 with constraints, criteria I1–I4 and E1–E4, scoring trace, ranking, and assumptions disclosure. |
| [Table_10.1_Species_1-to-5.jpeg](Table_10.1_Species_1-to-5.jpeg) | Companion visual for the report’s top-five species table. |
| README.md | Review guide for the framework artifact. |

## What the Record Demonstrates

- **Constraint definition:** United States scope; species in measurable decline; exclusion of species currently listed as Endangered under the ESA; a 10-year horizon; and low-intensity, distributed intervention.
- **Scoring structure:** Impact and Effort are separated into four named criteria each, scored on a fixed 1–5 scale and averaged before multiplication.
- **Mechanical ranking:** The report states that composite value alone determines order, with no qualitative override or post-hoc adjustment.
- **Assumption disclosure:** Pollinator leverage, habitat response, disease, nest-box and cavity response, agricultural constraints, and climate stability are listed with materiality and risk classifications. The report states that a failed assumption requires manual score, composite, and rank recalculation.
- **Traceable worksheets:** Candidate screening, species-level assignments, composite calculations, sensitivity notes, and ranking explanations are included in the report.

### Published Ranking

| Rank | Species | Impact | Effort | Composite |
|---:|---|---:|---:|---:|
| 1 | Monarch Butterfly | 4.50 | 4.50 | 20.25 |
| 2 | Western Bumble Bee | 3.75 | 4.25 | 15.94 |
| 3 | American Kestrel | 3.50 | 4.00 | 14.00 |
| 4 | Red-headed Woodpecker | 3.50 | 3.50 | 12.25 |
| 5 | Chimney Swift | 3.25 | 3.25 | 10.56 |
| 6 | Northern Bobwhite | 2.50 | 2.50 | 6.25 |

These values are the report’s deterministic outputs under its stated criteria and assumptions.

## Recorded Checks

- **PASS — repository inventory:** the tracked tree contains the report, the companion table image, and README.md.
- **RECORDED — framework lock:** the report marks its criteria, composite structure, and ecological-assumption disclosure as complete.
- **RECORDED — integrity seal:** the report displays a “Document Integrity Seal” string for its canonical text. No verifier is included in this repository, so the string is preserved as report metadata rather than asserted here as an independently checked cryptographic result.
- **NO EXECUTABLE TEST SUITE:** no source tree, package manifest, or test runner is included.

## Technical Significance

The strongest feature of EarthWise is the explicit separation of ecological impact from implementation effort, followed by a non-compensatory multiplicative composite. Because criteria, scale, ranking rule, and assumption-failure response are written down before interpretation, a reviewer can see how a ranking was formed and identify exactly what must be recomputed when the model changes.

## Keep These Propositions Separate

| Proposition | What this repository supports |
|---|---|
| Model capability | The report performs a documented scoring and ranking exercise; it does not establish ecological outcomes in the field. |
| Governed execution | The artifact records a fixed prompt, criteria, formulas, and ranking procedure; no runtime implementation is tracked. |
| Replay, provenance, and auditability | The report is structured for manual recalculation and includes scoring trace sections; no executable replay or independent verifier is included. |
| Product or artifact status | This is a public framework report and companion visual, not a deployed conservation service. |
| External validation | Independent ecological review, field replication, and current source-data verification are not included in the tracked files. |

## Evaluation and Integration Context

Potential evaluation uses include transparent conservation prioritization, scenario comparison, and review of distributed-intervention assumptions. An organization could use the report as a model specification for a future data-backed pilot, provided that species data, regulatory status, and ecological assumptions are independently checked.

Those are evaluation or integration scenarios, not functions demonstrated by a deployed product here. For technical evaluation, licensing, or collaboration discussions, contact Grounded DI LLC through the [Grounded DI GitHub organization](https://github.com/Grounded-DI).

## Authorship and Provenance

Git history records the repository under **Grounded DI LLC**. The [initial commit](https://github.com/Grounded-DI/Earthwise-Deterministic-Framework/commit/415c275c38871ab15dc4d671f3ec11507a1f442f) is dated February 23, 2026 in local commit metadata; the [latest commit](https://github.com/Grounded-DI/Earthwise-Deterministic-Framework/commit/c399bc715718080610ca712dcf652ab69c2427c3) updates this README. The report itself is dated February 21, 2026.

No patent application or filing receipt is included in this repository. No open-source license is currently provided in this repository.

© Grounded DI LLC / applicable authors. All rights reserved except as otherwise expressly stated.

## Repository Scope and Limitations

This repository is a documented model package, not an ecological data or deployment package. The report refers to ecological literature and mainstream ecological understanding, but no bibliography, independent source audit, field data, or external review is tracked here. “Material stabilization” is the report’s defined objective, not a guarantee of population recovery. The table of contents also points to an Appendix II configuration/verification section for which no corresponding section appears in the tracked text.

## How to Review

1. Read Sections 1–3 of the [report](Framework_for_Stabilizing_Declining_U.S._Species_10-Year_Horizon) for the canonical prompt, constraints, and formulas.
2. Read Sections 7–10 for screening, species-level scoring, and the published ranking.
3. Read Section 14 for ecological assumptions and the manual-recalculation rule.
4. Use [Table 10.1](Table_10.1_Species_1-to-5.jpeg) as the visual companion and inspect Git history for chronology.

## Status

**PUBLIC FRAMEWORK REPORT / DETERMINISTIC RANKING MODEL — v1.0**
