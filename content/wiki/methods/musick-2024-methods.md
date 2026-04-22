# Musick et al. 2024 — Methods

**Summary**: A 2 × 2 between-subjects experiment (N = 150) examining how explanation content (algorithmic vs. benefit) and timing (at disclosure vs. at recommendation) in a personality-based information-sharing recommender system affect user disclosure behaviour, trust competence, privacy concern, and satisfaction in temporary workplace teams.

**Sources**: Musick et al._Recommendations with benefits.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (2 × 2 between-subjects with baseline no-explanation control)

## Sample
- N: 150 (18–19 participants per condition)
- Population: general adult public (US workers)
- Domain: collaborative technology / workplace teams / recommender systems
- Country / region: United States
- Recruitment method: Prolific Academic

## Transparency operationalization
- Type: process transparency (algorithmic explanation) and outcome transparency (benefit explanation)
- Manipulation or measure: 2 × 2 factorial design crossing explanation content and explanation timing, plus a baseline no-explanation control: (1) content — algorithmic explanation (rationale based on system logic, e.g., "Based on how similar/different you and your teammate rank on this attribute and similar users...") vs. benefit explanation (rationale focused on team/individual benefits, e.g., "It is helpful for your teammates to understand how confident members are in their abilities..."); (2) timing — provided during disclosure stage (before personality sharing) vs. during recommendation stage (after sharing, when recommendations are delivered); participants completed a Big Five personality assessment, made binary disclosure decisions on eight personality facets, then received four recommendations for working with hypothetical teammates
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (trust competence) and dispositional (trust propensity)
- Measure: trust competence measured via 5-item scale (Benbasat & Wang, 2005) assessing perceived system expertise and ability to understand users' teamwork needs; trust propensity measured via 4-item dispositional trust scale (Jessup et al., 2019); privacy concern assessed via 3-item scale; system satisfaction and perceived helpfulness also collected
- Scale / instrument name: Benbasat & Wang (2005) trust competence scale; Jessup et al. (2019) trust propensity scale
- Number of items: 5 (trust competence), 4 (trust propensity), 3 (privacy concern)
- Behavioural vs self-report: self-report for all trust and attitude measures; disclosure decisions (binary: share or withhold each personality facet) serve as a behavioural outcome

## Moderators and covariates tested
- Trust propensity (dispositional trust): measured as individual difference covariate; positively predicted trust competence (β = 0.229, p = .013) and negatively predicted privacy concern (β = −0.273, p = .002) — relevant to RQ3 as an individual-level user factor
- Perceived accuracy of personality results: measured covariate; strongly predicted trust competence (β = 0.211, p = .045) and perceived helpfulness (β = 0.682, p = .007)
- Explanation timing (disclosure vs. recommendation): manipulated; interacted with content to shape trust effects
- User expertise / AI literacy: not measured or manipulated; sample is lay US adult workers with no AI expertise requirement

## Statistical approach
- Primary analysis method: structural equation modelling (SEM) / path analysis; one-tailed t-tests for directional hypotheses on trust and privacy outcomes; OLS regression for disclosure behaviour
- Software: not reported
- Key model fit or effect size reported: β = 0.470, p_one-tailed = .030 (benefit explanations at recommendation stage on trust competence); β = −0.323, p_one-tailed = .028 (benefit explanations on privacy concern reduction); trust propensity → trust competence β = 0.229, p = .013; privacy concern → satisfaction β = −0.535, p < .001

## Author-noted limitations
- Small N per cell (18–19) limits statistical power; some effects only marginally significant
- Single-session online study with hypothetical teammates; ecological validity for real temporary team contexts is limited
- Personality assessment accuracy was not validated; perceived accuracy varied and confounded trust effects
- No AI expertise measure collected; effects may differ for users with AI literacy
- Benefit explanation content was designed for this specific recommender system; generalisability to other recommendation domains is unclear
- Study does not examine long-term trust dynamics or repeated system interactions

## Related pages
- [[musick-recommendations-benefits]]
- [[process-transparency]]
- [[outcome-transparency]]
- [[disclosure]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[algorithmic-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
