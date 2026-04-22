# Karran 2022 — Methods

**Summary**: Two studies (N = 206 online MTurk; N = 19 eye-tracking lab) using a within-subjects design to test how adjacency and morphological clarity of AI explanation visualizations affect user confidence and cognitive load in a visual classification task.

**Sources**: Karran et al._Design for confidence.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
experimental (within-subjects; two studies: online survey experiment + lab eye-tracking study)

## Sample
- N: 206 (Study 1); 19 (Study 2)
- Population: general public / online panel (Study 1 ~60% male, avg. age 37.9); young adults recruited for lab study (Study 2 avg. age 24.9)
- Domain: general AI / computer vision (image classification)
- Country / region: North America (MTurk, Study 1); not reported (Study 2)
- Recruitment method: MTurk (Study 1); convenience / lab recruitment (Study 2)

## Transparency operationalization
- Type: visual attribution explanations (saliency/heatmap overlays on classified images)
- Manipulation or measure: 2 × 3 within-subjects manipulation — Adjacency (adjacent overlay vs. non-adjacent on black background) × Morphological Clarity (low: cloud of points / CP; medium: heatmap / HM; high: outline / ON); explanations generated via Integrated Gradients (CP and ON) and Grad-CAM (HM) using Xception model (ImageNet, accuracy 0.79); participants completed 50 visual decision-making trials
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (confidence in system correctness)
- Measure: single 7-point Likert item per trial: "Given the information above, I am confident that the system will correctly identify the next picture"; aggregated across 50 trials
- Scale / instrument name: not reported (custom single item adapted from Lankton et al., 2015)
- Number of items: 1 per trial
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- AI classification correctness (correct vs. incorrect AI output): measured; strong positive moderator of confidence (M = 5.27 correct vs. 4.29 incorrect, p < 0.001)
- Self-identified AI/Data expertise: 61 of 206 participants self-identified as AI/Data experts; main analysis does not break down results by expertise; noted as a future limitation (relevant to RQ3)
- Cognitive load (Study 2 only): measured via pupillometry (Tobii ε60); tested as mediator of adjacency/MC → confidence path; mediation not supported

## Statistical approach
- Primary analysis method: paired t-test (Study 1, adjacency comparison); ANOVA and post-hoc comparisons (MC levels); bootstrapped mediation analysis (Study 2, cognitive load as mediator)
- Software: not reported
- Key model fit or effect size reported: adjacency t(205) = 15.71, p < 0.001; MC effect p = 0.001 (low > high MC); mediation indirect effects: adjacency CI95% [−0.885; 0.408], MC CI95% [−0.615; 0.655] (both non-significant)

## Author-noted limitations
- No systematic analysis of user AI expertise as a moderator; 61 self-identified AI/Data experts were included but not separately analyzed
- Restriction to North American MTurk participants limits cultural generalizability
- Confidence (not trust) was the primary construct; the authors acknowledge trust and confidence are related but distinct
- No manipulation check confirming that participants perceived different MC levels as intended
- Study 2 small sample (N = 19) limits statistical power for mediation tests

## Related pages
- [[karran-design-for-confidence]]
- [[explainability]]
- [[cognitive-trust]]
- [[causability]]
- [[user-expertise]]
