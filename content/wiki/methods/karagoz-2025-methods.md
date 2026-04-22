# Karagoz 2025 — Methods

**Summary**: A dual-loop evaluation study combining predictive model-centered sanity checks with a randomized controlled trial of 97 medical experts to compare LIME and SHAP explanations on trust, confidence, and diagnostic agreement in chest X-ray classification.

**Sources**: Karagoz_XIMED.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (technical evaluation + randomized controlled trial)

## Sample
- N: 97 (human-centered component); 112,120 images (NIH Chest X-Ray dataset for predictive model)
- Population: medical experts (medical students, general practitioners, specialty trainees, and specialists)
- Domain: healthcare / medical imaging (chest X-ray diagnosis)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: post-hoc, model-agnostic local explanation (saliency/attribution maps)
- Manipulation or measure: between-subjects manipulation — participants assigned to LIME explanation group, SHAP explanation group, or no-XAI control group; explanations presented as visual overlays on chest X-rays highlighting regions influencing DenseNet121 predictions
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive; behavioural (secondary)
- Measure: pre/post Likert ratings of trust in the AI system (TRUSTpre, TRUSTpost); behavioural trust operationalized indirectly through diagnosis change (willingness to revise own diagnosis based on AI reasoning)
- Scale / instrument name: not reported (custom Likert items)
- Number of items: not reported
- Behavioural vs self-report: both (self-report primary; diagnosis change as behavioural measure)

## Moderators and covariates tested
- Initial trust (TRUSTpre): measured pre-explanation; found to be the strongest predictor of post-explanation trust
- Medical expertise level: participants spanned students through specialists; analyzed as a single group, not compared between levels (relevant to RQ3 as a gap)
- Diagnosis correctness: case-based analysis used correctness of initial diagnosis as a contextual moderator of agreement and trust outcomes
- Indicative vs. contra-indicative agreement (AGREEind, AGREEcont): novel operationalization distinguishing whether participants agreed with AI on disease-confirming vs. disease-ruling-out reasoning

## Statistical approach
- Primary analysis method: ANOVA (between-group trust and confidence comparisons); logistic/linear regression for diagnosis change and agreement outcomes; Pearson correlation (trust–confidence relationships by group)
- Software: not reported
- Key model fit or effect size reported: ANOVA F = 0.088, p = 0.916 (confidence); SHAP diagnosis change estimate = 0.2396, p = 0.033; AGREEcont SHAP c = −2.08, LIME c = −1.66; trust–confidence r = −0.24 (SHAP), 0.38 (LIME), 0.43 (control)

## Author-noted limitations
- Self-reported trust measures are limited; authors argue for complementing them with objective performance metrics (diagnosis correctness, diagnosis change rate)
- Single exposure to AI explanation may be insufficient to shift cognitive trust in clinical context
- Medical expertise levels were not compared statistically; between-expertise-level moderation is a noted gap
- Analysis is primarily group-level; case-based analysis is illustrative rather than confirmatory

## Related pages
- [[karagoz-ximed-medical-imaging]]
- [[explainability]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
