# Rezaeian 2025 — Methods

**Summary**: An interrupted time-series experiment with 28 clinicians (radiologists, oncologists, and other roles) comparing four progressively detailed levels of AI explanation in a breast cancer CDSS on self-reported trust, agreement, understandability, perceived accuracy, and objective diagnostic performance.

**Sources**: Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
quasi-experimental (interrupted time-series, within-subjects, four intervention conditions plus baseline)

## Sample
- N: 28 (17 radiologists, 5 oncologists, 6 other clinical roles)
- Population: domain professionals (clinicians)
- Domain: healthcare / oncology (breast cancer diagnosis)
- Country / region: not reported
- Recruitment method: not reported (hospital staff, convenience)

## Transparency operationalization
- Type: multi-level explanation including outcome disclosure, uncertainty visualization, and spatial saliency
- Manipulation or measure: Within-subjects progression through four intervention levels (after a no-AI baseline): Intervention I — AI classification only (no explanation); Intervention II — classification + per-class confidence scores; Intervention III — confidence scores + estimated tumor localization on ultrasound image; Intervention IV — tumor localization with both low- and high-confidence spatial bounds. Ten breast-tissue ultrasound images per condition. The AI system used a U-Net + CNN architecture with 81% accuracy.
- Scale / instrument name: not applicable (within-subjects experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported) and behavioural (agreement and diagnostic performance)
- Measure: (1) Self-reported trust — 5-point Likert scale per image ("How much do you trust the AI system?") and post-experiment survey item ("I trusted the AI suggestions"); (2) Behavioural trust — agreement scale (continuous; below-neutral agreement triggers manual override); (3) Objective diagnostic performance — whether final decisions were correct. Framework follows Kohn et al. (2021) dual-measure approach.
- Scale / instrument name: adapted from Kohn et al. (2021)
- Number of items: not reported
- Behavioural vs self-report: both used; Spearman correlation between agreement and trust reported (ρ = 0.85)

## Moderators and covariates tested
- Gender: measured; significantly predicted AI familiarity (men reported higher familiarity, χ² = 24.8, p < 0.001) but did not predict trust, performance, or agreement — relevant to RQ3
- Age: measured; not significantly associated with performance, trust, or agreement; older participants took longer to decide
- Years of clinical experience: measured; predicted AI familiarity and understandability (10–20 year group found AI most understandable); did not significantly predict behavioural trust or accuracy — relevant to RQ3

## Statistical approach
- Primary analysis method: mixed-effects linear models (with clinician as random effect; intervention as fixed effect) for trust, agreement, understandability, perceived accuracy, diagnostic accuracy, and decision time
- Software: not reported
- Key model fit or effect size reported: regression coefficients and p-values for each intervention vs. Intervention I; Spearman correlation ρ = 0.85 (agreement–trust); χ² = 24.8 (gender × AI familiarity)

## Author-noted limitations
- Small sample (N = 28) and single institution limit statistical power and generalisability
- Within-subjects design without counterbalancing means intervention order effects cannot be ruled out (all participants progressed from I to IV)
- AI system accuracy (81%) may not represent real-world clinical AI performance
- Only one imaging modality (ultrasound) and cancer type (breast) tested
- Self-reported AI familiarity may be a poor proxy for actual AI competence
- Recommendations for tailoring explanations to individual clinicians' expertise and preferences identified as future work

## Related pages
- [[rezaeian-ai-explanations-clinician-trust]]
- [[explainability]]
- [[uncertainty-visualization]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
