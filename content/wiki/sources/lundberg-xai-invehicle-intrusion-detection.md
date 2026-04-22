# Experimental Analysis of Trustworthy In-Vehicle Intrusion Detection System Using eXplainable Artificial Intelligence (XAI)

**Source file**: [Original article](../../raw/Lundberg et al._Experimental_Analysis_of_Trustworthy_In-Vehicle_Intrusion_Detection_System_Using_eXplainable_Artificial_Intelligence_XAI.pdf)

**Summary**: This paper proposes and evaluates VisExp, a SHAP-based visual explanation for a deep neural network intrusion detection system (IV-IDS) for automotive CAN bus data, finding that domain experts' trust in the system is significantly increased by the visual explanation compared to a rule-based textual explanation or raw model output.

**Sources**: Lundberg et al._Experimental_Analysis_of_Trustworthy_In-Vehicle_Intrusion_Detection_System_Using_eXplainable_Artificial_Intelligence_XAI.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Lundberg et al. (2022) address the problem of low interpretability and associated user distrust in AI-based in-vehicle intrusion detection systems (IV-IDS) operating on Controller Area Network (CAN) bus traffic. Anomaly-based IDSs using deep learning produce high false-alarm rates and offer little insight into why an alarm was generated, which leads to uncertainty and distrust among system operators.

The study trains a Deep Neural Network (DNN) on the "Survival" CAN bus dataset (1,735,840 instances, 183,314 attacks), achieving an accuracy of 0.9973 and F1-score of 0.9868 in 10-fold cross-validation. The authors then develop "VisExp," a pseudo-global visualization-based explanation built on SHAP (SHapley Additive exPlanations) using KernelSHAP. VisExp displays feature-level SHAP values as dual swarm plots with violin overlays for normal versus attack traffic, enabling experts to understand model behavior at both local and aggregate levels.

VisExp is compared against a rule-based textual explanation in a quantitative survey of 30 domain experts (AI, cybersecurity, wireless/IoT, automotive) recruited from Mid Sweden University and RISE Research Institutes of Sweden.

The domain is **automotive cybersecurity**.

## Key Findings

- Primary experts (AI, automotive, cybersecurity specialists) trust the IV-IDS significantly more when shown VisExp (mean = 2.786 on 0–4 Likert scale, "Agree") than when shown raw model input/output (mean = 2.000, "Undecided"); mean difference = 0.786, t(26) = 6.904, p < 0.001. (Domain: automotive cybersecurity)
- The rule-based explanation also raised trust over no explanation (mean diff = 0.357, p = 0.019), but less so than VisExp. VisExp outperformed the rule-based explanation for primary experts (mean diff = 0.429, t(26) = 3.122, p = 0.0081). (Domain: automotive cybersecurity)
- 72.4% of all participants rated VisExp as more trustworthy and understandable than the rule-based explanation; 77% said VisExp enhanced their understanding most; 79.3% agreed VisExp was more revealing and descriptive. (Domain: automotive cybersecurity)
- Secondary experts (wireless/IoT, data analysis, AI novices) showed smaller differences between the two explanation types, and AI novices did not show the same preference for VisExp over the rule-based explanation. This suggests a moderating effect of domain expertise on explanation effectiveness. (Domain: automotive cybersecurity)
- A positive correlation between understandability and trustworthiness of an explanation is indicated by the alignment of responses to Questions 6 (understanding) and 7 (trustworthiness). (Domain: automotive cybersecurity)
- The study notes that trust in the IV-IDS is already moderately high in a naturalistic in-vehicle context (65.5% would trust an in-vehicle alert), but trust in the AI system in general is lower (51.7%) and more contested (31% in disagreement). (Domain: automotive cybersecurity)

## Transparency Constructs

The paper operationalizes transparency through **explainability** and **interpretability** of AI model behavior. The primary explanation artifact, VisExp, is a **visualization-based explanation** (see [[explainability]]) that uses SHAP feature importance to produce a pseudo-global view of model decision logic — a form of [[process-transparency]] in that it reveals how input features drive attack/normal classifications. A rule-based textual alternative represents a simpler, more direct [[natural-language-explanations]] style of process transparency.

The paper distinguishes:
- **Local explanations**: per-instance SHAP values (how the model classified a specific CAN frame)
- **Pseudo-global explanations**: aggregated SHAP values across training instances (VisExp)
- **Post-hoc explanations**: applied after model training without modifying the model (SHAP/KernelSHAP)

Trustworthiness is treated as contingent on explainability — sufficiently transparent systems reduce the need for external oversight mechanisms.

## Trust Constructs

Trust is measured via Likert-scale questionnaire items asking whether participants would trust the IV-IDS when shown each explanation type. This aligns primarily with **cognitive trust** (belief in competence and reliability of the system; see [[cognitive-trust]]) and **behavioural trust** (willingness to rely on the system's alerts; see [[behavioural-trust]]). The paper also briefly invokes **institutional trust** in the broader automotive manufacturer context ([[institutional-trust]]).

The study uses the concept of **trustworthiness** as a system property that explanations can either support or undermine, and the concept of **appropriate reliance** is implicit in the argument that trust should be established through understanding rather than opacity ([[appropriate-reliance]]).

## Relevance to Research Questions

**RQ1**: The paper operationalizes transparency as explainability of AI decision-making (SHAP-based feature importance visualization) and measures trust through expert Likert-scale ratings of the system. It defines trustworthiness as a property achieved when explanations are provided and found understandable, connecting it to reduced need for oversight mechanisms. Contributes to understanding how transparency is defined in high-stakes cybersecurity contexts.

**RQ2**: Demonstrates a positive linear relationship between explanation quality/richness and expert trust in an AI-based intrusion detection system. Visual explanations increase trust significantly more than rule-based textual explanations or no explanation (p < 0.001). Results support the general hypothesis that providing explanations increases trust, with the strength of the effect varying by explanation type. One of relatively few studies providing quantitative evidence in the automotive cybersecurity domain.

**RQ3**: Reveals that user expertise moderates the effectiveness of explanation type. Primary experts (AI, cybersecurity, automotive specialists) benefit more from the rich visualization (VisExp) than secondary experts and AI novices. The rule-based explanation shows less differentiation across expertise groups. This suggests explanations must be matched to user expertise levels — complex visualizations may not benefit non-expert users.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
