# Diprose 2020 — Methods

**Summary**: A survey study (N = 170 physicians from New Zealand) examining relationships among understanding, explainability, and trust in ML risk calculator outputs, comparing no explanation, global model-agnostic, and local model-agnostic explanation conditions.

**Sources**: Diprose et al._Physician understanding.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
survey (cross-sectional, repeated-measures within each respondent across three explanation conditions)

## Sample
- N: 170 (out of 1,315 surveyed; 13% response rate)
- Population: domain professionals (physicians / clinicians)
- Domain: healthcare (pulmonary embolism risk prediction)
- Country / region: New Zealand
- Recruitment method: hospital staff (district health boards and primary health organisations across New Zealand)

## Transparency operationalization
- Type: explainability — post-hoc model-agnostic explanations (global and local)
- Manipulation or measure: Three within-respondent conditions presented sequentially: (1) No explanation — ML risk calculator output with no accompanying explanation (control); (2) Global model-agnostic explanation — variable importance plot or Individual Conditional Expectation (ICE) plot; (3) Local model-agnostic explanation — LIME or Shapley values (patient-specific feature attribution). Physicians rated each output on three items: how much it made sense, whether they could explain it to a patient, and whether they would follow the recommendation.
- Scale / instrument name: not applicable (researcher-designed items for each condition)
- Number of items: 3 items per condition (understanding, explainability, intended behaviour)

## Trust operationalization
- Type: behavioural (intended compliance)
- Measure: Single item: "Would you follow this recommendation?" — operationalised as intended clinical compliance/reliance. Captures behavioural trust rather than attitudinal trust.
- Scale / instrument name: not applicable (single researcher-designed item)
- Number of items: 1
- Behavioural vs self-report: self-report of intended behaviour (behavioural intention)

## Moderators and covariates tested
- Physician specialty and experience: captured in sample demographics; not formally tested as moderator
- Explanation format preference: qualitative word-cloud analysis of open-ended physician preferences (simplicity, patient specificity, confirmation of existing clinical knowledge) — not a formal moderator analysis
- Note: physicians are an expert user group whose domain expertise is the key user-role characteristic relevant to RQ3; no within-study moderator analysis of expertise levels performed

## Statistical approach
- Primary analysis method: Cochran-Mantel-Haenszel chi-square tests (for associations between understanding, explainability, and intended behaviour across explanation conditions); McNemar pairwise tests (for comparing intended behaviour across explanation types)
- Software: not reported
- Key model fit or effect size reported: Cochran-Mantel-Haenszel χ² = 156.3 (understanding-explainability association, p < .001); χ² = 128.7 (understanding-trust association, p < .001); χ² = 61.2 (explainability-trust association, p < .001); all McNemar pairwise comparisons for explanation type effects on intended behaviour non-significant

## Author-noted limitations
- Low response rate (13%) introduces potential response bias toward physicians more interested in AI/ML
- Hypothetical scenario using a simulated ML output (not real patient data); ecological validity limited
- All physicians exposed to all three conditions in the same order (no counterbalancing); order effects possible
- Study does not separately measure cognitive vs. affective dimensions of trust
- No comparison of different physician specialties' responses to explanation formats
- Potential mismatch between physician-defined "sufficient explanation" and GDPR legal standards not empirically resolved

## Related pages
- [[diprose-physician-understanding-ml]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
