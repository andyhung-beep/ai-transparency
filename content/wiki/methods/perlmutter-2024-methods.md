# Perlmutter 2024 — Methods

**Summary**: A within-subjects experiment with 24 expert oil-and-gas pipeline data analysts comparing three XAI interface conditions (baseline/no explanation, one-class example-based, two-class example-based) on trust, understanding, and objective decision performance.

**Sources**: Perlmutter et al._Impact of example-based XAI for neural networks on trust, understanding, and performance.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (within-subjects, three-condition repeated measures)

## Sample
- N: 24
- Population: domain professionals (data analysts at a single pipeline inspection company)
- Domain: industrial safety / oil-and-gas pipeline inspection
- Country / region: not reported
- Recruitment method: convenience (single company)

## Transparency operationalization
- Type: example-based explanation (prototype XAI / k-nearest training instances)
- Manipulation or measure: Within-subjects manipulation across three interfaces: (1) Baseline — CNN classification output only, no explanation; (2) XAI-1 — three closest training examples from the predicted class shown alongside the classification; (3) XAI-2 — three closest training examples from both classes shown, enabling contrastive comparison. Examples retrieved by comparing activation-graph fingerprints (keypoints from neural network hidden layers) of test images with training images.
- Scale / instrument name: not applicable (experimental manipulation)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (self-reported) and behavioural (ranked preference and performance)
- Measure: (1) Continuous 0–10 Likert scale for trust in the ML classification and trust in the human-machine team, rated after each interface; (2) Ranked preference ordering across the three interfaces collected at study end; (3) Objective performance (correct/incorrect classification decisions) as a behavioural trust proxy.
- Scale / instrument name: adapted from Wang et al. (2023) and Zhou et al. (2019)
- Number of items: not reported
- Behavioural vs self-report: both used

## Moderators and covariates tested
- Years of professional experience: measured covariate; significant negative relationship with trust in the human-machine team (Kruskal-Wallis p = 0.001, η² = 0.22); most experienced analysts (10+ years) trusted the team least — directly relevant to RQ3
- AI anxiety (scale item: "I feel that if I depend on robots or AI too much, something bad might happen"): measured covariate; significant predictor of human-machine team trust in the Baseline condition; effect attenuated by XAI interfaces
- Perceived agreement with AI: measured covariate correlated with trust

## Statistical approach
- Primary analysis method: Kruskal-Wallis tests (non-parametric; for ranked trust and understanding comparisons); Wilcoxon signed-rank tests (for within-subjects pair comparisons); Spearman correlations (trust–understanding); Random Forest Recursive Feature Elimination (RFE) for predictor identification; Chi-square test for performance comparisons
- Software: not reported
- Key model fit or effect size reported: η² (Kruskal-Wallis effect sizes: trust η² = 0.18, understanding η² = 0.15); Spearman r (trust–understanding for XAI-2: r = 1.00); Cohen's d = 0.73 (human-machine team vs. ML-alone trust)

## Author-noted limitations
- Small sample (N = 24) from a single company limits statistical power and generalisability
- Within-subjects design introduces order effects and potential carry-over between conditions
- Expert-only sample (pipeline data analysts) means results may not generalise to novice or general-public users
- Single domain (oil-and-gas pipeline inspection) limits broader applicability
- Participants expressed priming concerns (job threat from AI); researchers countered these but residual effects may remain
- Free-response analysis is qualitative and based on a small N

## Related pages
- [[perlmutter-example-based-xai-pipeline]]
- [[example-based-explanations]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
