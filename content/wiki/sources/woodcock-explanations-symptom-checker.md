# The Impact of Explanations on Layperson Trust in Artificial Intelligence-Driven Symptom Checker Apps: Experimental Study

**Source file**: [Original article](../../raw/Woodcock et al._The_Impact_of_Explanations_on_.pdf)

**Summary**: This cross-sectional experimental study (n = 750) examines how four explanation types (input influence, social proof, counterfactual, no explanation) affect layperson trust in an AI symptom checker, finding that trust differences between explanation types are contingent on users' prior knowledge of the diagnosed disease: for a well-known disease (migraine), explanation type has no significant effect, while for a lesser-known disease (temporal arteritis), explanation type marginally affects trust and disease knowledge significantly moderates all trust components.

**Sources**: Woodcock et al._The_Impact_of_Explanations_on_.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in the Journal of Medical Internet Research (2021, Vol. 23, No. 11), this Oxford Internet Institute study by Woodcock, Mittelstadt, Busbridge, and Blank investigates whether, and which types of, AI explanations build layperson trust in symptom-checking chatbot applications. The study is grounded in philosophical theories of contrastive explanation (Lewis, Hilton, Miller) and the information-gap theory of explanation seeking (Loewenstein).

Participants watched a 3-minute chatbot simulation video resulting in a diagnosis of either migraine (high-prevalence, well-known) or temporal arteritis (rare, lesser-known). Each diagnosis was accompanied by one of four explanation types: input influence (a how-explanation listing influential symptoms), social proof (a how-explanation citing similar prior cases), counterfactual explanation (a why-explanation stating what would need to change for a different diagnosis), or no explanation. Exploratory factor analysis was used to generate trust factors (Faith, Comprehension, Depth), which were compared across groups using MANOVA and t-tests.

## Key Findings

- For migraine (well-known disease), explanation type had no significant effect on any trust factor (MANOVA p = .65), suggesting that when users already have sufficient knowledge, explanations are not evaluated (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- For temporal arteritis (rare disease), explanation type produced a marginally significant MANOVA effect (p = .09), with individual ANOVA effects on Faith and Comprehension non-significant, indicating some but not definitive differentiation between explanation types (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- Holding explanation type constant and varying disease (well-known vs. rare) produced significant MANOVAs for three of four explanation types: input influence (p = .001), social proof (p = .049), no explanation (p = .006), and near-significant counterfactual (p = .053) — demonstrating that disease knowledge is the primary driver of trust differences (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- For input influence, Faith was higher for temporal arteritis than migraine (p = .053), attributed to the distinctiveness of temporal arteritis symptoms better closing the information gap and reducing causal discounting (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- For counterfactual explanations, migraine Comprehension was significantly higher than temporal arteritis (p = .03), because the foil (removing nausea) aligned with common knowledge of migraines but did not address the information gap for temporal arteritis (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- 91.5% of participants would consider using this type of SC, indicating high adoption intent despite moderate explanatory trust, suggesting that improvements in explanation could unlock significant gains (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- SC diagnoses were not subject to automation bias — users critically evaluated diagnoses rather than blindly accepting them (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).
- The conversational nature of the chatbot format itself conveyed explanatory information even in the no-explanation condition, attenuating differences between conditions (source: Woodcock et al._The_Impact_of_Explanations_on_.txt; domain: consumer digital health / mHealth).

## Transparency Constructs

The study evaluates three operationalizations of AI transparency in symptom-checking contexts:

- **Input influence** ([[explainability]]): lists the input features (symptoms) most influential to the diagnosis — a local, feature-importance how-explanation.
- **Social proof** (case-based reasoning / [[example-based-explanations]]): states how many prior cases with the same symptoms received this diagnosis — a simplified case-based how-explanation.
- **Counterfactual explanation** ([[counterfactual-explanations]]): states what symptom change would alter the diagnosis — a why-explanation grounded in contrastive explanation theory.

The paper argues that current symptom checkers predominantly use how-explanations (input influence, social proof) while human social cognition favors why-explanations. The counterfactual format is proposed as a theoretically superior why-explanation, though empirical advantages over how-explanations were not clearly established.

The concept of the user's **foil** (the implicit alternative diagnosis being contrasted) is introduced as a key driver of explanation effectiveness: explanations only close an information gap if they address the specific foil in the user's mind.

## Trust Constructs

A bespoke trust scale adapted from Hoffman's Explanation Satisfaction Scale was developed, generating three trust constructs via exploratory factor analysis:

- **Faith**: blind or general trust in the explanation and system (closest to [[cognitive-trust]] and [[affective-trust]]).
- **Comprehension**: understanding of the information transmitted by the explanation (epistemic dimension).
- **Depth** (emergent for some conditions): perceived richness and completeness of the explanation.

These factors correspond to different aspects of [[cognitive-trust]] (rational assessment) and connect to [[algorithmic-trust]] in a consumer health context. The paper also captures **reliance** intent (propensity to follow triage instructions), linking to [[behavioural-trust]].

## Relevance to Research Questions

**RQ1**: Provides a novel multi-dimensional trust scale for AI explanations in consumer health, distinguishing Faith, Comprehension, and Depth as separable components. Also clarifies the distinction between how-explanations (feature contribution, social proof) and why-explanations (counterfactual) as a foundational taxonomy for [[rq1-conceptualizations]].

**RQ2**: The central finding is that the transparency–trust relationship is conditional on the user's prior knowledge. When knowledge is sufficient (migraine), explanations have no effect — a null finding suggesting that transparency may be redundant for familiar diagnoses. When knowledge is insufficient (temporal arteritis), marginal effects emerge. This conditionality is an important pattern for [[rq2-relationships]].

**RQ3**: The study indirectly addresses user-side factors through the disease-knowledge manipulation, which acts as a proxy for domain expertise. Lay users with existing knowledge of a disease do not engage with or benefit from explanations. This has direct implications for [[rq3-user-roles]]: expertise/prior knowledge functions as a critical moderator of explanation effectiveness.

## Related pages

- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[explainability]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq2-relationships]]
