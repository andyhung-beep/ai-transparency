# Fairness, Explainability and In-Between: Understanding the Impact of Different Explanation Methods on Non-Expert Users' Perceptions of Fairness

**Source file**: [Original article](../../raw/Shulner_Fairness,_explainability_and_i.pdf)

**Summary**: ShulnerTal et al. run a between-subjects experiment with 425 participants comparing five explanation styles for an algorithmic recruitment system, finding that perceived fairness depends primarily on the system's outcome (positive vs. negative recommendation) rather than the explanation style provided, while explanations consistently improve understanding regardless of outcome.

**Sources**: Shulner_Fairness,_explainability_and_i.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *Ethics and Information Technology* (2022), this study examines how five different textual explanation styles affect non-expert users' fairness perceptions and outcome understanding for an algorithmic recruitment decision support system (DSS). The five styles tested are: case-based, demographic-based, input influence-based, sensitivity-based, and a novel certification-based style (reflecting an external system audit). The certification-based style is introduced as a mechanism to connect computational fairness (formal algorithmic fairness tests) with perceived fairness without disclosing decision-process details.

The study used a between-subjects design (N = 425 after filtering) in which participants read a job candidate profile and received one of the five explanation styles paired with either a positive or negative system recommendation. Domain: HR/recruitment.

## Key Findings

- Perceived fairness is dominated by the system's output: when the recommendation is negative, users tend to rate the system as unfair regardless of explanation style; when positive, users tend to rate it as fair (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- No significant difference in fairness perception was found across the five explanation styles for negative recommendations, but significant differences emerged for positive recommendations (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- For positive recommendations, the demographic-based explanation scored significantly lower in both fairness and understanding than all other styles, suggesting that population-level demographic comparisons are perceived as less fair and less comprehensible (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- The certification-based explanation scored highest in fairness for positive recommendations (average = 1.565) and second highest in understanding, even though it reveals no details about the decision process—suggesting that third-party audit signals can enhance fairness perception without algorithmic transparency (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- Sensitivity-based explanations were best for understanding in the negative-recommendation condition and achieved high understanding scores overall (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- All explanation styles improved users' understanding of the output compared to no explanation, confirming the general value of providing some form of explanation (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)
- The scenario (outcome direction) outweighs explanation style in determining perceived fairness, replicating and extending Binns et al. (2018) (domain: HR/recruitment). (source: Shulner_Fairness,_explainability_and_i.txt)

## Transparency Constructs

The paper evaluates five distinct [[explainability]] styles applied to the same algorithmic decision:
- **Case-based**: similar past cases used as reference (relates to [[example-based-explanations]])
- **Demographic-based**: comparison to demographic group averages
- **Input influence-based**: feature importance weighting (relates to [[algorithmic-transparency]])
- **Sensitivity-based**: how changes to inputs would change the output (relates to [[counterfactual-explanations]])
- **Certification-based**: external audit certification of system fairness (a novel form of [[outcome-transparency]] or institutional [[disclosure]])

The certification-based style is noteworthy as an example where perceived fairness is elevated by a procedural legitimacy signal rather than explanatory content—paralleling Schilke & Reimann's (2025) legitimacy mechanism, though in an inverse direction.

## Trust Constructs

This paper does not directly measure trust as a construct; it focuses on fairness *perception* and outcome *understanding*. However, fairness perception is widely treated as a component of [[cognitive-trust]] in algorithmic systems—users who perceive a system as fair are more likely to trust and rely on it. The study therefore contributes to understanding how explanation design shapes one dimension of [[algorithmic-trust]]. The finding that certification-based explanation enhances fairness perception without revealing any system internals suggests that institutional signals can substitute for explanatory transparency in forming trust.

## Relevance to Research Questions

**RQ1**: Provides concrete operationalizations of five explanation styles and maps them onto perceived fairness (a proxy for trust) and objective understanding. Establishes that fairness perception and outcome understanding are separable constructs that respond differently to explanation style and outcome direction—a methodological contribution to how transparency is measured in practice.

**RQ2**: Demonstrates a conditional (outcome-dependent) rather than straightforwardly positive effect of explanations on fairness perception. The transparency–trust (fairness) relationship is non-linear and asymmetric: explanations help when the outcome is positive but fail to rescue fairness perception when the outcome is negative. This is a significant finding for RQ2 on conditional and non-linear effects.

**RQ3**: The study focuses exclusively on non-expert users, making it directly relevant to RQ3. The finding that demographic-based explanations are particularly problematic for non-experts—likely because group-level comparisons are harder to interpret and feel less personal—has implications for explanation design for different user groups. Users without statistical background may misinterpret or distrust demographic-framing explanations.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[counterfactual-explanations]]
- [[algorithmic-trust]]
- [[cognitive-trust]]
- [[rq2-relationships]]
