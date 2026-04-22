# Knowing (Not) to Know: Explainable Artificial Intelligence and Human Metacognition

**Source file**: [Original article](../../raw/von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.pdf)

**Summary**: Two incentivised experiments with domain experts (real estate agents and finance professionals) demonstrate that global XAI explanations improve metacognitive accuracy — specifically by reducing overconfidence — which in turn causally increases both the frequency and quality of human-to-AI task delegation.

**Sources**: von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *Information Systems Research* (Articles in Advance, December 2025), this paper by Moritz von Zahn, Lena Liebich, Ekaterina Jussupow, Oliver Hinz, and Kevin Bauer (Goethe University Frankfurt; Leibniz Institute SAFE; TU Darmstadt) introduces a novel theoretical mechanism through which XAI affects human-AI collaboration: **metacognitive processes**.

The paper argues that prior XAI research has focused on how explanations affect object-level cognition (reasoning, learning, trust in specific predictions) while overlooking how explanations affect how people "think about their thinking" — i.e., metacognitive monitoring (confidence calibration) and metacognitive control (delegation decisions).

Two experiments were conducted:
- **Study 1** (n = 149): German real estate agents predicting apartment listing prices. XAI treatment: SHAP global dependence plots for each apartment feature.
- **Study 2** (n = 200, effective 152): Finance and insurance professionals predicting peer-to-peer loan repayment outcomes. XAI treatment: SHAP global dependence plots + local SHAP values for three example cases.

Both studies used a between-subjects design: XAI condition (access to AI's overall prediction logic) vs. black-box condition (no explanation). Participants could delegate each prediction task to an AI or retain it; AI predictions were hidden until the end. No intermediary feedback was given.

The XAI tool used was SHAP (Shapley Additive Explanations) global partial-dependence plots — a widely adopted feature-based explanation method.

## Key Findings

- XAI significantly improved **metacognitive calibration** (Study 1: overconfidence reduced from 43.3 to 29.3 percentage points, −32.3%, p < 0.01; Study 2: overconfidence gap reduced from 11.8 to 4.2 pp, −64.4%, p = 0.018). [domain: real estate pricing; financial services / P2P lending]
- The calibration improvement was driven entirely by **reduced confidence** in own abilities (not improved performance), indicating a metacognitive adjustment rather than learning from AI explanations. [domain: real estate, finance]
- XAI significantly increased **delegation frequency** (Study 1: 41% → 54%, +31.7%, p < 0.01; Study 2: 53.5% → 59.1%, +10.5%, p < 0.01). [domain: real estate, finance]
- XAI improved **delegation effectiveness**: participants in the XAI condition made better task-allocation decisions, reducing mean absolute prediction error for retained tasks by 39.2% (Study 1, p < 0.02). [domain: real estate]
- Causal mediation analysis confirmed that approximately 23% (Study 1) and 104% (Study 2) of XAI's effect on delegation frequency is mediated by improved metacognitive calibration. [domain: real estate, finance]
- XAI improved **metacognitive resolution** — confidence judgments better discriminated between tasks participants were likely to perform well and poorly, with confidence declining more sharply for difficult tasks (L-loans) than easy tasks (H-loans) (Study 2). [domain: financial services / P2P lending]
- XAI effects on metacognition occurred **primarily when participants perceived misalignment** between their own prediction logic and the AI's logic, triggering reduced confidence. Participants perceiving high alignment showed no meaningful calibration adjustment. [domain: real estate, finance]
- XAI modestly increased **cognitive trust** in the AI (+0.93 points on a 7-point scale, p < 0.01), but cognitive trust mediated only delegation frequency (31.4%), not delegation effectiveness, confirming that metacognitive accuracy — not trust — explains the key performance benefit. [domain: real estate]
- Despite improved delegation, humans and AI together did not achieve full complementarity: the XAI treatment condition's mean absolute error (€183,929) remained significantly above the AI-alone error (€113,524) and the ideal-delegation error (€92,450). [domain: real estate]
- Some experts in the XAI condition began to over-delegate, undervaluing their own abilities for tasks they were actually well-suited to perform — pointing to a risk of XAI-induced underconfidence. [domain: real estate, finance]

## Transparency Constructs

The paper operationalises XAI as **global explanations** — SHAP-based partial-dependence plots showing the average relationship between each input feature and the AI's predictions across the dataset. This is distinguished from **local explanations** (instance-specific reasoning).

The key transparency mechanism identified is the AI's **prediction logic disclosure**: making the AI's learned feature–outcome relationships visible. This form of transparency is a type of [[algorithmic-transparency]] and [[process-transparency]], operating at the aggregate (model) level rather than the case level.

The paper explicitly discusses global vs. local explanations as distinct forms of transparency, arguing that global explanations may be especially suited to delegation settings because they help users assess their own relative capability across task types rather than evaluate individual AI predictions.

## Trust Constructs

- **[[cognitive-trust]]**: Measured using Komiak and Benbasat's (2006) scale; found to increase with XAI (+0.93 points, p < 0.01). Partially mediates delegation frequency but not delegation effectiveness.
- **[[behavioural-trust]]** (delegation/reliance): The primary outcome — XAI increases both frequency and effectiveness of delegation to AI.
- **[[trust-calibration]]**: A core implicit construct. The metacognitive calibration improvement directly operationalises trust calibration at the individual level — humans become more accurate in assessing when to trust themselves vs. the AI.
- **[[appropriate-reliance]]**: The paper frames "effective delegation" as the ideal outcome: retaining tasks where human performance is superior, delegating where it is not. XAI moves humans toward appropriate reliance, though not fully.

## Relevance to Research Questions

**RQ1**: Introduces metacognitive accuracy (calibration and resolution) as a previously overlooked mechanism through which XAI affects human-AI collaboration. Operationalises XAI as global SHAP explanations. Conceptualises delegation as a metacognitive control decision governed by confidence judgments. Adds a new theoretical lens (metacognition) to XAI and trust research. (source: von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.txt)

**RQ2**: Documents that XAI improves trust calibration (reducing overconfidence) and delegation effectiveness through a metacognitive pathway — distinct from and complementary to the cognitive trust pathway. The relationship between transparency and reliance is positive but conditional on perceived logic misalignment. Identifies a risk of XAI-induced underconfidence (a potential negative transparency effect). The effect on delegation effectiveness operates primarily through metacognition rather than through trust change. [domain: real estate; P2P lending/finance] (source: von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.txt)

**RQ3**: Both studies recruited domain experts (real estate agents; finance/insurance professionals), making this a study of how expert users respond to XAI. In Study 1, more experienced real estate agents may respond differently to explanations that reveal divergence from their established reasoning. The paper does not explicitly compare expert vs. novice populations but the expert sample is a relevant constraint on generalisability. (source: von-zahn-et-al-2025-knowing-(not)-to-know-explainable-artificial-intelligence-and-human-metacognition.txt)

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
