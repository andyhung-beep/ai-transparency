# Lee (LIMEADE) 2023 — Methods

**Summary**: A mixed technical and user-study paper presenting LIMEADE (LIME Advice-taking by Example), evaluated via simulation on 20 binary image classifiers and a 21-participant in-person user study of a deployed paper recommender system comparing LIMEADE to a no-explanation baseline.

**Sources**: Lee et al._LIMEADE from AI explanations to advice taking.pdf

**Research questions addressed**: RQ1 / RQ2

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (technical framework paper + simulation evaluation + in-person user study)

## Sample
- N: 21 (in-person user study); 20 binary image classifiers built on COCO dataset (simulation)
- Population: computer science researchers (all 21 user-study participants were CS researchers)
- Domain: recommender systems / human-AI interaction (research paper recommendation — Semantic Sanity system); image classification (simulation — COCO dataset)
- Country / region: not reported
- Recruitment method: not reported (convenience — CS researcher community)

## Transparency operationalization
- Type: explainability / process transparency (actionable post-hoc explanations)
- Manipulation or measure: within-subjects comparison — all 21 participants used both LIMEADE interface (local LIME-derived explanations surfacing high-level interpretable features that users can endorse/reject to update the model) and a baseline interface (no explanation affordances); LIMEADE generates pseudo-instances representing endorsed/rejected features, weights by proximity, and retrains the original model on augmented data; explanation quality varied by display strategy (greedy vs. diversity-biased feature display) in technical evaluation
- Scale / instrument name: not applicable
- Number of items: not applicable

## Trust operationalization
- Type: cognitive; behavioural (adoption intent)
- Measure: (1) Binary forced-choice questions comparing LIMEADE vs. baseline on trust, control, and transparency (e.g., "which system do you trust more?"); (2) Likert-scale overall system rating (scale range not reported); (3) Objective feed quality (DCG, Average Precision) as behavioural outcome
- Scale / instrument name: not reported (custom binary forced-choice and Likert items)
- Number of items: not reported
- Behavioural vs self-report: both (subjective preference and Likert ratings; objective feed quality metrics)

## Moderators and covariates tested
- Display strategy (greedy vs. diversity-biased explanation display): manipulated in technical evaluation — greedy strategy reduces diversity over time; diversity-biased approach mitigated explanation-action tradeoff
- Training data volume: manipulated in simulation — LIMEADE benefits diminish with more training data; most valuable in low-supervision settings
- User expertise: not varied — all participants were CS researchers; no comparison across expertise levels (relevant to RQ3 as a gap; authors note motivation may not generalize to less expert users)

## Statistical approach
- Primary analysis method: sign test (binary forced-choice outcomes); t-test (overall system Likert rating); accuracy comparison (simulation, 20 classifiers)
- Software: not reported
- Key model fit or effect size reported: 17/21 trusted LIMEADE more (sign test significant); all 21 preferred LIMEADE for perceived control (p < 0.05); 18/21 found LIMEADE more transparent (p < 0.05); overall system rating M = 3.85 vs. 3.38, p = 0.043; simulation accuracy boost LIMEADE 9.33% vs. baseline 8.21%, p = 2.3 × 10⁻⁹; no significant difference in DCG or AP (objective feed quality)

## Author-noted limitations
- All participants were CS researchers; findings may not generalize to less expert or less motivated users
- No significant improvement in objective feed quality (DCG, AP) despite higher subjective trust and control ratings
- Explanation-action tradeoff: greedy display reduces diversity over time, limiting advice opportunities
- LIMEADE benefits diminish with more training data (most valuable in low-supervision settings)
- Within-subject design; order effects not fully reported
- User study sample very small (N = 21) and homogeneous

## Related pages
- [[lee-limeade-explanations-advice-taking]]
- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[process-transparency]]
