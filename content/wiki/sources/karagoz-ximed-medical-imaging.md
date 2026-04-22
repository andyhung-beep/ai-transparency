# XIMED: A Dual-Loop Evaluation Framework Integrating Predictive Model and Human-Centered Approaches for Explainable AI in Medical Imaging

**Source file**: [Original article](../../raw/Karagoz_XIMED.pdf)

**Summary**: Proposes and implements XIMED, a structured evaluation framework for XAI methods in medical image classification that integrates both predictive model-centered (faithfulness) and human-centered (trust, confidence, agreement) assessments, applied to LIME and SHAP explanations for chest X-ray diagnosis with 97 medical experts.

**Sources**: Karagoz_XIMED.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Karagoz, Ozcelebi, and Meratnia (2025) address a major gap in the XAI evaluation literature: most studies either evaluate explanations purely for technical fidelity to the model or purely for human usability, but rarely both together. Their review of 51 chest X-ray XAI papers found that 34 included no evaluation of explanations at all, and only 4 applied evaluation methods from both perspectives.

**XIMED** (XAI for MEDical imaging) is a dual-loop evaluation framework with two major components:

1. **Predictive model-centered evaluation** — three sanity checks:
   - *Model Parameter Randomization Check (MPRC)*: randomizing individual DenseNet121 layers to test if explanations reflect internal model structure.
   - *Incremental Deletion Check (IDC)*: sequentially masking top-10 features identified by each XAI method to test if explanations correctly identify input features driving predictions.
   - *Label Randomization Check (LRC)*: re-training with randomized labels to test if explanations discriminate between legitimate and random decision mappings.

2. **Human-centered evaluation** — a randomized controlled trial with 97 medical experts (medical students, general practitioners, specialty trainees, and specialists) assigned to LIME explanations, SHAP explanations, or a no-XAI control group. Outcomes: trust (pre/post), confidence in diagnosis (post), indicative agreement (AGREEind), contra-indicative agreement (AGREEcont), and diagnosis change.

The predictive model used was DenseNet121 pre-trained on the NIH Chest X-Ray dataset (112,120 images, 14 disease classes; mean AUC=0.80121).

## Key Findings

**Predictive model-centered findings:**
- Both LIME and SHAP are sensitive to internal model changes (MPRC), confirming both methods reflect the DenseNet121 architecture's decision-making. SHAP is more sensitive to changes in the last layers; LIME shows higher sensitivity to the latest (dense/softmax) layer. [Domain: healthcare / medical imaging]
- Both methods identify critical features correctly in the IDC: removing the top feature immediately drops the correct label's predicted probability, confirming they pinpoint decision-relevant regions. [Domain: healthcare / medical imaging]
- SHAP shows more structured sensitivity to label randomization (LRC), with stronger feature polarity inversions after randomization; LIME shows higher response to label changes on basic pixel-level error metrics. [Domain: healthcare / medical imaging]
- LIME's linear approximation captures less of the complexity from deep-layer changes; SHAP's Shapley-value mechanism provides finer attribution but at higher computational cost. [Domain: healthcare / medical imaging]

**Human-centered findings (97 medical experts, RCT):**
- Neither LIME nor SHAP significantly changed post-confidence levels compared to the control group (ANOVA F=0.088, p=0.916). Most participants in all groups reported no change in diagnostic confidence after seeing AI explanations. [Domain: healthcare]
- Trust levels (TRUSTpost) were not significantly different across LIME, SHAP, and control groups. Initial trust (TRUSTpre) was the strongest predictor of post-explanation trust. [Domain: healthcare]
- SHAP explanations were significantly associated with higher likelihood of diagnosis change (estimate=0.2396, p=0.033) compared to control; LIME was not significantly different from control. [Domain: healthcare]
- Both LIME and SHAP had significant negative effects on contra-indicative agreement (AGREEcont), more pronounced for SHAP (c=−2.08) than LIME (c=−1.66). Explanations made participants less likely to agree with the AI's contra-indicative (disease-ruling-out) reasoning. [Domain: healthcare]
- Case-based analysis revealed that explanations reinforce trust and agreement when participants' initial diagnoses were correct; SHAP effectively facilitated correct diagnostic changes in cases where participants had initially incorrect diagnoses (Case-4 pattern). [Domain: healthcare]
- The correlation between trust and confidence was notably negative for the SHAP group (r=−0.24), contrasting with positive correlations in LIME (0.38) and control (0.43) groups — tentatively explained by SHAP-driven diagnosis changes creating diagnostic uncertainty. [Domain: healthcare]
- No single XAI method was universally superior; LIME showed closer indicative agreement with expert diagnostic reasoning, while SHAP was more effective at driving correct diagnosis changes. [Domain: healthcare]

## Transparency Constructs

XIMED primarily concerns **post hoc, model-agnostic explainability** via [[explainability]] methods. LIME generates local surrogate linear models (super-pixel-level explanations), while SHAP assigns Shapley values to individual pixels to attribute each feature's contribution to the prediction. Both produce visual overlays on chest X-rays.

The framework's predictive model-centered component assesses **faithfulness** — a dimension of [[algorithmic-transparency]] concerned with whether the explanation accurately reflects the internal decision logic of the model. The human-centered component assesses **usability and trust impact** of the transparency.

A key conceptual contribution is distinguishing **indicative** (supportive) from **contra-indicative** (ruling-out) explanation regions, mapping XAI outputs to clinically meaningful diagnostic reasoning rather than treating explanations as monolithic.

## Trust Constructs

The study measures trust via pre/post Likert ratings, making it primarily a measure of **cognitive trust** — belief in the AI system's diagnostic ability. It also measures **behavioural trust** indirectly through diagnosis change (willingness to revise one's own diagnosis based on the AI's reasoning). The main null finding for trust change suggests that a single exposure to an AI explanation is insufficient to shift cognitive trust in a clinical context, even when it may change specific diagnostic decisions. See [[cognitive-trust]] and [[behavioural-trust]].

The paper explicitly notes the limitation of self-reported trust measures and argues for complementing them with objective performance metrics (e.g., diagnosis correctness, diagnosis change rate).

## Relevance to Research Questions

**RQ1**: XIMED operationalizes transparency through two evaluation lenses: technical faithfulness (predictive model-centered) and human usability (human-centered trust, confidence, agreement). It contributes a benchmark framework for how XAI should be evaluated in healthcare, going beyond anecdotal evidence or visual inspection. The distinction between indicative and contra-indicative agreement is a novel operationalization of explanation alignment with clinical reasoning. See [[rq1-conceptualizations]].

**RQ2**: The key finding is that XAI explanations (LIME/SHAP) did not significantly change overall trust or diagnostic confidence compared to a no-explanation control, despite influencing agreement and diagnosis changes. This is a conditional null finding for trust: the explanations have some impact (on agreement, diagnosis changes) but not on self-reported trust within a single exposure. SHAP's ability to drive correct diagnosis changes (when initially wrong) represents a positive behavioural trust outcome even in the absence of self-reported trust change. See [[rq2-relationships]].

**RQ3**: The study includes diverse medical expertise levels (students through specialists) but analyzes them primarily as a single group. The paper does not report between-expertise-level comparisons on trust or agreement outcomes, representing a gap. The case-based moderation by diagnosis correctness does partially operationalize user competence as a moderator. See [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[domain-context]]
- [[user-expertise]]
- [[rq2-relationships]]
