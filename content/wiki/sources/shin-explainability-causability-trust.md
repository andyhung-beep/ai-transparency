# The Effects of Explainability and Causability on Perception, Trust, and Acceptance: Implications for Explainable AI

**Source file**: [Original article](../../raw/Shin_The effects of explainability and causability on perception, trust, and acceptance.pdf)

**Summary**: Shin tests a structural model in a news recommendation context, showing that causability (users' subjective ability to understand explanations) acts as an antecedent of explainability and partially mediates the path from fairness, accountability, and transparency (FAT) perceptions to user trust and performance expectancy.

**Sources**: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *International Journal of Human–Computer Studies* (2021), this study examines the dual roles of explainability and causability in shaping user trust and behavioral acceptance of AI recommendation systems. The author applies the Heuristic-Systematic Model (HSM) to explain how users process AI features through two routes: heuristic processing (using FAT cues as quick assessments) and systematic processing (detailed evaluation through causability-mediated understanding). The empirical context is a news recommendation system, making this one of the few studies to examine XAI effects in media/journalism.

Causability is borrowed from the medical informatics literature (Holzinger et al.) and adapted to refer to the extent to which users can understand and evaluate the quality of AI explanations—it is a user-side construct, not a system property.

## Key Findings

- Causability strongly predicts explainability (standardized path coefficient = 0.939), indicating that users' capacity to make sense of AI explanations drives their appraisal of the system's explainability level (domain: news recommendation/media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)
- Explainability is positively associated with transparency (0.762), fairness (0.535), and accountability (0.693), which together predict trust (R² = 0.581) (domain: media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)
- Trust strongly predicts performance expectancy (path coefficient = 0.911), linking transparency-driven trust to behavioral acceptance (domain: media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)
- Causability partially mediates the relationships between FAT dimensions (transparency, fairness, accountability) and trust, with VAF values ranging from 31–50%, indicating both direct and causability-mediated paths are significant (domain: media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)
- Explanations of *why* certain articles are recommended generate cognitive trust, while causability—the *extent to which* users can understand explanations—provides emotional confidence (domain: media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)
- Heuristic processing (via FAT assessments) and systematic processing (via causability) operate as complementary trust-formation routes, with trust serving as the linking mechanism (domain: media). (source: Shin_The effects of explainability and causability on perception, trust, and acceptance.txt)

## Transparency Constructs

The paper maps [[explainability]] as a system-level property (the degree to which AI decision processes can be traced and communicated) and [[causability]] as a user-level property (the degree to which users can subjectively evaluate and make use of those explanations). This separation is a conceptual contribution: a system may be highly explainable by design, but causability is zero if users cannot process the explanations provided. The FAT framework links [[algorithmic-transparency]] (transparency dimension), [[outcome-transparency]] (accountability dimension), and fairness into a unified antecedent cluster.

## Trust Constructs

The study primarily captures [[cognitive-trust]], operationalized as user confidence in the AI system's competence and reliability. The paper also identifies an affective component: causability providing "emotional confidence," suggesting overlap with [[affective-trust]]. Trust is treated as a mediating variable between FAT perceptions and performance expectancy (a form of [[behavioural-trust]] proxied by intentions to use the service). The [[algorithmic-trust]] framing from prior work by the same author is implicitly present: trust is conceptualized as a multidimensional appraisal of an algorithm's transparency, fairness, and accountability.

## Relevance to Research Questions

**RQ1**: Provides clear operationalizations of both explainability (system property) and causability (user property), and maps both onto the FAT framework. Demonstrates via SEM that trust is a theoretically coherent latent variable with significant paths from all three FAT dimensions. Clarifies the conceptual distinction between system-side explainability and user-side interpretability—a gap often collapsed in the XAI literature.

**RQ2**: Demonstrates a positive linear path from explainability/causability through FAT perceptions to trust and performance expectancy. The dual-process mediation (partial mediation via causability) suggests the relationship is not purely additive: the systematic route through causability amplifies the heuristic route through FAT. No non-linear or negative effects of transparency are reported, in contrast to Schilke & Reimann (2025) in workplace contexts.

**RQ3**: Causability as a user construct is implicitly tied to [[user-expertise]] and cognitive capacity: users vary in their ability to understand explanations, and this variation drives differences in trust formation. The paper does not compare expert vs. novice groups but argues that designing for causability—making explanations interpretable at the user's level—is essential for inclusive XAI. This has clear implications for how transparency effects differ across user populations.

## Related pages

- [[explainability]]
- [[causability]]
- [[algorithmic-trust]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[rq1-conceptualizations]]
