# The Impact of AI Explanations on Clinicians' Trust and Diagnostic Accuracy in Breast Cancer

**Source file**: [Original article](../../raw/Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.pdf)

**Summary**: This interrupted time-series experiment with 28 clinicians tests four levels of AI explanation in a breast cancer CDSS and finds that increasing explanation complexity does not reliably improve trust or diagnostic performance — and that the most detailed explanation condition actually degraded understandability, perceived accuracy, and diagnosis accuracy relative to the simplest condition.

**Sources**: Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Rezaeian, Asan, and Bayrak (2025, *Applied Ergonomics*) present a human-subject experiment designed to assess how varying levels of AI explainability influence clinicians' trust and diagnostic performance in a breast cancer clinical decision support system (CDSS). The system uses a U-Net + CNN architecture (81% accuracy) to classify ultrasound images as healthy, benign tumor, or malignant tumor.

The study uses an interrupted time series (ITS) design where all 28 clinicians (17 radiologists, 5 oncologists, 6 other roles) progress through four intervention conditions with increasing levels of explanation, preceded by a no-AI baseline:

- **Baseline**: Clinicians diagnose alone, no AI support.
- **Intervention I (No Explanation)**: AI provides a 3-class diagnosis only.
- **Intervention II (AI Confidence)**: Diagnosis plus confidence scores per class.
- **Intervention III (Tumor Localization)**: Confidence scores plus estimated tumor location on the image.
- **Intervention IV (Enhanced Tumor Localization)**: Tumor location shown with both low- and high-confidence bounds.

Ten breast tissue images per condition, with self-reported trust, agreement, understandability, and perceived accuracy collected after each intervention, alongside objective performance and decision time.

The domain is healthcare / oncology.

## Key Findings

- Using AI (any intervention type) significantly improved diagnostic performance compared to the standalone baseline, confirming that CDSS support adds value for clinicians. [Domain: healthcare/oncology]
- Increasing explanation levels did not consistently improve trust. The mixed-effects model found no statistically significant trust differences across interventions; coefficients for Interventions II and IV were slightly negative relative to I (–0.049 and –0.145), while Intervention III was slightly positive (0.059). [Domain: healthcare/oncology]
- Overall trust increased above baseline after clinicians began using the AI, regardless of explanation type (all intervention coefficients significant vs. baseline: 0.888–0.944), suggesting that AI use itself — not explanation level — drives initial trust formation. [Domain: healthcare/oncology]
- The most detailed explanation condition (Intervention IV, enhanced tumor localization) significantly reduced understandability relative to Intervention I (coefficient –0.464, p = 0.013), suggesting cognitive overload from excessive detail. [Domain: healthcare/oncology]
- Perceived accuracy was significantly lower in Interventions II and IV than in Intervention I (–0.321, p = 0.011; –0.250, p = 0.048), indicating that confidence scores and complex localization information may undermine clinicians' confidence in the system. [Domain: healthcare/oncology]
- Diagnostic accuracy was significantly reduced in Interventions III and IV compared to Intervention I (–0.073, p = 0.005; –0.068, p = 0.009). The simplest AI explanation (no explanation beyond the classification) produced the best performance. [Domain: healthcare/oncology]
- The fourth intervention (highest explainability) also produced significantly longer decision times (p = 0.011), confirming increased cognitive load. [Domain: healthcare/oncology]
- Agreement was significantly lower in Intervention IV than in Intervention I (–0.149, p = 0.048). A strong positive Spearman correlation between agreement and trust was found (ρ = 0.85, p < 0.05). [Domain: healthcare/oncology]
- Clinicians' trust increased even when both the clinician and AI were incorrect (agreement with wrong AI output), replicating a pattern of trust persistence despite shared errors (consistent with Vicente & Matute, 2023). [Domain: healthcare/oncology]
- Gender significantly predicted AI familiarity (men reported higher familiarity, χ² = 24.8, p < 0.001) but did not predict behavioral measures of trust, performance, or agreement — suggesting self-reported familiarity is a poor proxy for actual interaction quality. [Domain: healthcare/oncology]
- Age was not significantly associated with performance, trust, or agreement, but older participants took longer to make decisions. Experience predicted AI familiarity and understandability, with 10-20 year experience group finding AI most understandable. [Domain: healthcare/oncology]
- Despite CDSS support, average clinical accuracy across all interventions remained below the standalone AI's 81% accuracy, indicating room for improvement in human-AI collaborative performance. [Domain: healthcare/oncology]

## Transparency Constructs

The study operationalizes transparency as a four-level ordinal progression:

1. **No explanation** — AI provides only the classification output (outcome transparency without rationale).
2. **Confidence scores** — Adds probability scores per class, a form of [[uncertainty-visualization]].
3. **Tumor localization** — Adds spatial visualization of likely tumor location, a form of saliency-based explanation embedded in the image.
4. **Enhanced localization with confidence bounds** — Two-level spatial heatmap (low vs. high confidence region), the most information-rich intervention.

This design explicitly tests whether more transparency is always better. The finding that Intervention IV degrades understandability and performance relative to Intervention I is a strong caution against equating more information with more transparency. The study aligns with [[explainability]] research showing cognitive load as a limiting factor for transparency benefits.

## Trust Constructs

The study uses a dual-measure approach following Kohn et al. (2021):

- **Self-reported trust**: 5-point Likert scale per image during experiment ("How much do you trust the AI system?") and post-experiment survey item ("I trusted the AI suggestions").
- **Behavioral trust (agreement/reliance)**: Whether the clinician accepted the AI suggestion (operationalized via a continuous agreement scale; below-neutral agreement triggers a manual override).
- **Behavioral trust (performance)**: Whether clinicians' final decisions were correct.

This decomposition separates [[cognitive-trust]] (self-reported confidence) from [[behavioural-trust]] (actual reliance). The study finds that these can diverge: behavioral trust (agreement, performance) degraded at high explanation levels even when self-reported trust remained stable. The strong correlation between agreement and trust (ρ = 0.85) suggests that in this domain, behavioral alignment with the AI serves as a proxy for trust.

The study also references the trust calibration framework (Lee & See, 2004): a central goal is achieving appropriate reliance, where clinicians trust the AI to the degree that reflects its actual reliability, rather than over- or under-relying.

## Relevance to Research Questions

**RQ1**: The study operationalizes both self-reported and behavioral trust alongside explainability level — a methodologically careful approach. It demonstrates that self-reported familiarity with AI diverges from behavioral measures, cautioning against using self-report as the sole trust indicator. Trust is conceptualized as a latent construct measured via multiple indirect indicators (source: Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.txt).

**RQ2**: A key non-linear finding: the relationship between explanation level and trust (and performance) is not monotonically positive. In fact, the highest-explanation condition is the worst-performing. This constitutes direct evidence for a cognitive-load threshold beyond which additional transparency backfires — sometimes called the "explainability paradox" (Evans et al., 2022). The simplest AI output format (classification only) maximized performance and minimized cognitive load, while the richest format impaired understandability, perceived accuracy, agreement, and decision accuracy (source: Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.txt).

**RQ3**: Self-reported demographic variables (gender, age, experience) significantly predict self-reported AI familiarity and understandability but do not predict behavioral trust, performance, or agreement. This is an important finding: experienced clinicians are not more responsive to complex explanations in terms of accuracy. Experience effects (if any) on behavioral outcomes are absent. The study recommends tailoring explanations to clinicians' specific expertise and preferences as future work (source: Rezaeian et al._The impact of AI explanations on clinician_s trust and disgnostic accuracy.txt).

## Related pages

- [[explainability]]
- [[uncertainty-visualization]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[domain-context]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
