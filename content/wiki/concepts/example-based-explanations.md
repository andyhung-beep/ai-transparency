# Example-Based Explanations

**Summary**: Example-based (or case-based) explanations justify AI decisions by showing similar instances from training data or past cases; they are intuitive for non-experts but can mislead through selective presentation and are not uniformly more effective than other explanation types.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Example-based explanations present one or more cases from the training data (or a reference set) that the AI considered similar to the current input when making its decision. Variants include:
- **Nearest-neighbour examples**: the most similar training cases
- **Prototypes**: representative cases from each class
- **One-class vs. two-class**: showing only same-class examples vs. showing both same-class and contrasting-class examples

They differ from [[counterfactual-explanations]] (which show what would change the decision) and [[natural-language-explanations]] (which provide free-text rationales).

## Key Findings

- Two-class example-based XAI (showing both similar-positive and similar-negative cases) significantly increases trust more than one-class examples or no explanation among domain experts; users develop asymmetric risk preferences reflecting the stakes of the domain (domain: industrial/oil-and-gas; Perlmutter et al., 2024).
- Nearest-neighbour examples significantly improve decision correctness and reduce over-trust compared to saliency maps (Grad-CAM), which show null effects (domain: general/lab mushroom classification; Humer et al., 2024).
- Example-based explanations are rated more understandable than local feature-importance explanations in clinical decision-making, but do not prevent overreliance on incorrect AI recommendations (domain: healthcare; Naiseh et al., 2023).
- In HR/recruiting contexts, example-based (case-based) explanations show inconsistent effects across studies and do not reliably outperform non-actionable sensitivity explanations for consumer trust (domain: e-commerce/consumer; Mourali et al., 2025).
- Adding explanations did not significantly affect user trust or motivation in automated essay scoring — outcome quality (the grade) dominated explanation effects (domain: education; Conijn et al., 2023).

## Strengths and Limitations

**Strengths**:
- Intuitive for users without statistical or ML training
- Supports analogical reasoning (see also He et al. on analogy-based explanations)
- Can build justified confidence when examples are representative and the AI is correct

**Limitations**:
- Vulnerable to confirmation bias: users may selectively attend to examples that confirm their prior beliefs
- Example selection is non-trivial: poorly chosen examples can mislead
- Effectiveness depends heavily on the domain and the user's ability to evaluate example similarity

## Moderating Factors

- **User expertise**: Technical experts benefit from two-class examples, which allow nuanced assessment; novices may not be able to evaluate example relevance (Perlmutter et al., 2024).
- **AI correctness**: Example-based explanations can reassure users even when the AI is wrong, potentially increasing overreliance (Humer et al., 2024).

## Related pages

- [[explainability]]
- [[counterfactual-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]

## References

Conijn, R., Kleijn, T., van der Graaf, J., Hubers, F., & Koreeda, Y. (2023). The effects of explanations in automated essay scoring systems. *Educational Technology & Society* [details TBD].

Humer, C., Streit, M., & Mara, M. (2024). Reassuring, misleading, debunking: Comparing effects of XAI methods on human decisions. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Mourali, M., Novakowski, D., Pogacar, F., & Brigden, R. (2025). Post hoc explanations improve consumer responses to algorithmic decisions. *Journal of Business Research* [details TBD].

Naiseh, M., Al-Thani, D., Jiang, N., & Ali, R. (2023). How the different explanation classes impact trust calibration: The case of clinical decision support systems. *International Journal of Human-Computer Studies* [details TBD].

Perlmutter, S., Gifford, T., & Krening, S. (2024). Impact of example-based XAI for neural networks on trust, understanding, and performance. *International Journal of Human-Computer Studies* [details TBD].
