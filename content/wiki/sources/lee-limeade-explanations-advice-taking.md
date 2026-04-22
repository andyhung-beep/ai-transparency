# LIMEADE: From AI Explanations to Advice Taking

**Source file**: [Original article](../../raw/Lee et al._LIMEADE from AI explanations to advice taking.pdf)

**Summary**: Introduces LIMEADE, a general framework that translates post-hoc AI explanations into updates to opaque machine-learned models, and reports that enabling users to act on explanations significantly increases perceived trust, control, and satisfaction in a deployed paper recommender system.

**Sources**: Lee et al._LIMEADE from AI explanations to advice taking.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Lee, Downey, Lo, and Weld (2023) present LIMEADE (LIME Advice-taking by Example), a framework for bridging the gap between post-hoc explanations and actionable human feedback for opaque ML models. While explanation methods such as LIME and SHAP can generate local, interpretable descriptions of model behaviour, prior to LIMEADE no general mechanism existed for translating such explanations into corrections to an arbitrary underlying model. LIMEADE does so by generating pseudo-instances that represent the features the user has endorsed or rejected, weighting them by proximity to the explained instance, and retraining the original model on the augmented dataset.

The paper reports two case studies: (1) simulated advice-taking for 20 binary image classifiers built on neural embeddings from the COCO dataset, and (2) a deployed research-paper recommender system (Semantic Sanity) with real users. The second case study included a 21-participant in-person user study comparing a LIMEADE-enabled interface against a baseline with no explanation affordances.

Domain: recommender systems / human-AI interaction (computer science).

## Key Findings

- LIMEADE-processed advice outperformed the labelling-only baseline on 16 of 20 image classification tasks, with an overall accuracy boost of 9.33% vs. 8.21% for the baseline (p = 2.3 × 10⁻⁹). [domain: image classification]
- In the user study, 17 of 21 participants trusted the LIMEADE system more than the baseline; all 21 preferred it for perceived control; 18 of 21 found it more transparent (all statistically significant). [domain: paper recommendation]
- LIMEADE received significantly higher overall system ratings (M = 3.85 vs. 3.38; p = 0.043). [domain: paper recommendation]
- No statistically significant difference in objective feed quality (DCG, AP) between LIMEADE and baseline feeds, indicating perceived improvements in trust and control did not straightforwardly translate into measurably better recommendations in this study.
- An explanation-action tradeoff was identified: greedy explanation strategies that surface the most salient terms reduce diversity over time, eventually limiting users' opportunities to give new advice; a diversity-biased display approach mitigated this.
- LIMEADE benefits diminish with more training data; it is most valuable in low-supervision settings where spurious correlations are most likely to dominate.

## Transparency Constructs

LIMEADE operationalises [[explainability]] as the surfacing of high-level, interpretable features (n-gram topics for text; superpixels for images) derived from a linear explanatory model that locally approximates the opaque model. This is a form of [[process-transparency]]: users receive not just a prediction but a vocabulary of reasons they can interrogate and act upon. The paper also raises the distinction between transparency that informs and transparency that enables action, framing explanation quality partly in terms of the actionability it affords rather than accuracy of the explanation itself.

Transparency is measured subjectively through binary forced-choice questions ("which system is more transparent?") and Likert-scale overall ratings.

## Trust Constructs

Trust is measured via subjective, user-reported preference ("which system do you trust more?") and Likert-scale ratings. The dominant construct is [[behavioural-trust]] (willingness to rely on and use again) and [[cognitive-trust]] (confidence that the system reflects the user's actual interests). Affective or institutional dimensions of trust are not explicitly separated. The paper frames trust as something that actionable explanations augment: users feel more confident when they can inspect and correct the model.

## Relevance to Research Questions

**RQ1**: LIMEADE operationalises explainability as a bidirectional interface—explanations are not just outputs but inputs that enable users to reshape model behaviour. This extends standard operationalisations of XAI transparency by coupling disclosure with [[appropriate-reliance]]-oriented control. Transparency is assessed subjectively rather than through validated psychometric instruments.

**RQ2**: The paper demonstrates that enabling users to act on explanations increases self-reported trust and perceived control even when measurable accuracy gains are mixed. This is consistent with a pattern in which process transparency boosts cognitive and affective trust independently of whether it improves objective performance—a finding relevant to understanding when transparency–trust relationships are (or are not) mediated by performance improvements.

**RQ3**: All 21 user-study participants were computer science researchers (task experts), so the study provides no contrast between user expertise levels. The paper notes that each user was "implicitly incentivised to understand and improve the recommender," which may limit generalisation to less expert or less motivated users.

## Related pages

- [[explainability]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
- [[rq1-conceptualizations]]
