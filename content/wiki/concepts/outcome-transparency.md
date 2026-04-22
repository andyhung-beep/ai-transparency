# Outcome Transparency

**Summary**: Outcome transparency provides information about what an AI system decided and its consequences; evidence suggests that the quality of the outcome itself often drives trust more than the transparency of the process, presenting a boundary condition for XAI effects.

**Sources**: Multiple — see individual source pages.

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Definition

Outcome transparency communicates the *result* of an AI process — the decision made, the score assigned, or the recommendation produced — and any immediately visible consequences. It overlaps with:
- **Decision disclosure**: telling a user what the AI decided (e.g., loan rejected, essay score = 72)
- **Confidence/accuracy disclosure**: telling a user how accurate the AI generally is

Outcome transparency is distinct from [[process-transparency]] (how the system works) and [[explainability]] (why a particular decision was made).

## Key Finding: Outcome Quality as the Dominant Driver

Several papers document that the quality of the AI's output drives trust responses more strongly than transparency mechanisms:

- In automated essay scoring, neither full-text global explanations nor accuracy statements significantly affected student trust or motivation. The dominant predictor was the **grade discrepancy** — the gap between the student's self-estimated grade and the AI-assigned score. This implies that students judge AI systems primarily by their outputs, not by the explanations accompanying them (domain: education; Conijn et al., 2023).
- In a large-scale online experiment on AI dating recommendations, transparency effects on trust were minimal when AI performance met user expectations. Transparency only added value when performance violated expectations — either negatively or positively (domain: e-commerce/dating; Sun et al., 2026).
- Perceived fairness in HR/recruiting contexts is driven primarily by whether the decision favored or disfavored the user, not by the style of explanation provided (domain: HR; Shulner, 2022).

## Implications

These findings suggest a **boundary condition** for XAI: when AI systems perform consistently with user expectations or are perceived as fair, the marginal contribution of process transparency or explanations to trust is small. Transparency effects are amplified when outcomes are surprising, negative, or ambiguous.

This has practical implications: explanations may be most needed — and most impactful — precisely in the cases where the AI errs or confounds user expectations.

## Outcome Valence as Moderator

The direction of the outcome (positive vs. negative) consistently moderates transparency effects:
- Actionable sensitivity explanations improve consumer trust and fairness perceptions primarily for negative decisions; positive decisions show attenuated effects (domain: e-commerce/consumer; Mourali et al., 2025).
- Counterfactual explanation effects on trust calibration are clearest when the AI produces an incorrect recommendation (domain: healthcare; Lee & Chew, 2023).

## Related pages

- [[process-transparency]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]

## References

Conijn, R., Kleijn, T., van der Graaf, J., Hubers, F., & Koreeda, Y. (2023). The effects of explanations in automated essay scoring systems. *Educational Technology & Society* [details TBD].

Lee, J., & Chew, E. (2023). Understanding the effect of counterfactual explanations on trust and reliance on AI for human-AI collaborative clinical decision making. *Proceedings of the ACM on Human-Computer Interaction* (CSCW2), 7.

Mourali, M., Novakowski, D., Pogacar, F., & Brigden, R. (2025). Post hoc explanations improve consumer responses to algorithmic decisions. *Journal of Business Research* [details TBD].

Shulner, T. (2022). Fairness, explainability and in-between: Understanding the impact of different explanation methods on non-expert users' perceptions of fairness. *Ethics and Information Technology* [details TBD].

Sun, Q., Shi, X., Zhang, T., & Liu, J. (2026). Does transparency matter when an AI system meets performance? *Computers in Human Behavior* [details TBD].
