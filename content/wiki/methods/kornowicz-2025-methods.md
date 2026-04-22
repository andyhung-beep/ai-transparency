# Kornowicz 2025 — Methods

**Summary**: An incentivised between-subjects online behavioural experiment (n = 216) using a judge-advisor system paradigm to test whether the method used to select features for an ML model (algorithm-based, expert-based, or combined) affects user preferences and actual advice reliance across two decision domains.

**Sources**: Kornowicz & Thommes_Algorithm, expert, or both_.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects incentivised online behavioural experiment; judge-advisor system)

## Sample
- N: 216 (after exclusions)
- Population: general public (59.7% women, mean age 34.2, UK-based)
- Domain: medical (cardiovascular disease classification — "Cardio") and sports (soccer match outcome prediction — "Football")
- Country / region: United Kingdom
- Recruitment method: Prolific

## Transparency operationalization
- Type: process transparency (feature-selection method disclosure)
- Manipulation or measure: between-subjects manipulation of feature-selection method — (1) Algorithm: features selected by a data-driven algorithm; (2) Expert: features selected by domain experts; (3) Combination: features selected jointly by algorithm and experts; participants could see which 6 of 12 features the model used (partial outcome transparency); two treatment arms: Choice (participants selected preferred method before tasks) and No Choice (method randomly assigned)
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: behavioural trust (reliance); attitudinal preference (proxy for cognitive/affective trust)
- Measure: (1) Switch to Advice — whether a participant changed a binary decision to align with the ML model's prediction when the two initially disagreed (incentivised revealed-preference measure; primary DV); (2) Stated preferences — pre-task preference for feature-selection method (proxy for attitudinal trust)
- Scale / instrument name: not applicable (behavioural measure); not reported (attitudinal preference item)
- Number of items: not applicable
- Behavioural vs self-report: both (behavioural Switch to Advice primary; self-report stated preferences secondary)

## Moderators and covariates tested
- Decision domain (Cardio vs. Football): significant positive moderator — reliance 17.98 percentage points higher in Cardio than Football despite identical payoff structures (relevant to RQ2 conditional effect)
- Self-reported confidence in initial decision: measured; negatively associated with reliance
- Age: measured; older participants relied less on AI
- Openness (Big Five personality): measured; negatively associated with reliance
- Risk-taking propensity: measured; higher risk-taking associated with preference for Algorithm and Combination over Expert
- Technology affinity and AI attitude: measured as covariates; not reported as significant
- User choice (Choice vs. No Choice treatment): tested; did not significantly affect reliance (H3 rejected)
- User expertise / AI literacy: not measured as a formal moderator; lay sample only (relevant to RQ3 as a gap)

## Statistical approach
- Primary analysis method: logistic regression (Switch to Advice as binary DV); chi-square tests (stated preferences); linear mixed-effects models
- Software: not reported
- Key model fit or effect size reported: no significant effect of feature-selection method on Switch to Advice in No Choice treatment; domain effect = 17.98 percentage points (p < 0.05); Combination selected most in Choice treatment (47.7%), deviating significantly from chance

## Author-noted limitations
- Lay participants only — authors argue known biases are similar across lay and professional populations, but domain-expert generalizability is not established
- No between-method differences on reliance despite strong stated preferences — attitude–behaviour gap is theorized but not explained by any measured variable
- Domain manipulation confounded with task characteristics (medical vs. sports); objective stakes were held constant by design but subjective salience may differ
- Short-term laboratory-like task; no longitudinal follow-up on reliance patterns

## Related pages
- [[kornowicz-algorithm-expert-reliance]]
- [[algorithm-aversion]]
- [[behavioural-trust]]
- [[process-transparency]]
- [[appropriate-reliance]]
- [[domain-context]]
