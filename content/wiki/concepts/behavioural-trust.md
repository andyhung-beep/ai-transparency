# Behavioural Trust

**Summary**: Behavioural trust is trust expressed through action — reliance, adoption, advice-following, and override behaviour — and frequently dissociates from self-reported (subjective) trust in this corpus, making it a critical but underutilised outcome measure.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

Behavioural trust refers to the observable manifestations of trust in AI systems:
- **Reliance**: following or agreeing with AI recommendations
- **Override**: choosing not to follow AI recommendations
- **Adoption**: deciding to use an AI system
- **Advice-taking**: applying AI-generated feedback to one's work
- **Delegation**: assigning tasks to an AI system

Behavioural trust is distinct from subjective (self-reported) trust measures, which capture attitudes and beliefs. In well-designed studies, both are measured, allowing researchers to assess the gap between what users say they trust and how they actually behave.

## The Self-Report vs. Behaviour Dissociation

A recurring finding across the corpus is that self-reported trust and behavioural trust diverge in systematic ways:

- Wang & Ding (2024) find that SHAP-based XAI improves decision accuracy and behavioural reliance (AI consistency) significantly, but does NOT improve self-reported trust scores. Even irrational (randomly permuted) explanations improve decision accuracy — suggesting explanations work through implicit cues rather than genuine understanding (domain: e-commerce; Wang & Ding, 2024).
- Kornowicz & Thommes (2025) document a large attitude–behaviour gap: users strongly prefer feature-selection methods that include human expertise, but this preference does not translate into higher advice reliance in incentivised decisions (domain: general/lab; Kornowicz & Thommes, 2025).
- Suffian et al. (2025) find that user-feedback counterfactuals improve task performance and reliance significantly but self-reported trust and satisfaction do not reach statistical significance (domain: general/lab; Suffian et al., 2025).
- Diprose et al. (2020) show that 88% of physicians prefer explanations, but adding explanations does not significantly change their intended clinical behaviour (domain: healthcare; Diprose et al., 2020).

## Operationalizations

Key operationalizations of behavioural trust in this corpus:

1. **Agreement rate / reliance rate**: proportion of AI recommendations the user accepts (e.g., Lee & Chew; Naiseh; Tatasciore).
2. **Override rate on error trials**: proportion of incorrect AI recommendations the user correctly rejects — the most direct measure of calibrated reliance (e.g., Lee & Chew; Leichtmann; Humer).
3. **WoA (Weight of Advice)**: how much users shift their estimate toward the AI's suggestion (e.g., Kornowicz; Musick).
4. **Adoption intention**: stated likelihood of using the system in the future (e.g., Cramer; Bigras).
5. **Delegation**: assigning decisions to the AI (e.g., von Zahn et al.).
6. **System usage**: actual engagement with the system in a real-world setting (e.g., Bigras; van Zetten).

## Key Findings

- Counterfactual explanations reduce overreliance (improve override rate on wrong AI trials) more effectively than feature-importance explanations in clinical settings (domain: healthcare; Lee & Chew, 2023).
- XAI improves delegation frequency (+31.7%) by improving metacognitive calibration, not by changing explicit trust beliefs (domain: real estate; von Zahn et al., 2025).
- Automation bias (excessive reliance on AI) is induced by high transparency under cognitive load, showing that transparency can harm calibrated reliance in dual-task conditions (domain: unmanned vehicles; Tatasciore et al., 2023).
- The credibility of model description (advanced vs. basic framing) significantly affects advice-following behaviour even without changing trust scores (domain: general/lab; Chu et al., 2023).

## Related pages

- [[cognitive-trust]]
- [[affective-trust]]
- [[appropriate-reliance]]
- [[trust-calibration]]
- [[algorithm-aversion]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]

## References

Chu, Z., Wang, J., & Cao, J. (2023). User judgement of an AI model: The effect of initial AI performance and explanation credibility on subsequent trust and reliance. *CHI Conference on Human Factors in Computing Systems* [details TBD].

Diprose, J. P., Buist, N., Chu, N., Edlin, R., Milinovich, A., & Nunns, M. (2020). Physician understanding, explainability, and trust in a hypothetical machine learning risk calculator. *Journal of the American Medical Informatics Association*, 27(4), 592–600 [details TBD].

Kornowicz, J., & Thommes, K. (2025). Algorithm, expert, or both? Determinants of algorithm adoption in managerial decision-making. *Journal of Behavioral Decision Making* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Suffian, M., Panigutti, C., Ntoutsi, E., Pedreschi, D., & Giannotti, F. (2025). The role of user feedback in enhancing understanding and trust in counterfactual explanations for explainable AI. *International Journal of Human-Computer Studies* [details TBD].

Tatasciore, M., Bowden, V., & Loft, S. (2023). Do concurrent task demands impact the benefit of automation transparency? *Applied Ergonomics*, 110, 104022.

von Zahn, M., Liebich, L., Jussupow, E., Hinz, O., & Bauer, K. (2025). Knowing (not) to know: Explainable artificial intelligence and human metacognition. *Information Systems Research* [details TBD].

Wang, D., & Ding, Y. (2024). The rationality of explanation or human capacity? A study of human-AI collaboration in clinical decision support. *Journal of the American Medical Informatics Association* [details TBD].
