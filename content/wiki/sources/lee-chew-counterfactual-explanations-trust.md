# Understanding the Effect of Counterfactual Explanations on Trust and Reliance on AI for Human-AI Collaborative Clinical Decision Making

**Source file**: [Original article](../../raw/Lee & Chew_Understanding the effect of counterfactual explanations on trust.pdf)

**Summary**: A within-subject experiment with 7 therapists and 10 laypersons on stroke rehabilitation assessment shows that counterfactual (what-if) explanations reduce overreliance on wrong AI outputs by 21% compared to salient feature explanations, while simultaneously producing lower self-reported trust scores — suggesting counterfactual explanations promote more calibrated rather than higher trust.

**Sources**: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Lee and Chew (2023), published in *Proceedings of the ACM on Human-Computer Interaction (CSCW2)*, investigate how two types of AI explanations affect users' trust and reliance in a clinical decision-support context. The task is physical stroke rehabilitation assessment — specifically, rating the Range of Motion (ROM) and Compensation of post-stroke patients performing arm exercises. The AI model is a feed-forward neural network trained on kinematic sensor data from 15 post-stroke survivors.

Two conditions are compared within-subjects:
- **Condition A (Features)**: AI prediction score + salient feature analysis (top-3 SHAP features displayed as a radar chart comparing unaffected and affected sides).
- **Condition B (Counterfacts)**: Condition A + counterfactual explanations — text descriptions of which feature values would need to change to flip the AI's prediction, generated via DiCE.

Each condition included 8 cases: 3 with correct AI outputs ("right") and 5 with incorrect AI outputs ("wrong"). Cognitive forcing functions were applied to both conditions (hidden AI outputs until requested, brief loading delay). The within-subject order was counterbalanced.

Outcomes: task performance (F1 score), agreement level, counts of right/wrong decisions, decision duration, and usability questionnaires including a 100-point trust scale.

## Key Findings

- Counterfactual explanations reduced overreliance on wrong AI outputs by 21% (29/136 decisions) overall; by 8% (5/56) for therapists and by 30% (24/80) for laypersons (domain: healthcare / stroke rehabilitation). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- When right AI outputs were presented, both salient feature and counterfactual explanations improved performance relative to human-alone; when wrong AI outputs were presented, both conditions degraded performance, but counterfactual degradation was lower (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- Therapists had lower performance degradation with wrong outputs than laypersons: 8.6 vs 18.0 F1-score degradation with salient features; 2.8 vs 14.0 F1-score degradation with counterfactual explanations (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- Salient feature explanations increased agreement level even when AI outputs were wrong (i.e., drove participants toward the wrong answer in concert), while counterfactual explanations decreased agreement level for wrong outputs, indicating that participants were more willing to diverge from each other and from the AI (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- Self-reported trust was significantly higher for the salient-feature condition (mean 73.78/100) than for the counterfactual condition (mean 45.20/100), despite the counterfactual condition producing better decision outcomes; the counterfactual trust score was closer to the actual AI accuracy (0.375 = 3 right / 8 total) (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- Participants generally preferred the salient feature system (7 participants) over the counterfactual system (7 participants), with 1 neutral — an even split despite worse performance outcomes with salient features; feature-based system was rated as more useful, requiring less effort, more transparent and trustworthy. (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- Counterfactual explanations took on average 18 more seconds per decision than salient feature explanations (75 vs 57 seconds total), confirming additional cognitive burden (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- The positive correlation between (self-reported) trust and reliance was confirmed: higher trust predicted higher reliance even on wrong AI outputs, consistent with Bussone et al. (2015) (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)
- A gap between subjective usability perceptions and objective performance is documented: users perceived the feature-based system as more trustworthy, useful, and transparent, yet it produced worse team performance (domain: healthcare). (source: Lee & Chew_Understanding the effect of counterfactual explanations on trust.txt)

## Transparency Constructs

The study directly compares two forms of local explanation:

- **Salient feature analysis**: SHAP-based feature-importance scores displayed as a radar chart. This is the standard instance-level [[explainability]] approach providing positive confirmation of the AI's reasoning.
- **Counterfactual explanations**: DiCE-generated what-if descriptions — textual statements of how input features would need to change to alter the AI prediction. This is [[counterfactual-explanations]], a form of contrastive explanation.

The paper's central theoretical argument is that salient feature explanations confirm existing reasoning (confirming heuristics), while counterfactual explanations function as **cognitive forcing functions** — prompting users to analytically consider alternative scenarios rather than automatically accepting the AI output. This is a functionally distinct mechanism of transparency, linking [[counterfactual-explanations]] to over-reliance mitigation.

Both conditions also included multiple cognitive forcing strategies (hidden AI output by default, brief loading delay) applied equally, so differences are attributable to explanation type.

## Trust Constructs

The paper operationalises multiple trust-related constructs:

- **Self-reported trust**: single 100-point Likert item; this subjective measure diverges from behavioural outcomes, illustrating the gap between [[cognitive-trust]] (felt trust) and actual calibration.
- **Reliance (behavioural trust)**: measured as agreement with AI outputs, with separate counts for agreeing with right vs wrong AI outputs, rejecting right vs wrong outputs — a fine-grained [[behavioural-trust]] measure.
- **Trust calibration**: the paper explicitly argues that counterfactual explanations produce better-calibrated trust — trust more aligned with actual AI performance — even though subjective trust scores are lower. See [[trust-calibration]].
- **Overreliance**: operationalised as agreeing with a wrong AI output — a critical form of miscalibrated trust that the paper addresses. See [[appropriate-reliance]].
- **Affective trust dimensions**: usability questionnaires include items on frustration, usage intent, and trust, capturing both cognitive and affective dimensions.

## Relevance to Research Questions

**RQ1**: The paper operationalises both explanation types and trust carefully, distinguishing subjective trust from behavioural reliance and from calibration. This is a key contribution to understanding how explanation type shapes different facets of trust. The finding that subjective trust and calibrated reliance are in tension with each other challenges single-metric operationalisations of trust. See [[rq1-conceptualizations]].

**RQ2**: The central finding is a conditional relationship: counterfactual explanations reduce overreliance on wrong AI outputs (a positive calibration effect) while also producing lower subjective trust. The direction of the transparency-trust relationship thus depends on which trust facet is measured. For self-reported trust, counterfactuals produce lower scores; for actual calibration and decision quality, they produce better outcomes. This non-linear / conditional pattern is directly relevant to RQ2. See [[rq2-relationships]].

**RQ3**: The comparison between therapists (domain experts with average 12.85 years of experience) and laypersons (students with no rehabilitation experience) is a core design feature. Therapists showed consistently lower performance degradation and lower overreliance on wrong AI outputs than laypersons across both explanation conditions. Counterfactual explanations benefited both groups but the benefit was proportionally larger for laypersons in reducing overreliance. This is direct empirical evidence that user expertise moderates the transparency-trust-reliance relationship. See [[rq3-user-roles]].

## Related pages

- [[counterfactual-explanations]]
- [[explainability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq3-user-roles]]
- [[rq2-relationships]]
