# Shin 2021 — Methods

**Summary**: A survey-based structural equation modeling study (N not reported) examining how causability (user-side interpretation ability) mediates the relationships between fairness, accountability, and transparency (FAT) perceptions and user trust and performance expectancy in a news recommendation AI system.

**Sources**: Shin_The effects of explainability and causability on perception, trust, and acceptance.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
survey (cross-sectional, structural equation modeling)

## Sample
- N: not reported
- Population: news recommendation system users (general public)
- Domain: media / news recommendation
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: explainability (system-level property) and causability (user-level ability to evaluate explanations); embedded within FAT (fairness, accountability, transparency) framework
- Manipulation or measure: Survey-based measure — participants assessed their perceptions of the AI news recommendation system's explainability (degree to which AI decision processes can be traced and communicated), transparency, fairness, and accountability using Likert-scale items. Causability operationalized as the extent to which users can subjectively understand and evaluate the quality of AI explanations (adapted from Holzinger et al.'s medical informatics construct). Explanations in the system describe why certain articles are recommended.
- Scale / instrument name: author-developed scales based on the Heuristic-Systematic Model (HSM) and FAT framework; causability adapted from Holzinger et al.
- Number of items: not reported

## Trust operationalization
- Type: cognitive trust (confidence in system competence and reliability); affective component noted (causability providing "emotional confidence")
- Measure: Self-report Likert-scale items for trust in the AI recommendation system. Trust treated as a latent variable mediating FAT perceptions and performance expectancy. Performance expectancy (behavioral intention to use the service) used as the downstream behavioral outcome.
- Scale / instrument name: author-developed trust scale; performance expectancy adapted from technology acceptance literature
- Number of items: not reported
- Behavioural vs self-report: self-report (trust and performance expectancy are both self-reported intentions)

## Moderators and covariates tested
- None explicitly tested as moderators; the model is fully mediated through causability and trust. Causability is implicitly tied to user expertise and cognitive capacity (users vary in their ability to process explanations), but no subgroup comparisons by expertise level are conducted — relevant to RQ3 as an identified gap

## Statistical approach
- Primary analysis method: structural equation modeling (SEM) with partial least squares (PLS) or covariance-based SEM (specific variant not confirmed in source); mediation analysis via variance accounted for (VAF)
- Software: not reported
- Key model fit or effect size reported: standardized path coefficients (causability → explainability = 0.939; trust → performance expectancy = 0.911; trust R² = 0.581); VAF values for mediation (31–50% across FAT dimensions); specific model fit indices not reported in source

## Author-noted limitations
- Cross-sectional survey design limits causal inference
- Sample characteristics not reported; generalisability unknown
- Single domain (news recommendation) may limit applicability to higher-stakes contexts
- Causability construct adapted from medical informatics context; validity in media domain not established independently
- Expert vs. novice users not compared; assumes homogeneous user population

## Related pages
- [[shin-explainability-causability-trust]]
- [[explainability]]
- [[causability]]
- [[algorithmic-trust]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
