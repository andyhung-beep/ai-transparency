# Angerschmid et al. (2022) — Methods

**Summary**: Online user study (N = 25) using a 3 × 3 mixed factorial design to examine how explanation type (none, example-based, feature importance-based) and introduced fairness level (no information, low, high) jointly affect trust and perceived fairness in AI-assisted health decision making.

**Sources**: Angerschmid et al._Fairness_and_Explanation_in_AI.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (online user study; mixed within-between factorial design)

## Sample
- N: 25
- Population: general public (online participants)
- Domain: healthcare (health insurance decision-making and medical treatment decision-making)
- Country / region: Austria / Australia (study affiliations; participant country not reported)
- Recruitment method: not reported

## Transparency operationalization
- Type: explanation (feature importance-based and example-based XAI explanations); fairness disclosure (introduced fairness level)
- Manipulation or measure: within-subjects manipulation across nine conditions per scenario — three explanation conditions (no explanation; example-based explanation presenting similar past cases; feature importance-based explanation showing variable contributions and magnitudes) × three fairness conditions (no fairness information; low introduced fairness stated as unfair distribution across demographic groups; high introduced fairness stated as fair distribution). Fairness was operationalized as a stated percentage of fair vs. unfair decision distribution across groups, not a traditional XAI explanation.
- Scale / instrument name: not applicable (experimental manipulation, not a scale)
- Number of items: not applicable

## Trust operationalization
- Type: general (single undifferentiated trust construct; not disaggregated into cognitive vs. affective)
- Measure: self-report Likert-type scale of user trust in AI-informed decision making; ratings were normalized within-subjects to control for individual rating-style differences
- Scale / instrument name: not reported (custom Likert-type trust item(s))
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Application scenario (health insurance vs. medical treatment): manipulated by design; moderated the relative advantage of feature importance vs. example-based explanations on trust
- Introduced fairness level (low, high, no information): manipulated by design; low fairness consistently reduced trust; high fairness did not significantly increase trust above the no-information baseline
- Note: user expertise was NOT examined as a variable; relevant to RQ3 as a gap

## Statistical approach
- Primary analysis method: one-way and two-way ANOVA with Bonferroni-corrected pairwise comparisons
- Software: not reported
- Key model fit or effect size reported: p-values reported (e.g., explanation effect p < 0.001; low fairness effect p < 0.001; feature importance under low fairness p = 0.006; health insurance scenario difference p = 0.021); effect sizes not reported in source summary

## Author-noted limitations
- Small sample size (N = 25) limits statistical power and generalizability
- Trust measured as a single aggregate construct; cognitive vs. affective trust not disaggregated
- Explanation type and fairness introduced jointly in a controlled scenario may not reflect natural AI interactions
- Study limited to two health-related scenarios; other domains may produce different patterns
- Participant demographics and recruitment method not detailed in available summary

## Related pages
- [[angerschmid-fairness-explanation-ai]]
- [[explainability]]
- [[example-based-explanations]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References
Angerschmid, A., et al. (2022). *Fairness and explanation in AI-informed decision making*. [Journal not reported in source summary.]
