# Recommendations with Benefits: Exploring Explanations in Information Sharing Recommender Systems for Temporary Teams

**Source file**: [Original article](../../raw/Musick et al._Recommendations with benefits.pdf)

**Summary**: A between-subjects study (N = 150) examines how the content (benefit-focused vs. algorithmic) and timing (at disclosure vs. at recommendation) of explanations in an information-sharing recommender system affect user disclosure, trust, and satisfaction, finding that benefit-focused explanations at the recommendation stage increase trust competence and reduce privacy concerns.

**Sources**: Musick et al._Recommendations with benefits.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Musick, Hauptman, Flathmann, McNeese, and Knijnenburg (2024, International Journal of Human-Computer Interaction) investigate how explanations from a personality-based information-sharing recommender system influence user behavior (information disclosure) and system perceptions (trust, privacy concern, satisfaction) in temporary workplace teams. The study is motivated by the challenge that temporary teams lack time to build relationships naturally and so may benefit from AI-mediated sharing of personality information.

The study uses a 2 (explanation content: algorithmic vs. benefit) × 2 (explanation occurrence: during disclosure vs. during recommendation) × 2 (baseline: no explanation at either stage) between-subjects design with 150 US participants recruited via Prolific, yielding 18–19 participants per condition. Participants completed a Big Five personality assessment and made binary decisions about which of eight personality facets to disclose to a simulated recommender system, then received four recommendations for working with hypothetical teammates.

Two types of explanations were tested:
- **Algorithmic explanations**: rationale based on system logic, e.g., "Based on how similar/different you and your teammate rank on this attribute and similar users..."
- **Benefit explanations**: rationale focused on team/individual benefits, e.g., "It is helpful for your teammates to understand how confident members are in their abilities..."

The domain is **collaborative technology / workplace teams / recommender systems**.

## Key Findings

- Providing benefit-related explanations during the recommendation stage significantly increased trust competence in the system (β = 0.470, p_one-tailed = .030). (Domain: collaborative tech/teamwork)
- Benefit-related explanations significantly reduced system-specific privacy concerns (β = −0.323, p_one-tailed = .028). (Domain: collaborative tech/teamwork)
- An interaction effect showed that algorithmic explanations provided during disclosure had a negative effect on trust competence compared to benefit explanations in the same condition (β = −0.602, p = .080). Explanation content (benefit vs. algorithmic) had a larger impact on perceptions than explanation timing.
- Benefit explanations provided during the recommendation stage had a larger positive effect on perceived helpfulness compared to algorithmic explanations in that condition (β = 1.420, p = .085).
- Disclosure levels showed only a near-significant trend: benefit explanations during disclosure increased disclosure (β = 0.67, p_one-tailed = .054); algorithmic explanations during disclosure had a smaller, non-significant positive effect. Timing mattered less than content for disclosure behavior.
- Trust propensity (individual trait) positively predicted trust competence (β = 0.229, p = .013) and negatively predicted privacy concern (β = −0.273, p = .002), confirming the role of dispositional trust.
- Perceived accuracy of personality results strongly predicted both trust competence (β = 0.211, p = .045) and perceived helpfulness (β = 0.682, p = .007) — suggesting system validity perceptions are a gateway to trust.
- Privacy concern negatively mediated the trust-to-satisfaction path (β = −0.292, p = .001 for privacy → trust; β = −0.535, p < .001 for privacy → satisfaction).

## Transparency Constructs

The paper operationalizes explanation type as **disclosure transparency** (algorithmic rationale) versus **benefit transparency** — whether the explanation reveals system logic or highlights user-relevant value. This maps onto distinct aspects of [[process-transparency]] (how the system works) versus [[outcome-transparency]] (what the user gains). The finding that benefit explanations outperform algorithmic explanations for trust and privacy concerns suggests that, in disclosure contexts, transparency about *benefit* is more relevant than transparency about *mechanism*.

The study also touches on [[disclosure]] as a construct: explanations serve partly to encourage user information sharing, which is itself a form of reciprocal transparency between user and system.

## Trust Constructs

The study measures multiple trust-related constructs:
- **Trust competence** (5-item scale from Benbasat & Wang, 2005): the system's expertise and ability to understand users' teamwork needs — a measure of [[cognitive-trust]]
- **Trust propensity** (4-item scale from Jessup et al., 2019): individual dispositional tendency to trust — [[dispositional trust]] moderator
- **Privacy concern** (3-item scale): inverse indicator of [[behavioural-trust]] and willingness to rely on the system
- **System satisfaction**: downstream outcome of trust and helpfulness

The full structural model shows that trust competence mediates from explanation content to system satisfaction, with privacy concern as a negative mediator — a complex trust pathway not captured by single-item trust measures.

## Relevance to Research Questions

**RQ1**: The paper contributes to understanding how trust is operationalized in recommender system contexts, decomposing it into competence trust, privacy concern, satisfaction, and helpfulness. The distinction between algorithmic and benefit explanations is a novel operationalization of what counts as "transparency" for end-users: users prioritize understanding what they gain (benefit transparency) over understanding how the system works (algorithmic transparency) in a disclosure context.

**RQ2**: Demonstrates a conditional effect of explanation content on trust: benefit explanations improve trust competence and reduce privacy concerns, while algorithmic explanations do not (and can even reduce trust competence at disclosure stage). The timing × content interaction adds nuance — benefit explanations at recommendation time produce the strongest trust effects. This is consistent with a conditional, not universally positive, transparency–trust relationship.

**RQ3**: The study does not manipulate user expertise. However, it captures trust propensity as an individual difference variable that moderates trust competence and privacy concern. The finding that individual trust propensity (dispositional trust) independently affects system trust perceptions is a relevant contribution to understanding user-level factors in transparency–trust dynamics. The temporary team context (workers with varying team experience) also provides ecological validity for understanding non-expert system users.

## Related pages

- [[process-transparency]]
- [[outcome-transparency]]
- [[disclosure]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[algorithmic-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
