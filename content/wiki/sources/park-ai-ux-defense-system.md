# Designing and Evaluating User Experience of an AI-Based Defense System

**Source file**: [Original article](../../raw/Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.pdf)

**Summary**: This study develops and validates a 9-factor AI UX evaluation questionnaire and applies it to improve the user interface of a military AI defense system, demonstrating significant improvements across most UX dimensions including trust, explainability, and causality.

**Sources**: Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Park et al. (2023) address a gap in AI UX research: the lack of a generalizable, validated evaluation instrument for AI systems, and the absence of documented processes for applying UX principles to improve real AI systems. The study proceeds in two stages. First, a 9-factor AI UX questionnaire is developed through systematic literature review of 120 papers, administered to 105 AI speaker users, and validated via exploratory and confirmatory factor analysis. Second, the validated instrument is used to guide a three-step UX upgrade process (task hierarchy analysis, ideation, and prototyping) applied to an AI-based military defense system that performs terrain change detection and airborne target detection. A usability test with 20 participants evaluates the before/after systems.

The domain is national defense / military surveillance (South Korea). The AI system uses a dense Siamese network for change detection and YOLOv3 for target detection, both black-box neural architectures.

## Key Findings

- After UX upgrade, 8 of 9 AI UX factors showed statistically significant improvements: satisfaction (5.28 → 8.25), controllability (5.77 → 8.07), trust (5.42 → 7.90), causality (3.48 → 6.88), efficiency (6.60 → 8.68), accountability (4.73 → 7.23), explainability (5.25 → 8.05), and safety (5.50 → 6.87). [Domain: national defense]
- Fairness was the one factor that did not improve significantly, which the authors attribute to the absence of algorithmic bias concerns in the specific defense task. [Domain: national defense]
- Causality showed the largest absolute gain (3.48 → 6.88), consistent with the view that explaining the reasoning behind AI judgments is a primary UX concern for opaque systems. [Domain: national defense]
- 90% of participants responded positively to the upgraded system; interview analysis highlighted the importance of friendly UI design and additional result explanations alongside AI-specific transparency features.
- The AI UX evaluation questionnaire yielded strong internal consistency (Cronbach's alpha: trust = 0.925, satisfaction = 0.923, safety = 0.918) and good confirmatory fit (CFI = 0.961, RMSEA = 0.057).
- A 9-factor structure was confirmed: satisfaction, safety, controllability, trust, causality, fairness, efficiency, accountability, explainability. This extends prior frameworks by explicitly including causality and explainability as distinct UX dimensions. [Domain: general/AI speakers initially, national defense for applied test]
- Gender and educational background have been noted in prior work as significant moderators of trust and XAI comprehension (citing Reeder et al., 2023); the study acknowledges the need for diverse participant samples. [Domain: recommendation systems]
- Novice AI users were found to prefer local over global explanations (citing Aechtner et al., 2022). [Domain: general]

## Transparency Constructs

The study operationalizes transparency primarily through two distinct questionnaire factors:

- **Explainability**: Items measuring the degree to which the system communicates how it works and why it makes particular judgments. Post-upgrade score improved from 5.25 to 8.05.
- **Causality**: Items capturing users' understanding of the causal basis for AI decisions. This is treated as distinct from explainability and showed the largest gain in the upgrade (3.48 → 6.88). The authors reference Shin's (2021) causability construct as inspiration.

Additional transparency-adjacent constructs in the questionnaire:
- **Accountability**: Items related to the system's ability to justify decisions and take responsibility. Score improved from 4.73 to 7.23.
- **Fairness**: Items related to algorithmic bias and equitable treatment. No significant improvement was observed.

The upgrade process introduced: (a) help functions and tutorials explaining system use; (b) additional data panels displaying the basis for change-detection and target-detection judgments; (c) disabled-state representations clarifying when functions were unavailable; (d) color coding for unity across detection modalities.

## Trust Constructs

Trust is treated as a single composite UX factor in the questionnaire. It is operationalized through self-report survey items measuring users' confidence in the system and willingness to rely on it. Trust improved significantly from 5.42 to 7.90 (on a 0-10 scale) following the interface upgrade. The study frames trust as behaviorally relevant (influencing adoption) but does not decompose it into cognitive, affective, and behavioural sub-dimensions. The trust measure aligns most closely with [[cognitive-trust]] (confidence based on system understanding).

## Relevance to Research Questions

**RQ1**: The study contributes a validated 9-factor operationalization of AI UX that explicitly separates explainability, causality, and transparency as distinct measurable dimensions. This instrument extends existing frameworks and represents a generalizable tool for measuring AI-related UX constructs including trust. The inclusion of causality as a standalone factor alongside explainability is a distinctive conceptual contribution (source: Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.txt).

**RQ2**: The study provides pre-post causal evidence that adding explanatory and transparency-enhancing interface features to a black-box AI system significantly improves user trust (5.42 → 7.90), causality perception (3.48 → 6.88), and explainability ratings (5.25 → 8.05), while maintaining or improving satisfaction, safety, controllability, efficiency, and accountability. The fairness dimension did not respond to the intervention, suggesting that not all AI UX factors are equally amenable to interface-level fixes. This constitutes evidence of a positive, intervention-driven transparency-trust relationship in a defense domain (source: Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.txt).

**RQ3**: The study notes that participants were non-experts in national defense and AI, deliberately recruited to minimize knowledge differences. Prior work cited (Reeder et al., 2023) demonstrates that gender and educational background moderate trust and XAI comprehension in recommendation systems. The study calls for future work with diverse user types. User role effects are acknowledged as a limitation rather than systematically studied here (source: Park et al._Designing_and_Evaluating_User_Experience_of_an_AI-Based_Defense_System.txt).

## Related pages

- [[explainability]]
- [[causability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq2-relationships]]
