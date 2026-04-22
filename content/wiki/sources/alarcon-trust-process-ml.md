# The Trust Process Applied to Machine Learning Algorithms: The Influence of Calibrated Confidence Estimates

**Source file**: [Original article](../../raw/Alarcon et al._The Trust Process Applied to Machine Learning Algorithms The Influence of Calibrated Confidence Estimates.pdf)

**Summary**: Across three online experiments (total N = 396), Alarcon et al. compare user task performance and trustworthiness perceptions when working with either a calibrated classification model (CCM) or an uncalibrated classification model (UCM), finding that CCMs improve performance in difficult conditions and yield qualitatively higher trust descriptions, though quantitative trustworthiness differences are inconsistent.

**Sources**: Alarcon et al._The Trust Process Applied to Machine Learning Algorithms The Influence of Calibrated Confidence Estimates.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

This study investigates how calibrated confidence estimates — a form of performance transparency in ML image-classification models — affect user task performance, perceived trustworthiness, and reliance intentions. The authors situate the work within the Lee and See (2004) trust-in-automation framework, which decomposes trustworthiness perceptions into performance, purpose, and process components, alongside reliance intentions and actual reliance behaviors.

Three between-subjects online experiments were conducted using Amazon Mechanical Turk (CloudResearch), each with approximately 130 participants (N = 130, 134, 132 after cleaning). Participants monitored an image-binning task in which a ResNet50-based algorithm classified images of cats, dogs, and (in Studies 2–3) out-of-distribution animals. The CCM condition displayed color-coded confidence borders (green = high confidence ≥ 80%; yellow = low confidence < 80%), while the UCM displayed uniformly high confidence regardless of out-of-distribution content. Trustworthiness was measured with the 15-item System Trustworthiness Scale (STS), and reliance intentions with a 10-item scale.

The three studies sequentially added complexity: Study 1 used only in-distribution images; Studies 2 and 3 added out-of-distribution images; Study 3 also collected open-ended qualitative strategy data. The domain is a controlled laboratory analogue with no specific applied domain, though findings are positioned as relevant to image classification applications such as medical screening.

## Key Findings

- In Studies 2 and 3 (with out-of-distribution data), participants in the CCM condition performed significantly better on harder task rounds (those requiring five corrections), but not on easier rounds (domain: laboratory image classification).
- Decision time was significantly faster for CCM users in Studies 2 and 3 (p = 0.018; p < 0.001), indicating greater reliance on the algorithm's color-coded signals rather than manual inspection of each image (domain: laboratory image classification).
- Quantitative trustworthiness perceptions (performance, purpose, process subscales) did not differ significantly between CCM and UCM conditions in Studies 2 and 3; in Study 1, performance and purpose perceptions increased over time for all participants regardless of condition (domain: laboratory image classification).
- Performance and process perceptions were unique positive predictors of reliance intentions across all three studies (performance: β = 1.07, p < 0.001; process: β = 0.30, p = 0.002 in Study 3), while purpose was not a significant independent predictor (domain: laboratory image classification).
- Qualitative analysis in Study 3 revealed that CCM users described trusting the algorithm 40% more frequently and "low trust" 100% less frequently than UCM users; CCM users also reported focusing on the yellow confidence borders as their primary strategy, indicating behavioral reliance differences not fully captured by quantitative scales (domain: laboratory image classification).
- Users of UCMs more often reported ignoring the algorithm entirely (150% more than CCM users), underscoring that miscalibrated confidence estimates can suppress appropriate reliance (domain: laboratory image classification).

## Transparency Constructs

The study operationalizes **performance transparency** through calibrated confidence estimates — color-coded uncertainty signals indicating the probability that a classification is correct. This is distinct from process transparency (how the decision was made) or outcome transparency (what the decision was). The CCM's lower confidence signal for out-of-distribution data is treated as a transparent indicator of model uncertainty. The authors note that process perceptions did not differ between conditions, confirming that confidence displays convey performance information without revealing the underlying model process.

## Trust Constructs

Trust is decomposed into three trustworthiness dimensions:
- **Performance perceptions**: judgments about the system's ability to do the task
- **Purpose perceptions**: beliefs about appropriate and intended use of the system
- **Process perceptions**: sense of understanding how the machine reaches decisions

Reliance intentions (attitudinal willingness to rely) and actual reliance behavior (decision time, concurrence rate) are measured as downstream outcomes. The study uses behavioral reliance as a key dependent variable alongside self-report, consistent with the Lee and See (2004) model.

## Relevance to Research Questions

**RQ1**: The paper operationalizes trustworthiness as a three-component construct (performance, purpose, process) using the System Trustworthiness Scale (STS), providing a validated instrument relevant to AI transparency research. It distinguishes confidence/uncertainty displays as a form of performance transparency, separate from explainability or process transparency.

**RQ2**: The relationship between transparency and trust is **conditional**: calibrated confidence estimates improved behavioral reliance and decision speed, but did not consistently alter self-reported trustworthiness perceptions across all studies. The effect on task performance was contingent on task difficulty (out-of-distribution data, harder rounds). Qualitative data showed a positive trust relationship with the CCM that quantitative measures failed to capture — suggesting measurement artifact as a moderator.

**RQ3**: The study used exclusively novice participants (recruited via MTurk with no domain expertise), explicitly noting that experienced AI/ML practitioners may respond differently to confidence estimates. Expert users are identified as a key gap; the between-subjects design was chosen in part to avoid learning confounds rather than to examine expertise effects.

## Related pages

- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[rq2-relationships]]
