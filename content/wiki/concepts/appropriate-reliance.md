# Appropriate Reliance

**Summary**: Appropriate reliance is the calibrated behavioural outcome in which users follow AI recommendations when they are correct and override them when they are wrong; it is increasingly used as the primary dependent variable in XAI research as a more diagnostic measure than general trust ratings.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Appropriate reliance (also termed calibrated reliance or appropriate trust in behaviour) requires:
1. **Relying on correct AI recommendations** (agreement when AI is right)
2. **Overriding incorrect AI recommendations** (disagreement when AI is wrong)

Users who over-rely follow the AI even when it is wrong (automation bias). Users who under-rely fail to follow the AI even when it is right. Both are forms of miscalibration.

Appropriate reliance is operationally defined as a combination of hit rates and correct rejection rates in signal detection theory, or decomposed as separate measures of agreement-with-correct and agreement-with-incorrect recommendations.

## Key Findings

- [[Counterfactual-explanations]] significantly improve appropriate reliance by reducing overreliance on incorrect AI recommendations without diminishing agreement with correct ones, compared to feature-importance explanations (domain: healthcare; Lee & Chew, 2023).
- Visual XAI (Grad-CAM combined with example-based explanations) reduced overreliance in a high-risk mushroom classification task (N = 410), with the reduction driven by example-based components rather than saliency maps (domain: general/lab; Leichtmann et al., 2023).
- Imperfect (incorrect) explanations increase a metric called Deception of Reliance (DoR): users rely on explanations even when the explanations are wrong, worsening human-AI team performance. This is more pronounced for novices than experts (domain: general/lab; Spitzer et al., 2025).
- High automation transparency under concurrent cognitive load induces automation bias — users over-rely on the automation despite having more transparency information, not less (domain: unmanned vehicles; Tatasciore et al., 2023).
- XAI improves delegation appropriateness (a form of appropriate reliance) by first improving metacognitive calibration — users become better aware of their own uncertainty, which drives them to delegate more appropriately to the AI (domain: real estate; von Zahn et al., 2025).
- Demand-driven transparency (user-controlled information access) improves reliance accuracy compared to sequential transparency in multi-vehicle management tasks (domain: defense; Vered et al., 2020).

## Operationalizations

- **Override rate on error trials**: percentage of incorrect AI recommendations that the user correctly rejects
- **Agreement rate on correct trials**: percentage of correct AI recommendations that the user accepts
- **d' (discriminability)**: signal detection measure of how well users distinguish correct from incorrect AI recommendations
- **Automation use accuracy**: composite measure combining correct acceptance and correct rejection rates (used in Tatasciore series)
- **Deception of Reliance (DoR)**: novel metric from Spitzer et al. measuring reliance on imperfect/incorrect explanations

## Relationship to Trust Calibration

Appropriate reliance is the behavioural manifestation of [[trust-calibration]]. Trust calibration is the cognitive/attitudinal alignment between beliefs and AI reliability; appropriate reliance is the corresponding behavioural expression. The two do not always co-occur — users can have calibrated beliefs yet still show behavioural overreliance under cognitive load.

## Related pages

- [[trust-calibration]]
- [[behavioural-trust]]
- [[algorithm-aversion]]
- [[counterfactual-explanations]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Leichtmann, B., Humer, C., Hinterreiter, A., Streit, M., & Mara, M. (2023). Effects of explainable artificial intelligence on trust and human behavior in a high-risk decision task. *Computers in Human Behavior* [details TBD].

Spitzer, M., Schlegel, U., & Keim, D. A. (2025). Imperfections of XAI: Phenomena influencing AI-assisted decision-making. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022.

Vered, M., Shani, G., & Karpas, E. (2020). Demand-driven transparency for monitoring intelligent agents. *AAAI Conference on Artificial Intelligence* [details TBD].

von Zahn, M., Liebich, L., Jussupow, E., Hinz, O., & Bauer, K. (2025). Knowing (not) to know: Explainable artificial intelligence and human metacognition. *Information Systems Research* [details TBD].
