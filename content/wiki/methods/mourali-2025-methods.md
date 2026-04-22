# Mourali et al. 2025 — Methods

**Summary**: A series of five preregistered between-subjects experiments (total N ≈ 2,000+) comparing the effects of sensitivity-based and case-based post-hoc explanations of algorithmic decisions on consumer perceptions of transparency, fairness, trust, and behavioural intentions across multiple consumer and high-stakes domains.

**Sources**: Mourali et al._Post hoc explanations improve consumer responses to algorithmic decisions.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (five preregistered between-subjects experiments)

## Sample
- N: approximately 2,000+ (Study 1: N = 443; Study 5: N = 764; Studies 2–4 not individually reported in available sources)
- Population: general adult consumers (US and Canadian)
- Domain: consumer / e-commerce / finance (car insurance pricing, credit cards, bonus eligibility); extended to criminal justice, healthcare, and professional training in Study 4
- Country / region: United States and Canada
- Recruitment method: Prolific Academic

## Transparency operationalization
- Type: outcome transparency and process transparency — local post-hoc explanations of individual algorithmic decisions
- Manipulation or measure: three between-subjects conditions across most studies: (1) no explanation; (2) sensitivity explanation — counterfactual format showing what input values would need to change to alter the decision outcome (e.g., "If 10% or less of your driving took place at night, you would have qualified for the cheapest tier"); (3) case-based explanation — a similar historical case from the training data presented for comparison; actionability of sensitivity explanations further varied in Study 3 (actionable factors the consumer can change vs. non-actionable factors the consumer cannot change)
- Scale / instrument name: perceived transparency: 3-item scale (α = 0.95); source not explicitly named in available sources
- Number of items: 3 (perceived transparency scale)

## Trust operationalization
- Type: cognitive and affective (combined Attitude index: fairness + trust)
- Measure: combined Attitude index comprising perceived fairness and trust in the algorithmic system; separate behavioural intentions scale (likelihood to do business with the deploying company); α = 0.92 for combined Attitude index
- Scale / instrument name: custom Attitude index (fairness + trust composite); source not explicitly named
- Number of items: not reported for individual sub-scales; composite α = 0.92
- Behavioural vs self-report: self-report for all measures (perceived transparency, attitude, behavioural intentions)

## Moderators and covariates tested
- Actionability of explanation: manipulated in Study 3 — actionable sensitivity explanations (factors the consumer can change) versus non-actionable (factors the consumer cannot change); actionable explanations significantly outperformed non-actionable ones; relevant to RQ2
- Decision outcome valence (positive vs. negative outcome): manipulated in Study 5 — explanation benefits on attitude and behavioural intention were eliminated when the decision outcome was positive; relevant to RQ2
- Domain / scenario type: Study 4 tested four domains (credit card, parole, health insurance, professional training) as a replication check; relevant to RQ2
- User expertise / AI literacy: not manipulated or measured; paper focuses on lay consumers and acknowledges that global explanations are more relevant for technical users — relevant to RQ3 implicitly
- Perceived controllability: measured as a mediating mechanism in a post-test; identified as the primary driver of actionable over non-actionable explanation advantage

## Statistical approach
- Primary analysis method: ANOVA (one-way and factorial); PROCESS macro for mediation; planned contrasts; preregistered hypotheses
- Software: not reported
- Key model fit or effect size reported: Study 1 η² for transparency = 0.356 (very large effect size); Attitude index α = 0.92; perceived transparency scale α = 0.95

## Author-noted limitations
- Sensitivity explanations are necessarily selective and may not faithfully represent underlying model computations, raising the risk of misleading transparency
- All studies conducted online with Prolific; ecological validity in real consumer decision contexts not established
- Case-based explanations may be more effective for positive outcomes or different decision domains not tested here
- User expertise and AI literacy not controlled or measured; effects may vary with technical sophistication
- The study does not assess long-term trust effects or repeated interactions with algorithmic systems
- Sensitivity explanation format was fixed; different framings or levels of detail may alter effects

## Related pages
- [[mourali-posthoc-explanations-consumer]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
