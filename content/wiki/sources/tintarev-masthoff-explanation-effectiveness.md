# Evaluating the Effectiveness of Explanations for Recommender Systems: Methodological Issues and Empirical Studies on the Impact of Personalization

**Source file**: [Original article](../../raw/Tintarev & Masthoff_Evaluating_the_effectiveness_o.pdf)

**Summary**: A methodological paper and series of four empirical studies in movie and camera domains examining how personalized versus non-personalized feature-based explanations affect the effectiveness (decision quality) and satisfaction of recommender system users; finds that personalization improves satisfaction but is consistently detrimental to decision-making effectiveness.

**Sources**: Tintarev & Masthoff_Evaluating_the_effectiveness_o.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Tintarev and Masthoff (2012, *User Modeling and User-Adapted Interaction*, 22, 399–439) provide a foundational methodological contribution to the explanation evaluation literature and report four empirical studies on explanation effectiveness in recommender systems. The paper:

1. Defines **seven aims for explanations** in recommender systems: transparency, scrutability, trust, effectiveness, persuasiveness, efficiency, and satisfaction — and establishes that these aims can be mutually incompatible.
2. Critically reviews metrics for measuring explanation **effectiveness** (the aim of helping users make good decisions), identifying limitations of existing approaches.
3. Proposes using Bilgic and Mooney's (2005) metric: the discrepancy between a user's pre-consumption rating of an item (after seeing the explanation) and their post-consumption rating.
4. Reports four experiments (N=46, 33, 47, 48 respectively) comparing baseline, non-personalized feature-based, and personalized feature-based explanations in movie (Experiments 1, 2, 4) and camera (Experiment 3) domains.

This is an early and frequently cited paper establishing a conceptual taxonomy of explanation aims and identifying key trade-offs, particularly the **effectiveness–satisfaction tension** in personalized recommendation explanations.

---

## Key Findings

- **Explanations help users form opinions**: Across all experiments, feature-based explanations significantly reduced opt-out rates (decisions where users had insufficient information to form an opinion) compared to baseline explanations, and especially compared to seeing only a movie title (Experiment 4: opt-out rate dropped from 35.6% after title alone to 15.9% after explanation, p<.001). [Domain: e-commerce/recommender systems — movies, cameras]
- **Personalization was detrimental to effectiveness in most conditions**: Across three experiments (Movies I, II, Cameras), non-personalized feature-based explanations consistently produced numerically better (lower absolute difference between pre- and post-consumption ratings) effectiveness than personalized explanations. In Experiment 3 (cameras), this was statistically significant (p<.01, non-personalized better than personalized). [Domain: e-commerce — movies, cameras]
- **Personalization increased user satisfaction**: In Experiments 1–3, personalized explanations received significantly higher satisfaction ratings than non-personalized (e.g., Experiment 3: personalized M=3.27 vs. non-personalized M=2.38, p<.01). [Domain: e-commerce — movies, cameras]
- **Effectiveness and satisfaction are in conflict**: The same explanation type (personalized, feature-based) that users preferred was consistently less effective for decision-making. This fundamental tension undermines assuming user satisfaction as a proxy for explanation quality. [Domain: e-commerce]
- **Final evaluation (Experiment 4, real experience)**: When participants actually watched the movies rather than reading reviews, baseline explanations achieved the best effectiveness — but they also had the highest opt-out rate (28.9%), lowest satisfaction, and were least helpful in enabling users to form an opinion. Non-personalized explanations achieved intermediate results on both effectiveness and satisfaction. [Domain: e-commerce — short movies]
- **Seven aims taxonomy**: The paper establishes that explanations can serve transparency (exposing system reasoning), scrutability (allowing user correction), trust (increasing confidence), effectiveness (decision support), persuasiveness (convincing purchase), efficiency (speed), and satisfaction (enjoyment). Importantly, an explanation optimizing one aim may harm another — e.g., a persuasive explanation may lower effectiveness; transparency may either raise or lower trust depending on whether the revealed reasoning is reassuring. [Domain: e-commerce/recommender systems conceptual]
- **Domain matters for explanation evaluation**: Overestimation (inflated pre-consumption ratings) was more damaging in high-investment, objective domains (cameras) than low-investment, subjective domains (movies). This suggests effectiveness metrics cannot be straightforwardly ported across domains. [Domain: e-commerce — movies vs. cameras comparative]
- **Opt-out rates are an important supplementary metric**: Baseline explanations that appeared effective by the core metric had high opt-out rates, indicating the metric was misleading. Evaluating explanations requires examining both the effectiveness score and the proportion of items users felt unable to rate. [Domain: e-commerce methodological contribution]

