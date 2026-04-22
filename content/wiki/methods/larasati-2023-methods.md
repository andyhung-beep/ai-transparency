# Larasati 2023 — Methods

**Summary**: A participatory, stage-based mixed-methods study combining expert and lay co-design (N = 3 AI/ML experts, 3 junior doctors, 12 lay users) with two online surveys (First: n = 55 within-subjects; Second: n = 88 with control group) and 7 semi-structured interviews to evaluate 14 explanation design guidelines and the CARE breast cancer self-assessment prototype on non-expert users' trust.

**Sources**: Larasati et al._Meaningful explanation effect on user_s trust in an AI medical system.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (participatory design + survey experiments + qualitative interviews)

## Sample
- N: 18 (design phase: 3 AI/ML experts, 3 junior doctors, 12 lay users); 55 (First Survey, within-subjects); 88 (Second Survey, with control group); 7 (semi-structured interviews)
- Population: AI/ML practitioners, junior medical doctors, and lay users (stratified by dispositional trust: sceptics, open-minded, enthusiasts) in design phase; general public / non-expert users in evaluation surveys (recruited via Mechanical Turk)
- Domain: healthcare (breast cancer thermography self-assessment)
- Country / region: not reported
- Recruitment method: MTurk (survey phases); purposive sampling for design phase and interviews

## Transparency operationalization
- Type: multi-component meaningful explanation (natural language, outcome transparency, process transparency, uncertainty visualization, counterfactual/contrastive elements)
- Manipulation or measure: within-subjects (First Survey) — participants interacted with CARE prototype before/after trust measurement; between-subjects (Second Survey) — explanation group (CARE prototype) vs. no-explanation control group; CARE prototype delivers 14 Explanation Design Guidelines (EDGs) covering: disease information, treatment, next steps, system input, input comparison visualization, system process, system output (AI prediction), system information, empathy, and more
- Scale / instrument name: not applicable (prototype interaction as manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: multi-dimensional (cognitive, affective, behavioural)
- Measure: multi-item Human-AI Trust in AI Healthcare scale (derived from Jian et al., adapted) measuring: perceived understandability, perceived reliability, perceived technical competence, faith (affective), personal attachment (affective), helpfulness, institution credibility, user autonomy; also single global trust item; System Usability Scale (SUS)
- Scale / instrument name: Human-AI Trust in AI Healthcare scale (Jian et al. derivative, adapted); System Usability Scale (SUS)
- Number of items: not reported (multi-item scale); 1 (global trust item); 10 (SUS)
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Dispositional trust (trust propensity): controlled by stratifying lay design participants into sceptics, open-minded, and enthusiasts; not formally tested as moderator in evaluation phase
- Expert vs. lay user role: core design variable — Expert Explanation Models (from AI/ML and medical experts) vs. User Explanation Model (from lay users) contrasted to reveal expertise-dependent explanation preferences (highly relevant to RQ3)
- Expert type (AI/ML expert vs. medical expert): compared within expert group — medical experts prioritized disease information and empathy; AI experts prioritized process transparency; AI experts doubted non-experts' interest in algorithmic details
- System Usability Scale: measured (SUS = 81.34, excellent range); not used as moderator

## Statistical approach
- Primary analysis method: Wilcoxon signed-rank test (within-subjects pre/post trust differences, First Survey); Mann-Whitney U test (between-groups, Second Survey); Bonferroni correction applied; descriptive statistics (median ratings for EDG relevance)
- Software: not reported
- Key model fit or effect size reported: perceived technical competence p = 0.001 (survived Bonferroni correction, threshold p = 0.00148); perceived reliability p = 0.009; personal attachment p = 0.015; helpfulness p = 0.029; SUS = 81.34; EDG System Output highest relevance mean 4.67; EDG System Information lowest mean 4.11

## Author-noted limitations
- MTurk convenience sample may not represent the full range of non-expert users in healthcare contexts
- Single exposure to prototype; longitudinal effects of explanation on trust not assessed
- Bonferroni correction is conservative; some effects may be real but underpowered
- Self-reported trust only; no behavioural reliance measures
- Generalizability beyond breast cancer self-assessment domain is not established
- Small design-phase samples (3 AI experts, 3 doctors, 12 lay users) limit representativeness of Explanation Models

## Related pages
- [[larasati-meaningful-explanations-medical-ai]]
- [[explainability]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[trust-calibration]]
- [[user-expertise]]
