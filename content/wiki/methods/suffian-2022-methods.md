# Suffian et al. (2022) — Methods

**Summary**: A technical paper proposing and evaluating the Feedback-based Counterfactual Explanation (FCE) method on a bank loan classification dataset (N = 100 test instances), using user-specified feature constraints to generate more actionable counterfactual explanations via SVM and Random Forest classifiers.

**Sources**: Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf

**Research questions addressed**: RQ1

**Last updated**: 2026-04-19

---

## Study design
technical paper (algorithm development and computational evaluation; no user study or human-subjects experiment conducted)

## Sample
- N: 100 (test instances from bank loan classification dataset; not human participants)
- Population: not applicable (evaluation is computational, not human-subjects)
- Domain: finance / credit scoring (bank loan approval classification)
- Country / region: not reported
- Recruitment method: not applicable

## Transparency operationalization
- Type: counterfactual explanation — user-feedback-driven generation of minimal feature changes that would flip an AI classification decision to a desired outcome
- Manipulation or measure: two-stage user feedback process — (1) pre-generation: users specify acceptable numerical feature ranges and binary categorical change preferences to constrain counterfactual search space; (2) post-generation: users evaluate produced counterfactuals; algorithm evaluated computationally on validity (target-class rate), proximity (MAD distance), and actionability
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: not applicable (trust is discussed conceptually as a motivation but not empirically measured)
- Measure: trust not measured as a dependent variable; the paper argues theoretically that user-aligned explanations improve trust and adoption, but no user study instruments were administered
- Scale / instrument name: not applicable
- Number of items: not applicable
- Behavioural vs self-report: not applicable

## Moderators and covariates tested
- None reported; no human-subjects variables examined — user expertise or role not studied (relevant to RQ3 as a gap)

## Statistical approach
- Primary analysis method: computational evaluation — 10-fold cross-validation comparing SVM and Random Forest classifiers on the bank loan dataset; counterfactual quality assessed via validity rate (proportion reaching target class), proximity (MAD distance), and actionability rate
- Software: Python (implementation language; specific libraries not reported)
- Key model fit or effect size reported: Random Forest achieved higher accuracy and F-measure than SVM in 10-fold cross-validation (specific values not reported in source summary); FCE validity rate = 84% (84 of 100 counterfactuals reached target class); 16% failed actionability criterion

## Author-noted limitations
- No user study conducted; trust and acceptance improvements are assumed rather than empirically demonstrated
- Evaluation limited to a single dataset (bank loan classification); generalisability to other domains and model types not established
- The 16% failure rate in actionability reflects challenges when user-specified constraints are overly restrictive; no strategy for handling over-constrained feedback is proposed
- The paper does not examine how different user types (e.g., expert vs. novice) engage with the feedback elicitation interface
- Proximity metric (MAD distance) penalises income and mortgage features because dataset distributions differ from user-provided ranges, creating a metric artefact

## Related pages
- [[suffian-fce-counterfactual-feedback]]
- [[counterfactual-explanations]]
- [[explainability]]
- [[algorithmic-trust]]
- [[rq1-conceptualizations]]

## References
Suffian, M., et al. (2022). FCE: Feedback-based counterfactual explanations for explainable AI. *IEEE Access*, 10, 72363–72374.
