# Toward Personalized XAI: A Case Study in Intelligent Tutoring Systems

**Source file**: [Original article](../../raw/Conati et al._Toward personalized XAI.pdf)

**Summary**: A controlled between-subjects study (N = 47 who received hints) examining whether explanations of an intelligent tutoring system's adaptive hints improve student trust, perceived usefulness, and learning, and whether these effects are moderated by user characteristics including Need for Cognition, Conscientiousness, and Reading Proficiency, providing evidence that one-size-fits-all XAI is insufficient.

**Sources**: Conati et al._Toward personalized XAI.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Conati et al. (2021) present a case study in personalized Explainable AI (XAI) within an Intelligent Tutoring System (ITS) context. The system, the Adaptive CSP (ACSP) applet, teaches the AC-3 algorithm for constraint satisfaction problems. It uses a machine learning user model (k-means clustering + associative classification rules) to classify students as Higher or Lower Learning Gain users, then delivers adaptive hints directing students toward more effective interaction patterns.

The authors added a multi-level explanation interface to this system, providing "why" and "how" explanations across six pages (WhyHint, WhyLow, WhyRules, HowScore, HowHint, HowRank). The explanations were designed to be iterative (incremental depth), sound, and complete — though completeness was partially sacrificed to avoid cognitive overload. A between-subjects design compared 30 students with access to explanations (of whom 24 accessed at least one) to 17 students in a control condition with no explanations.

Critically, the study measured a battery of user characteristics (Big-5 personality, Need for Cognition, Reading Proficiency, Perceptual Speed, Visual Working Memory, and two dimensions of Curiosity) to investigate how these modulate explanation usage and effectiveness — a direct contribution toward personalized XAI.

## Key Findings

- Students in the explanation condition reported significantly higher trust in the ACSP's adaptive hints (Wilcoxon-Mann-Whitney, p = .0088, r = .41) compared to the control condition. (Domain: computer science education / intelligent tutoring)
- Students with explanation access rated the hints as significantly more helpful (p = .0016, r = .49) and reported higher intention to use the hints again (p = .0044, r = .44). (Domain: education)
- No significant overall difference in learning gains (percentage learning gain, PLG) was found between explanation and control conditions (p = .7). (Domain: education)
- Conscientiousness moderated the effect of explanations on learning: students with low conscientiousness learned significantly better with explanations, while high-conscientiousness students showed no benefit or a slight negative trend (F(1,37) = 4.76, p = .035, partial η² = .11). (Domain: education)
- Need for Cognition (N4C) significantly predicted attention to explanations: high-N4C students spent more time on explanations (F(1,22) = 8.51, p = .008, partial η² = .28). Low-N4C students were less likely to engage with explanations, potentially reducing their benefit. (Domain: education)
- Reading Proficiency moderated the effect of explanations on hint confusion: high reading proficiency students found hints less confusing with explanations; low reading proficiency students found hints more confusing when explanations were present (χ² = 9.97, p = .0016, r = .49). (Domain: education)
- Participants accessed "why" explanations far more than "how" explanations (WhyHint and WhyLow together constituted approximately two-thirds of all page accesses), consistent with prior literature on user explanation preferences.
- Of 30 students in the explanation condition, 6 never accessed explanations; their stated reasons were that hints were self-explanatory or not useful to begin with.
- Most participants initiated explanations for their very first hint (mean hints before first initiation = 1.08), and accessed explanations for ~75% of subsequent hints.

## Transparency Constructs

The paper operationalises [[explainability]] in an ITS context as explicit "why" and "how" explanations of pedagogical decisions:

- **"Why" explanations** explain why a student is classified as lower-learning and why a particular hint was selected — addressing both high-level goal alignment (what-for) and causal reasoning (how-come).
- **"How" explanations** explain the computational processes: how the student's score was computed, how the hint was chosen, and how the hint's rank was calculated.

The explanation interface embodies [[process-transparency]] (exposing the AI's user modeling and classification mechanisms) and [[outcome-transparency]] (showing how the student's current behaviour pattern led to the hint). This is more granular than an Open Learner Model (OLM), which typically only shows assessed student state without explaining the underlying AI mechanisms.

The design principles used (iterative, sound, complete, not overwhelming) come from Kulesza et al. (2015) and are applied within an [[algorithmic-transparency]] framework.

## Trust Constructs

The study measures [[cognitive-trust]] via questionnaire items directly asking about trust in the hints:

- "I trust the system to deliver appropriate hints" (H8 in the Perception of Hints Questionnaire, adapted from USE questionnaire and XAI literature).
- "I understand why hints were delivered to me in general" and "I understand why specific hints were delivered to me" — reflecting the understanding component of cognitive trust.

[[behavioural-trust]] is partially captured by "intention to use hints again" (H1), perceived helpfulness (H3), and actual explanation access patterns (logged interaction data + eye tracking).

The paper does not measure affective trust directly but acknowledges user characteristics (curiosity dimensions) may reflect affective engagement.

## Relevance to Research Questions

**RQ1**: Provides a detailed operationalisation of XAI in ITS as layered "why/how" explanations grounded in the system's actual AI mechanisms. Operationalises trust via Perception of Hints items. The study also operationalises user characteristics (N4C, Conscientiousness, Reading Proficiency) as theoretically grounded moderators.

**RQ2**: Finds a positive effect of explanations on self-reported trust and perceived helpfulness, but no direct effect on learning outcomes in the overall sample. The relationship between explanations and trust is thus domain-specific and moderated: not all students benefit equally. The interaction effects for Conscientiousness and Reading Proficiency show non-linear, conditional relationships between explanation access and outcomes.

**RQ3**: Strongly relevant. The study is an explicit investigation of personalized XAI, showing that user characteristics (N4C, Conscientiousness, Reading Proficiency) systematically moderate both engagement with and benefit from explanations. This is one of the most thorough empirical treatments of [[user-expertise]] and cognitive moderators in XAI for education. The results provide direct evidence that one-size-fits-all XAI is suboptimal and that explanation design should be personalized.

## Related pages

- [[explainability]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
