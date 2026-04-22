# Explainability / Interpretability

**Summary**: Explainability refers to the degree to which an AI system's outputs, reasoning, or internal logic can be communicated to users in an understandable form; it is the most widely studied transparency construct in this corpus.

**Sources**: Multiple — see individual source pages for primary citations.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition and Scope

Explainability (also termed interpretability) is a system-level property: the capacity of an AI to make its predictions or decisions comprehensible to a human audience. It is distinct from [[causability]], which is a user-level property (the user's ability to reach a causal understanding). The literature distinguishes several key dimensions:

- **Post-hoc vs. by-design**: Post-hoc methods (SHAP, LIME, Grad-CAM) explain an existing black-box model after training; interpretable-by-design approaches (decision trees, fuzzy classifiers, rule lists) build transparency into the model architecture (Gunning & Aha, 2019; Yeganejou et al., 2020).
- **Local vs. global**: Local explanations (LIME, SHAP local, counterfactuals) explain a single prediction; global explanations describe overall model behaviour (La Gatta et al., 2021).
- **Feature-based**: highlight which input features drove the prediction (SHAP, LIME, LASSO).
- **Example-based**: show similar training instances (nearest neighbours, prototypes).
- **Rule-based**: express decisions as if–then rules or decision trees.
- **Counterfactual**: describe what minimal change to the input would flip the output (see [[counterfactual-explanations]]).
- **Natural language**: produce free-text rationales (see [[natural-language-explanations]]).
- **Visual/saliency**: highlight relevant regions in images (Grad-CAM, integrated gradients, LRP).
- **CIU (Contextual Importance and Utility)**: computes *contextual importance* (how much the feature's range affects the output in context) and *contextual utility* (how favorable the current feature value is for the predicted class); does not use a surrogate model, making it more stable than LIME and more lightweight than Kernel SHAP (Knapic et al., 2021).

## Operationalization in the Corpus

Across the 86 sources, explainability is operationalized in two broad ways:

1. **As a manipulation**: researchers expose participants to explanations of different types or depths and measure downstream outcomes (trust, reliance, accuracy).
2. **As a self-report construct**: users rate how well they understand the system (e.g., perceived understandability, perceived transparency).

Importantly, objective explanation quality and perceived understandability are not the same — [[traceability]] research (Schrills & Franke) shows users can feel they understand a system without objective comprehension gains.

## Transparency, Interpretability, and Explainability Distinguished

Knapic et al. (2021) articulate a useful three-way distinction often collapsed in the literature:

- **Transparency**: a model is understandable on its own (applies to inherently simple models)
- **Interpretability**: outputs can be described meaningfully to humans; does not imply the internal logic is accessible
- **Explainability**: the internal logic and dynamics of a model are accessible to human understanding; does not automatically follow from interpretability alone

Interpretability does not imply explainability and vice versa; both are required for trustworthy human-AI collaboration (Knapic et al., 2021).

## Key Findings

- Explanations generally improve user trust and reliance compared to no explanation, but the effect is highly contingent on explanation type, domain, and user characteristics (domain: general/lab; Gunning & Aha, 2019).
- Feature-importance explanations (SHAP, LIME) do not reliably improve decision accuracy and can mislead users when the explanation is imperfect or the AI is wrong (domain: general/lab; Humer et al., 2024; Spitzer et al., 2025).
- The most detailed explanation is not always the most effective: Rezaeian et al. found the highest-information explanation condition degraded clinician diagnostic accuracy and understandability compared to no explanation (domain: healthcare; Rezaeian et al., 2025).
- Explanation type interacts with user expertise: novice users struggle with standard SHAP/LIME outputs but prefer having them (domain: healthcare/Global South; Okolo et al., 2024).
- Visual and saliency-based explanations are preferred by domain experts with strong visual-spatial reasoning skills (domain: healthcare; Xian et al., 2026; Ihongbe et al., 2024).
- Intrinsic (interpretable-by-design) explanations do not reliably outperform post-hoc explanations for first-time users in HR contexts (domain: HR/recruiting; Fleiß et al., 2024).
- Among LIME, SHAP, and CIU applied to medical image classification (video capsule endoscopy), none significantly improved lay-user decision accuracy; SHAP users performed directionally *worse* with explanations than without, suggesting SHAP's complexity induces overload in non-expert populations; CIU produced the highest satisfaction and best error-detection ability (domain: healthcare; Knapic et al., 2021).

## Performance–Explainability Trade-off

The DARPA XAI program (Gunning & Aha) identified an inverse relationship between model performance and explainability for deep learning models. Later work has challenged the universality of this trade-off: hybrid architectures (Jaziri & Sassi; Yeganejou et al.) achieve reasonable accuracy with embedded transparency, accepting a small performance cost (≈4%) in exchange for significant trust gains.

## Relationship to Trust

Explainability is a means to an end — [[trust-calibration]] — not an end in itself. Multiple papers document that users can trust an AI more or less than its actual reliability warrants, and that explanations can improve, worsen, or have no effect on this calibration depending on their quality and alignment with user needs.

## Related pages

- [[causability]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[natural-language-explanations]]
- [[traceability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Fleiß, J., Hiebl, J., & Müller, S. (2024). Mitigating algorithm aversion in recruiting. *Journal of Business and Psychology* [details TBD].

Gunning, D., & Aha, D. (2019). DARPA's explainable artificial intelligence (XAI) program. *AI Magazine*, 40(2), 44–58.

Humer, C., Streit, M., & Mara, M. (2024). Reassuring, misleading, debunking: Comparing effects of XAI methods on human decisions. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Ihongbe, T., Abubakar, S., & Yan, R. (2024). Evaluating explainable artificial intelligence (XAI) techniques in chest radiology imaging through a human-centered lens. *PLOS ONE* [details TBD].

Knapic, S., Malhi, A., Saluja, R., & Frömling, K. (2021). Explainable artificial intelligence for human decision support system in the medical domain. *Machine Learning and Knowledge Extraction*, 3, 740–770.

La Gatta, V., Moscato, V., Postiglione, M., & Sperlì, G. (2021). PASTLE: Pivot-aided space transformation for local explanations. *Pattern Recognition Letters* [details TBD].

Okolo, C. T., Agarwal, Y., Dell, N., & Vashistha, A. (2024). "If it is easy to understand then it will have value": Examining perceptions of explainable AI with community health workers in rural India. *Proceedings of the ACM on Human-Computer Interaction* (CSCW), 8.

Rezaeian, A., Asan, O., & Bayrak, A. E. (2025). The impact of AI explanations on clinicians' trust and diagnostic accuracy in breast cancer. *Applied Ergonomics* [details TBD].

Spitzer, M., Schlegel, U., & Keim, D. A. (2025). Imperfections of XAI: Phenomena influencing AI-assisted decision-making. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Xian, Y., Mehandjiev, N., Constantinides, M., Chen, Y., Quboa, Q., & Kitchen, G. (2026). Clinician preferences for explainable AI in critical care. *International Journal of Medical Informatics*, 210 [details TBD].

Yeganejou, M., Dick, S., & Miller, J. (2020). Interpretable deep convolutional fuzzy classifier. *IEEE Transactions on Fuzzy Systems*, 28(7) [details TBD].
