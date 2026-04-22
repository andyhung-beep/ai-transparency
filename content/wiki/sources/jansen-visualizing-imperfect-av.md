# Visualizing Imperfect Situation Detection and Prediction in Automated Vehicles: Understanding Users' Perceptions via User-Chosen Scenarios

**Source file**: [Original article](../../raw/Jansen et al._Visualizing imperfect situation detection and prediction.pdf)

**Summary**: Two online studies (N=76 replication; N=22 user-uploaded scenarios) using the EDULICIT method to simultaneously elicit public-perceived challenging AV scenarios and evaluate how visualizing AV uncertainty in Situation Detection and Prediction affects user trust, situation awareness, and capability assessments.

**Sources**: Jansen et al._Visualizing imperfect situation detection and prediction.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Jansen et al. (2024) present two studies that use a publicly accessible website to expose general-population participants to automated vehicle (AV) perception visualizations and collect their reactions. The paper introduces **EDULICIT** (Educate & Elicit), a novel method for simultaneously educating the public about real AV capabilities/limitations and eliciting scenarios that users consider challenging for AVs.

**Experiment A** (N=76 US participants, Prolific) replicated results from Colley et al. (2022) comparing a baseline (no visualization) with a combined visualization of Situation Detection, Situation Prediction, and Trajectory Planning in a pre-defined urban driving video.

**Experiment B** (N=22 participants recruited via university flyers, Germany) allowed participants to upload their own videos of scenarios they considered difficult for AVs. The website automatically applied neural-network-based Situation Detection (Detectron2 R101-FPN panoptic segmentation) and Situation Prediction (pedestrian intention via Mordan et al., 2021) to their uploaded footage.

Both experiments measured trust, perceived safety, cognitive load, situation awareness (SART), predictability, and perceived AV capability using the same instruments as Colley et al. (2022).

## Key Findings

- In Experiment A, cognitive load was significantly higher with visualizations (V=825.00, p=0.004, r=−0.39), but no significant effects on trust, perceived safety, or perceived AV capability were found — successfully replicating the non-significant trust effects from Colley et al. (2022). [Domain: automated vehicles]
- Visualizations caused significant visual clutter (V=132.50, p<0.001, r=−0.85), replicating that finding from prior work. [Domain: automated vehicles]
- In Experiment A, participants requested significantly more perception-related and prediction-related information when there was no visualization (baseline), confirming an "information deficit" that could drive over- or undertrust. [Domain: automated vehicles]
- In Experiment B, situation awareness increased significantly with visualizations (t(21)=−3.65, p=0.001, r=−0.75), while trust and perceived safety showed no significant change. [Domain: automated vehicles]
- Lateral control perception and visual reasonability/necessity of visualizations improved significantly in Experiment B. [Domain: automated vehicles]
- Qualitative analysis of user-uploaded videos found that most scenarios deemed challenging by the public involved large intersections and/or multiple vulnerable road users (pedestrians and cyclists); vehicle-only scenarios were less common. [Domain: automated vehicles / public perception]
- Open feedback in both experiments showed participants were surprised (both positively and negatively) by model imperfections such as false detections of pedestrians (e.g., shop window mannequins, construction posts), missed vehicles, and rapid flickering of prediction labels. [Domain: automated vehicles]
- Public misconceptions about AV capabilities were evident: some participants were unaware that AVs could make such detection errors, reinforcing the need for public education tools. [Domain: automated vehicles / public perception]
- Visualizations did not significantly alter trust in either experiment despite increasing information provision and situation awareness, suggesting that the trust–transparency relationship is not simply linear and may require additional factors (e.g., error-free visualization performance, longer exposure) to manifest. [Domain: automated vehicles]

## Transparency Constructs

The paper operationalizes transparency as **visual overlay** of the AV's Situation Detection (semantic segmentation coloring detected objects) and Situation Prediction (pedestrian crossing intention icons) in real-time on driving video. This is an instance of [[uncertainty-visualization]] and [[process-transparency]] at low abstraction level — users see the raw neural network outputs including false positives, misclassifications, and uncertain predictions rather than a summary metric.

The paper distinguishes this approach from higher-abstraction displays (bars, percentages) and argues that showing raw model behavior is more informative about the *causes* of uncertainty, enabling better calibration of user expectations.

The EDULICIT method additionally functions as an education and public communication tool — a form of [[disclosure]] about real AV capabilities to counteract "autonowashing" (Dixon, 2020).

## Trust Constructs

Trust is measured using Körber's (2019) Trust in Automation questionnaire (Trust in Automation and Predictability/Understandability subscales, 5-point Likert). Perceived safety is measured via Faas et al.'s (2020) semantic differentials. The Situational Trust Scale for Automated Driving (Holthausen et al., 2020) sub-scales (Performance, Judgment, Reaction) were also used.

Trust is conceptualized following Lee and See (2004): an attitude toward the system under uncertainty. The explicit goal is **calibrated trust** (Muir & Moray, 1996) — matching user confidence to actual AV reliability to prevent over- and undertrust. The non-significant trust effects, combined with significant situation awareness increases, suggest that visualizations may first improve understanding without necessarily immediately shifting trust ratings, pointing to a temporal gap between comprehension and trust formation. See [[trust-calibration]].

## Relevance to Research Questions

**RQ1**: The study operationalizes AV transparency via situated visual overlays of neural network outputs and trust via the Körber (2019) scale. It contributes a nuanced conceptualization: transparency can increase information provision and situation awareness without directly altering expressed trust, suggesting that trust and comprehension are distinct constructs. See [[rq1-conceptualizations]].

**RQ2**: Both experiments find that visualizing AV uncertainty increases information provision and situation awareness (Experiment B) but does not significantly alter trust in either direction. This is a null finding for trust but a positive finding for situation awareness. The result is consistent with prior work (Colley et al., 2022) and suggests that the transparency–trust relationship may be conditional on other factors (e.g., visualization quality, exposure duration, error rates). See [[rq2-relationships]].

**RQ3**: The study uses general-population samples (not domain experts) in both experiments, so findings reflect lay-user reactions. Experiment B's sample skewed younger and more educated (50% college students), limiting generalizability to older or less tech-savvy users. The paper does not explicitly examine expertise as a moderator. See [[rq3-user-roles]].

## Related pages

- [[uncertainty-visualization]]
- [[trust-calibration]]
- [[process-transparency]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
