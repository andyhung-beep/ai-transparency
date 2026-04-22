# Physician Understanding, Explainability, and Trust in a Hypothetical Machine Learning Risk Calculator

**Source file**: [Original article](../../raw/Diprose et al._Physician understanding.pdf)

**Summary**: A survey study of 170 New Zealand physicians examining the relationships among understanding, explainability, and trust in ML risk calculator outputs, finding significant associations among all three constructs and a preference for local over global model-agnostic explanations.

**Sources**: Diprose et al._Physician understanding.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Diprose et al. (2020), published in the *Journal of the American Medical Informatics Association*, investigated whether physician understanding of ML outputs is related to their ability to explain those outputs to patients (explainability) and their willingness to follow the ML recommendation (operationalised as trust/intended behaviour). Using a survey built around a hypothetical ML risk calculator for pulmonary embolism, the study exposed physicians to three consecutive ML output conditions: (1) no explanation (control), (2) a global model-agnostic explanation (variable importance or individual conditional expectation plot), and (3) a local model-agnostic explanation (LIME or Shapley values). Physicians were asked three questions after each output: how much it made sense to them, whether they could explain it to a patient, and whether they would follow the recommendation.

The study was conducted in New Zealand across several district health boards and primary health organisations, with 1,315 physicians surveyed and 170 completing the instrument (13%). The study context—physicians as expert intermediaries who must both understand and communicate AI outputs to patients—makes it particularly relevant to both [[user-expertise]] and [[process-transparency]] questions.

## Key Findings

- Physician understanding and explainability were significantly associated (Cochran–Mantel–Haenszel χ² = 156.3, p < .001); higher understanding predicted greater reported ability to explain to patients. (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- Physician understanding and intended behaviour (trust) were significantly associated (χ² = 128.7, p < .001); no physician reporting "not at all" understanding indicated they would follow the recommendation. (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- Explainability and trust were significantly associated (χ² = 61.2, p < .001). (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- 88% of physicians preferred ML outputs that included a model-agnostic explanation over the unexplained control. (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- Local explanations (LIME 32%, Shapley values 30%) were preferred over global explanations (variable importance 18%, ICE plots 20%). (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- No particular explainability method had a greater effect on intended physician behaviour (all McNemar pairwise comparisons non-significant). (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- 76% of physicians reported the unexplained ML output as trustworthy—suggesting empirical performance information alone is often sufficient to elicit initial trust, even without mechanistic explanation. (source: Diprose et al._Physician understanding.txt; domain: healthcare)
- Qualitative word-cloud analysis revealed that physicians valued simplicity, patient specificity, and confirmation of existing clinical knowledge in their preferred explanations. (source: Diprose et al._Physician understanding.txt; domain: healthcare)

## Transparency Constructs

The study operationalises **explainability** in a distinct, practically-oriented way: physician ability to re-explain an ML output to a patient. This intermediary explainability construct sits between model interpretability and the patient's right to a "meaningful explanation" under GDPR. The study tests **model-agnostic post-hoc explanations** (LIME, Shapley values, variable importance, ICE plots), which map onto both [[explainability]] and [[algorithmic-transparency]]. The distinction between global (population-level) and local (patient-specific) explanations is explicitly examined, with local explanations corresponding to [[counterfactual-explanations]] and instance-level reasoning.

The authors note a potential mismatch between what physicians regard as "sufficient" explanation and what legal frameworks (GDPR Article 22) require, highlighting a tension between [[process-transparency]] as a social/legal norm and as a cognitive aid.

## Trust Constructs

Trust is operationalised behaviourally as intended compliance ("would you follow this recommendation?"), placing the study squarely in the [[behavioural-trust]] / [[appropriate-reliance]] literature. The study does not separately measure cognitive or affective dimensions of trust, but the association between perceived understanding and intended compliance implies [[cognitive-trust]] mechanisms are at work. The finding that 76% of physicians would follow a well-performing ML without explanation further connects to questions of [[algorithm-aversion]] (its absence here) and [[trust-calibration]] (whether trust is appropriately calibrated when explanation is absent).

## Relevance to Research Questions

**RQ1**: The study provides a healthcare-specific operationalisation of explainability (physician ability to relay ML logic to patients) that is distinct from standard AI explainability definitions. Trust is operationalised as intended clinical compliance, a behavioural rather than attitudinal measure. Together these constructs connect to [[rq1-conceptualizations]].

**RQ2**: Significant positive linear associations are found among understanding, explainability, and trust. However, adding explanations did not significantly alter intended behaviour beyond the high baseline trust already elicited by the unexplained condition—a ceiling effect that qualifies the simple "more explanation = more trust" story. This nuanced pattern is relevant to [[rq2-relationships]].

**RQ3**: Physicians are a clearly defined expert user group whose domain knowledge mediates their interpretation of ML outputs. The preference for local (patient-specific) explanations aligns with the hypothetico-deductive clinical reasoning style, suggesting expertise shapes the explanation format most conducive to trust. Relevant to [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
