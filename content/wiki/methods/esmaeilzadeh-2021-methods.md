# Esmaeilzadeh 2021 — Methods

**Summary**: A 2×3 between-subjects experimental survey (N = 634 US patients) comparing patient perceptions of trust, risk, communication barriers, transparency, liability, and usage intention across six AI-physician encounter scenarios varying illness type and AI autonomy level.

**Sources**: Esmaeilzadeh et al_2021_Patients_ perceptions toward human-artificial intelligence interaction in health care.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (2×3 between-subjects survey experiment with propensity score matching for demographic comparability)

## Sample
- N: 634
- Population: general public / patients (US adults)
- Domain: healthcare (clinical encounters for acute and chronic illness)
- Country / region: United States
- Recruitment method: crowdsourced online (Amazon Mechanical Turk; data collected May 2020)

## Transparency operationalization
- Type: institutional / regulatory transparency — perceived transparency of regulatory standards
- Manipulation or measure: Transparency not directly manipulated as an XAI-type intervention; rather, the study measures perceived transparency of regulatory standards as a dependent variable across three encounter type conditions: (1) AI-only (substituting physician); (2) AI+physician (augmenting physician); (3) Physician-only (traditional, no AI). The encounter type manipulation varies the degree of AI autonomy, which indirectly operationalises transparency/opacity of the clinical AI system. Participants responded to a multi-item scale on whether they believed regulatory guidelines to assess AI safety are yet to be formalised (transparency as governance concern).
- Scale / instrument name: researcher-designed scale for perceived transparency of regulatory standards
- Number of items: not reported

## Trust operationalization
- Type: cognitive and institutional (multi-item self-report)
- Measure: 5-item scale adapted from Luxton (2014) measuring patients' belief that the clinical encounter is trustworthy, capturing both institutional trust in the healthcare delivery mechanism and cognitive trust in AI/physician reliability and competence.
- Scale / instrument name: Luxton (2014) trust scale (adapted)
- Number of items: 5 (α = .92)
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Illness type (acute vs. chronic): manipulated (2 levels); moderated effects of encounter type on perceived benefits (chronic patients more negative toward AI-only), privacy concerns (acute patients more sensitive in AI+physician condition), and intention to use — relevant to RQ3 as patient role/context moderator
- Propensity score matching: used post-hoc to ensure demographic comparability across six conditions (approximately 100–113 per condition); demographic variables treated as controls

## Statistical approach
- Primary analysis method: MANOVA / ANOVA (between-subjects comparisons across the 2×3 design for nine dependent variables); propensity score matching for group comparability; pairwise comparisons with p-value corrections
- Software: not reported
- Key model fit or effect size reported: specific F-statistics and p-values reported per dependent variable (e.g., trust AI-only vs. physician-only: chronic p = .004; acute p < .001); marginal means reported for trust (18.4 physician-only vs. 17.1 AI+physician vs. 16.0 AI-only); α = .92 (trust scale)

## Author-noted limitations
- Hypothetical vignette design; actual clinical AI encounter would involve more contextual information and interaction
- MTurk sample may not represent the full diversity of patients in real clinical settings
- Data collected during COVID-19 pandemic (May 2020); heightened health anxiety may have influenced perceptions
- No manipulation of actual XAI features (explanations, disclosures); only encounter type varied
- Transparency operationalised as perceived regulatory adequacy rather than actual explanation quality
- Does not measure physician or clinician perspectives (patient-only sample)

## Related pages
- [[esmaeilzadeh-patients-perceptions-ai-healthcare]]
- [[institutional-trust]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[process-transparency]]
- [[disclosure]]
- [[domain-context]]
- [[perceived-risk]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
