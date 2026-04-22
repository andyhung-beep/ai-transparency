# Woodcock 2021 — Methods

**Summary**: A 2×4 between-subjects cross-sectional experiment (N = 750) in which participants watched an AI symptom checker video and rated trust across three factors (Faith, Comprehension, Depth), finding that explanation type effects on trust are contingent on prior disease knowledge rather than universally effective.

**Sources**: Woodcock et al._The_Impact_of_Explanations_on_.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, 2×4 factorial design; cross-sectional; online)

## Sample
- N: 750
- Population: general public (laypersons; no medical expertise required)
- Domain: consumer digital health / mHealth (AI symptom checker application)
- Country / region: United Kingdom (Oxford Internet Institute)
- Recruitment method: not reported (online experiment)

## Transparency operationalization
- Type: explainability (feature importance / input influence), example-based explanation (social proof), counterfactual explanation, and no-explanation control
- Manipulation or measure: 2×4 factorial between-subjects design crossing disease type (well-known: migraine vs. lesser-known: temporal arteritis) with four explanation types: (1) Input influence — lists symptoms most influential to the diagnosis (how-explanation); (2) Social proof — cites how many prior similar cases received this diagnosis (case-based how-explanation); (3) Counterfactual — states what symptom change would alter the diagnosis (why-explanation); (4) No explanation. All delivered via a 3-minute chatbot simulation video. Each cell: approximately 93–94 participants.
- Scale / instrument name: not applicable (between-subjects manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: multi-dimensional (Faith, Comprehension, Depth) — components of cognitive trust and perceived explanation quality
- Measure: Bespoke trust scale adapted from Hoffman's Explanation Satisfaction Scale; exploratory factor analysis (EFA) generated three trust factors: (1) Faith — general trust/belief in the explanation and system; (2) Comprehension — perceived understanding of the information conveyed; (3) Depth — perceived richness and completeness of the explanation (emergent for some conditions). Reliance intent also captured (propensity to follow AI triage instructions).
- Scale / instrument name: Adapted from Hoffman's Explanation Satisfaction Scale; factor structure derived via EFA
- Number of items: not reported (EFA-derived subscales)
- Behavioural vs self-report: self-report (with reliance intent as a behavioural intention proxy)

## Moderators and covariates tested
- Disease knowledge / prior familiarity: primary moderator — manipulated via disease type (migraine = high knowledge vs. temporal arteritis = low knowledge); disease type was the dominant driver of trust differences, with explanation type mattering only for lesser-known disease (relevant to RQ3 as proxy for domain expertise)
- Explanation type × disease knowledge interaction: tested via MANOVA; significant for input influence (p = .001), social proof (p = .049), and no explanation (p = .006); marginal for counterfactual (p = .053)

## Statistical approach
- Primary analysis method: MANOVA (multivariate ANOVA) with three trust factors as dependent variables; follow-up univariate ANOVAs and t-tests for individual factor comparisons; exploratory factor analysis (EFA) for trust scale development
- Software: not reported
- Key model fit or effect size reported: MANOVA p-values reported (e.g., explanation type for migraine p = .65 [ns]; temporal arteritis p = .09; disease × explanation interaction p-values per condition); EFA factor structure reported; Cronbach's α not reported for individual factors

## Author-noted limitations
- Video-based simulation (not real AI interaction); ecological validity limited
- The conversational nature of the chatbot format conveyed explanatory information even in the no-explanation condition, attenuating condition differences
- Trust scale developed post-hoc via EFA from this study; external validation not established
- Single symptom checker scenario type; generalisability to other medical AI contexts unknown
- Disease knowledge was manipulated via disease type (common vs. rare) rather than directly measured; participant knowledge variance within each disease group not controlled
- The study does not examine actual diagnostic accuracy or triage outcomes

## Related pages
- [[woodcock-explanations-symptom-checker]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[explainability]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
