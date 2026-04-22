# Conijn 2023 — Methods

**Summary**: A between-subjects experiment (N = 150 university students) comparing three transparency conditions — no explanation, accuracy statement, and full-text global explanation — in an automated essay scoring context, finding null effects of both explanation types on trust and motivation.

**Sources**: Conijn et al._The effects of explanations in automated essay scoring systems.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects)

## Sample
- N: 150
- Population: university students
- Domain: higher education / automated essay scoring
- Country / region: not reported
- Recruitment method: convenience (university students; two focus groups of N = 11 used for explanation needs-elicitation prior to the main study)

## Transparency operationalization
- Type: algorithmic transparency — outcome transparency (accuracy statement) and process transparency (full-text global explanation)
- Manipulation or measure: Three between-subjects conditions: (1) Control — system grade only, no explanation; (2) Accuracy statement — brief confidence statement noting the system is accurate approximately 90% of the time; (3) Full-text global explanation — detailed description of the system's features (content, structure, cohesiveness, plagiarism, basic writing features), training methodology, and worked examples. Explanations designed using XAI guidelines (Kulesza et al., 2015; Lim & Dey, 2010; Mueller et al., 2021) and a prior user needs-elicitation focus group.
- Scale / instrument name: not applicable (between-subjects manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report) and behavioural (grade adaptation)
- Measure: (1) Trust in Automation (TiA) scale — subjective trust; (2) Weight of Advice (WoA) — behavioural measure of the degree to which students adjusted their self-estimated grade toward the system grade after seeing it.
- Scale / instrument name: Trust in Automation (TiA) scale (Jian et al., 2010); Propensity to Trust Technology (PTT) scale (Jessup et al., 2019) as dispositional covariate
- Number of items: 12 items (TiA; 1–7 scale; α = .88)
- Behavioural vs self-report: both used (TiA = self-report; WoA = behavioural)

## Moderators and covariates tested
- Propensity to Trust Technology (PTT): measured as dispositional trust covariate; significantly predicted subjective trust (B = 0.25, p = .020)
- Need for Cognition: measured; small interaction with accuracy statement on motivation (p = .03) but no significant moderation of trust; relevant to RQ3
- Grade discrepancy (system grade minus self-estimated grade): measured as continuous covariate; large non-linear (quadratic) effect on both subjective trust and behavioural trust — dominant predictor of both outcomes

## Statistical approach
- Primary analysis method: OLS regression (with trust and WoA as outcomes; explanation condition, covariates, and non-linear grade discrepancy terms as predictors); ANOVA for omnibus test of explanation condition on TiA (F(2,147) = 2.14, p = .12)
- Software: not reported
- Key model fit or effect size reported: F(2,147) = 2.14, p = .12 (TiA omnibus); regression coefficients and p-values for individual predictors; Cronbach's α = .88 for TiA; correlation between TiA and WoA reported as non-significant (B = 0.12, p = .44)

## Author-noted limitations
- Only global (whole-system) explanations tested; absence of local (essay-specific) and counterfactual explanations limits conclusions
- Wizard-of-Oz system providing fixed grades may not reflect real AES use
- Students may not represent the full range of stakeholders (teachers absent from study)
- No independent verification of whether students read and understood the full-text explanation fully
- Grade discrepancy effect dominates: students who received lower-than-expected grades showed lower trust regardless of explanation
- Single domain (university essay assessment); findings may not generalise to other educational or grading contexts

## Related pages
- [[conijn-explanations-essay-scoring]]
- [[algorithmic-transparency]]
- [[outcome-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[dispositional-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
