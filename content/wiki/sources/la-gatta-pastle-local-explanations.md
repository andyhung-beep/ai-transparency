# PASTLE: Pivot-Aided Space Transformation for Local Explanations

**Source file**: [Original article](../../raw/La Gatta et al._PASTLE pivot-aided space transformation for local explanations.pdf)

**Summary**: PASTLE is a novel model-agnostic, local XAI technique that enriches standard feature-importance explanations with directional information about how changing feature values would shift a black-box model's prediction, achieved by transforming the instance space using representative "pivot" points and fitting a linear surrogate on the transformed space.

**Sources**: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

La Gatta, Moscato, Postiglione, and Sperlì (2021), published in *Pattern Recognition Letters*, propose PASTLE (Pivot-Aided Space Transformation for Local Explanations). Like LIME and SHAP, PASTLE is a local, model-agnostic explanation method — it explains any black-box model's prediction for a specific instance without assuming access to model internals. The key innovation over standard feature-importance approaches is the introduction of a pivot-based space transformation.

**Pivots** are representative training instances (selected by clustering, random sampling, or perturbation) that characterise distinct regions of the input space where the model behaves differently. PASTLE projects each instance into a new space whose dimensions are proximity values to the pivots, then fits a transparent linear model on this transformed space. The weights of that linear model indicate how the proximity to each pivot influences the prediction — framing explanation as a sum of attractive and repulsive force vectors.

The resulting "explanation vector" points towards the region most supportive of the prediction, while its opposite direction indicates how features must be changed to reverse the prediction. This enriches the explanation with what-if / counterfactual-flavoured directional guidance without requiring fully enumerated counterfactual examples.

Experiments were conducted across eight datasets (Bank, Titanic, Diabetes, Magic, Spambase, Digits, Breast Cancer Wisconsin, Wholesale Customer) and four classifiers (Random Forest, SVM, MLP, XGBoost). A user study with 36 participants compared PASTLE explanations to LIME explanations on a ranking task.

## Key Findings

- The pivot-aided space transformation consistently improved or maintained the adjusted-R² of the local linear surrogate model compared to fitting in the original space, across all classifiers and datasets (domain: general/cross-domain benchmark). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)
- Linear proximity functions (those with linear dependence on distance, e.g., P3 and P5) outperformed nonlinear proximity functions; cosine distance performed best on average, but Euclidean and Minkowski distances gave best peak results (domain: general/benchmark). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)
- Clustering and random pivot-selection strategies both significantly outperformed perturbation-based strategies in most datasets; perturbation failed on text-frequency datasets (Spambase) because it only modified existing word frequencies rather than introducing new ones (domain: general/benchmark). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)
- In the user study, PASTLE outperformed LIME in Mean Average Precision (mAP) on both datasets (Wholesale: 0.301 vs 0.201; Breast Cancer: 0.357 vs 0.113), with statistical significance for the Breast Cancer dataset via F-ratio analysis (domain: healthcare/retail). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)
- The advantage was larger for the Breast Cancer dataset, where features are less intuitively interpretable — consistent with the claim that directional guidance from PASTLE helps when feature semantics are less obvious (domain: healthcare). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)
- The paper invokes psychological research showing that counterfactual reasoning ("what would have to change?") is a natural way humans process decisions and build acceptance/trust (Byrne, 2016). (source: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.txt)

## Transparency Constructs

PASTLE contributes primarily to **explainability / interpretability** — specifically local, instance-level explanation. It extends feature-importance explanations (like those produced by LIME or SHAP) with:

- **Counterfactual-flavoured directional guidance**: the explanation vector indicates which direction in feature space to move to increase or decrease the probability of the predicted class. This is a hybrid between [[example-based-explanations]] (pivots as representative instances) and [[counterfactual-explanations]] (directional what-if guidance).
- **Traceability**: by exposing the influence of specific training instances (pivots) on a prediction, PASTLE adds a layer of traceability — connecting predictions to known training data regions. See [[traceability]].

The paper distinguishes between audiences:
- End-users benefit from understanding why a decision was made and how to change it.
- Developers/expert analysts can use pivot-influence values to audit model biases, which relates to [[causability]] (understanding the cause of a prediction in a user-appropriate way).

See [[explainability]], [[counterfactual-explanations]], [[example-based-explanations]].

## Trust Constructs

The paper's stated motivation is to "enhance human trust towards AI decisions" (abstract). Trust is not formally measured as a multi-dimensional construct but is operationalised implicitly through user-study performance:

- Better ranking accuracy after seeing PASTLE explanations (vs. LIME explanations) is taken as evidence of enhanced **cognitive trust** — users better understood the model's decision logic and could predict its behaviour on unseen instances.
- The paper cites DARPA XAI goals explicitly: enabling users to "understand, appropriately trust, and effectively manage" AI partners (Gunning & Aha, 2019).
- The claim that counterfactual/what-if thinking promotes acceptance of decisions links to **affective trust** dimensions (decision acceptance and psychological closure).

See [[cognitive-trust]], [[trust-calibration]].

## Relevance to Research Questions

**RQ1**: PASTLE provides a technical operationalisation of local explainability that extends beyond feature-attribution scores by adding directional guidance. The paper's motivation connects explainability to trust, and its user study implicitly operationalises trust through task performance rather than self-report. The distinction between end-user and expert-analyst audiences also maps onto dual operationalisations of explainability (lay understanding vs. technical auditing). See [[rq1-conceptualizations]].

**RQ2**: The user study provides evidence that richer local explanations (those including directional guidance) improve users' ability to model the system's behaviour compared to standard feature-importance explanations. This supports a positive transparency–understanding–trust pathway, at least for cognitively demanding domains (Breast Cancer features > Wholesale features). The lack of effect on the Wholesale dataset suggests conditional effects moderated by feature interpretability. See [[rq2-relationships]].

**RQ3**: The paper explicitly acknowledges different user audiences (end-users vs. expert analysts) and tailors explanation design to each. Expert analysts can use controlled pivot selection and detailed pivot-influence analysis; end-users receive the simplified directional summary. This distinction is a conceptual rather than empirically tested moderation of transparency effects by user role. See [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
