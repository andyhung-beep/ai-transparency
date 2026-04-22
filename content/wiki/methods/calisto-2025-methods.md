# Calisto et al. (2025) — Methods

**Summary**: Within-subject user study (N = 52 clinicians from eleven Portuguese clinical institutions) comparing three AI communication styles (conventional, assertive, non-assertive) across four clinician expertise strata (intern, junior, middle, senior) in a breast cancer multimodal imaging diagnosis task, with measures of diagnostic time, accuracy, trust, workload, and usability.

**Sources**: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (within-subject counterbalanced user study with professional participants)

## Sample
- N: 52
- Population: domain professionals (clinicians from eleven Portuguese clinical institutions; categorized as interns, juniors, middles, and seniors by years of clinical experience)
- Domain: healthcare (breast cancer diagnosis via multimodal imaging — mammography, ultrasound, MRI)
- Country / region: Portugal
- Recruitment method: clinical institution recruitment (11 Portuguese clinical institutions)

## Transparency operationalization
- Type: personalized, contextual explanation (natural language clinical argumentation combined with visual indicators and severity predictions adapted to communication assertiveness)
- Manipulation or measure: within-subjects manipulation of three AI communication style conditions, counterbalanced across clinicians — (1) conventional agent: provides only numerical BIRADS scores and model accuracy metrics (minimal outcome transparency); (2) assertive agent: actively imposes AI recommendations with direct, confident language, detailed clinical explanations (lesion morphology, shape, margin, density, calcification patterns), patient-specific context (family and personal history), visual severity indicators, and visual highlights on regions of interest — equivalent to process-level explanations adapted to clinical reasoning; (3) non-assertive agent: provides the same clinical explanations in tentative, suggestive language. Each clinician diagnosed 289 patients across all three conditions. AI backend: DenseNet for 2D MG and US; 3D ResNet for MRI.
- Scale / instrument name: not applicable (experimental manipulation via AI interface design)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (understanding, competence dimensions) and affective (thoughtfulness dimension)
- Measure: three-dimensional trust scale assessing — (1) understanding: whether the clinician comprehends the agent's reasoning; (2) competence: whether the agent is seen as capable; (3) thoughtfulness: whether the agent appears to reflect care for the patient. Overall trust rating also collected. Behavioral trust assessed via acceptance/rejection rates of AI suggestions (proportion of AI recommendations adopted).
- Scale / instrument name: custom three-dimensional trust scale (understanding, competence, thoughtfulness); specific scale source not reported in source summary
- Number of items: not reported
- Behavioural vs self-report: both (acceptance/rejection rate of AI suggestions as behavioral; three-dimensional trust scale as self-report)

## Moderators and covariates tested
- Clinician expertise level (intern, junior, middle, senior): primary moderating variable measured as years of clinical experience and seniority category; this is the central RQ3-relevant variable. Assertive communication improved outcomes for interns/juniors; non-assertive communication was more effective for middle/senior clinicians (directly relevant to RQ3 as a detailed expertise-by-explanation-style interaction)
- Cognitive workload (NASA-TLX): measured as a covariate; no significant workload differences between conditions
- System usability (SUS): measured as a covariate; no significant usability differences between conditions

## Statistical approach
- Primary analysis method: repeated-measures ANOVA for within-subjects comparisons of diagnostic time, accuracy (precision, recall, F1), trust dimensions, workload, and usability across conditions; pairwise post-hoc comparisons by expertise stratum
- Software: not reported
- Key model fit or effect size reported: F-statistics and p-values reported (e.g., diagnostic time: F = 11.32, p = 0.005, large effect r = 0.49; competence trust: p = 0.04; thoughtfulness trust: p = 0.001; assertive preference: F = 8.35, p = 0.001); classification accuracy reported by condition and expertise stratum (e.g., interns/juniors: 81.59% correct with assertive vs. 69.70% conventional)

## Author-noted limitations
- Small professional sample (N = 52) limits statistical power, particularly for fine-grained expertise stratum comparisons
- Within-subject design with 289 patients per condition may produce fatigue effects despite counterbalancing
- Results are specific to breast cancer imaging; generalizability to other radiology specialties or AI-assisted clinical domains is uncertain
- The assertive vs. non-assertive communication style manipulation is a novel operationalization; relationships to established XAI transparency taxonomies (e.g., feature importance, counterfactuals) are indirect
- No long-term follow-up; effects of sustained AI-assisted practice on trust calibration and expertise development are unknown

## Related pages
- [[calisto-personalized-explanations-breast-imaging]]
- [[user-expertise]]
- [[explainability]]
- [[causability]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[rq3-user-roles]]

## References
Calisto, F. M., Abrantes, A., Santiago, C., Nunes, N., & Nascimento, J. C. (2025). *Personalized explanations for clinician-AI interaction in breast imaging diagnosis by adapting communication to expertise levels*. *International Journal of Human-Computer Studies, XX*(XX), XXXX. [Volume and page not reported in source summary.]
