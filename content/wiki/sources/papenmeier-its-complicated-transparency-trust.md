# It's Complicated: The Relationship between User Trust, Model Accuracy and Explanations in AI

**Source file**: [Original article](../../raw/Papenmeier et al._It_s complicated.pdf)

**Summary**: A large-scale online between-subjects study (N = 959) in which participants classify offensive tweets using a decision-support system at three accuracy levels (high 96%, medium 76%, antagonistic 4%) with faithful, random, or no word-highlight explanations; finds that explanation effects on trust depend critically on accuracy level, that faithful explanations can reduce self-reported trust for high-accuracy systems, and that self-reported and behavioural trust measures are not interchangeable.

**Sources**: Papenmeier et al._It_s complicated.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *ACM Transactions on Computer-Human Interaction* (August 2022) by Papenmeier, Kern, Englebienne, and Seifert, this large-scale study uses a 3 (accuracy: high/medium/antagonistic) × 3 (explanation: faithful/random/none) between-subjects design to investigate how explanation faithfulness and system accuracy jointly shape user trust in a text-classification decision-support system. The use case is detection of offensive language in tweets for a youth content platform.

The study contributes two methodological advances: (1) a direct comparison of behavioural trust (switching rate toward the classifier between blocks 1 and 2) and self-reported trust (Körber's validated 19-item automation trust questionnaire), and (2) examination of trust effects across a wide accuracy range rather than at a single fixed accuracy level.

Explanations are word highlights in the tweet text: faithful highlights are the top-4 words most decisive for the classifier (via L2X algorithm), while random highlights are 4 words chosen at random (validated to retain about 74% label agreement by chance, lower than 98% for faithful).

## Key Findings

- For a **high-accuracy classifier**: any explanation (faithful or random) significantly reduced self-reported trust compared to no explanation; however, faithful explanations did not significantly reduce behavioural trust. (Domain: social media moderation / content classification)
- For a **medium-accuracy classifier**: random explanations significantly reduced self-reported trust compared to no explanation; faithful explanations did not significantly differ from no explanation. (Domain: social media moderation)
- For an **antagonistic (near-zero accuracy) classifier**: explanation type had no significant effect on either self-reported or behavioural trust; all conditions were equally (and correctly) distrusted. (Domain: social media moderation)
- The effect pattern "trust adapts to accuracy" holds when no explanation is given (C_HN > C_MN > C_AN), but adding an explanation disrupts this pattern: a random explanation on a high-accuracy system can reduce self-reported trust to the level of a medium-accuracy system. (Domain: social media moderation)
- **Self-reported and behavioural trust measures show weak positive correlation** (r = 0.30 overall) and diverge substantially in the high-accuracy conditions (r = 0.025 for C_H conditions). They cannot and should not be used interchangeably. (Domain: across conditions)
- **Faithful explanations are the only type to improve classification performance** (how accurately users detect offensive language): performance gains were significant in C_HF and weakly significant in C_HN, not in C_HR. (Domain: social media moderation)
- **Random explanations most consistently harm trust**: C_HR (high accuracy, random explanation) yields self-reported trust scores comparable to medium-accuracy systems; random explanations confuse users about the classifier's logic. (Domain: social media moderation)
- **Propensity to trust was significantly affected by condition** despite random assignment, suggesting that interacting with the decision-support system changed participants' beliefs about their own capacity to trust—a potentially novel secondary effect of AI explanation design.

## Transparency Constructs

- **Explainability**: Two minimal/local text explanations—faithful (L2X word highlights) and random (arbitrary word highlights). The manipulation of explanation faithfulness (vs. mere presence) is the central independent variable. See [[explainability]].
- **Algorithmic transparency**: Transparency is operationalised at the level of information exposure: faithful explanations expose the inner decision mechanism; random explanations provide the surface form of transparency without the informational content. See [[algorithmic-transparency]].
- The paper defines transparency, interpretability, and explanation as a nested hierarchy: transparency = information exposure; interpretability = meaningfulness to a human; explanation = mechanism for communicating transparency. These definitions are useful anchors for the wiki taxonomy.

## Trust Constructs

- **Cognitive trust (self-reported)**: Measured via Körber's (2020) validated 19-item trust in automation questionnaire, covering reliability/competence, predictability/understanding, familiarity, intention of developers, propensity to trust, and trust in automation. See [[cognitive-trust]].
- **Behavioural trust**: Measured as the switching rate—how often participants change their classification to match the classifier between block 1 (no system) and block 2 (with system). See [[behavioural-trust]].
- **Trust calibration**: The paper frames appropriate trust as aligning with system accuracy; both over-trust (following an antagonistic classifier) and under-trust (ignoring a high-accuracy classifier) are failures. See [[trust-calibration]].
- **Algorithm aversion**: Not a central focus, but the antagonistic condition effectively tests a scenario where algorithm aversion would be rational—and users do display lower trust and less switching in those conditions. See [[algorithm-aversion]].

## Relevance to Research Questions

**RQ1**: Provides explicit, operationally distinct definitions of transparency, interpretability, and explanation that can anchor the wiki taxonomy. Operationalises trust in two mutually non-interchangeable ways (behavioural switching rate and validated self-report questionnaire). Demonstrates that the choice of trust measure fundamentally changes which conclusions can be drawn. See [[rq1-conceptualizations]].

**RQ2**: Central finding is a **non-linear, accuracy-conditional effect of explanations on trust**: the direction and magnitude of the explanation effect reverse across accuracy levels. For high-accuracy systems, explanations reduce self-reported trust; for medium-accuracy systems, only unfaithful explanations reduce trust; for antagonistic systems, explanation type is irrelevant. This challenges the common claim that explanations improve user trust. The paper explicitly describes this as more complex than previously reported. A further complication: behavioural trust and self-reported trust show different patterns, meaning the relationship depends also on how trust is measured. See [[rq2-relationships]].

**RQ3**: Demographic variables (age, gender, language proficiency) did not significantly moderate trust outcomes—a notable null finding suggesting that at least in this relatively homogeneous crowdsourced sample, individual differences do not drive the accuracy × explanation interaction. However, the paper does not examine domain expertise or AI literacy as moderators, which are important gaps. See [[rq3-user-roles]], [[user-expertise]].

## Related pages

- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[algorithmic-transparency]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
