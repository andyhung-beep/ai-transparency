# Knapic et al. (2021) — Explainable AI for Human Decision Support in the Medical Domain

**Source file**: [Original article](../../raw/Knapic et al._Explainable_Artificial_Intelli.pdf)

**Summary**: Three between-subjects user studies (N=60 total) comparing LIME, SHAP, and CIU visual explanations for a CNN-based gastric bleeding detection system, finding null effects on decision accuracy for all three explanation types but significant advantages for CIU on user satisfaction and error detection.

**Sources**: `Knapic et al._Explainable_Artificial_Intelli.pdf`

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Reference

Knapic, S., Malhi, A., Saluja, R., & Frömling, K. (2021). Explainable Artificial Intelligence for Human Decision Support System in the Medical Domain. *Machine Learning and Knowledge Extraction*, 3, 740–770.

---

## Study Overview

- **Domain**: Healthcare / medical imaging (video capsule endoscopy; gastric bleeding detection)
- **Task**: Participants classified endoscopy images as bleeding or non-bleeding, with and without visual XAI explanations from a CNN model achieving 98.58% validation accuracy
- **Design**: Between-subjects; three groups (N=20 each): LIME, SHAP, CIU explanation conditions, each also completed a no-explanation baseline phase
- **Sample**: 60 university students and staff with STEM backgrounds; no medical expertise; predominantly male; ages 20s–30s; ~50% had prior XAI knowledge
- **XAI methods compared**: LIME, SHAP (Kernel SHAP), and CIU (Contextual Importance and Utility)
- **Outcome measures**: Decision accuracy (correct classifications), explanation satisfaction (Likert 0–5), self-reported understanding, time on task, and error detection (can users identify incorrect explanations?)

---

## The CIU Method

CIU (Contextual Importance and Utility) is the primary novel contribution of this paper. Unlike LIME and SHAP, CIU does not use an intermediate surrogate model or make linearity assumptions. Instead, it computes two values for each feature:

- **Contextual Importance (CI)**: the degree to which the feature's value range influences the output in the current context
- **Contextual Utility (CU)**: how favorable or unfavorable the current feature value is for the predicted class, relative to its importance

This contextual, non-surrogate approach produces explanations that are more stable (no sampling randomness as in LIME), faster to compute, and — in this study — more satisfying and comprehensible to lay users.

---

## Key Findings

### Decision Accuracy: Null Effects Across All Methods

None of the three XAI conditions significantly improved decision accuracy compared to the no-explanation baseline (domain: healthcare; source: `Knapic et al._Explainable_Artificial_Intelli.pdf`):

| Condition | p-value (vs. no explanation) | Direction |
|---|---|---|
| LIME | 0.738 | Slight improvement with explanation |
| SHAP | 0.464 | Worse with explanation than without |
| CIU | 0.158 | Improvement with explanation (highest magnitude) |

SHAP is the only condition where users made more correct decisions *without* explanations than with them — a near-negative effect consistent with information overload from SHAP's more complex visual output.

### CIU Superior on Secondary Outcomes

- **Satisfaction**: CIU significantly higher than LIME (p<0.001) and directionally higher than SHAP (p=0.144, ns)
- **Error detection**: CIU users significantly better at identifying incorrect explanations than LIME users (p=0.009) and SHAP users (p=0.037)
- **Speed**: CIU users completed the study in less time than SHAP users (p=0.016); comparable to LIME

### SHAP Complexity and Confusion

SHAP users took significantly longer to complete the study (mean 23.18 min) than both LIME (15.57 min, p=0.011) and CIU users (16.30 min, p=0.016). The additional complexity of SHAP's two-color bidirectional visualization appears to increase cognitive load without commensurate accuracy gains.

### Interesting Correlation

For LIME users, *lower satisfaction* with explanations correlated with *better decision accuracy* (p=0.019). Users who recognized LIME's limitations may have engaged more critically with the images rather than relying on the explanation.

---

## Conceptual Contributions

The paper articulates a three-way distinction between related terms:

- **Transparency**: a model is understandable on its own (applies to simple models like linear regression)
- **Interpretability**: outputs can be described or given meaning by humans; does not imply internal logic is accessible
- **Explainability**: the model's internal logic and dynamics are accessible; does not automatically follow from interpretability

This distinction maps closely to the [[algorithmic-transparency]] taxonomy but is more precise than most corpus sources.

---

## Limitations

1. Lay (non-medical) users only — the authors explicitly acknowledge this is the main limitation; findings may not generalize to physician users
2. Small samples (N=20 per group) — insufficient power for the between-group comparisons that approach but fail to reach significance (e.g., CIU vs. LIME accuracy, p=0.120)
3. Single medical data set (Red Lesion Endoscopy); generalizability across imaging modalities untested
4. CIU still in early development (2021); less mature tooling than LIME/SHAP

---

## Contributions to Research Questions

**RQ1**: Introduces CIU as a distinct post-hoc XAI method with a non-surrogate, contextual approach; provides a three-way transparency/interpretability/explainability conceptual distinction.

**RQ2**: Adds three null effects (LIME, SHAP, CIU vs. no explanation on decision accuracy) to the corpus; demonstrates near-negative effect for SHAP under lay users; shows that satisfaction and error detection can differ from accuracy even when accuracy effects are null.

**RQ3**: Reinforces the systematic gap identified in rq3-user-roles — uses a non-expert STEM sample in a medical domain; authors acknowledge that application-grounded evaluation with domain experts is needed.

---

## Related pages

- [[explainability]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
