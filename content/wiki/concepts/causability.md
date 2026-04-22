# Causability

**Summary**: Causability is a user-level property — the degree to which a person can achieve a causal understanding of an AI system's output from its explanation — and is conceptually distinct from explainability, which is a system-level property.

**Sources**: Shin_The effects of explainability and causability on perception, trust, and acceptance.pdf

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Definition

The term causability was introduced in the AI transparency literature to capture the user side of the transparency equation. While [[explainability]] describes what a system provides, causability describes what a user can do with it: reach a meaningful, causal understanding of why the AI made a particular decision.

Shin (2021) operationalizes causability in the context of news recommendation as:
- The degree to which users can grasp the AI's causal logic
- The user's subjective confidence that they understand the "why" behind a recommendation
- A prerequisite for engaging in systematic (analytical) processing of explanations

This parallels the concept of **understandability** in other papers, but emphasises causal rather than merely descriptive comprehension.

## Dual-Process Mechanism

Shin proposes that transparency-related constructs operate through two parallel processing routes:

1. **Heuristic processing** (fast, low-effort): Causability acts as a heuristic cue — if users feel they *could* understand the AI's reasoning, they trust it more, even without deeply engaging. This is similar to how the *availability* of an explanation increases trust regardless of comprehension.
2. **Systematic processing** (slow, analytical): Explainability operates through careful evaluation of the explanation's content. Users who engage systematically evaluate the quality and coherence of the explanation.

Causability is argued to precede and enable explainability: users first assess whether they *could* understand (causability), then actually engage with the content (explainability). Empirically, causability strongly predicts explainability (β = 0.939) and partially mediates the FAT (fairness–accountability–transparency) → trust pathway (domain: news recommendations; Shin, 2021).

## Relationship to Trust

Both causability and explainability contribute positively to algorithmic trust through perceived FAT (fairness, accountability, transparency). Trust in turn strongly predicts performance expectancy (β = 0.911). The dual-process model suggests that even without deep comprehension, the feeling that one *could* understand an AI promotes trust through a heuristic shortcut (domain: news recommendations; Shin, 2021).

## Implications

The causability concept has important implications for explanation design:
- Explanations that feel accessible (even if not deeply processed) may build trust through the heuristic route.
- This may explain why users often express positive attitudes toward explanations they do not fully understand (e.g., Okolo et al. found CHWs valued SHAP/LIME explanations they could not interpret).
- It also suggests a risk: heuristic trust from causability cues may not translate to appropriate [[trust-calibration]] if the actual explanation content is misleading.

## Related pages

- [[explainability]]
- [[traceability]]
- [[cognitive-trust]]
- [[algorithmic-trust]]
- [[appropriate-reliance]]
- [[rq1-conceptualizations]]

## References

Shin, D. (2021). The effects of explainability and causability on perception, trust, and acceptance: Implications for explainable AI. *International Journal of Human-Computer Studies*, 146, 102551.
