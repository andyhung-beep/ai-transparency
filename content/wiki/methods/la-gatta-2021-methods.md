# La Gatta 2021 — Methods

**Summary**: A technical paper proposing PASTLE, a novel local model-agnostic XAI method, evaluated on eight benchmark datasets across four classifiers and validated in a small user study (N = 36) comparing PASTLE explanations to LIME on a feature-ranking task.

**Sources**: La Gatta et al._PASTLE pivot-aided space transformation for local explanations.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
technical paper (algorithmic development with benchmark evaluation and user study component)

## Sample
- N: 36 (user study); not applicable (benchmark evaluation)
- Population: not reported (user study participants); benchmark datasets (Bank, Titanic, Diabetes, Magic, Spambase, Digits, Breast Cancer Wisconsin, Wholesale Customer)
- Domain: cross-domain benchmark (healthcare, retail, finance, general classification); user study domain: healthcare (Breast Cancer Wisconsin) and retail (Wholesale Customer)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: explainability / interpretability (local, model-agnostic feature-importance explanation with directional guidance)
- Manipulation or measure: between-subjects comparison of two explanation methods — PASTLE (pivot-aided space transformation with directional explanation vector) vs. LIME (standard local surrogate linear model); participants in user study saw explanations for instances from two datasets and ranked features by predicted importance; technical evaluation measured adjusted-R² of local linear surrogate across four classifiers (Random Forest, SVM, MLP, XGBoost) and eight datasets, varying proximity functions and pivot-selection strategies
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (implicit, operationalized through task performance)
- Measure: trust is not formally measured via a validated scale; user study operationalizes understanding/trust implicitly through Mean Average Precision (mAP) — how well participants' feature rankings matched the model's ground-truth feature importance after viewing explanations; the paper frames improved mAP as evidence of enhanced cognitive trust
- Scale / instrument name: not applicable
- Number of items: not applicable
- Behavioural vs self-report: behavioural (task performance measure only)

## Moderators and covariates tested
- Dataset / feature interpretability: moderates explanation effectiveness — PASTLE advantage over LIME was larger for Breast Cancer dataset (less intuitive features) than Wholesale Customer dataset (more intuitive features)
- Pivot-selection strategy (clustering, random sampling, perturbation): manipulated in technical evaluation; clustering and random strategies outperformed perturbation
- Proximity function type (linear vs. nonlinear; cosine, Euclidean, Minkowski distances): manipulated in technical evaluation; linear functions and cosine distance performed best on average
- User expertise / role: not formally measured or manipulated; paper conceptually distinguishes end-users vs. expert analysts as audiences but does not test this empirically (relevant to RQ3 as conceptual contribution)

## Statistical approach
- Primary analysis method: F-ratio analysis (user study mAP comparisons); adjusted-R² comparison across classifiers and datasets (technical evaluation)
- Software: not reported
- Key model fit or effect size reported: PASTLE mAP vs. LIME — Wholesale: 0.301 vs. 0.201; Breast Cancer: 0.357 vs. 0.113 (Breast Cancer F-ratio significant); adjusted-R² improvements documented across all eight datasets

## Author-noted limitations
- Small user study sample (N = 36); limited statistical power for some comparisons
- User study used a ranking task rather than a real-world decision task; ecological validity limited
- Trust was not formally measured; mAP as a proxy for understanding/trust is indirect
- Pivot selection strategies require further investigation; perturbation-based pivots failed on sparse text datasets

## Related pages
- [[la-gatta-pastle-local-explanations]]
- [[explainability]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[cognitive-trust]]
- [[user-expertise]]
