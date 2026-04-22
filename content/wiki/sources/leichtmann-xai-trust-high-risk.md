# Effects of Explainable Artificial Intelligence on Trust and Human Behavior in a High-Risk Decision Task

**Source file**: [Original article](../../raw/Leichtmann et al._Effects of Explainable Artificial Intelligence on trust and human behavior in a high-risk decision task.pdf)

**Summary**: A 2 × 2 between-subjects online experiment (N = 410) using a mushroom-classification scenario finds that visual XAI explanations (attribution-based Grad-CAM and example-based nearest neighbours) improved decision accuracy and produced better-calibrated trust, while an educational intervention about how AI works had no significant effect.

**Sources**: Leichtmann et al._Effects of Explainable Artificial Intelligence on trust and human behavior in a high-risk decision task.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Leichtmann, Humer, Hinterreiter, Streit, and Mara (2023) report an exploratory experiment in which participants used a fictional smartphone app ("Forestly") to decide whether photographed mushrooms were edible or poisonous. Two independent variables were crossed: (1) presence vs. absence of visual XAI explanations (Grad-CAM attribution maps and example-based nearest-neighbour images from training data), and (2) presence vs. absence of a brief educational intervention explaining how image-classification neural networks work. Dependent variables included task performance (edibility assessment accuracy, picking intention), self-reported trust, self-reported comprehension, and AI system evaluation.

The study recruited 410 Austrian participants via an online panel (market research company), deliberately targeting a non-expert, general-population sample to maximise ecological validity.

Domain: high-risk consumer decision-making / food safety.

## Key Findings

- Participants who received visual XAI explanations significantly outperformed those who did not on edibility assessment (all 10 items: effect size W = 0.44, p < 0.001) and on the subset of items where the AI's recommendation was incorrect (W = 0.35, p = 0.004). [domain: food safety / high-risk consumer decision]
- The educational intervention (text + illustrations about CNN functioning) had no statistically significant effect on any dependent variable, including performance, trust, or comprehension. [domain: same]
- Participants with visual explanations reported significantly lower trust in the AI's classification (p < 0.001, W = 0.36) and lower self-reported comprehension compared to those without explanations—interpreted as evidence that explanations prevented overtrust rather than undermining appropriate reliance. [domain: same]
- Higher self-reported trust predicted poorer performance on items where the AI classified incorrectly (β = −0.40, p < 0.001, R² = 0.15), confirming that overtrust led to harmful decisions in this high-stakes context. [domain: same]
- Participants who received explanations rated the app less positively (M = 3.77 vs. 4.12, p = 0.003) and expressed lower intention to use it again—attributed to explanations making the AI's imperfect performance more visible. [domain: same]
- Neither domain-specific mushroom knowledge nor general AI knowledge predicted task performance, contrary to expectations from the AI literacy and digital literacy literature.

## Transparency Constructs

The study employs two complementary transparency approaches:

1. **Attribution-based explanations** (Grad-CAM): highlights image regions important to the AI's prediction—a form of [[explainability]] focused on local feature attribution.
2. **Example-based explanations**: nearest training images for each predicted class—a form of [[example-based-explanations]] that allows users to compare the input image with known prototypes.

Both are post-hoc, local, model-specific techniques applied to a deep convolutional neural network. The educational intervention represents a distinct construct closer to [[process-transparency]] at the system level (how AI in general works) rather than instance-level explanation.

Transparency is not measured directly; its effects are inferred through task performance, trust ratings, and comprehension test scores.

## Trust Constructs

Trust is operationalised as a single-item Likert-scale rating after each mushroom image ("I TRUST this mushroom identification of the AI"), aggregated across the 10 task items. This is a narrow measure of [[cognitive-trust]] (confidence in a specific system output). The study also distinguishes overtrust (following an incorrect AI recommendation) as a behavioural measure of [[behavioural-trust]] / [[appropriate-reliance]] failure.

The concept of [[trust-calibration]] is central: the authors explicitly frame the goal as neither maximising nor minimising trust but achieving trust that matches the AI's actual capabilities and error profile.

## Relevance to Research Questions

**RQ1**: The paper operationalises transparency through two distinct XAI modalities (attribution-based, example-based) and measures trust via item-level self-report rather than validated multi-item scales. This is consistent with a pattern in the XAI literature of using proxy or ad-hoc trust measures in task-specific studies. Trust calibration (alignment between trust and AI capability) is used as the primary normative criterion rather than trust magnitude.

**RQ2**: Explanations decreased self-reported trust ratings while simultaneously improving performance—a counterintuitive pattern that suggests the relationship between XAI and trust is non-linear and moderated by AI error rate and the quality of the explanations themselves. When explanations clearly flagged AI errors (e.g., by highlighting irrelevant image regions), they reduced overtrust; the authors note this effect may reverse if explanations consistently appear to validate a reliable AI. This is an important conditional, context-dependent finding that complicates simple positive transparency–trust claims.

**RQ3**: The study was designed with a general lay population (no mushroom or AI expertise required). AI knowledge and domain-specific (mushroom) knowledge were measured but neither predicted performance, challenging the assumption that pre-existing expertise moderates XAI effectiveness in this context. The authors suggest the experimental design may have suppressed the role of AI knowledge by preventing exploratory interaction.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
