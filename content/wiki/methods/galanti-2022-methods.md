# Galanti 2022 — Methods

**Summary**: A user study (N = 20 process analysts) evaluating a SHAP-based explainable predictive process analytics framework integrated into the IBM Process Mining Suite, assessing intelligibility, usability, and user experience across 18 tasks.

**Sources**: Galanti et al._An explainable decision support system for predictive process Analytics.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
technical paper with user study evaluation (single-condition, task-based evaluation; no control/comparison condition)

## Sample
- N: 20
- Population: domain professionals (process analysts with business process management knowledge)
- Domain: business process management / enterprise IT
- Country / region: not reported
- Recruitment method: not reported (domain professionals recruited through professional contacts implied)

## Transparency operationalization
- Type: algorithmic transparency and explainability — SHAP-based global and local explanations
- Manipulation or measure: No between-group transparency manipulation; all participants used the same SHAP-based explanation system. Two types of explanation provided: (1) Global explanations — bar charts aggregating average Shapley Values across all process instances in a dataset, providing model-level transparency; (2) Local explanations — bar charts for individual running cases showing which attributes contribute to and by how much a specific prediction deviates from the average KPI. Participants completed 18 tasks requiring interpretation of these explanations within the IBM Process Mining Suite dashboard.
- Scale / instrument name: not applicable (single-condition evaluation; no manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: not directly measured as a primary construct
- Measure: Trust not measured with a validated scale; intelligibility (task accuracy, perceived difficulty) and usability (PSSUQ) treated as proxies for conditions enabling trust. Theoretical position adopted from Nunes & Jannach (2017) and Doshi-Velez & Kim (2017) that explanation is a necessary precondition for trust — trust treated as an assumed downstream outcome rather than directly assessed.
- Scale / instrument name: not applicable
- Number of items: not applicable
- Behavioural vs self-report: not applicable

## Moderators and covariates tested
- Prior experience with IBM Process Mining Suite: measured; users familiar with the tool performed better on tasks involving color-coded frequency explanations — relevant to RQ3 as user expertise moderator
- Self-rated process mining knowledge: measured (average self-rating = 3.5/5); used as sample characteristic; not formally tested as moderator

## Statistical approach
- Primary analysis method: descriptive statistics (mean task accuracy, mean perceived difficulty, mean usability scores); Post-Study System Usability Questionnaire (PSSUQ) normative comparisons; User Experience Questionnaire (UEQ) scoring against benchmark data
- Software: not reported
- Key model fit or effect size reported: mean task accuracy = 0.86 (SD = 0.11); mean perceived difficulty = 2.39/5; PSSUQ overall satisfaction = 2.83 (SD = 1.24); UEQ ratings: "Good" for Efficiency, Dependability, Stimulation; "Above Average" for Attractiveness and Novelty; Perspicuity slightly below average

## Author-noted limitations
- No control condition (no-explanation baseline); causal effect of explanation on comprehension or trust cannot be directly established
- Small sample (N = 20) limits statistical power
- Participants are domain-knowledgeable process analysts; findings may not generalise to lay users or managers without BPM background
- Hardest tasks involved features added by the system rather than original process attributes, revealing domain-knowledge gaps not addressable by explanation design alone
- Perspicuity below average attributed to limited familiarity with the IBM Process Mining host tool, not the explanation framework itself
- Study is a preprint (arXiv); not peer-reviewed at time of analysis

## Related pages
- [[galanti-explainable-process-analytics]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
