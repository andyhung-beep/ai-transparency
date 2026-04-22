# Naiseh et al. 2023 — Methods

**Summary**: A within-subject empirical study with 41 medical practitioners comparing how four XAI explanation classes (Local, Example-based, Counterfactual, Global) affect trust calibration in a clinical decision support system for chemotherapy prescription screening, combining quantitative trust ratings with semi-structured interviews.

**Sources**: Naiseh et al._How the different explanation classes impact trust calibration.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (within-subject experiment with quantitative trust ratings and semi-structured qualitative interviews)

## Sample
- N: 41
- Population: medical practitioners — doctors and pharmacists with experience in prescription screening
- Domain: healthcare / clinical decision support (chemotherapy prescription screening)
- Country / region: not reported
- Recruitment method: not reported

## Transparency operationalization
- Type: explainability — four model-agnostic XAI explanation classes compared
- Manipulation or measure: within-subject design; each participant encountered all five conditions (four explanation classes plus no-explanation control) using a mock chemotherapy prescription screening tool with both correct and incorrect AI recommendations; the four XAI classes were: (1) Local — feature importance scores for the specific case; (2) Example-based — similar training data cases presented for comparison; (3) Counterfactual — what-if feature changes that would alter the recommendation; (4) Global — model-wide feature rankings across all training instances
- Scale / instrument name: not applicable (experimental manipulation using a purpose-built mock clinical decision support interface)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported) and behavioural
- Measure: cognitive trust measured via Madsen and Gregor's (2000) Human-Computer Trust (HCT) scale covering three components: perceived understandability, perceived reliability, and perceived technical competence; behavioural trust measured via three indicators: (1) agreement with AI recommendation, (2) switch from initial AI recommendation, (3) Human-AI team performance score on the classification task
- Scale / instrument name: Madsen and Gregor (2000) Human-Computer Trust (HCT) scale
- Number of items: not reported (HCT scale item count not specified in available sources)
- Behavioural vs self-report: both — self-report for HCT cognitive trust components; behavioural for agreement rate, switch rate, and team performance score

## Moderators and covariates tested
- Explanation class (five levels: Local, Example-based, Counterfactual, Global, No explanation): primary within-subject manipulation; each explanation class produced distinct trust calibration profiles — relevant to RQ2
- User expertise (clinical vs. AI expertise): the sample consists of clinical domain experts (doctors, pharmacists) who lack AI statistical expertise; participants misinterpreted Local/Global feature-importance scores through clinical rather than statistical lenses, demonstrating that clinical expertise shapes explanation effectiveness — directly relevant to RQ3
- Correctness of AI recommendation: both correct and incorrect AI recommendations were presented to test whether explanations help participants identify errors; findings show all explanation classes increased over-reliance on incorrect recommendations

## Statistical approach
- Primary analysis method: within-subject ANOVA or equivalent repeated-measures analysis for quantitative trust components; thematic analysis of semi-structured interview data for qualitative findings
- Software: not reported
- Key model fit or effect size reported: not reported (specific F-statistics, p-values, or effect sizes not enumerated in available sources beyond directional significance statements)

## Author-noted limitations
- Within-subject design risks order effects and carry-over between explanation conditions
- Small expert sample (N = 41); limited statistical power for sub-group analyses
- Mock clinical tool used rather than a live deployed system; ecological validity is limited
- Only correct and incorrect AI recommendations tested; does not examine how explanations behave with ambiguous or borderline cases
- The study tests four predetermined explanation classes; hybrid or tailored explanations are not evaluated
- Qualitative interview findings based on self-report and may not fully capture actual decision processes

## Related pages
- [[naiseh-explanation-classes-trust-calibration]]
- [[trust-calibration]]
- [[explainability]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[appropriate-reliance]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
