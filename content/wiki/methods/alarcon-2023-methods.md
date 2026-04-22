# Alarcon et al. (2023) — Methods

**Summary**: Three between-subjects online experiments (total N = 396) comparing user task performance and trustworthiness perceptions when working with a calibrated versus uncalibrated ML image-classification model recruited via Amazon Mechanical Turk (CloudResearch).

**Sources**: Alarcon et al._The Trust Process Applied to Machine Learning Algorithms The Influence of Calibrated Confidence Estimates.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (three between-subjects online experiments conducted sequentially)

## Sample
- N: 396 (Study 1: N = 130; Study 2: N = 134; Study 3: N = 132, after data cleaning)
- Population: general public, no domain expertise required
- Domain: laboratory image classification (no specific applied domain; positioned as relevant to image-classification applications such as medical screening)
- Country / region: United States (Amazon Mechanical Turk / CloudResearch)
- Recruitment method: Amazon Mechanical Turk via CloudResearch platform

## Transparency operationalization
- Type: performance transparency (calibrated confidence estimates / uncertainty communication)
- Manipulation or measure: between-subjects manipulation — Calibrated Classification Model (CCM) displayed color-coded confidence borders (green ≥ 80% confidence; yellow < 80% confidence) around classified images; Uncalibrated Classification Model (UCM) displayed uniformly high confidence regardless of image type or out-of-distribution status
- Scale / instrument name: not applicable (transparency was a design manipulation, not a scale)
- Number of items: not applicable

## Trust operationalization
- Type: cognitive (performance, purpose, process perceptions); behavioural (reliance)
- Measure: trustworthiness measured with the 15-item System Trustworthiness Scale (STS) capturing three subscales — performance perceptions, purpose perceptions, and process perceptions; reliance intentions measured with a 10-item self-report scale; behavioral reliance measured as decision time and concurrence rate with algorithm classifications
- Scale / instrument name: System Trustworthiness Scale (STS); reliance intentions scale (10 items)
- Number of items: 15 (STS); 10 (reliance intentions)
- Behavioural vs self-report: both (decision time and concurrence rate as behavioral; STS and reliance intentions as self-report)

## Moderators and covariates tested
- Task difficulty (easy vs. hard rounds based on number of required corrections): measured by design; distinguishes conditions where CCM benefit appeared versus did not
- Study phase (Study 1 = in-distribution only; Studies 2–3 = with out-of-distribution images): manipulated by design; out-of-distribution content was necessary for CCM advantage to manifest
- Note: user expertise was NOT included as an independent variable; all participants were novice MTurk workers with no ML/AI domain expertise (relevant to RQ3 as a limitation)

## Statistical approach
- Primary analysis method: ANOVA and mixed-model repeated-measures ANOVA for quantitative STS and reliance outcomes; thematic analysis of open-ended strategy descriptions in Study 3
- Software: not reported
- Key model fit or effect size reported: β coefficients for regression of STS subscales onto reliance intentions reported (e.g., performance: β = 1.07, p < 0.001; process: β = 0.30, p = 0.002 in Study 3); p-values reported for ANOVA comparisons; Cronbach's α not reported explicitly in the source summary

## Author-noted limitations
- Sample was exclusively novice users recruited from MTurk; experienced AI/ML practitioners may respond differently to confidence estimates
- The between-subjects design precluded learning-effects analysis within participants
- Quantitative trustworthiness measures (STS) may be insensitive to condition differences that are apparent qualitatively — a potential measurement artifact
- The laboratory image-binning task lacks ecological validity for real-world AI deployment contexts
- Studies 1 and 2 did not collect open-ended qualitative data, limiting triangulation across all three studies

## Related pages
- [[alarcon-trust-process-ml]]
- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[cognitive-trust]]
- [[rq2-relationships]]

## References
Alarcon, G. M., et al. (2023). *The trust process applied to machine learning algorithms: The influence of calibrated confidence estimates*. [Journal not reported in source summary.]

Lee, J. D., & See, K. A. (2004). Trust in automation: Designing for appropriate reliance. *Human Factors, 46*(1), 50–80.
