# von Zahn 2025 — Methods

**Summary**: Two incentivised between-subjects experiments with domain experts (Study 1: N = 149 real estate agents; Study 2: N = 152 finance/insurance professionals) demonstrating that global SHAP explanations improve metacognitive calibration and increase delegation to AI, partially mediated by reduced overconfidence.

**Sources**: von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects; two independent studies)

## Sample
- N: Study 1: 149; Study 2: 200 recruited, 152 effective (after exclusions)
- Population: domain experts — Study 1: German real estate agents; Study 2: finance and insurance professionals
- Domain: Study 1: real estate pricing; Study 2: financial services / peer-to-peer lending
- Country / region: Germany (both studies)
- Recruitment method: not reported (incentivised participation with monetary rewards tied to accuracy)

## Transparency operationalization
- Type: algorithmic transparency / process transparency (global explanation via SHAP)
- Manipulation or measure: Two between-subjects conditions: (1) XAI condition — access to SHAP global partial-dependence plots showing the average relationship between each input feature and the AI's predictions across the dataset; Study 2 also included local SHAP values for three example cases; (2) Black-box condition — AI predictions available but no explanation of how they were generated. Participants could delegate each prediction task to the AI.
- Scale / instrument name: not applicable (between-subjects manipulation using SHAP visualizations)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report) and behavioural (delegation/reliance)
- Measure: (1) Cognitive trust measured using Komiak and Benbasat (2006) scale (+0.93 points on 7-point scale, p < 0.01); (2) Behavioural trust operationalised as delegation frequency (proportion of prediction tasks delegated to AI) and delegation effectiveness (mean absolute prediction error for retained vs. delegated tasks)
- Scale / instrument name: Komiak and Benbasat (2006) cognitive trust scale
- Number of items: not reported
- Behavioural vs self-report: both — cognitive trust scale (self-report) plus behavioural delegation decisions

## Moderators and covariates tested
- Perceived logic alignment: participants who perceived misalignment between their own prediction logic and the AI's logic showed greater metacognitive calibration adjustment (reduced confidence); participants perceiving high alignment showed no meaningful adjustment — moderates XAI effect on metacognition (relevant to RQ2)
- Domain expertise (within expert samples): Study 1 notes that more experienced real estate agents may respond differently but does not formally test experience as a moderator (relevant to RQ3)
- Metacognitive calibration (overconfidence): measured as a mediating variable; XAI reduced overconfidence by 32.3% (Study 1) and 64.4% (Study 2)
- Metacognitive resolution: confidence discriminability between easy and hard tasks; measured and improved by XAI in Study 2

## Statistical approach
- Primary analysis method: causal mediation analysis (for metacognitive calibration and cognitive trust as mediators of delegation outcomes); t-tests and proportional difference tests for between-group comparisons; mean absolute error comparisons for delegation effectiveness
- Software: not reported
- Key model fit or effect size reported: mediation proportions reported (23% Study 1; 104% Study 2 of XAI delegation effect mediated by metacognitive calibration); p-values for group comparisons (e.g., overconfidence reduction p < 0.01; delegation frequency increase p < 0.01)

## Author-noted limitations
- Expert samples (real estate, finance) limit generalisability to lay users or other domains
- Global explanations only; local explanation effects not isolated in Study 1
- No intermediary feedback provided during task; learning effects over sessions not fully disentangled
- Risk of XAI-induced underconfidence identified (some experts over-delegated) but not formally modelled
- Human-AI teams did not achieve full complementarity even with XAI; ideal-delegation performance substantially exceeded actual performance
- Study 2 N reduced from 200 to 152 after exclusions; exclusion criteria and attrition not fully detailed

## Related pages
- [[von-zahn-xai-metacognition]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
