# Post Hoc Explanations Improve Consumer Responses to Algorithmic Decisions

**Source file**: [Original article](../../raw/Mourali et al._Post hoc explanations improve consumer responses to algorithmic decisions.pdf)

**Summary**: A series of five preregistered experiments (total N ≈ 2,000+) demonstrates that actionable sensitivity-based post-hoc explanations improve consumers' perceptions of transparency, fairness, and trust in algorithmic decision systems, while non-actionable explanations sometimes backfire; case-based explanations show inconsistent effects.

**Sources**: Mourali et al._Post hoc explanations improve consumer responses to algorithmic decisions.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Mourali, Novakowski, Pogacar, and Brigden (2025, Journal of Business Research) investigate how different types of post-hoc explanations of algorithmic decisions affect consumer perceptions of transparency, fairness, trust, and behavioral intentions toward the deploying organization. The research is motivated by widespread consumer algorithm aversion and the growing regulatory pressure (e.g., GDPR) for algorithmic transparency.

Building on Binns et al.'s (2018) taxonomy of model-agnostic explanations, the study focuses on two types of **local** post-hoc explanations:
1. **Sensitivity explanations** — show what input values would need to change to alter the decision outcome (counterfactual format); e.g., "If 10% or less of your driving took place at night, you would have qualified for the cheapest tier."
2. **Case-based explanations** — present a similar historical case from the training data; e.g., "A similar case to yours is a previous customer: She was 38 years old..."

Five preregistered between-subjects experiments were run on Prolific Academic with US and Canadian participants. Contexts spanned car insurance pricing, bonus eligibility, credit cards, parole decisions, health insurance, and professional training. Key outcome variables: perceived transparency, attitude (combined fairness + trust), and behavioral intentions (likelihood to do business with the company).

The domain is primarily **consumer/e-commerce and finance**, with extension to **criminal justice, healthcare, and professional training** in Study 4.

## Key Findings

- Sensitivity explanations (actionable) significantly increased perceived transparency, attitude, and behavioral intentions versus both case-based and no-explanation conditions in Studies 1–4. (Domain: consumer/finance)
- Study 1 (N = 443): Sensitivity > Case > No explanation on transparency, attitude, and intentions (all p < 0.001 for sensitivity vs. no explanation; η² for transparency = 0.356, a very large effect). Contrary to hypothesis H2, case-based explanations outperformed no explanation in Study 1, though this was not replicated consistently.
- Studies 2, 3, 4: Case-based explanations did not reliably improve attitudes or intentions compared to no explanation. The weight of evidence across five studies supports treating case-based explanations as no better than providing none.
- Actionability is the key mechanism: **actionable** sensitivity explanations (highlighting factors under the consumer's control) consistently outperformed **non-actionable** sensitivity explanations (factors the consumer cannot change). Non-actionable explanations sometimes produced lower attitudes and intentions than no explanation (backfire effect), particularly across the parole, health insurance, and professional training scenarios. (Domain: consumer, criminal justice, healthcare)
- Study 5 (N = 764): The benefit of sensitivity explanations on attitude and behavioral intentions was entirely eliminated when the decision outcome was positive. Explanations only improved attitudes and intentions when the decision was negative (unfavorable to the consumer). The effect on perceived transparency remained significant but attenuated even with positive outcomes. (Domain: consumer/insurance)
- Perceived controllability (not perceived relevance) was identified as the primary mechanism driving the advantage of actionable over non-actionable explanations in a post-test across five scenarios.
- Effects replicated across multiple domains in Study 4 (credit card, parole, health insurance, professional training), supporting generalizability across high-stakes contexts.

## Transparency Constructs

The paper operationalizes **transparency** through perceived transparency scales (3 items, α = 0.95): whether consumers understand how the algorithmic system made its decision. This is closest to [[outcome-transparency]] and [[process-transparency]] — understanding both what was decided and why. Post-hoc explanations are the mechanism for providing this transparency without modifying the underlying model.

The paper distinguishes between:
- **Local explanations**: focused on a specific individual decision (the focus of this paper)
- **Global explanations**: describe aggregate model behavior (not studied here, acknowledged as more relevant for technical users)

Sensitivity-based explanations are closely related to [[counterfactual-explanations]], as they specify what changes would alter the outcome. Case-based explanations are a form of [[example-based-explanations]].

The paper also raises concerns that sensitivity explanations are necessarily selective and may not faithfully represent model computations, echoing debates about the risk of misleading transparency.

## Trust Constructs

Trust is measured as a combined **Attitude** index (perceived fairness + trust in algorithmic system, std. α = 0.92), reflecting both [[cognitive-trust]] (rational evaluation of system reliability) and [[affective-trust]] (fairness perceptions). Behavioral intentions (likelihood to do business with the company) capture [[behavioural-trust]]. The study does not separately analyze dispositional trust, though it situates itself in the literature on [[algorithm-aversion]].

The research demonstrates that explanations can shift consumer attitudes from mistrust toward greater acceptance — a direct contribution to [[trust-calibration]] in consumer-facing algorithmic systems.

## Relevance to Research Questions

**RQ1**: Operationalizes transparency as consumer-perceived understanding of algorithmic decisions, and trust/fairness as a combined attitudinal construct. Demonstrates that transparency (perceived) mediates the relationship between explanation type and trust/fairness attitudes. Contributes a consumer-psychology framework for understanding how different explanation contents activate or fail to activate transparency perceptions.

**RQ2**: Provides strong multi-study evidence for conditional effects of post-hoc explanations on trust: (a) actionable sensitivity explanations reliably increase trust and positive attitudes; (b) non-actionable sensitivity explanations can backfire (decrease trust below baseline); (c) case-based explanations have inconsistent and generally null effects on trust/attitudes; (d) outcome valence moderates the effectiveness of explanations — benefits appear only for negative outcomes. These conditional patterns are a key contribution to understanding non-linear and boundary effects in the transparency–trust relationship.

**RQ3**: The paper does not directly examine user expertise or AI literacy as a moderator. However, it focuses on lay consumers (not experts), and acknowledges that global explanations are more relevant for technical users (programmers, managers), while local explanations serve end-users seeking to understand specific decisions. This implies an implicit expertise moderator that future work could test explicitly.

## Related pages

- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