---

## Transparency Constructs

This paper operationalizes **[[outcome-transparency]]** and **[[process-transparency]]** through the lens of recommender system explanations:
- **Baseline explanations** (e.g., "This movie is in the top 100 on IMDB") provide minimal information about the system's reasoning but signal external validation — a form of [[institutional-trust]] cuing rather than transparency per se.
- **Non-personalized feature-based explanations** (e.g., "This movie is a Drama directed by X") expose item features without revealing user-model reasoning — closer to **[[outcome-transparency]]** (describing the item) than process transparency.
- **Personalized feature-based explanations** (e.g., "This movie stars your favorite actor...") reveal user-model attributes driving the recommendation — an operationalization of **[[process-transparency]]** at the level of the personalization logic.

The paper also introduces **scrutability** as a distinct transparency-related aim — the ability for users to tell the system that its model of them is wrong — which is related to but distinct from [[explainability]].

The paper's seven-aims taxonomy is foundational to the [[rq1-conceptualizations]] conceptual landscape, providing a systematic decomposition of what "explanation" means that predates much of the XAI literature.

---

## Trust Constructs

- **[[cognitive-trust]]**: One of the seven aims is explicitly "trust" — increasing users' confidence in the system. However, in the empirical studies, trust is not the primary dependent variable; the focus is effectiveness and satisfaction.
- **[[behavioural-trust]]**: Effectiveness as measured by the Bilgic–Mooney metric captures actual decision quality — whether users accept or reject recommendations in ways that match their post-experience preferences. This is a behavioral operationalization of whether users act appropriately on system advice.
- **[[algorithm-aversion]]**: Not directly studied, but the discussion of persuasiveness vs. effectiveness raises the concern that explanations which increase user acceptance of recommendations may simultaneously mislead them — a form of automation misuse analogous to [[algorithm-aversion]]'s inverse (over-reliance).
- The paper explicitly notes: "transparency may lead to an increase or decrease in trust, depending how much confidence users have in the internal working of the system shown to them." This is an early articulation of what later literature calls [[trust-calibration]] — the idea that transparency effects on trust are conditional rather than uniformly positive.

---

## Relevance to Research Questions

**RQ1**: Highly relevant. The seven-aims taxonomy is a foundational conceptualization of what explanations do and why they matter. It provides a structured vocabulary that distinguishes trust as one distinct aim alongside effectiveness, satisfaction, transparency, and scrutability. The paper also operationalizes explanation transparency narrowly as process/outcome-level feature disclosure in recommender systems, contributing to [[rq1-conceptualizations]].

**RQ2**: Relevant. The central finding — that personalization improves satisfaction but reduces effectiveness — documents a clear **negative relationship between one form of transparency (personalized feature disclosure) and decision quality**. The finding that transparency can increase or decrease trust depending on revealed system competence is an early empirical anchor for the non-linear transparency–trust relationship discussed in [[rq2-relationships]]. The domain-dependence of overestimation effects also contributes to understanding conditional effects.

**RQ3**: Moderately relevant. The paper does not explicitly examine user expertise as a moderator. However, Experiment 3 screened out participants unlikely to buy cameras (low domain involvement), and the discussion notes that feature personalization failed when users lacked the expertise to recognize named actors or directors in short movies. This is an implicit finding that **user familiarity with item features moderates the benefit of personalized explanations** — connecting to [[user-expertise]] and [[rq3-user-roles]].

---

## Related pages

- [[explainability]]
- [[outcome-transparency]]
- [[process-transparency]]
- [[trust-calibration]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
