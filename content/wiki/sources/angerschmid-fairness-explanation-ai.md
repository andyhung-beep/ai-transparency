# Fairness and Explanation in AI-Informed Decision Making

**Source file**: [Original article](../../raw/Angerschmid et al._Fairness_and_Explanation_in_AI.pdf)

**Summary**: Angerschmid et al. conduct a user study (N = 25) across two health-related decision scenarios — health insurance and medical treatment — to examine how different explanation types (example-based and feature importance-based) and introduced fairness levels (low, high, no information) jointly affect user trust and perceived fairness in AI-assisted decision making, finding that explanations generally increase trust and fairness perceptions, while low introduced fairness consistently decreases both.

**Sources**: Angerschmid et al._Fairness_and_Explanation_in_AI.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

This paper investigates the combined effects of AI explanation type and introduced algorithmic fairness on user trust and perceived fairness in AI-assisted decision making. The motivation is that transparency/explanation and fairness are frequently studied in isolation, yet in practice they appear together in sociotechnical AI systems. The authors draw on prior work relating causability, feature importance, and example-based explanations to trust, alongside procedural justice and fairness theory.

An online user study was conducted with 25 participants across two scenarios: (1) health insurance decision-making and (2) medical treatment decision-making. The experimental design was a 3 (fairness: no information, low, high) × 3 (explanation: no explanation, example-based, feature importance-based) mixed factorial, yielding nine conditions per scenario. Trust and perceived fairness were both measured on Likert-type scales and normalized at the individual level to control for rating-style differences. Statistical analysis used one-way and two-way ANOVA tests with Bonferroni corrections for pairwise comparisons.

The study is positioned within the human-centered AI and responsible AI literature and is affiliated with groups in Austria and Australia, with a focus on healthcare and medical decision-making domains.

## Key Findings

- Explanations (both example-based and feature importance-based) significantly increased user trust compared to no explanation at all (p < 0.001); the two explanation types did not differ significantly from each other in their effect on overall trust (domain: healthcare/health insurance).
- Low introduced fairness significantly decreased user trust relative to both the high-fairness and no-information conditions (p < 0.001); high introduced fairness did not significantly increase trust above the no-information control (domain: healthcare/health insurance).
- Feature importance-based explanations significantly increased user trust even when fairness information was absent or low (p = 0.006 under low fairness), whereas example-based explanations did not produce a significant trust increase under low fairness conditions (domain: healthcare/health insurance).
- Both explanation types significantly increased users' perception of fairness compared to no explanation (p < 0.001); no significant difference between the two explanation types was found for perceived fairness (domain: healthcare/medical treatment).
- Low introduced fairness reduced perceived fairness significantly, while high introduced fairness increased perceived fairness significantly (domain: healthcare/health insurance and medical treatment).
- The application scenario moderated results: for health insurance decisions, feature importance-based explanations generated higher trust than example-based explanations (p = 0.021), whereas in medical treatment decisions the two types performed equally (domain: healthcare).

## Transparency Constructs

The study examines two primary transparency/explainability types:
- **Feature importance-based explanations**: global-style explanations showing which input variables contributed most to the AI's decision and by how much; aligned with post-hoc saliency and SHAP-style approaches.
- **Example-based explanations**: instance-level explanations presenting similar past cases used to train or inform the model; equivalent to case-based or nearest-neighbour explanations in XAI taxonomy.

Introduced fairness is treated as a separate dimension of transparency/accountability rather than as an explanation, operationalized as a stated percentage indicating how fair or unfair the AI's decision distribution was across demographic groups.

## Trust Constructs

Trust is measured as a single construct using a self-report Likert-type scale (user trust in AI-informed decision making), normalized within-subjects. The paper does not disaggregate trust into cognitive versus affective components, but the manipulation of explanations addresses cognitive transparency pathways, while the fairness manipulation has both cognitive and affective implications. The paper also discusses perceived fairness as a closely related construct influencing trust.

## Relevance to Research Questions

**RQ1**: The paper conceptualizes trust in AI-assisted decision making as influenced by two parallel constructs — explanation type and algorithmic fairness — and measures them with self-reported ratings normalized within individual participants. This contributes to operationalization debates by showing that introduced fairness and explanation type must be considered simultaneously.

**RQ2**: The relationship between explanation and trust is **conditional** on the level of introduced fairness and on the application scenario. Explanations universally increased trust relative to no explanation, but the relative advantage of feature importance vs. example-based explanations depended on whether fairness was low or high and on the scenario (health insurance vs. medical treatment). Low fairness exerted a negative effect on trust that explanations could only partially offset. A notable asymmetry is that high fairness did not boost trust above the no-information baseline, whereas low fairness reliably depressed it.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
