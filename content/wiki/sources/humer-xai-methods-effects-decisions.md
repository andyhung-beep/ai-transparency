# Reassuring, Misleading, Debunking: Comparing Effects of XAI Methods on Human Decisions

**Source file**: [Original article](../../raw/Humer et al._Reassuring, misleading, debunking.pdf)

**Summary**: This between-subjects experiment (N = 501) compares three XAI methods — Grad-CAM attributions, nearest-neighbor examples, and network-dissection concepts — on trust calibration in a high-risk mushroom identification task, finding that nearest-neighbor examples most reliably improve decision correctness and help users avoid overtrust, while the effects of Grad-CAM and network-dissection are inconclusive or context-dependent.

**Sources**: Humer et al._Reassuring, misleading, debunking.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Humer et al. (2024), published in *ACM Transactions on Interactive Intelligent Systems*, investigate which XAI methods are most effective at calibrating user trust in AI-assisted decision-making. The study is embedded in a gamified virtual mushroom-hunting scenario — a relatable, high-stakes context (wrong decisions could be dangerous). Participants (N = 501) were randomly assigned to one of four conditions: no explanation (control), Grad-CAM attribution maps (E1), nearest-neighbor image examples (E2), or network-dissection concept labels with highlighted regions (E3). Performance was measured as correct edibility assessments and correct take/leave decisions across 10 task items. The study builds on two prior studies by the same group and contributes item-level and subset analyses that illuminate when and why specific explanations help or mislead.

## Key Findings

- Nearest-neighbor examples (E2) significantly improved overall decision performance (edibility assessment and take/leave decisions) compared to the control group; Grad-CAM (E1) and network-dissection (E3) effects did not reach statistical significance at the aggregate level. [domain: general/public/nature-identification]
- For wrongly classified items (measuring overtrust), nearest-neighbor (E2) showed significantly better performance, suggesting it helps users identify AI errors. Network-dissection (E3) showed a trend toward helping users avoid distrust (follow correct AI predictions), but was not significant. [domain: general/public/nature-identification]
- Helpful explanations (those whose content accorded with the AI's reliability on a given item) produced larger positive effects; the effect of misleading explanations could not be statistically confirmed but performance was lower than for helpful explanations. [domain: general/public/nature-identification]
- Effects on self-reported trust, system evaluation, and intention to use did not reach statistical significance for any explanation method — replicating the null subjective-trust result from the authors' prior festival study, but contradicting an earlier online study that found reduced trust with explanations. [domain: general/public/nature-identification]
- Correlation analysis showed that nearest-neighbor (E2) and network-dissection (E3) participants relied less on their general propensity to trust automation when rating trust in the specific system — suggesting explanations helped participants form more system-specific (calibrated) trust judgments. [domain: general/public/nature-identification]
- Grad-CAM alone (without nearest-neighbor examples) yielded inconclusive effects; the authors speculate that positive effects in prior studies were primarily due to the nearest-neighbor component of the combined interface. [domain: general/public/nature-identification]
- No single explanation method served all items well: explanations can both reassure (validate correct predictions), mislead (validate incorrect predictions), or debunk (expose incorrect predictions) depending on item characteristics. [domain: general/public/nature-identification]

## Transparency Constructs

The paper examines three operationalizations of [[explainability]] for image classification:
- **Grad-CAM** (attribution-based): highlights image regions driving predictions — a form of [[outcome-transparency]] linking input features to outputs.
- **Nearest-neighbor examples** ([[example-based-explanations]]): displays training images closest to the input per predicted class, enabling users to compare similarity.
- **Network-dissection** (concept-based): assigns semantic concept labels (e.g., "gills of mushroom species X") to neural network units and highlights the corresponding image region, combining [[causability]] cues with visual attribution.

## Trust Constructs

The primary outcome is [[trust-calibration]], operationalized behaviourally (decision correctness on correct vs. incorrect AI items) and via self-report (Trust in Automation questionnaire, system evaluation, intention to use). The paper frames appropriate reliance as the union of two failure modes: overtrust (following wrong AI predictions) and distrust (overriding correct AI predictions). This dual operationalization of [[appropriate-reliance]] is a key methodological contribution. [[behavioural-trust]] is the primary measured construct; self-reported trust (closer to [[cognitive-trust]]) showed no significant effects.

## Relevance to Research Questions

**RQ1**: The paper operationalizes trust calibration through both behavioural and self-report measures and provides a clear framework distinguishing overtrust from distrust as the two failure modes of inappropriate reliance. It operationalizes three types of XAI explanations with distinct information theories (attribution, example, concept), contributing to how XAI methods are categorized and measured.

**RQ2**: The paper directly addresses which explanation methods produce positive, null, or negative effects on decision correctness and trust calibration. Nearest-neighbor examples show a consistent positive relationship; Grad-CAM is largely null; network-dissection shows possible benefits for distrust reduction. The item-level analysis is especially valuable, showing that explanation effects are not uniform and that even effective methods can mislead on certain inputs — documenting the non-uniform, context-conditional nature of XAI–trust relationships.

**RQ3**: The sample was explicitly designed to represent end-users (general public, not AI experts or domain experts). The study reports that domain knowledge (mushroom and AI knowledge) did not differ significantly across groups, and prior studies found domain knowledge had no significant effect on performance. This directly addresses the question of how non-expert user populations respond to XAI — though the paper does not compare expert vs. non-expert subgroups within this study.

## Related pages

- [[explainability]]
- [[example-based-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[rq2-relationships]]
