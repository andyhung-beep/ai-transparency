# Aoki et al. (2023) — Methods

**Summary**: Two pre-registered online survey experiments (total N = 1,200 Japanese corporate officers) testing whether four XAI explanation types differentially affect perceived accuracy, fairness, and trustworthiness of adverse governmental algorithmic decisions across two decision scenarios (grant rejection and tax audit).

**Sources**: Aoki et al._Explainable AI for government.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (two pre-registered between-subjects online survey experiments)

## Sample
- N: 1,200 (600 per study)
- Population: corporate officers (senior officers at stock companies registered in Japan)
- Domain: public administration / e-government (Study 1: government grant application rejection; Study 2: tax authority on-site inspection selection)
- Country / region: Japan
- Recruitment method: not reported (online survey panel; surveys conducted December 2022)

## Transparency operationalization
- Type: explanation (four XAI explanation types operationalizing distinct transparency mechanisms in public administration)
- Manipulation or measure: between-subjects manipulation — participants randomly assigned to one of five conditions: (1) no explanation; (2) input-based explanation (feature-contribution / SHAP-style, indicating which input variables drove the decision); (3) group-based explanation (outcome distribution stating the proportion of similar entities receiving the same decision); (4) case-based explanation (similar past case from training data presented for comparison); (5) counterfactual explanation (smallest input change that would produce a favorable outcome). Both studies used the same five conditions applied to different decision scenarios.
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: institutional (trustworthiness perceived by the affected party regarding a governmental algorithmic decision and, by extension, the public institution making it)
- Measure: self-reported rating of the perceived trustworthiness of the algorithmic decision, assessed on a scale after reading the scenario and explanation; perceived fairness and perceived accuracy were assessed as separate but related outcomes
- Scale / instrument name: not reported (custom self-report rating items)
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Decision context / scenario (Study 1: grant rejection vs. Study 2: tax audit): varied between studies; moderated which explanation type was most effective across the three outcome variables — no single explanation type uniformly outperformed others in both contexts
- Note: user expertise and role were not examined as independent variables; all participants were senior corporate officers (a professional but non-technical sample). Relevant to RQ3 only as a partially homogeneous professional group.

## Statistical approach
- Primary analysis method: ANOVA (between-subjects comparisons across explanation conditions) with pairwise comparisons for each outcome variable (perceived fairness, perceived accuracy, perceived trustworthiness); regression analyses also referenced in source summary
- Software: not reported
- Key model fit or effect size reported: p-values and significance levels reported; specific effect sizes not reported in source summary

## Author-noted limitations
- Effects of specific explanation types were inconsistent across the two scenarios, limiting generalizable conclusions about which type is best
- Participants were Japanese corporate officers — a professional but narrow and culturally specific sample; findings may not generalize cross-culturally or to lay citizens
- Scenarios were hypothetical; actual affectee responses to real governmental decisions may differ
- The study does not examine the mechanisms by which explanation type influences perceptions (e.g., comprehension, procedural justice perceptions) separately
- The normative legal framework mandating the right to explanation (GDPR-style) is not fully aligned with empirical evidence from this study

## Related pages
- [[aoki-xai-government]]
- [[counterfactual-explanations]]
- [[explainability]]
- [[process-transparency]]
- [[institutional-trust]]
- [[algorithmic-transparency]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References
Aoki, N., et al. (2023). *Explainable AI for government: Does the type of explanation matter to the accuracy, fairness, and trustworthiness of an algorithmic decision as perceived by those who are affected?* [Journal not reported in source summary.]

Lee, J. D., & See, K. A. (2004). Trust in automation: Designing for appropriate reliance. *Human Factors, 46*(1), 50–80.
