# Counterfactual Explanations

**Summary**: Counterfactual explanations (also called "what-if" explanations) describe the minimal change to an input that would produce a different AI output; they are among the most studied explanation types in this corpus and show consistent advantages for trust calibration and reducing overreliance.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Definition

A counterfactual explanation answers the question: "What would have needed to be different about this case for the AI to make a different decision?" For example: "If your income had been £5,000 higher, your loan application would have been approved." This format is inherently contrastive and aligns with how humans naturally reason about causation.

Counterfactuals are distinct from:
- **Feature importance** explanations, which say *what* influenced the decision but not *how* to change it.
- **Example-based** explanations (see [[example-based-explanations]]), which show similar cases.
- **Natural language** rationales (see [[natural-language-explanations]]), which may incorporate counterfactual reasoning but are not necessarily contrastive.

Actionable counterfactuals specifically constrain suggestions to factors the user can realistically change (Mourali et al., 2025; Suffian et al., 2022).

## Key Findings

- Counterfactual explanations reduce overreliance on incorrect AI recommendations by approximately 21% compared to feature-based explanations in clinical decision-making (domain: healthcare; Lee & Chew, 2023).
- Self-reported trust is paradoxically *lower* with counterfactuals than with feature-based explanations, yet counterfactual trust is better calibrated to actual AI accuracy — highlighting the distinction between subjective trust and [[trust-calibration]] (domain: healthcare; Lee & Chew, 2023).
- Counterfactuals are rated as more understandable and improve perceived technical competence compared to local (feature importance) and global explanations in clinical settings (domain: healthcare; Naiseh et al., 2023).
- Actionable counterfactuals (focusing on factors users can change) improve consumer fairness perceptions and trust; non-actionable sensitivity explanations backfire and reduce trust compared to no explanation (domain: e-commerce/consumer decisions; Mourali et al., 2025).
- Laypersons prefer counterfactual explanations over input-influence or social-proof explanations in AI-based symptom checkers, particularly for unfamiliar diseases (domain: healthcare/consumer; Woodcock et al., 2021).
- User-feedback-enriched counterfactuals (UFCE) outperform standard DiCE counterfactuals on task performance and feature understanding (domain: general/lab; Suffian et al., 2025).

## Tension: Cognitive Forcing vs. Reassurance

Counterfactuals function as a **cognitive forcing function** — they prompt users to actively evaluate rather than passively accept AI advice. This is why they reduce overreliance but also lower subjective trust: users who engage critically with AI output may report lower confidence in the system even as their decisions improve (Lee & Chew, 2023).

This contrasts with feature-importance explanations, which tend to reassure or confirm existing intuitions (Humer et al., 2024).

## Moderating Factors

- **User expertise**: Domain experts (therapists) benefit more from counterfactuals than laypeople in clinical tasks — they have enough knowledge to evaluate the counterfactual's plausibility (domain: healthcare; Lee & Chew, 2023).
- **Actionability**: Counterfactual benefits are strongest when the suggested changes are within the user's control (Mourali et al., 2025).
- **Decision valence**: Effects are stronger for negative outcomes (rejected applications) than positive ones (Mourali et al., 2025).

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq2-relationships]]

## References

Humer, C., Streit, M., & Mara, M. (2024). Reassuring, misleading, debunking: Comparing effects of XAI methods on human decisions. *ACM Transactions on Interactive Intelligent Systems* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Mourali, M., Novakowski, D., Pogacar, F., & Brigden, R. (2025). Post hoc explanations improve consumer responses to algorithmic decisions. *Journal of Business Research* [details TBD].

Naiseh, M., Al-Thani, D., Jiang, N., & Ali, R. (2023). How the different explanation classes impact trust calibration: The case of clinical decision support systems. *International Journal of Human-Computer Studies* [details TBD].

Suffian, M., Panigutti, C., Ntoutsi, E., Pedreschi, D., & Giannotti, F. (2022). FCE: Feedback-based counterfactual explanations for explainable AI. *IEEE Access* [details TBD].

Suffian, M., Panigutti, C., Ntoutsi, E., Pedreschi, D., & Giannotti, F. (2025). The role of user feedback in enhancing understanding and trust in counterfactual explanations for explainable AI. *International Journal of Human-Computer Studies* [details TBD].

Woodcock, A., Mittelstadt, B., Busbridge, D., & Blank, G. (2021). The impact of explanations on layperson trust in artificial intelligence-driven symptom checker apps: Experimental study. *Journal of Medical Internet Research*, 23(11), e29386.
