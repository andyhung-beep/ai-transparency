# Cau & Spano (2026) — Methods

**Summary**: Pre-registered online between-subjects experiment (N = 288) comparing six AI assistance conditions including four XAI explanation styles (example-based, feature-based, rule-based, counterfactual) in a high-stakes loan approval task, with AI confidence and correctness as within-subjects covariates and Need for Cognition as a user characteristic moderator.

**Sources**: Cau & Spano_Exploring the impact of explainable AI and cognitive capabilities.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (pre-registered online mixed-factorial design; between-subjects on AI assistance condition; within-subjects on AI confidence and correctness)

## Sample
- N: 288 (144 male, 144 female; mean age 32.42)
- Population: general public (Prolific panel participants)
- Domain: finance (loan approval decision-making using a publicly available Loan Prediction Problem Dataset)
- Country / region: not reported (Prolific platform; international)
- Recruitment method: Prolific platform; LimeSurvey for instrument delivery

## Transparency operationalization
- Type: explanation (four XAI explanation styles) and AI information disclosure (prediction, confidence score, test-set accuracy)
- Manipulation or measure: between-subjects manipulation of six AI assistance conditions — (1) no AI assistance; (2) AI prediction only (label + confidence score + stated test-set accuracy = 83%); (3) AI + example-based explanation (three nearest-neighbor training instances with highlighted differing features, generated via k-NN retrieval); (4) AI + feature-based explanation (SHAP feature contributions as interactive vertical bar chart showing positive/negative attribute influence); (5) AI + rule-based explanation (Anchors-generated if-then predicates with precision and coverage statistics); (6) AI + counterfactual explanation (DiCE-generated diverse counterfactual instances showing feature changes that would alter prediction). Within-subjects: AI confidence level (low vs. high) and AI correctness (correct vs. wrong) varied across eight task trials per participant (plus eight practice trials). Monetary bonus for correct decisions to simulate high-stakes conditions.
- Scale / instrument name: not applicable for manipulation; perceived understandability assessed via self-report rating per explanation condition
- Number of items: not applicable

## Trust operationalization
- Type: behavioural (reliance on AI per trial as primary proxy for trust); no dedicated psychometric trust scale administered
- Measure: reliance on AI operationalized as binary agreement with AI prediction per trial (agree / disagree with AI recommendation); cognitive load assessed per trial with Single Ease Question (SEQ, 7-point scale); perceived understandability rated per explanation condition. Appropriate reliance (agreeing with correct AI, disagreeing with incorrect AI) computed as a secondary accuracy metric.
- Scale / instrument name: Single Ease Question (SEQ, 7-point); custom reliance dichotomy per trial
- Number of items: 1 (SEQ per trial)
- Behavioural vs self-report: both (per-trial reliance agreement as behavioral; SEQ cognitive load and understandability as self-report)

## Moderators and covariates tested
- AI confidence level (low vs. high): within-subjects covariate; high confidence significantly increased reliance (Log-Odds = 1.22, p < .01) and reduced cognitive load (Log-Odds = −0.41, p < .01); post-hoc analysis showed high confidence shifted attention from explanations to AI prediction itself
- AI correctness (correct vs. wrong): within-subjects covariate; moderated the effect of explanation style on reliance accuracy
- Need for Cognition (NFC): individual difference measured via 6-item NCS-6 scale; did not significantly moderate accuracy or cognitive load outcomes in this high-stakes task, contrary to findings from lower-stakes domains (relevant to RQ3 — NFC as AI-literacy-adjacent cognitive style)
- Information prioritization (ranked by participants): measured as attention check; both NFC groups prioritized loan attributes > explanations > AI information

## Statistical approach
- Primary analysis method: multilevel logistic regression (for binary reliance outcome, with participant as random effect); mixed ANOVA or equivalent for continuous outcomes (cognitive load, understandability); post-hoc analyses for interaction effects by AI confidence and correctness
- Software: not reported
- Key model fit or effect size reported: Log-Odds coefficients with p-values (high confidence → reliance: Log-Odds = 1.22, p < .01; high confidence → cognitive load: Log-Odds = −0.41, p < .01); Cronbach's α for NCS-6 not reported in source summary; NFC moderator effects non-significant

## Author-noted limitations
- NFC did not moderate outcomes as predicted — this may be task-specific (high complexity, high stakes); findings may not generalize to simpler AI-assisted tasks where NFC typically has predictive power
- Reliance measured as binary agreement per trial rather than more nuanced behavioral measures (e.g., decision time, confidence in own judgment)
- Feature-based explanations (SHAP) did not significantly improve accuracy, which may reflect limitations of SHAP visualization design rather than the method itself
- Online recruitment via Prolific produces heterogeneous sample but limits control over external distractors and attention
- Counterfactual explanations' accuracy benefit was nuanced and interacted with AI correctness in complex ways requiring replication

## Related pages
- [[cau-spano-xai-cognitive-capabilities]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[explainability]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Cau, F. M., & Spano, L. D. (2026). *Exploring the impact of explainable AI and cognitive capabilities on users' decisions*. *User Modeling and User-Adapted Interaction, XX*(XX), XXXX. [Volume and page not reported in source summary.]
