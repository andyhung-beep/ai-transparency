# Trust Calibration

**Summary**: Trust calibration refers to the alignment between a user's subjective trust in an AI system and the system's actual reliability; it is increasingly framed as the primary goal of XAI — not maximizing trust, but achieving appropriate trust that reflects true system capability.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Trust calibration is the degree to which a user's trust corresponds to the AI system's actual performance. A well-calibrated user:
- Trusts the system when it is likely to be correct (relies appropriately)
- Distrusts the system when it is likely to be wrong (overrides appropriately)
- Does not exhibit systematic over-trust or under-trust

Calibration is distinct from trust level per se: a user can be highly trusting and well-calibrated (if the AI is reliably accurate) or highly trusting and poorly calibrated (if the AI is unreliable). The goal of XAI is often framed as achieving calibrated trust, not maximum trust.

## Operationalizations

Trust calibration is operationalized in this corpus in several ways:

1. **Behavioral accuracy on error trials**: measuring how often users override incorrect AI recommendations — lower override rates indicate overreliance / poor calibration (Lee & Chew, 2023; Naiseh et al., 2023).
2. **Discrepancy between self-reported trust and actual AI accuracy**: if users rate trust at 73/100 while AI accuracy is 37.5%, calibration is poor (Lee & Chew, 2023).
3. **Decision sensitivity (d')**: signal detection measures distinguishing correct AI advice from incorrect advice (Tatasciore et al., 2023).
4. **Metacognitive calibration**: alignment between confidence in own judgments and actual task performance (von Zahn et al., 2025).

## Key Findings

- [[Counterfactual-explanations]] improve trust calibration by reducing overreliance on wrong AI outputs, even though they lower self-reported trust (domain: healthcare; Lee & Chew, 2023).
- Different XAI explanation classes produce different trust calibration profiles: example-based and counterfactual explanations improve understandability and perceived technical competence; reliability perceptions do not vary by class (domain: healthcare; Naiseh et al., 2023).
- XAI improves metacognitive calibration by reducing overconfidence, which then causally increases appropriate delegation to the AI (domain: real estate; von Zahn et al., 2025).
- High transparency can induce automation bias (over-reliance) when combined with cognitive load, paradoxically *harming* calibration in dual-task conditions (domain: unmanned vehicles; Tatasciore et al., 2023).
- Trust calibration may be a more sensitive outcome measure than self-reported trust for detecting genuine XAI benefits (domain: general; Naiseh et al., 2024).
- The MAST framework produces well-calibrated trust perceptions but does not translate to better collaborative performance — a dissociation between trust and performance (domain: government/security; Salehi et al., 2024).

## Overreliance and Under-reliance

Two forms of miscalibration are documented:

- **Overreliance** (automation bias): users follow AI recommendations even when they are incorrect. Exacerbated by feature-importance explanations (Humer; Spitzer), time pressure (Tatasciore & Loft 2024), and cognitive load (Tatasciore et al. 2023).
- **Under-reliance** (algorithm aversion): users distrust or ignore AI recommendations despite adequate accuracy. Addressed in [[algorithm-aversion]].

## The C-XAI Framework

Naiseh et al.'s C-XAI framework explicitly targets trust calibration as a design goal, identifying XAI technical properties (generalizability, novelty, soundness, completeness) as risk factors for over- or under-trust and proposing mitigation strategies through participatory design (Naiseh et al., 2024).

## Related pages

- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[behavioural-trust]]
- [[counterfactual-explanations]]
- [[explainability]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Naiseh, M., Al-Thani, D., Jiang, N., & Ali, R. (2023). How the different explanation classes impact trust calibration: The case of clinical decision support systems. *International Journal of Human-Computer Studies* [details TBD].

Naiseh, M., Simkute, A., Zieni, R., Jiang, N., & Ali, R. (2024). C-XAI: A conceptual framework for designing XAI tools that support trust calibration. *Journal of Responsible Technology* [details TBD].

Salehi, A., Bhatt, U., Wachter, S., Russell, C., & Sherrat, R. S. (2024). Towards trustworthy AI-enabled decision support systems: Validation of the multisource AI scorecard table (MAST). *Journal of Artificial Intelligence Research* [details TBD].

Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022.

von Zahn, M., Liebich, L., Jussupow, E., Hinz, O., & Bauer, K. (2025). Knowing (not) to know: Explainable artificial intelligence and human metacognition. *Information Systems Research* [details TBD].
