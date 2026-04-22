# Algorithm Aversion

**Summary**: Algorithm aversion is the tendency to distrust or avoid using algorithmic recommendations, particularly after witnessing an algorithm error; it is most pronounced in high-stakes or personal-impact domains, and can be mitigated — but not eliminated — by appropriate transparency interventions.

**Sources**: Fleiß et al._Mitigating algorithm aversion in recruiting.pdf; Zhao et al._Perceived opacity leads to algorithm aversion in the workplace.pdf; Kornowicz & Thommes_Algorithm, expert, or both_.pdf; Guo & Chen_Investigating whether AI will replace human physicians.pdf; Mourali et al._Post hoc explanations improve consumer responses to algorithmic decisions.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Algorithm aversion is a negative disposition toward algorithmic decision-making — a reluctance to use, trust, or follow algorithmic recommendations — that is disproportionately strong relative to the algorithm's actual performance. It was originally documented by Dietvorst et al. (2015) and has been extensively studied in AI trust research.

Key characteristics:
- Persists even when algorithms outperform human judges
- Particularly triggered by witnessing algorithm errors
- Stronger in high-stakes, personal-impact, or moral domains
- Distinct from rational distrust based on actual poor performance

Algorithm aversion is the inverse of [[algorithmic-trust]] and related to but distinct from [[appropriate-reliance]] (appropriate calibration of reliance to actual AI performance).

## Key Findings

### Opacity as a Driver

Zhao et al. (2024) identify perceived opacity as a proximal cause of algorithm aversion in Chinese workplace contexts (N = 1,211 across four experiments). When users perceive algorithms as opaque black boxes, they are less likely to rely on them for hiring and performance evaluation decisions. Critically, providing transparency information causally reduces algorithm aversion, and anthropomorphism (making the AI feel more human) provides additional attenuation (domain: HR/workplace; Zhao et al., 2024).

### Task Objectivity Moderates XAI Mitigation

Fleiß et al. (2024) test whether post-hoc explanations or intrinsic transparent models reduce algorithm aversion in HR recruiting. Key finding: explanations significantly increase acceptance compared to no explanation, but the type of task matters more than the type of explanation. Verifiable, objective skills assessments elicit higher acceptance than soft skill assessments, regardless of explanation type. XAI is not a universal antidote to algorithm aversion (domain: HR; Fleiß et al., 2024).

### Preference–Reliance Gap

Kornowicz & Thommes (2025) document that users strongly prefer expert-involved feature selection over purely algorithmic selection (47.7% vs. 20.2%), but this stated preference produces no difference in actual reliance on advice (incentivised decisions). This preference–behaviour gap suggests algorithm aversion can be latent in attitudes without manifesting in behaviour (domain: general/lab; Kornowicz & Thommes, 2025).

### Domain and Stakes as Moderators

- Algorithm aversion is particularly strong in healthcare: patients consistently prefer human physicians over AI-only consultations even when functional outcomes are similar (domain: healthcare; Guo & Chen, 2025).
- Actionable sensitivity explanations reduce algorithm aversion in consumer decision contexts, but only for negative outcomes; positive outcomes require less mitigation (domain: e-commerce/consumer; Mourali et al., 2025).
- Error salience amplifies algorithm aversion: algorithm errors create stronger negative trust responses than equivalent human errors (domain: HR; Zhao et al., 2024).

## Distinction from Under-reliance

Algorithm aversion is a *dispositional* construct (a prior attitude toward algorithms generally) whereas under-reliance is a *behavioural* outcome (not following AI recommendations in a specific interaction). The two are related but not identical: a user may have high algorithm aversion yet still follow AI recommendations in low-stakes contexts.

## Related pages

- [[algorithmic-trust]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[behavioural-trust]]
- [[outcome-transparency]]
- [[disclosure]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Fleiß, J., Hiebl, J., & Müller, S. (2024). Mitigating algorithm aversion in recruiting. *Journal of Business and Psychology* [details TBD].

Guo, B., & Chen, Z. (2025). Investigating whether AI will replace human physicians and understanding the interplay of the source of consultation, health-related stigma, and explanations of diagnoses on patients' evaluations of medical consultations. *Journal of Medical Internet Research*, 27, e66760. https://doi.org/10.2196/66760

Kornowicz, J., & Thommes, K. (2025). Algorithm, expert, or both? Determinants of algorithm adoption in managerial decision-making. *Journal of Behavioral Decision Making* [details TBD].

Mourali, M., Novakowski, D., Pogacar, F., & Brigden, R. (2025). Post hoc explanations improve consumer responses to algorithmic decisions. *Journal of Business Research* [details TBD].

Zhao, Y., Xu, L., Yu, F., & Jin, W. (2024). Perceived opacity leads to algorithm aversion in the workplace. *Acta Psychologica Sinica*, 56(4), 497–514.
