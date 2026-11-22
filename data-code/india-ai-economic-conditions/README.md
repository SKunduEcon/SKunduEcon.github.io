# India AI Economic Conditions Index (IAECI)

Independent research project by Shiny Kundu.

## Purpose

The IAECI is designed to measure the economic diffusion and consequences of AI adoption in India. It is informed by the Anthropic Economic Index and the task-based labour-market framework developed by Maxim Massenkoff and Peter McCrory, but is an independent project and is not affiliated with or endorsed by Anthropic.

## Current status: baseline framework, not a published composite

The first public edition is a methodological baseline. It does not report a single 0–100 index value. Anthropic's India country brief is based on one short Claude.ai sampling window (13–20 November 2025), while firm and labour-market indicators have different populations, frequencies and reference periods. Combining these into a headline score would create false precision.

A composite will be released only after a comparable India-level panel has been assembled and the treatment of missing data, weights, indicator direction and structural breaks has been documented.

## Proposed architecture

The composite is designed around three equally weighted pillars:

1. **Diffusion and access (D):** per-capita use, enterprise adoption and production deployment, state/sector/occupation breadth, concentration, connectivity and skills.
2. **Productive integration (P):** work-related use, automation versus augmentation, task complexity and success, autonomy, task time savings, process redesign and firm-level productivity/ROI.
3. **Labour-market transmission (L):** employment, hiring, entry-level job starts, hours, real earnings, separations, unemployment and occupational transitions among more- and less-exposed work.

Proposed headline formula once the panel is available:

IAECI(t) = [D(t) + P(t) + L(t)] / 3

Indicators will be oriented so that higher values consistently represent stronger economic conditions, standardised against a fixed reference distribution, and aggregated transparently. Concentration enters the diffusion pillar with a negative sign. Labour-market indicators will be interpreted relative to appropriate comparison groups. Equal pillar weights are the initial specification; alternative weights and aggregation methods will be reported as sensitivity tests.

## First baseline: Anthropic India brief

The Anthropic India country brief reports the following for Claude.ai conversations sampled 13–20 November 2025:

- India: 5.8% of global Claude.ai use; second-largest national share.
- Per-capita ranking: 101st of 116 countries with sufficient observations, adjusted for working-age population.
- Four largest state shares: Maharashtra 15.5%, Tamil Nadu 13.2%, Karnataka 12.7%, Delhi 10.5%; combined 51.9%.
- Software-related tasks: 45.2% of India's O*NET-mapped use.
- Work-related conversations: 51.3%; global comparison 46.0%.
- Estimated time without AI: 3.8 hours; estimated time with AI: 14.8 minutes.
- Autonomy score: 3.60/5; global comparison 3.38/5.
- Tasks estimated completable by a human alone: 84.6%; global comparison 87.9%.

These are platform-use statistics, not nationally representative estimates of AI adoption, labour productivity or employment effects. The time-compression estimate is a task-level measure and is not equivalent to measured firm-level productivity.

## Data sources for the next phase

- Anthropic Economic Index public dataset: https://huggingface.co/datasets/Anthropic/EconomicIndex
- Anthropic India country brief: https://www.anthropic.com/research/india-brief-economic-index
- Anthropic observed exposure paper: https://www.anthropic.com/research/labor-market-impacts
- World Bank India Enterprise Survey AI follow-up 2026: https://microdata.worldbank.org/catalog/8552/study-description
- PLFS microdata catalogue: https://microdata.gov.in/nada/index.php/catalog/PLFS
- PLFS Annual Report 2025: https://www.mospi.gov.in/uploads/latestReleases/latest_release_1774607827733_3e8964a9-268b-4cc9-ad65-cfc8a9e32f08_Press_note_AR_PLFS_2025_23032025_V2.1_260326_final.pdf

## Critical methodological steps

1. Verify whether the June 2026 Anthropic release provides a consistent India-level monthly panel; do not splice it mechanically with the November 2025 country cross-section.
2. Map O*NET task and SOC occupation codes to India's NCO-2015, documenting many-to-many mappings and uncertainty.
3. Use World Bank Enterprise Survey weights and its target population. The 2026 AI follow-up covers registered establishments with at least five employees; it does not represent informal and micro enterprises.
4. Use PLFS weights, survey redesign breaks and occupational coding consistently. Distinguish usual status from current weekly status.
5. Test the sensitivity of the composite to weights, normalisation, missingness and the treatment of concentration.
6. Keep descriptive monitoring separate from causal evaluation. Adoption and exposure are not causal estimates of productivity or job displacement.

## Citation

Shiny Kundu (2026), *India AI Economic Conditions Index: Framework and Baseline*, research project and methodological note.
