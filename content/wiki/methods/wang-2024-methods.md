# Wang 2024 — Methods

**Summary**: A three-condition laboratory experiment (N = 109) with a competitive e-commerce sales forecasting task comparing rational SHAP XAI, irrational/randomised SHAP, and AI-only baseline, finding that explanation effects on behavioural trust and accuracy differ systematically by users' data analysis capacity.

**Sources**: Wang & Ding_The rationality of explanation or human capaciy_.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
experimental (between-subjects, three conditions; laboratory)

## Sample
- N: 109 (valid participants after exclusions)
- Population: general public / student participants (competitive commercial prediction task)
- Domain: e-commerce (cross-border product sales forecasting on Wish.com platform)
- Country / region: China (Central China Normal University)
- Recruitment method: convenience (laboratory experiment; monetary incentives tied to accuracy rank)

## Transparency operationalization
- Type: explainability (feature contribution explanation; post-hoc local model-agnostic)
- Manipulation or measure: Three between-subjects conditions: (1) Rational XAI — SHAP waterfall plots showing actual feature contributions to the model's prediction for each product; (2) Irrational XAI — visually identical SHAP waterfall plots with randomly permuted values (cue present, content invalid); (3) AI-only baseline — model predictions displayed without any explanation. Monetary incentives tied to accuracy rank. All conditions received the same AI predictions.
- Scale / instrument name: not applicable (between-subjects manipulation using SHAP waterfall plots)
- Number of items: not applicable

## Trust operationalization
- Type: self-report (cognitive) and behavioural
- Measure: (1) Self-report trust — post-decision Likert-style item ("Do you trust the prediction justification?"); found insensitive to XAI manipulation; (2) Behavioural trust — (a) reliance on AI: stated strategy slider indicating proportion of AI guidance used (0–100%); (b) consistency with AI: percentage of trials where participant's prediction agreed with AI prediction
- Scale / instrument name: not reported (single-item self-report trust measure)
- Number of items: 1 (self-report); continuous measures for behavioural trust
- Behavioural vs self-report: both — self-report single item plus two behavioural reliance measures

## Moderators and covariates tested
- Data analysis capacity (task-related capacity): key moderator; measured via self-assessment of data analysis skill; low-capacity users showed placebo effect (both rational and irrational XAI improved accuracy and reliance equally via peripheral ELM route); high-capacity users required rational explanation content for behavioural consistency improvement (central ELM route) — directly relevant to RQ3
- Trial number / time on task: tracked to examine whether AI agreement changes over time; high-capacity users without explanation showed declining AI agreement over trials as they detected AI errors
- Prediction accuracy: primary performance outcome measured per trial

## Statistical approach
- Primary analysis method: ANOVA and post-hoc pairwise comparisons (between-condition differences); moderation analysis (capacity × condition interactions); descriptive time-series tracking of AI agreement rates across trials
- Software: not reported
- Key model fit or effect size reported: p-values reported (e.g., rational XAI accuracy improvement p < 0.01; reliance improvement p < 0.01; consistency p < 0.05); percentage-point differences in outcomes reported; Elaboration Likelihood Model (ELM) used as theoretical framework

## Author-noted limitations
- Single domain (cross-border e-commerce forecasting); generalisability to other prediction tasks unknown
- Self-report trust insensitive to XAI; measurement validity of single-item trust questioned
- Competitive monetary incentive framing may not generalise to non-competitive or non-incentivised settings
- Capacity measured via self-assessment, which may not capture objective skill accurately
- Laboratory setting may not reflect naturalistic human-AI collaboration dynamics
- The irrational XAI condition isolates the cue effect but may not represent real-world XAI deployment scenarios

## Related pages
- [[wang-ding-rationality-explanation-capacity]]
- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
