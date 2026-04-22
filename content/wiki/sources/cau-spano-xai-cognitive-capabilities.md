# Exploring the Impact of Explainable AI and Cognitive Capabilities on Users' Decisions

**Source file**: [Original article](../../raw/Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.pdf)

**Summary**: A pre-registered online experiment (N = 288) comparing six AI assistance conditions — including four XAI explanation styles (example-based, feature-based, rule-based, counterfactual) — in a loan approval task, finding that high AI confidence increases reliance while reducing cognitive load, that counterfactual explanations uniquely improve overall accuracy despite lower perceived understandability, and that Need for Cognition (NFC) does not differentiate accuracy or cognitive load outcomes in this complex, high-stakes task.

**Sources**: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Cau and Spano (2026, published in User Modeling and User-Adapted Interaction) conduct an online user study (N = 288; 144 male, 144 female; mean age 32.42) using the Prolific platform and LimeSurvey to investigate how different forms of AI assistance affect loan approval decision-making. The study employs a mixed-factorial design: AI assistance condition was a between-subjects factor (six levels — no AI; AI prediction only; AI + example-based; AI + feature-based; AI + rule-based; AI + counterfactual), while AI confidence (low vs. high) and AI correctness (correct vs. wrong) were within-subjects covariates.

The AI model was a Random Forest Classifier (83% test-set accuracy) trained on a publicly available Loan Prediction Problem Dataset. Explanation methods included: SHAP for feature-based explanations, Anchors for rule-based, DiCE for counterfactual, and nearest-neighbor retrieval for example-based. Each participant completed eight main-session tasks (plus eight practice trials). Participants were incentivized with monetary bonuses for correct decisions to simulate high-stakes conditions. The study also measured the Need for Cognition (NFC) personality trait (six-item NCS-6 scale) and examined whether NFC moderated the effects of AI assistance on accuracy, cognitive load, and prioritization of interface elements. Attention checks were embedded throughout.

The study is notable for using a one-stage AI paradigm (AI assistance shown alongside the task), testing four distinct explanation styles under a single protocol, and examining the role of AI confidence level as a within-subjects moderator.

## Key Findings

- High AI confidence significantly increased users' reliance on AI predictions compared to low AI confidence (Log-Odds = 1.22, p < .01), and significantly reduced cognitive load (Log-Odds = -0.41, p < .01), confirming the central role of confidence calibration in shaping AI reliance behavior (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)
- Feature-based explanations (SHAP) did not significantly improve users' accuracy compared to other AI assistance conditions, contradicting the hypothesis that feature attribution would best satisfy trust calibration desiderata in tabular-data tasks (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)
- Counterfactual explanations (DiCE) were perceived as less understandable but showed a positive trend toward improving overall accuracy; specifically, they increased reliance on AI and reduced cognitive load when AI predictions were correct, though they showed a trend toward decreasing accuracy in those same correct-prediction contexts, suggesting a nuanced trade-off (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)
- Both low and high NFC participants prioritized loan application attributes first (rank 1), explanations second (rank 2), and AI information third (rank 3), contrary to the hypothesis that low NFC individuals would prioritize AI information over explanations (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)
- No significant differences were found between low and high NFC groups in accuracy or cognitive load when exposed to explanations, suggesting that NFC's predictive value for AI-assisted decisions may diminish as task complexity and stakes increase (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)
- Post hoc analysis showed that when AI confidence is high, users shift from prioritizing explanations equally with AI information (low confidence condition) to prioritizing AI information over explanations, suggesting high confidence anchors attention on the AI prediction itself rather than accompanying justifications (finance/loan approval domain). (source: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.txt)

## Transparency Constructs

The study systematically compares four distinct XAI explanation styles applied to a tabular-data classification task:

- **Example-based explanations** ([[example-based-explanations]]): Three nearest-neighbor training instances with highlighted differing features, intended to illustrate the AI's predicted class through analogous cases.
- **Feature-based explanations** ([[explainability]]): SHAP feature contributions displayed as an interactive vertical bar chart, showing each attribute's positive or negative influence on the AI prediction.
- **Rule-based explanations**: Anchors-generated if-then predicates with precision and coverage statistics, providing a transparent decision boundary.
- **Counterfactual explanations** ([[counterfactual-explanations]]): DiCE-generated diverse counterfactual instances showing what feature changes would alter the prediction, representing contrastive "what-if" reasoning.

AI information (prediction, confidence score in percentage, and test-set accuracy) is also examined as a transparency mechanism distinct from explanation styles. The study addresses [[uncertainty-visualization]] implicitly through the role of AI confidence level.

## Trust Constructs

Trust is not measured through a dedicated psychometric scale. The study uses **reliance on AI** (agreement with AI prediction per trial) as the primary behavioral proxy for trust, which maps to [[behavioural-trust]] and [[appropriate-reliance]]. **Cognitive load** (Single Ease Question, 7-point scale) is used as a secondary outcome. The paper extensively discusses [[trust-calibration]] — the importance of calibrating AI confidence estimates to reflect actual correctness so that users do not over- or under-rely. The study also touches on [[algorithm-aversion]] implicitly, noting that users may under-rely on correct AI suggestions when AI confidence is low. The role of AI stated accuracy as a trust anchor aligns with [[cognitive-trust]] (rational evaluation of AI competence based on reported metrics).

## Relevance to Research Questions

**RQ1**: The paper systematically operationalizes four distinct explanation styles in a controlled tabular-data context, contributing a comparative empirical reference for how different forms of XAI transparency influence decision outcomes. It also distinguishes AI information (prediction, confidence, accuracy) as a distinct transparency class from explanations, with separable effects on reliance and cognitive load.

**RQ2**: The study reports a complex pattern: high AI confidence increases reliance and reduces cognitive load regardless of explanation style; feature-based explanations (conventionally favored) do not reliably improve accuracy; counterfactual explanations show a non-intuitive pattern of improving accuracy overall while reducing understandability, and showing an interaction with AI correctness. These findings illustrate that the transparency-trust-performance relationship is non-linear and depends on the type of transparency mechanism and the correctness of the AI prediction.

**RQ3**: Need for Cognition (NFC), a personality-based proxy for cognitive engagement, is the key user characteristic examined. Contrary to prior literature in low-stakes domains (music recommendation, nutrition), NFC did not moderate accuracy or cognitive load outcomes in this high-stakes loan task. The study concludes that NFC's discriminating power may be task-specific, diminishing under high complexity. This constitutes direct evidence that standard individual-difference moderators may not generalize across domain contexts, with implications for RQ3.

## Related pages

- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[explainability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
