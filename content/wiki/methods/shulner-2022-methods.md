# Shulner 2022 — Methods

**Summary**: A between-subjects online experiment (N = 425) comparing five explanation styles (case-based, demographic-based, input influence-based, sensitivity-based, certification-based) crossed with positive vs. negative system recommendations on non-expert users' fairness perceptions and outcome understanding for an algorithmic recruitment decision support system.

**Sources**: Shulner_Fairness,_explainability_and_i.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, 5 explanation styles × 2 recommendation outcomes)

## Sample
- N: 425 (after filtering)
- Population: general public (non-expert users)
- Domain: HR / algorithmic recruitment
- Country / region: not reported
- Recruitment method: online (platform not specified)

## Transparency operationalization
- Type: local explanation / explainability (five distinct textual explanation styles)
- Manipulation or measure: Between-subjects manipulation across five explanation styles applied to the same algorithmic recruitment decision: (1) Case-based — similar past cases used as reference; (2) Demographic-based — comparison to demographic group averages; (3) Input influence-based — feature importance weighting; (4) Sensitivity-based — how changes to inputs would change the output (counterfactual); (5) Certification-based — external audit certification confirming system fairness (novel style). Each style paired with either a positive or negative system recommendation (crossed). A control condition (no explanation) was not included; all conditions received one of the five styles.
- Scale / instrument name: not applicable (experimental manipulation; textual vignette stimuli)
- Number of items: not applicable

## Trust operationalization
- Type: not directly measured; fairness perception used as a proxy for algorithmic trust; outcome understanding measured as a secondary construct
- Measure: (1) Fairness perception — Likert-scale self-report items assessing perceived fairness of the algorithmic recruitment decision; (2) Outcome understanding — self-report items assessing how well the participant understood the system's decision on the basis of the explanation provided. Trust is not measured as an independent construct but fairness perception is treated as a component of cognitive/algorithmic trust.
- Scale / instrument name: not reported (author-developed fairness perception and understanding items)
- Number of items: not reported
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Recommendation outcome (positive vs. negative): primary crossed factor — dominates fairness perception; users receiving a negative recommendation rate the system as unfair regardless of explanation style; relevant to RQ2
- Non-expert status of all participants: sample characteristic — findings apply specifically to non-expert users; expert vs. novice comparison not conducted (relevant to RQ3)
- Note: no individual difference moderators (e.g., statistical literacy, domain expertise) formally tested, but identified as a limitation

## Statistical approach
- Primary analysis method: ANOVA or factorial analysis comparing fairness perception and understanding scores across explanation style conditions and recommendation outcomes; post-hoc pairwise comparisons
- Software: not reported
- Key model fit or effect size reported: mean fairness scores per condition reported (certification-based positive: M = 1.565); significance of pairwise comparisons reported; specific effect sizes not specified in source

## Author-noted limitations
- All participants are non-experts; results may not generalise to domain specialists or HR professionals
- No control (no-explanation) condition included; relative benefit of any explanation over none cannot be directly tested
- Textual vignette design may not capture real-world algorithmic decision contexts
- Statistical literacy and domain background not measured; individual differences in explanation comprehension not accounted for
- Single recruitment domain; generalisability to other algorithmic decision contexts unknown
- Certification-based style is novel and untested in prior work; interpretation may differ across cultural contexts

## Related pages
- [[shulner-fairness-explainability]]
- [[explainability]]
- [[example-based-explanations]]
- [[counterfactual-explanations]]
- [[algorithmic-trust]]
- [[cognitive-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
