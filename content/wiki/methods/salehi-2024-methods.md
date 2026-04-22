# Salehi 2024 — Methods

**Summary**: A two-platform quasi-experimental study comparing High-MAST vs. Low-MAST AI decision-support systems with domain experts — 146 airport TSOs (Facewise) and 23 DHS intelligence analysts (READIT) — examining the relationship between the 9-criterion MAST trustworthiness checklist and trust perceptions, credibility, perceived risk, and objective performance.

**Sources**: Salehi et al._Towards trustworthy AI-enabled decision support systems.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
quasi-experimental (between-subjects, two-condition: High-MAST vs. Low-MAST, across two platforms)

## Sample
- N: 146 (Facewise — Transportation Security Officers, TSOs) + 23 (READIT — DHS intelligence analysts); total N = 169
- Population: domain professionals (government security and intelligence experts)
- Domain: national security (airport security screening; intelligence analysis)
- Country / region: United States
- Recruitment method: not reported (government agency staff)

## Transparency operationalization
- Type: multi-dimensional trustworthy AI design (process transparency, uncertainty visualization, algorithmic transparency, outcome transparency, visualization)
- Manipulation or measure: Between-subjects manipulation — High-MAST vs. Low-MAST system versions. MAST criteria embedded in High-MAST versions: (1) Sourcing — identifies underlying data and training methodology; (2) Uncertainty — indicates and explains output uncertainty; (3) Distinguishing — separates derived results from underlying data; (4) Analysis of Alternatives — identifies and assesses alternative results; (5) Customer Relevance — presents information in user-relevant way; (6) Logic — explains how results were derived; (7) Change — indicates consistency or change from prior analyses; (8) Accuracy — communicates accuracy of judgments; (9) Visualization — uses appropriate visual displays. Low-MAST versions matched on usability and engagement to isolate MAST criteria effects.
- Scale / instrument name: Multisource AI Scorecard Table (MAST; 9 criteria rated by participants)
- Number of items: 9 (one per MAST criterion, each rated by participants)

## Trust operationalization
- Type: cognitive (self-reported perceptions of trustworthiness)
- Measure: Two trust instruments administered: (1) Jian et al. (2000) — 12-item automation trust scale with both positively and negatively valenced items (range 1–7); (2) Chancey et al. (2017) — 15-item scale decomposing trust into purpose trust, process trust, and performance trust (all positive valence). Also measured: message credibility (Appelman & Sundar, 2016), perceived risk, perceived benefit, and objective task performance.
- Scale / instrument name: Jian et al. (2000) Trust in Automation Scale; Chancey et al. (2017) Trust Scale
- Number of items: Jian: 12 items; Chancey: 15 items
- Behavioural vs self-report: primarily self-report; objective performance also measured (identification accuracy for Facewise; report quality for READIT)

## Moderators and covariates tested
- Platform / domain (Facewise vs. READIT): structural moderator — different patterns of MAST–trust associations observed across platforms
- Usability (SUS): measured as covariate; no significant between-condition difference, confirming usability was successfully controlled
- Engagement: measured as covariate; no significant between-condition difference
- User expertise: all participants are domain experts; no within-sample expertise variation tested — relevant to RQ3 as a noted limitation

## Statistical approach
- Primary analysis method: ordinary least squares (OLS) regression (MAST-total predicting trust, credibility, risk, benefit); independent-samples t-tests for between-condition comparisons; principal component analysis (PCA) for outcome variable reduction
- Software: not reported
- Key model fit or effect size reported: R² values per regression (Facewise: trust R² = 0.31–0.37; READIT: trust R² = 0.58–0.61; credibility R² = 0.70); PCA explained variance (Facewise: 84%; READIT: 87.65%)

## Author-noted limitations
- READIT sample is very small (N = 23); insufficient power for subgroup analyses
- No variation in user expertise within samples; cannot test how MAST effects differ across novice vs. expert users
- High-MAST TSOs spent significantly more time on task without accuracy gains, suggesting cognitive load as an unresolved concern
- No significant performance differences between High- and Low-MAST conditions on either platform; MAST/trust and actual calibration (performance) are dissociable
- Item valence (positively vs. negatively worded trust items) affected which trust instrument detected significant differences — measurement instrument sensitivity is a confound

## Related pages
- [[salehi-mast-trustworthy-ai-dss]]
- [[algorithmic-transparency]]
- [[uncertainty-visualization]]
- [[process-transparency]]
- [[explainability]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[institutional-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
