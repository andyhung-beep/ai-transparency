# The Effects of Transparency on Trust in and Acceptance of a Content-Based Art Recommender

**Source file**: [Original article](../../raw/Cramer et al._The_effects_of_transparency_on.pdf)

**Summary**: A between-subjects experiment (N = 60) with a content-based art recommender (CHIP, Rijksmuseum collection) comparing three transparency conditions — no transparency, "why" explanations (reasons for recommendations), and confidence ratings ("sure" percentages) — finding that "why" explanations increased acceptance of individual recommendations and actual understanding of the system, but did not increase overall trust in or adoption of the recommender system itself.

**Sources**: Cramer et al._The_effects_of_transparency_on.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Cramer et al. (2008) is a foundational empirical study on transparency in user-adaptive recommender systems, conducted in the cultural heritage / e-culture domain. Participants interacted with the CHIP system — a content-based art recommender drawing on the Rijksmuseum Amsterdam's digitised collection — and were randomly assigned to one of three conditions:

1. **Non-transparent (Non)**: Recommendations shown with no explanation.
2. **Transparent (Why)**: A "why?" link below each recommendation that opened a pop-up listing the shared artwork properties that triggered the recommendation (e.g., "This artwork was recommended because you liked works by Rembrandt and this is also a work by Rembrandt").
3. **Confidence rating (Sure)**: A percentage below each recommendation indicating how confident the system was that the user would find the artwork interesting.

Participants were given the task of selecting six artworks for a short personal presentation on their art interests. Sessions included think-aloud observation, a post-task questionnaire, structured interview, and a follow-up questionnaire eight weeks later.

The study is widely cited as an early empirical demonstration of the distinction between acceptance of recommendations and acceptance of the recommender system as a whole, and as evidence that transparency does not automatically increase trust.

## Key Findings

- The "why" explanation condition was perceived as significantly more transparent than the non-transparent condition (Mann-Whitney U, p(1-tailed) = .025). (Domain: cultural heritage / e-culture)
- Participants in the "why" condition had significantly better actual understanding of how the system made recommendations, assessed by independent coding of interview responses (Mann-Whitney U, p(1-tailed) = .0065). (Domain: e-culture)
- Critically, there was no significant correlation between perceived understanding and actual understanding (Spearman's rho = .005), illustrating that users cannot reliably assess their own comprehension of a recommender system. (Domain: e-culture)
- Acceptance of individual recommendations was significantly higher in the "why" condition: participants included significantly more recommended artworks in their final selection compared to the non-transparent condition (p(1-tailed) = .013). (Domain: e-culture)
- However, acceptance of the system itself — measured by willingness to delegate artwork selection to the recommender — did not differ significantly between "why" and non-transparent conditions. (Domain: e-culture)
- Trust in the system was not significantly higher in the "why" condition (p(1-tailed) = .224), contradicting the hypothesis that transparency increases trust. (Domain: e-culture)
- The "sure" (confidence rating) condition produced no significant effects on perceived transparency, understanding, acceptance of recommendations, acceptance of system, or trust compared to the non-transparent condition. Confidence percentages were generally poorly understood and found slightly not useful (mean 3.70 on 1–7). (Domain: e-culture)
- Perceived understanding correlated positively with trust (rho = .450) and with intent to use the system (rho = .517), suggesting that understanding plays an important role in trust formation — but the experimental manipulation did not reliably translate perceived understanding gains into trust gains. (Domain: e-culture)
- Trust was strongly correlated with intent to use the system (rho = .805), confirming trust as a key mediator of system adoption. (Domain: e-culture)
- Long-term follow-up (8 weeks) showed no change in attitudes, suggesting that initial session impressions were stable. (Domain: e-culture)
- Qualitative observations revealed that some "why" condition participants showed "filtering behaviour" — actively adjusting their ratings to shape the system's recommendations — indicating that understanding can affect user-system interaction patterns beyond simple acceptance. (Domain: e-culture)

## Transparency Constructs

The study tests two contrasting forms of transparency:

- **"Why" explanations** ([[process-transparency]] / [[outcome-transparency]]): Content-based rationale explanations showing which shared artwork properties drove a specific recommendation. These expose the system's decision criteria for individual recommendations — a form of local [[explainability]] consistent with content-feature-based transparency.
- **Confidence ratings** ([[uncertainty-visualization]]): Numerical percentage confidence scores indicating the system's estimated probability that the user will like an artwork. These communicate uncertainty about a specific recommendation without revealing the reasoning process.

The distinction between these two transparency types operationalises an important theoretical point: communicating confidence (outcome uncertainty) is different from communicating reasoning (process transparency), and the two have different effects on user understanding and behaviour.

The study operationalises transparency manipulation as a between-subjects factor, with [[algorithmic-transparency]] (understanding of recommendation criteria) as both an outcome and a mediator.

## Trust Constructs

The study uses a rich multi-method trust measurement approach:

- **[[cognitive-trust]]** (questionnaire): Adapted from Jian et al. (2000), 10 items capturing trust in system competence and benevolence (e.g., "I trust the system", "I can depend on the system", "The system is reliable"). Scale reliability α = .901.
- **[[behavioural-trust]]** (acceptance of recommendations): Number of recommended artworks included in the participant's final selection of six artworks — a direct behavioural measure of reliance on the system's outputs.
- **[[behavioural-trust]]** (system adoption): Acceptance scenario question measuring willingness to delegate the artwork selection task to the system versus browsing a catalogue manually under time pressure.
- **Intent to use**: Three-item scale (α = .914) measuring future usage intentions.

The paper demonstrates that these trust and acceptance constructs are not interchangeable: explanations can improve acceptance of individual recommendations without improving trust in or overall adoption of the system — a critical conceptual distinction for the field.

## Relevance to Research Questions

**RQ1**: This paper is foundational for RQ1. It provides early empirical operationalisations of transparency (why-explanations, confidence ratings), trust (cognitive + behavioural, multi-method), and acceptance in a recommender system context. The distinction between recommendation acceptance and system acceptance is a key conceptual contribution. The paper also operationalises "actual understanding" via independent assessment, going beyond self-report.

**RQ2**: The results constitute a landmark null finding for trust: transparency in the form of "why" explanations increased understanding and recommendation acceptance, but did not increase trust in the system itself. This dissociation between transparency → understanding → acceptance of recommendations, and transparency → trust → system adoption, is a central result for the literature on transparency–trust relationships. The confidence ratings had no effect on any outcome, suggesting that numeric uncertainty information is not processed as a meaningful transparency cue by lay users. These are important conditional effects indicating the relationship between transparency and trust is neither simple nor universal.

**RQ3**: The study does not directly manipulate user expertise. However, qualitative analysis revealed that one art expert participant was more critical of the "why" explanations due to oversimplification of artwork labelling. This aligns with the broader literature suggesting that experts may respond differently to explanations than novices. The study highlights that both domain knowledge (art expertise) and technical knowledge (familiarity with recommender systems) may moderate transparency effects — a gap the study acknowledges as needing further investigation. Relevant to [[user-expertise]] and [[domain-context]].

## Related pages

- [[process-transparency]]
- [[outcome-transparency]]
- [[uncertainty-visualization]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
