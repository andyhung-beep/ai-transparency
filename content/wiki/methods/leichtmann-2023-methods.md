# Leichtmann 2023 — Methods

**Summary**: A 2 × 2 between-subjects online experiment (N = 410) using a mushroom-classification task to test whether visual XAI explanations (Grad-CAM + example-based nearest neighbours) and/or an educational intervention about AI functioning affect decision accuracy, self-reported trust, and comprehension in a general lay population.

**Sources**: Leichtmann et al._Effects of Explainable Artificial Intelligence on trust and human behavior in a high-risk decision task.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (2 × 2 between-subjects online experiment)

## Sample
- N: 410
- Population: general public (Austrian adults; deliberately non-expert, no mushroom or AI expertise required)
- Domain: high-risk consumer decision-making / food safety (mushroom edibility classification)
- Country / region: Austria
- Recruitment method: online panel (market research company)

## Transparency operationalization
- Type: (1) attribution-based explanation (Grad-CAM visual saliency); (2) example-based explanation (nearest training images); (3) educational intervention (process transparency at system level)
- Manipulation or measure: 2 × 2 between-subjects factorial design — Factor 1: presence vs. absence of visual XAI explanations (Grad-CAM attribution maps highlighting image regions + example-based nearest-neighbour training images); Factor 2: presence vs. absence of a brief educational intervention (text + illustrations explaining how image-classification neural networks work); participants used a fictional smartphone app ("Forestly") to classify 10 mushroom images as edible or poisonous; fictional AI system presented as a deep convolutional neural network
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (item-level self-report); behavioural (overtrust / appropriate reliance)
- Measure: (1) Self-reported trust — single Likert item per mushroom image ("I TRUST this mushroom identification of the AI"), aggregated across 10 items; (2) Overtrust (behavioural) — agreeing with incorrect AI recommendations; (3) Task performance (edibility assessment accuracy, picking intention) as behavioural trust-adjacent outcomes; (4) App evaluation and intention to use again
- Scale / instrument name: not reported (custom single item per trial)
- Number of items: 1 per trial (aggregated to scale)
- Behavioural vs self-report: both (behavioural accuracy and overtrust; self-report trust)

## Moderators and covariates tested
- Domain-specific mushroom knowledge: measured; did not predict task performance (contrary to expectation)
- General AI knowledge: measured; did not predict task performance (relevant to RQ3 — expertise did not moderate XAI effectiveness in this design)
- Self-reported trust (as predictor): higher trust predicted poorer performance on incorrect AI items (β = −0.40, p < 0.001, R² = 0.15) — overtrust mechanism confirmed
- Educational intervention × XAI interaction: tested; educational intervention had no significant effect on any outcome

## Statistical approach
- Primary analysis method: Wilcoxon rank-sum test (between-group performance comparisons); linear regression (trust as predictor of performance on incorrect AI items); ANOVA (app evaluation)
- Software: not reported
- Key model fit or effect size reported: XAI vs. no-XAI on all 10 items W = 0.44, p < 0.001; XAI vs. no-XAI on incorrect AI items W = 0.35, p = 0.004; self-reported trust β = −0.40, p < 0.001, R² = 0.15 (trust predicting performance on incorrect items); app rating M = 3.77 (XAI) vs. 4.12 (no XAI), p = 0.003

## Author-noted limitations
- Experimental design may have suppressed AI knowledge effects by preventing exploratory interaction (standardized stimulus presentation)
- Single exposure in artificial task; ecological validity of the mushroom scenario is limited
- Self-reported trust measured with a single item per trial rather than a validated multi-item scale
- General population sample; no domain experts for comparison (relevant to RQ3)
- Effect of XAI on trust may reverse if explanations consistently validate a reliable AI (context-dependent)
- Educational intervention effects may require more extensive exposure or active engagement to manifest

## Related pages
- [[leichtmann-xai-trust-high-risk]]
- [[explainability]]
- [[example-based-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
