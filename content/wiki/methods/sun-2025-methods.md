# Sun et al. (2025) — Methods

**Summary**: A two-study mixed-methods investigation (online survey N = 142; laboratory study N = 40) using a 2 × 2 × 3 factorial design to examine how the actual source (human professional vs. LLM) and disclosed label (human vs. AI) of online health information independently affect trust, measured via self-report, eye-tracking, and physiological sensing.

**Sources**: Sun et al._Understanding trust toward human versus AI-generated health information.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (two complementary studies: Study 1 — online survey with qualitative thematic analysis; Study 2 — laboratory experiment with physiological and eye-tracking instrumentation)

## Sample
- N: Study 1: N = 142; Study 2: N = 40
- Population: Study 1 — general public (online panel); Study 2 — general public / convenience laboratory sample
- Domain: online health information (general health, symptom, and treatment information articles)
- Country / region: not reported
- Recruitment method: Study 1 — online panel (platform not specified); Study 2 — laboratory recruitment (method not specified)

## Transparency operationalization
- Type: disclosure — source-attribution labeling; operationalizes transparency as whether the authorship of health information is disclosed as human professional or AI
- Manipulation or measure: 2 (actual source: human professional-authored vs. LLM-generated) × 2 (disclosed label: labeled as "Human Professional" vs. labeled as "AI") × 3 (information type: general, symptom, treatment) factorial design; source was between-subjects; label and information type were within-subjects in Study 1; all factors within-subjects in Study 2
- Scale / instrument name: not applicable (transparency was a disclosure label manipulation, not a scale)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive trust (self-report); affective trust (physiological proxies); behavioural trust (gaze-based proxies)
- Measure: Study 1 and Study 2 self-report: 13-item validated trust-in-online-health-information questionnaire (Cronbach's α = .92) assessing objectivity, reliability, and credibility; Study 2 physiological: ECG-derived HRV (RMSSD), electrodermal activity (EDA), and skin temperature as affective arousal indicators; Study 2 gaze: fixation count, fixation duration, saccade count, and pupil diameter on information area and label area via Tobii Pro Fusion eye-tracker; Machine learning (binary SVM classification) used to predict trust level from gaze and physiological features
- Scale / instrument name: 13-item trust-in-online-health-information questionnaire (source not named in summary; validated scale)
- Number of items: 13
- Behavioural vs self-report: both (self-report trust scale + implicit behavioral/physiological measures in Study 2)

## Moderators and covariates tested
- AI literacy: measured via 10-item MAILS scale; shown to correlate more strongly with trust in LLM-sourced content than human-sourced content — relevant to RQ3
- Propensity to trust in technology (PPT): measured via 6-item scale; individual difference moderator of source-label trust effects — relevant to RQ3
- eHealth literacy: measured (specific scale not named); individual difference covariate
- Information type (general, symptom, treatment): within-subjects factor tested as potential moderator; non-significant

## Statistical approach
- Primary analysis method: Study 1 — repeated-measures ANOVA and mixed ANOVA for self-report trust; thematic analysis of qualitative open-ended responses (four themes identified); Study 2 — repeated-measures ANOVA for physiological and gaze measures; binary SVM machine learning classification for trust level and source prediction from implicit signals
- Software: not reported
- Key model fit or effect size reported: Study 1 — LLM > human source: d = .14 medium, p = .024; human > AI label: d = -.39 medium, p < .001; Study 2 — LLM > human source: d = .35 medium, p < .01; human > AI label: d = -.23 medium, p = .01; ML trust classification accuracy = 73%; source classification accuracy = 65%; Cronbach's α = .92 for trust scale

## Author-noted limitations
- Study 2 sample is small (N = 40), limiting statistical power for physiological and gaze analyses
- The health information stimuli were created or collected for the study; ecological validity as naturally occurring online health content may be limited
- The decoupled source × label design is novel but artificial — in natural settings users rarely know actual vs. disclosed source independently
- Physiological measures (HRV, EDA, skin temperature) are indirect proxies for affective trust and are open to alternative interpretations
- The study does not manipulate or control for health literacy beyond measuring eHealth literacy as a covariate
- Results are based on English-language health content; cross-linguistic and cross-cultural generalisability is not established

## Related pages
- [[sun-trust-human-vs-ai-health-info]]
- [[disclosure]]
- [[cognitive-trust]]
- [[affective-trust]]
- [[algorithmic-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Sun, Y., et al. (2025). Understanding trust toward human versus AI-generated health information through behavioral and physiological sensing. *International Journal of Human-Computer Studies* (accepted; arXiv preprint).
