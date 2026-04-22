# Designing for Confidence: The Impact of Visualizing Artificial Intelligence Decisions

**Source file**: [Original article](../../raw/Karran et al._Design for confidence.pdf)

**Summary**: Two studies (N=206 online; N=19 eye-tracking lab) examining how visualization design choices — specifically adjacency (overlay vs. separate display) and morphological clarity (low/medium/high visual precision) of AI explanation visualizations — affect user confidence in AI decision systems, finding that adjacent, lower-clarity explanations maximize confidence.

**Sources**: Karran et al._Design for confidence.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Karran, Demazure, Hudon, Senecal, and Léger (2022) investigate how the visual design of AI explanation visualizations (EVs) affects user *confidence* in AI systems. The authors argue that existing XAI research has focused too heavily on algorithmic correctness and too little on the human cognitive experience of consuming explanations. They use Cognitive Fit Theory (Vessey, 1991) as a theoretical frame: when the format of information matches the cognitive requirements of the task, processing is more efficient and performance is better.

Two design factors are manipulated:
- **Adjacency**: whether the explanation overlay appears directly on the original image (adjacent) or on a black background separated from the image (non-adjacent).
- **Morphological Clarity (MC)**: three levels — low (cloud of points, CP: pixel-level attribution, high noise), medium (heatmap, HM: focal activation), high (outline, ON: clean boundary but low pixel-level precision).

**Study 1** (N=206 online via MTurk, ~60% male, avg. age 37.9) used a 2×3 within-subjects design. Participants completed 50 visual decision-making trials: they saw an image, its AI classification, an explanation visualization, and were asked "Given the information above, I am confident that the system will correctly identify the next picture" (7-point Likert).

**Study 2** (N=19 lab, avg. age 24.9) replicated with eye-tracking (Tobii ε60) to measure cognitive load via pupillometry, and a mediation analysis tested whether cognitive load mediated the confidence effect.

The AI system used was Xception (pretrained on ImageNet, accuracy 0.79), with explanations generated via Integrated Gradients (for CP and ON visualizations) and Grad-CAM (for HM visualizations).

## Key Findings

- Adjacent EVs resulted in significantly higher confidence than non-adjacent EVs (M=5.01 vs. M=4.55, t(205)=15.71, p<0.001). [Domain: general AI / computer vision]
- Unexpectedly, **low MC (cloud of points) EV produced higher confidence than high MC (outline)** (M=4.85 vs. M=4.73, p=0.001) — opposite to the hypothesis that cleaner visualizations would be more confidence-inspiring. [Domain: general AI / computer vision]
- The interaction showed that adjacent EVs of all three MC levels were approximately equivalent in confidence impact; the significant MC effect was driven by non-adjacent conditions where low MC outperformed medium and high MC. [Domain: general AI / computer vision]
- In non-adjacent conditions, low MC allowed users to still perceive the object's shape (e.g., monkey's head visible in the point-cloud EV), whereas medium and high MC non-adjacent EVs were too abstract to identify forms — explaining why low MC maintained higher confidence even when separated from the image. [Domain: general AI / computer vision]
- Correct AI classifications resulted in significantly higher confidence than incorrect ones (M=5.27 vs. M=4.29, p<0.001), confirming that AI accuracy is a strong moderator of confidence. [Domain: general AI / computer vision]
- In Study 2, cognitive load was directly affected by both adjacency (p<0.001) and MC (p<0.001), but cognitive load did **not** mediate the effect of adjacency or MC on confidence (H3 not supported). The indirect effect via cognitive load was non-significant for both adjacency (CI95%[−0.885; 0.408]) and MC (CI95%[−0.615; 0.655]). [Domain: general AI / computer vision]
- Counterintuitively, low MC adjacent visualizations showed the lowest cognitive load despite having the highest information density — the authors suggest this may reflect a shift from cognitive to perceptual processing, or engagement of "fast thinking" (System 1 in Kahneman's framework). [Domain: general AI / computer vision]
- 61 of 206 participants self-identified as AI/Data experts; the main analysis does not break down results by expertise, but the authors note as a future limitation that AI expertise may moderate the confidence–EV relationship. [Domain: general AI / computer vision]

## Transparency Constructs

The paper operationalizes transparency as **visual attribution explanations** — explanation visualizations (EVs) that highlight which regions of an input image drove the AI's classification. This is a form of [[explainability]] (specifically image-based attribution/saliency) operationalized through two design parameters: how explanations are spatially positioned relative to the original image (adjacency) and how precise/noisy the explanation is (morphological clarity).

The paper contributes an important nuance: **more information in an explanation (low MC) can increase perceived transparency and confidence** even when that information includes noise. This aligns with findings by Brunk et al. (2019) that black-box algorithms are perceived as more transparent and trustworthy when additional information is present, regardless of its usefulness. The finding challenges the common assumption that cleaner, higher-precision explanations are always better.

The authors also introduce **causability** (Holzinger et al., 2020) as a desirable property — the ability of an explanation to reach a specified level of causal understanding for a user — and suggest it as a more appropriate measurement target than simple transparency for future XAI research.

## Trust Constructs

The authors deliberately use **confidence** rather than trust as their primary construct, arguing that trust in AI is not a psycho-affective relationship in the same sense as trust in humans (citing DeCamp and Tilburt, 2019). Confidence is defined as a measure of how sure users are that they received correct suggestions and whether the system is reliable, functional, and helpful (Lankton et al., 2015).

This conceptualization maps most closely onto [[cognitive-trust]] — the rational/competence-based component of trust — specifically the belief that the system will correctly perform its function. The paper shows that design choices in explanation visualization can significantly shift this confidence level, with adjacency being the dominant factor.

The mediation results showing cognitive load does not mediate the confidence effect are notable: design affects confidence through pathways *other than* cognitive load reduction alone, suggesting that visual affordances (enabling perceptual processing) or epistemic uncertainty reduction may be proximal mechanisms.

## Relevance to Research Questions

**RQ1**: The paper operationalizes transparency as EV design (adjacency + MC) and measures confidence (a form of cognitive trust) via 7-point Likert scale. It contributes a user-centered, design-focused approach to operationalizing transparency — distinguishing between different visual formats of the same underlying explanation and measuring their differential impact on confidence. See [[rq1-conceptualizations]].

**RQ2**: The paper reports that transparency (explanation visualization) positively affects confidence when designed with adjacency, but the relationship is conditional on design choices: non-adjacent high-MC visualizations can produce lower confidence than no explanation at all. This is a key conditional finding — not all explanations help, and poorly designed transparency can backfire. The effect of MC is opposite to theoretical expectation (low MC > high MC), pointing to a non-obvious, non-linear relationship. See [[rq2-relationships]].

**RQ3**: The study does not systematically analyze user expertise as a moderator, though 61 participants self-identified as AI/Data experts. The authors explicitly flag this as a limitation and suggest future work should investigate whether AI expert confidence responds differently to EV types. The restriction to North American MTurk participants avoids linguistic confounds but limits generalizability to other cultural contexts. See [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[cognitive-trust]]
- [[causability]]
- [[algorithmic-transparency]]
- [[user-expertise]]
- [[rq2-relationships]]
