# Panigutti et al. 2023 — Methods

**Summary**: An iterative co-design study presenting Doctor XAI — an ontology-aware local rule-based explainer for clinical decision support — validated in a within-subject online experiment (N = 41 healthcare providers) measuring implicit trust (Weight of Advice), explicit trust, and behavioural intention, followed by qualitative interface redesign.

**Sources**: Panigutti et al._Co-design of human-centered, explainable AI for clinical decision.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (within-subject experiment with quantitative trust measures and qualitative design iteration)

## Sample
- N: 41
- Population: healthcare professionals — doctors, nurses, and paramedics
- Domain: healthcare / clinical decision support (acute myocardial infarction risk prediction)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: explainability — local, rule-based, natural language explanations from a domain-specific XAI method (Doctor XAI)
- Manipulation or measure: within-subject Judge-Advisor System (JAS) design; each participant provided estimates for multiple patients under two conditions: (1) AI suggestion only (no explanation); (2) AI suggestion plus explanation — Doctor XAI produces local, rule-based, natural language explanations extracted from a multi-label decision tree trained on a synthetic neighbourhood of the patient instance, using ICD-9 ontology-linked sequential patient data; participants saw both conditions (counterbalanced); the initial interface displayed the full ICD-code history with colour-coded relevance marks; a redesigned progressive-disclosure interface was developed after qualitative feedback (natural language first → highlighted diagnoses → full ICD-coded timeline)
- Scale / instrument name: not applicable (experimental manipulation); explanation quality measured post-hoc via satisfaction/quality scale
- Number of items: not applicable for manipulation; explanation quality scale item count not reported

## Trust operationalization
- Type: implicit cognitive (Weight of Advice), explicit cognitive, and behavioural intention
- Measure: (1) Weight of Advice (WOA) — behavioural proxy computed as the degree to which participants shifted their risk estimate toward the AI's prediction; primary implicit trust measure; (2) explicit trust — 5-item questionnaire assessing reliability, predictability, and efficiency of the AI system; (3) behavioural intention — intention to use the system (UTAUT/TAM constructs); (4) confidence — self-reported confidence in estimates; explanation quality satisfaction scale also administered
- Scale / instrument name: Weight of Advice (JAS methodology); custom explicit trust questionnaire (5 items); UTAUT/TAM behavioural intention items; satisfaction/quality scale (item count not reported)
- Number of items: 5 (explicit trust questionnaire); WOA and BI item counts not individually reported
- Behavioural vs self-report: both — WOA is a behavioural measure (computed from estimate shifts); explicit trust, behavioural intention, and confidence are self-report

## Moderators and covariates tested
- Task familiarity: measured covariate; WOA in the no-explanation condition was significantly negatively correlated with task familiarity (rs = −0.51, p < 0.001) — less familiar participants relied more heavily on AI without explanation; relevant to RQ3
- Explanation quality / satisfaction: measured post-hoc; strongly positively correlated with behavioural intention (rs = 0.60, p < 0.001); identified as the key mechanism linking explanations to adoption — relevant to RQ2
- User role (doctor vs. nurse vs. paramedic): all healthcare professionals but role-specific differences not formally tested; algorithm aversion (fear of replacement) emerged qualitatively — relevant to RQ3
- User expertise / AI literacy: not formally measured; clinical domain expertise assumed for all participants; no AI literacy measure collected

## Statistical approach
- Primary analysis method: Wilcoxon signed-rank test for WOA comparison between explanation and no-explanation conditions; Spearman correlation for examining relationships between WOA, task familiarity, and explanation quality; thematic analysis of qualitative open-ended responses for interface redesign
- Software: not reported
- Key model fit or effect size reported: WOA with explanation Mdn = 0.33 vs. WOA without explanation Mdn = 0.12 (significant, Wilcoxon); WOA × task familiarity rs = −0.51, p < 0.001 (no-explanation condition); explanation quality × behavioural intention rs = 0.60, p < 0.001; no significant effect of explanations on explicit trust or behavioural intention

## Author-noted limitations
- Only correct AI predictions were used in the experiment; over-reliance risk from explanations under incorrect predictions was not tested
- Explicit trust and behavioural intention measures were not sensitive to the explanation manipulation; initial Doctor XAI explanations were perceived as ill-suited (too technical, ICD-code-heavy), likely attenuating effects
- Small N (41); limited statistical power for sub-group analyses by professional role
- Single disease domain (acute myocardial infarction); generalisability to other clinical prediction tasks is unknown
- Within-subject design risks carry-over and practice effects
- Uncertainty information (model accuracy/reliability) was not provided in the explanation interface; participants explicitly requested this
- The redesigned progressive-disclosure interface was not re-evaluated in a new controlled study; its effectiveness remains to be empirically confirmed

## Related pages
- [[panigutti-codesign-xai-clinical]]
- [[natural-language-explanations]]
- [[trust-calibration]]
- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
