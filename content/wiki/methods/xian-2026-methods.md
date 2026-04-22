# Xian 2026 — Methods

**Summary**: An online survey study (N = 206 clinicians) evaluating three novel time-aware SHAP-based visualization formats for an ICU intubation prediction model, finding that a dual-encoded heatmap was most preferred and perceived as most usable despite scoring lowest on objective comprehension accuracy.

**Sources**: Xian et al._Clinician preference for explainable AI in critical care.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
survey (online; within-subjects evaluation of three explanation formats; preceded by ML model development on archival ICU data)

## Sample
- N: 206
- Population: clinicians (mix of clinical specialties; minority were practicing ICU clinicians; includes physicians, nurses, and other healthcare professionals)
- Domain: critical care / ICU (intubation decision support)
- Country / region: United Kingdom (University of Manchester); survey distributed via Prolific
- Recruitment method: Prolific (online research participant platform)

## Transparency operationalization
- Type: explainability (SHAP-based feature contribution explanations; temporal / time-series variant)
- Manipulation or measure: Within-subjects evaluation of three novel time-aware SHAP visualization formats, all applied to the same Random Forest ICU intubation prediction model (AUC = 0.94; MIMIC-III dataset, 4,608 patients, 10 medical variables over 7-hour window): (1) Temporal force plot — segments and color-codes SHAP values by time intervals; (2) Temporal bar chart — aggregates absolute feature contributions over time windows; (3) Dual-encoded heatmap — overlays SHAP contribution values (color intensity) with raw variable values (text), enabling simultaneous assessment of feature importance and clinical measurements. Participants rated each format on TAM3 constructs and answered comprehension questions.
- Scale / instrument name: Technology Acceptance Model 3 (TAM3) — Perceived Ease of Use, Perceived Usefulness, Behavioral Intention to Use subscales
- Number of items: not reported (TAM3 subscales; 5-point scale)

## Trust operationalization
- Type: cognitive (technology acceptance as trust proxy) and behavioural intention
- Measure: TAM3 constructs: Perceived Usefulness (M = 3.84 for heatmap), Perceived Ease of Use (M = 3.84), and Behavioral Intention to Use (M = 3.79) on a 5-point scale; preference ranking across the three formats; objective comprehension accuracy (proportion of comprehension questions answered correctly per format)
- Scale / instrument name: Technology Acceptance Model 3 (TAM3)
- Number of items: not reported
- Behavioural vs self-report: self-report (TAM3 and preference) plus quasi-behavioural comprehension test

## Moderators and covariates tested
- Clinician type / specialty: sample included mixed clinical roles; formal moderation by specialty or ICU experience not reported; acknowledged as a limitation (relevant to RQ3)
- Visualization format (within-subjects factor): primary independent variable — heatmap preferred by ~55%, force plot by ~30%, bar chart by ~15%
- Cognitive fit (theoretical moderator): theorised but not formally measured — alignment between visualization format and clinicians' mental task model is used to explain the heatmap preference

## Statistical approach
- Primary analysis method: descriptive statistics and within-subjects comparisons across TAM3 subscale scores and comprehension accuracy by visualization format; preference frequencies reported; inferential tests not fully specified in source summary
- Software: not reported
- Key model fit or effect size reported: AUC = 0.94 (Random Forest model); comprehension accuracy by format (heatmap 76%, bar chart 90%, force plot 92%); TAM3 mean scores per format reported on 5-point scale; overall comprehension accuracy 78%

## Author-noted limitations
- Minority of survey participants were practicing ICU clinicians; sample may not fully represent target end-user population
- Online survey via Prolific may not reflect real clinical decision-making contexts
- Objective comprehension accuracy discrepancy (heatmap preferred but lowest comprehension) not fully explained — possible halo effect or workflow-alignment preference
- Visualization formats evaluated in isolation from real-time clinical workflows; ecological validity limited
- Sample does not allow formal comparison by clinical specialty or years of ICU experience
- Temporal SHAP approach validated only for intubation prediction; generalisability to other ICU decision tasks unknown

## Related pages
- [[xian-clinician-xai-critical-care]]
- [[explainability]]
- [[uncertainty-visualization]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
