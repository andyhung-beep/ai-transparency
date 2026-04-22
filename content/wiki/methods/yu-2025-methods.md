# Yu 2025 — Methods

**Summary**: An empirical mixed-methods study with 42 clinicians in a Chinese radiology setting comparing explainable vs. black-box AI and high- vs. low-autonomy AI for chest X-ray interpretation, finding that transparency increases trust but also accelerates trust erosion when AI errors occur, with more experienced clinicians showing higher trust and reliance.

**Sources**: Yu et al._Research-and-Analysis-of-Trust-and-Control-in-Huma.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (quasi-experimental within a tertiary-care hospital setting; quantitative measures supplemented by semi-structured interviews with thematic coding)

## Sample
- N: 42 (32 radiologists, physicians, and residents; 10 medical students)
- Population: domain professionals (clinical staff and medical students at a Chinese tertiary-care hospital)
- Domain: healthcare / radiology (AI-assisted chest X-ray interpretation)
- Country / region: China (Northeastern University China; China Medical University)
- Recruitment method: hospital staff (convenience sample within a single tertiary-care institution)

## Transparency operationalization
- Type: algorithmic transparency / explainability (AI reasoning provision vs. black-box opacity)
- Manipulation or measure: Two crossed experimental conditions: (1) Explainability condition — AI-powered CDSS provided visual and clinical rationale for diagnostic recommendations (highlighted diagnostic indicators, clinical indicator explanations); (2) Black-box condition — AI output provided without reasoning. Also crossed with: (3) High-autonomy AI condition — AI issued recommendations with reduced opportunities for human override; (4) Low-autonomy AI condition — human retained greater control over final decisions. Participants completed diagnostic tasks under unaided vs. AI-assisted conditions.
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-report) and behavioural (override frequency and reliance)
- Measure: (1) Cognitive trust — Likert-scale items assessing trust in AI recommendations; regression coefficient β = 0.42 (p = 0.001, R² = 0.48) for explainability predicting trust; (2) Behavioural trust — AI recommendation acceptance rate and override frequency; higher AI autonomy led to higher override rates (t = 3.89, p = 0.005); (3) Qualitative trust assessment — semi-structured interviews coded thematically (trust calibration dynamics, error responses)
- Scale / instrument name: not reported (Likert-scale trust items; instrument not named)
- Number of items: not reported
- Behavioural vs self-report: both — Likert self-report plus behavioural override frequency and recommendation acceptance rate

## Moderators and covariates tested
- Clinical experience / expertise: primary moderator; more experienced clinicians trusted AI more (r = 0.52, p = 0.002) and showed higher reliance (r = 0.41, p = 0.011); experience predicts higher trust (β = 0.28, p = 0.015, R² = 0.32) — directly relevant to RQ3
- AI autonomy level: tested as experimental factor; high-autonomy AI led to higher override rates, suggesting less perceived control reduces acceptance
- AI error events: tracked qualitatively; errors disproportionately eroded trust relative to successes rebuilding it (asymmetric trust dynamics)
- Clinician type (radiologist/physician/resident vs. student): participants segmented by role; students represent lower expertise group

## Statistical approach
- Primary analysis method: independent samples t-tests (unaided vs. AI-assisted accuracy; explainable vs. black-box trust; autonomy × override rate); Pearson correlations (experience vs. trust; experience vs. reliance); OLS regression (explainability predicting trust β; experience predicting trust β); thematic coding of semi-structured interviews (qualitative component)
- Software: not reported
- Key model fit or effect size reported: R² = 0.48 (explainability model); R² = 0.32 (experience model); β = 0.42 (explainability → trust); β = 0.28 (experience → trust); r = 0.52 (experience–trust); r = 0.41 (experience–reliance); t-statistics reported for group comparisons

## Author-noted limitations
- Small sample size (N = 42) from a single institution; limited statistical power and generalisability
- Single domain (chest X-ray radiology) and single country (China); cultural factors in AI trust may not generalise
- Convenience sample from one hospital; potential selection bias toward AI-familiar clinicians
- The cybernetic feedback model is theoretical; the full dynamic model was not formally tested (e.g., no time-series modelling of trust recalibration)
- Qualitative component based on interview coding; inter-rater reliability not reported
- The paradox finding (transparency accelerates trust loss after errors) is identified qualitatively but not formally modelled statistically

## Related pages
- [[yu-trust-control-human-ai-healthcare]]
- [[trust-calibration]]
- [[algorithmic-transparency]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
