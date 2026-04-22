# Perceived Risk / Stakes

**Summary**: Perceived risk — the user's assessment of the potential harm from an incorrect AI decision — is a key moderator of transparency–trust relationships, typically amplifying both the demand for transparency and the trust consequences of AI errors.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Perceived risk in AI contexts refers to the user's subjective assessment of the consequences of trusting or following an AI recommendation when it might be wrong. High perceived risk is associated with:
- High personal stakes (medical diagnosis, hiring decisions, legal rulings)
- High societal stakes (public safety, security systems)
- Irreversibility of the decision
- Personal vulnerability of the affected party

## Key Findings

### Risk Amplifies Transparency Effects

- In high-risk decision tasks (mushroom identification with stated health consequences), XAI explanations significantly improve [[appropriate-reliance]] — the high stakes motivate analytical processing of explanations rather than heuristic processing (domain: general/lab; Leichtmann et al., 2023).
- Clinical domains (healthcare AI) consistently show higher demands for transparency and higher sensitivity to AI errors than lower-stakes domains (Hassan et al., 2025; Rezaeian et al., 2025).
- High-stakes security contexts (IV-IDS) require and benefit more from visual SHAP explanations than low-stakes contexts (domain: automotive security; Lundberg et al., 2022).

### Risk as a Driver of Algorithm Aversion

- [[Algorithm-aversion]] is particularly pronounced in domains with high personal impact and irreversibility (hiring decisions, medical diagnoses) compared to low-stakes domains (domain: HR; Fleiß et al., 2024; Zhao et al., 2024).
- Patients' concerns about AI in healthcare are dominated by privacy, liability, and regulatory risk — dimensions of perceived risk that go beyond task accuracy (domain: healthcare; Esmaeilzadeh et al., 2021).

### Risk Shapes Reliance Asymmetries

- In high-stakes industrial inspection (pipeline anomaly detection), expert analysts show asymmetric risk preferences: they deliberately bias toward over-classifying anomalies because the cost of a false negative (missed defect) vastly exceeds the cost of a false positive (domain: industrial; Perlmutter et al., 2024).
- Under high time pressure (a form of risk from operational urgency), transparency benefits disappear without interaction — time pressure degrades performance independently of explanation provision (domain: unmanned vehicles; Tatasciore & Loft, 2024).

## Measurement

Perceived risk is measured across the corpus as:
- Self-reported risk perceptions (domain-specific scales; Esmaeilzadeh)
- Experimental manipulation (high-stakes vs. low-stakes task framing; Leichtmann)
- Task consequence framing (monetary penalties, health consequences)
- Domain selection (inherently high-stakes domains as natural moderator)

## Related pages

- [[domain-context]]
- [[user-expertise]]
- [[algorithm-aversion]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Esmaeilzadeh, P., Mirzaei, T., & Dharanikota, S. (2021). Patients' perceptions toward human–artificial intelligence interaction in health care: Experimental study. *Journal of Medical Internet Research*, 23(11), e25856.

Fleiß, J., Hiebl, J., & Müller, S. (2024). Mitigating algorithm aversion in recruiting. *Journal of Business and Psychology* [details TBD].

Hassan, N. R., Nguyen, T., Finserås, S. M., Adde, L., Strømke, R., & Støen, R. (2025). Unlocking the black box: Enhancing human-AI collaboration in high-stakes healthcare scenarios through explainable AI. *Technological Forecasting & Social Change*, 219, 124265. https://doi.org/10.1016/j.techfore.2025.124265

Leichtmann, B., Humer, C., Hinterreiter, A., Streit, M., & Mara, M. (2023). Effects of explainable artificial intelligence on trust and human behavior in a high-risk decision task. *Computers in Human Behavior* [details TBD].

Lundberg, J., Riveiro, M., & Bång, M. (2022). Experimental analysis of trustworthy in-vehicle intrusion detection system using eXplainable artificial intelligence (XAI). *IEEE Access* [details TBD].

Perlmutter, S., Gifford, T., & Krening, S. (2024). Impact of example-based XAI for neural networks on trust, understanding, and performance. *International Journal of Human-Computer Studies* [details TBD].

Rezaeian, A., Asan, O., & Bayrak, A. E. (2025). The impact of AI explanations on clinicians' trust and diagnostic accuracy in breast cancer. *Applied Ergonomics* [details TBD].

Tatasciore, M., & Loft, S. (2024). Can increased automation transparency mitigate the effects of time pressure on automation use? *Applied Ergonomics*, 114, 104142.

Zhao, Y., Xu, L., Yu, F., & Jin, W. (2024). Perceived opacity leads to algorithm aversion in the workplace. *Acta Psychologica Sinica*, 56(4), 497–514.
