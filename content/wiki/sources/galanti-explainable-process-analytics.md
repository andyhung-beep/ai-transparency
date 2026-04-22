# An Explainable Decision Support System for Predictive Process Analytics

**Source file**: [Original article](../../raw/Galanti et al._An explainable decision support system for predictive process Analytics.pdf)

**Summary**: Galanti et al. propose and evaluate a Shapley Value-based explainable predictive process analytics framework integrated into the IBM Process Mining Suite, demonstrating through a user study (n = 20 process analysts) that SHAP-powered global and local explanations are intelligible, usable, and trusted by end users in business process management contexts.

**Sources**: Galanti et al._An explainable decision support system for predictive process Analytics.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Galanti, de Leoni, Monaro, Navarin, Marazzi, Di Stasi, and Maldera (2022; arXiv preprint submitted to Elsevier, 26 July 2022) address a gap in predictive business process monitoring: existing frameworks prioritize prediction accuracy without providing explanations, which prevents stakeholders from trusting and adopting the technology. The paper makes three distinct contributions: (1) a comparative evaluation of Catboost and LSTM for process prediction, finding Catboost preferable due to speed with comparable accuracy; (2) the design of a SHAP-based explanation framework generating both global (model-level) and local (instance-level) explanations; and (3) a rigorous user study deploying the framework within a commercial product (IBM Process Mining Suite) and evaluating 20 process analysts on 18 tasks.

The paper is technically oriented but culminates in a human-subjects evaluation whose results are directly relevant to how users understand and trust AI-generated explanations in the business process management (BPM) domain.

## Key Findings

- Users achieved an average task accuracy of 0.86 (SD = 0.11) across 18 tasks requiring interpretation of SHAP-based explanations, demonstrating that the explanations are generally comprehensible to process analysts with domain knowledge. (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt; domain: business process management / enterprise IT)
- Perceived task difficulty averaged 2.39 out of 5 (between "easy" and "neither easy nor difficult"), with the hardest tasks involving features added by the system (not original process attributes), pointing to a domain-knowledge gap rather than an explanation design flaw. (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt; domain: BPM / enterprise IT)
- Post-Study System Usability Questionnaire (PSSUQ) scores fell within the normative range for overall satisfaction (2.83, SD = 1.24), system usefulness (2.70), and interface quality (2.82), confirming adequate usability. (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt; domain: BPM / enterprise IT)
- User Experience Questionnaire (UEQ) scores rated the system as "Good" for Efficiency, Dependability, and Stimulation, and "Above Average" for Attractiveness and Novelty; Perspicuity was slightly below average, attributed to users' limited familiarity with the host process mining tool. (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt; domain: BPM / enterprise IT)
- Users familiar with the IBM Process Mining Suite performed better on tasks involving color-coded frequency of explanations, suggesting that prior tool experience moderates comprehension. (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt; domain: BPM / enterprise IT)
- The paper cites prior literature establishing that explanations are a necessary condition for trust in predictive monitoring technology and hence adoption (Nunes & Jannach, 2017; Doshi-Velez & Kim, 2017). (source: Galanti et al._An explainable decision support system for predictive process Analytics.txt)

## Transparency Constructs

The paper operationalizes transparency through two types of SHAP-based explanations:

- **Global explanations**: Bar charts aggregating average Shapley Values across all process instances in a dataset, providing a "helicopter view" of the most influential factors driving the predictive model. This constitutes a form of [[algorithmic-transparency]] and [[process-transparency]] at the model level.
- **Local explanations**: Bar charts for individual running cases showing which attributes contribute to and by how much a specific prediction deviates from the average KPI, constituting instance-level [[explainability]] (feature attribution).

Explanations are rendered as interactive visualizations inside the IBM Process Mining Suite dashboard. The framework is model-agnostic (implemented for Catboost), addressing both remaining-time prediction (numeric KPI) and activity-occurrence prediction (Boolean KPI). The paper is notably silent on [[counterfactual-explanations]], though it cites Hsieh et al. (2021) and Huang et al. (2021) as related counterfactual approaches for the BPM field.

## Trust Constructs

Trust is not measured as a primary dependent variable with a validated scale; rather, the study treats intelligibility and usability as proxies for the conditions enabling trust. The authors adopt a theoretical position (citing Nunes & Jannach, 2017; Doshi-Velez & Kim, 2017) that explanation is a necessary precondition for trust in predictive monitoring, making trust an assumed downstream outcome of explanation quality rather than a directly tested construct. This is an indirect operationalization of [[cognitive-trust]] through comprehension and usability.

The paper also alludes to the risk of [[algorithm-aversion]] as the motivation for explainability: without explanation, process analysts would be unlikely to adopt the predictive technology.

## Relevance to Research Questions

**RQ1**: The paper provides a concrete operationalization of explainability in a BPM/enterprise IT domain using SHAP-based feature attribution at both global and local levels. It illustrates how "explanation" is decomposed into model-level transparency and instance-level attribution, contributing to the taxonomy of transparency constructs in non-clinical, organizational contexts.

**RQ2**: The user study provides evidence that well-designed explanations (SHAP bar charts integrated into a commercial dashboard) do improve user comprehension and usability ratings, which the authors treat as indicative of trust. However, the study does not test a no-explanation condition, so the causal effect of explanation on trust cannot be directly assessed. The intelligibility results support the relationship between explanation quality and user performance, which is relevant to RQ2's interest in conditional effects.

**RQ3**: User expertise moderates comprehension: process analysts with prior IBM Process Mining experience performed better on specific tasks. The study samples only domain-knowledgeable process analysts (average self-rated process mining knowledge: 3.5/5), limiting generalizability to lay users. This provides limited but suggestive evidence for RQ3.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
