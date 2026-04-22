# The Rationality of Explanation or Human Capacity? Understanding the Impact of Explainable AI on Human-AI Trust and Decision Performance

**Source file**: [Original article](../../raw/Wang & Ding_The rationality of explanation or human capaciy_.pdf)

**Summary**: This quasi-experimental study investigates how SHAP-based XAI affects trust and decision accuracy in a competitive commercial prediction task (cross-border e-commerce sales forecasting), and reveals that the impact of explanations on trust and performance varies systematically by users' task-related (data analysis) capacity. Low-capacity users are persuaded by the mere presence of an explanation (a placebo effect), while high-capacity users require the rationality of explanation content to improve behavioral trust.

**Sources**: Wang & Ding_The rationality of explanation or human capaciy_.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in Information Processing and Management (Vol. 61, 2024), this paper by Ping Wang and Heng Ding from Central China Normal University examines the dual roles of XAI — as an informational cue and as substantive causal content — through the lens of the Elaboration Likelihood Model (ELM). Using a laboratory experiment with 109 valid participants assigned to three conditions (rational XAI via SHAP, irrational/randomized SHAP, and AI-only baseline), the study tests whether explainability improves human performance and trust, and whether effects vary by data analysis capacity.

The task was a competitive commercial scenario: participants forecasted sales for products on a cross-border e-commerce platform (Wish.com), with monetary incentives tied to accuracy rank. SHAP waterfall plots were used as the explanation format.

## Key Findings

- XAI significantly improved AI-assisted decision accuracy in competitive commercial tasks: accuracy increased by 10.8 percentage points for rational XAI (p < 0.01) and 9.2 pp for irrational XAI (p < 0.01), versus AI-only (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- Rational XAI achieved hybrid intelligence — combined XAI + human accuracy (75.6%) exceeded AI alone (75%), which AI + human (67.5%) did not (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- XAI did not improve self-reported trust in AI in either explanation condition; self-report trust is unreliable in competitive prediction tasks (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- XAI improved reliance on AI (behavioral trust surrogate) significantly: rational XAI +9.4 pp (p < 0.01), irrational XAI +6.2 pp (p < 0.05) (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- Only rational XAI significantly improved behavioral consistency with AI (answer agreement rate, +8.4%, p < 0.05); irrational XAI did not (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- **Placebo effect for low-capacity users**: both rational and irrational explanations improved prediction accuracy and reliance equally for low task-related capacity participants; the cue of explanation suffices for peripheral persuasion (ELM peripheral route) (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- **High-capacity users**: explanation rationality was necessary for improving behavioral consistency with AI; high-capacity users without explanation showed declining AI agreement over time as they detected AI errors (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).
- Decision efficiency (time per prediction) was not significantly improved by either XAI condition (source: Wang & Ding_The rationality of explanation or human capaciy_.txt; domain: e-commerce).

## Transparency Constructs

The study uses SHAP (SHapley Additive exPlanations) waterfall plots as the explanation format, representing **feature contribution explanations** — a type of [[explainability]] that shows how each input feature drives the model's output. This is a post-hoc, local, model-agnostic explanation technique.

The paper distinguishes two attributes of XAI:
1. **Cue** (the visual presence of an explanation interface) — acts as a peripheral persuasion signal.
2. **Rationality** (the substantive quality and logical consistency of explanation content) — acts as a central persuasion signal.

The "irrational" XAI condition (randomly permuted SHAP values) served as a manipulation to isolate the cue effect from content quality. This is a key methodological innovation for studying [[algorithmic-transparency]] in human-AI decision-making.

## Trust Constructs

The paper distinguishes two trust measurement approaches:

- **Self-report trust**: Post-decision Likert-style question ("Do you trust the prediction justification?") — found to be insensitive to XAI manipulation, corroborating prior critiques of survey-only trust measurement.
- **Behavioral trust**: Measured as (1) reliance on AI (stated strategy slider) and (2) consistency with AI (percentage of trials agreeing with AI prediction). These [[behavioural-trust]] indicators were more sensitive to XAI and to explanation rationality.

The authors explicitly position their work within the [[trust-calibration]] literature, arguing that rational explanations help users build appropriate (neither over- nor under-trusting) relationships with AI.

## Relevance to Research Questions

**RQ1**: Contributes dual operationalization of trust (self-report vs. behavioral) in an AI-assisted decision context, and distinguishes XAI as having both cue and content components. The ELM-grounded framework provides a theoretically principled account of how transparency constructs operate differently depending on user capacity. See [[rq1-conceptualizations]].

**RQ2**: Provides evidence for a conditional (moderated) rather than universal positive effect of XAI on trust. The relationship between transparency and behavioral trust is positive, but only for rational explanations and only for high-capacity users. Self-reported trust shows no effect. This null result for subjective trust alongside positive behavioral trust effects is a key nuanced finding for [[rq2-relationships]].

**RQ3**: One of the few studies to explicitly segment users by task-related capacity (data analysis skill) and demonstrate differentiated XAI impact. Low-capacity users exhibit the placebo effect; high-capacity users show central-route processing. This directly informs [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq3-user-roles]]
