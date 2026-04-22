# Patients' Perceptions Toward Human–Artificial Intelligence Interaction in Health Care: Experimental Study

**Source file**: [Original article](../../raw/Esmaeilzadeh et al_2021_Patients_ perceptions toward human-artificial intelligence interaction in health care.pdf)

**Summary**: A 2×3 experimental survey study (N = 634 US patients) comparing perceptions of trust, risk, communication barriers, transparency, liability, and intention to use across six AI healthcare encounter scenarios, finding that traditional physician-only encounters consistently elicit higher trust and lower concern than AI-based alternatives.

**Sources**: Esmaeilzadeh et al_2021_Patients_ perceptions toward human-artificial intelligence interaction in health care.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Esmaeilzadeh, Mirzaei, and Dharanikota (2021), published in the *Journal of Medical Internet Research*, designed a 2 (illness type: acute vs. chronic) × 3 (encounter type: AI-only/substituting, AI+physician/augmenting, physician-only/traditional) between-subjects experiment to examine how patients perceive nine outcome dimensions—performance risk, social biases, privacy concerns, trust, communication barriers, transparency of regulatory standards, liability issues, benefits, and intention to use. Data were collected from 634 participants via Amazon Mechanical Turk (May 2020). Propensity score matching ensured demographic comparability across groups (approximately 100–113 per condition).

The study operationalises three distinct forms of clinical AI encounter—AI substituting the physician, AI augmenting the physician (collaborative intelligence), and no AI—enabling comparison of how the degree of AI autonomy in healthcare affects patient perceptions.

## Key Findings

- Patients reported significantly lower trust in AI-only encounters compared to traditional physician-only visits for both chronic (p = .004) and acute (p < .001) conditions. (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Trust followed a consistent ordering: physician-only > AI+physician > AI-only across both illness types (marginal means: 18.4 vs. 17.1 vs. 16.0 on a 5-item scale). (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Communication barriers were significantly higher for both AI-only and AI+physician encounters versus physician-only for both acute and chronic patients (all p ≤ .03). The concern that AI reduces human relational aspects of care was persistent even when the physician remained involved. (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Transparency concerns about regulatory standards were significantly greater for AI encounters (AI-only and AI+physician) than for physician-only visits for both illness types (all p ≤ .02). (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Liability concerns were elevated for AI encounters over physician-only visits, particularly for AI+physician in acute patients (p = .003) and AI-only in chronic patients (p = .04). (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Intention to use was significantly higher for physician-only encounters than for AI-only in both acute (p = .01) and chronic conditions (p < .001), and also higher than AI+physician for chronic patients (p = .006). (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Perceived benefits were significantly higher for physician-only encounters than AI-only for chronic patients only (p = .004), suggesting illness type moderates benefit perceptions. (source: Esmaeilzadeh et al_2021; domain: healthcare)
- No significant differences were found across scenarios for perceived performance risk and perceived social biases—suggesting these concerns are background-level regardless of encounter type. (source: Esmaeilzadeh et al_2021; domain: healthcare)
- Privacy concerns were significantly higher for acute patients in AI+physician (vs. physician-only, p = .03), but not for chronic patients, indicating illness acuity shapes sensitivity to data sharing. (source: Esmaeilzadeh et al_2021; domain: healthcare)
- The pattern of results implies that incompatibility with technical, ethical, or regulatory values is a primary driver of AI rejection in healthcare, beyond mere performance uncertainty. (source: Esmaeilzadeh et al_2021; domain: healthcare)

## Transparency Constructs

The study introduces **perceived transparency of regulatory standards** as a distinct construct: the extent to which patients believe regulatory guidelines to assess AI safety are yet to be formalised. This is not the conventional XAI sense of transparency (making model internals visible) but rather an [[institutional-trust]] and governance-oriented dimension—closer to [[process-transparency]] at the systemic/regulatory level. The study highlights that patients perceive AI clinical applications as "black boxes" (post-ANN training, decision logic is described as essentially opaque) and that the absence of regulatory accountability frameworks compounds this concern.

The paper references the IEEE P7001 "Transparency in Autonomous Systems" standard as a potential remediation mechanism, framing transparency as a policy and regulatory challenge, not solely a technical or interface-design one.

## Trust Constructs

Trust is operationalised with a 5-item scale (α = .92) adapted from Luxton (2014) measuring patients' belief that the clinical encounter is trustworthy. This captures **institutional trust** in the healthcare delivery mechanism as well as **cognitive trust** in the reliability and competence of AI or physician. The consistent ordering (physician-only > AI+physician > AI-only) maps directly to the [[institutional-trust]] literature: human providers carry accumulated relational and legitimacy-based trust that AI systems cannot yet replicate. The study also touches on [[affective-trust]] through its communication barriers construct—the perceived absence of empathy and compassion in AI encounters is presented as a driver of distrust.

## Relevance to Research Questions

**RQ1**: The study develops a multidimensional operationalisation of patient concerns about AI in healthcare, distinguishing nine conceptually distinct dimensions. Trust is measured separately from performance risk, communication quality, and regulatory transparency—an unusually granular decomposition. This multi-construct approach contributes significantly to [[rq1-conceptualizations]], especially by introducing regulatory transparency and liability concerns as distinct factors.

**RQ2**: The study provides robust evidence that the relationship between AI presence and trust is negative in the healthcare domain—even augmented AI (physician + AI) is trusted less than physician-only. This stands in contrast to domains where AI explanations increase trust. The effect is consistent and statistically significant, contributing a domain-specific corrective to simplistic "XAI raises trust" conclusions in [[rq2-relationships]]. The interaction between illness type (acute vs. chronic) and encounter type provides conditional/moderated effects.

**RQ3**: Illness type (acute vs. chronic) functions as a patient-level characteristic that moderates perceptions. Chronic patients showed stronger negative reactions to AI-only encounters (lower trust, higher liability concern) than acute patients, possibly because chronic disease management requires ongoing relational trust. While this is not user expertise per se, it is a meaningful patient role/context factor that influences AI trust responses, relevant to [[rq3-user-roles]].

## Related pages

- [[institutional-trust]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[process-transparency]]
- [[disclosure]]
- [[domain-context]]
- [[perceived-risk]]
