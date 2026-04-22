# DARPA's Explainable Artificial Intelligence (XAI) Program

**Source file**: [Original article](../../raw/Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.pdf)

**Summary**: Gunning and Aha provide a programmatic overview of DARPA's four-year XAI initiative, which aims to develop ML techniques that produce explainable models while maintaining performance, and to establish a psychologically grounded evaluation framework for measuring explanation effectiveness through user understanding, trust, and task performance.

**Sources**: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Gunning and Aha (2019), published in *AI Magazine* (Summer 2019, pp. 44–58), describe the DARPA Explainable Artificial Intelligence (XAI) program launched in May 2017. The program is a four-year, multi-team research initiative involving 11 technical developer teams (TA1) and one psychological/evaluation team (TA2, Florida Institute for Human and Machine Cognition, IHMC). The program defines explainable AI as AI systems that can "explain their rationale to a human user, characterize their strengths and weaknesses, and convey an understanding of how they will behave in the future." It explicitly targets two operationally relevant challenge domains: data analytics (supervised classification) and autonomy (reinforcement learning for autonomous systems).

The article serves as both a program description and a conceptual framework paper for the field of XAI, articulating the fundamental tension between ML performance and explainability, proposing three development strategies, and specifying how explanation effectiveness should be measured.

## Key Findings

- There is an inherent performance–explainability trade-off: the highest-performing ML methods (e.g., deep learning) are the least explainable, while the most explainable (e.g., decision trees) are the least accurate. DARPA frames XAI as an attempt to navigate this trade-off without sacrificing too much of either. (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt; domain: defense/intelligence analysis and autonomous systems)
- Three strategies for improving explainability are proposed: (1) Deep explanation — modified deep learning techniques that learn more explainable features; (2) Interpretable models — structured, causal, or rule-based models; (3) Model induction — post-hoc, model-agnostic techniques that infer approximate explanations from black-box behavior (e.g., LIME). (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt)
- DARPA's target is an end user who depends on AI decisions and needs to understand the system's rationale — not just its output — in order to appropriately trust and manage it. (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt; domain: defense/intelligence)
- The IHMC psychological model of explanation identifies four measurable categories of explanation effectiveness: (1) user satisfaction (clarity, utility ratings); (2) mental model (accuracy, completeness of user's understanding); (3) task performance (does explanation improve user decisions?); and (4) appropriate trust and reliance. (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt)
- Simply summarizing the inner workings of a system does not yield a sufficient explanation; explainability must be assessed against the user's psychological needs and task context. (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt)
- Appropriate trust — distinguished from over-trust (automation bias) and under-trust (algorithm aversion) — is a central outcome variable in the XAI evaluation framework. (source: Gunning & Aha_DARPA's explainable artificial intelligence (XAI) program.txt)

## Transparency Constructs

The paper defines and taxonomizes transparency constructs at a programmatic level:

- **Deep explanation**: A form of [[explainability]] embedded in modified deep learning architectures, generating post-hoc or introspective explanations.
- **Interpretable models**: Corresponds to [[algorithmic-transparency]] in the sense that the model itself is structured to be understandable (e.g., Bayesian rule lists, causal models).
- **Model induction**: Corresponds to post-hoc [[explainability]] — [[counterfactual-explanations]], saliency maps, LIME-style surrogate models — applied to any black-box model.
- **Explanation interfaces**: The program emphasizes HCI principles for presenting explanations — visual, natural language, or interactive — bridging the gap between technical transparency and user-facing communication.

The paper defines the XAI concept in terms of user-facing goals: users should be able to answer "Why did you do that?", "When can I trust you?", "When do you fail?", and "How do I correct an error?" — mapping to [[outcome-transparency]], [[trust-calibration]], and system correctability.

## Trust Constructs

The paper's primary trust construct is **appropriate trust** — calibrated reliance on AI that reflects the system's actual capabilities and limitations. This is explicitly contrasted with:
- Over-trust / automation bias: trusting an AI system beyond its warranted limits.
- Under-trust / [[algorithm-aversion]]: distrust that leads to disuse of reliable AI.

The IHMC model proposes that explanation → mental model → appropriate trust → appropriate use, providing a causal chain that links transparency to [[trust-calibration]] and [[behavioural-trust]]. [[cognitive-trust]] is implicit in the mental model construct. The program frames trust as a downstream outcome of explanation quality, measured in controlled experiments.

## Relevance to Research Questions

**RQ1**: This paper is one of the most cited programmatic definitions of XAI in the literature. It provides a structured taxonomy of transparency constructs (deep explanation, interpretable models, model induction) and a psychologically grounded framework for operationalizing explanation effectiveness. The four measurement categories (satisfaction, mental model, task performance, appropriate trust) define how transparency and trust have been conceptualized in the XAI research agenda, making this paper essential for RQ1.

**RQ2**: The program's evaluation framework explicitly hypothesizes that better explanations → better mental models → appropriate trust → better task performance. The paper frames the performance–explainability trade-off as a core challenge, anticipating that different transparency techniques will produce different trust and performance outcomes. While empirical results from the evaluations are only briefly referenced (Phase 1 completed May 2018), the framework sets up the research agenda for testing these relationships. The emphasis on "appropriate" trust signals awareness of non-linear effects (both under- and over-trust are problems).

**RQ3**: User expertise is implicitly addressed: the "target user" (intelligence analyst, drone operator) is framed as a domain expert who needs to understand AI recommendations within a task context. The program's challenge domains require expert users, and the IHMC model assumes users bring a prior mental model that explanations update. However, the paper does not systematically vary user expertise as a moderator.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[counterfactual-explanations]]
- [[trust-calibration]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[cognitive-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
