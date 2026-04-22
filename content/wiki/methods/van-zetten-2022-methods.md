# van Zetten et al. (2022) — Methods

**Summary**: A research-by-design case study at a Dutch financial institution that developed two XAI prototype systems — MLX1 (SHAP/Anchor-based local interpretability for mortgage reviewers) and MLX2 (global interpretability and fairness auditing for data scientists and compliance officers) — and evaluated MLX1 with 11 daily users, finding statistically significant improvements in trust, explanation satisfaction, and perceived performance.

**Sources**: van Zetten et al._Increasing trust and fairness in machine learning applications within the mortgage industry.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
quasi-experimental (research-by-design case study with pre/post within-subjects comparison for MLX1; expert evaluation for MLX2)

## Sample
- N: 11 (daily mortgage application reviewers who evaluated MLX1); additional stakeholders (data scientists, legal, risk, and compliance officers) evaluated MLX2 qualitatively
- Population: domain professionals — mortgage reviewers (non-expert ML users) and data scientists / compliance officers
- Domain: financial services / mortgage fraud detection (Dutch insurer / mortgage provider)
- Country / region: Netherlands
- Recruitment method: organisational convenience sample (employees of a single Dutch financial institution)

## Transparency operationalization
- Type: local interpretability (MLX1) and global interpretability plus fairness transparency (MLX2)
- Manipulation or measure: MLX1 — SHAP (TreeSHAP) and Anchor used to generate textual, ranked feature-importance explanations for individual mortgage applications classified as fraud risk, replacing a 22-rule hand-crafted explanation system; MLX2 — What If? tool and BlackBoxAuditing for global model interpretability; Aequitas fairness audit toolkit for demographic bias detection (false positive rate parity by migration background); evaluated via pre/post within-subjects comparison (before vs. after MLX1 deployment) and qualitative stakeholder interviews for MLX2
- Scale / instrument name: Hoffman et al. (2018) Trust Scale (3 items); explanation satisfaction (custom items); perceived performance (custom items)
- Number of items: 3 (trust scale); additional satisfaction and performance items (exact count not reported)

## Trust operationalization
- Type: cognitive trust (self-report); behavioural trust (proxied by reported decision quality and intent to use)
- Measure: Hoffman et al. (2018) Trust Scale measuring confidence in model, predictability, reliability, and believability; explanation satisfaction assessed via custom Likert items; perceived performance assessed via custom items; t-test comparison of overall user experience before and after MLX1 deployment
- Scale / instrument name: Hoffman et al. (2018) Trust Scale (3 items); Explanation Goodness Checklist (Hoffman et al., 2018) for qualitative evaluation
- Number of items: 3 (Hoffman trust scale); additional items not specified
- Behavioural vs self-report: both (self-report trust and satisfaction scales; reported behavioural outcomes including decision speed and quality improvements)

## Moderators and covariates tested
- User role / expertise: explicitly examined — three distinct role groups with different information needs and trust profiles: (1) daily mortgage reviewers (non-expert ML users needing local explanations), (2) data scientists (needing global interpretability), (3) legal/compliance/risk officers (needing auditable fairness metrics); role differences in information needs and explanation preferences are a central finding — directly relevant to RQ3
- Prior explanation system: MLX1 compared against the legacy 22-rule hand-crafted explanation system (pre/post design); not a moderator per se but frames the baseline comparison

## Statistical approach
- Primary analysis method: paired t-test for overall user experience comparison (MLX1 vs. rule-based baseline); descriptive statistics and median ratings for individual trust and satisfaction items; qualitative thematic analysis for MLX2 stakeholder evaluation
- Software: not reported
- Key model fit or effect size reported: overall user experience improvement t-value = 2.58, p = 0.014 (statistically significant); 10 of 11 reviewers reported MLX1 gave better guidance; median rating on trust and explanation satisfaction items = "Agree"; specific Cronbach's α for trust scale not reported

## Author-noted limitations
- Very small sample (N = 11 mortgage reviewers); statistical power is limited and findings may not generalise beyond this organisation
- Single-organisation case study conducted at one Dutch financial institution; results may reflect institutional-specific factors (culture, prior AI exposure, regulatory context)
- The authors warn that higher-detail explanations risk automation bias — reviewers may defer to model recommendations uncritically if they perceive the AI as more knowledgeable than warranted
- A more informative MLX1 variant (including context-based thresholds) was rejected by management due to concerns about compromising reviewer independence, illustrating organisational constraints on XAI design
- MLX2 evaluation was qualitative and did not include pre/post quantitative comparison with the same rigour as MLX1
- No control group; the pre/post design cannot rule out confounds such as novelty effects or training effects from the MLX1 deployment

## Related pages
- [[van-zetten-trust-fairness-mortgage-ml]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[institutional-trust]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
van Zetten, W., Ramackers, G. J., & Hoos, H. H. (2022). Increasing trust and fairness in machine learning applications within the mortgage industry. *Machine Learning with Applications, 10*, 100406.

Hoffman, R. R., Mueller, S. T., Klein, G., & Litman, J. (2018). Metrics for explainable AI: Challenges and prospects. arXiv:1812.04608.
