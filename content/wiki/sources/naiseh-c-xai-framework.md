# C-XAI: A Conceptual Framework for Designing XAI Tools That Support Trust Calibration

**Source file**: [Original article](../../raw/Naiseh et al._C-XAI a conceptual framework for designing XAI tools.pdf)

**Summary**: This paper introduces C-XAI (Calibrated-XAI), a participatory design framework for creating XAI interfaces that explicitly address trust calibration errors (over-trust and under-trust) in human-AI collaboration, evaluated through expert review and a case study in healthcare prescription screening.

**Sources**: Naiseh et al._C-XAI a conceptual framework for designing XAI tools.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Naiseh, Simkute, Zieni, Jiang, and Ali (2024, Journal of Responsible Technology) present C-XAI, a four-phase participatory design framework that guides the creation of XAI user interfaces with trust calibration as an explicit design goal. The framework responds to a recognized gap: while XAI research produces many explanation techniques, system designers lack structured methods to anticipate and mitigate trust calibration errors at the design stage.

Trust calibration errors encompass both **over-trust** (users rely on AI recommendations without sufficient scrutiny) and **under-trust** (users ignore valid AI recommendations). Both errors reduce the quality of human-AI collaborative decision-making in high-stakes settings such as healthcare and criminal justice.

C-XAI framework has four main phases:

1. **Identification Phase**: Recruit diverse stakeholders; conduct Human-AI Task Analysis (HAI-TA) to map AI recommendation tasks; elicit XAI requirements and match them to available XAI methods.
2. **Assessment Phase**: (a) Technical assessment of XAI method properties using the Explainability Facts Sheets (EFS) framework across five dimensions (Functional, Operational, Usability, Safety, Validation); (b) Human factors assessment — risk assessment of how technical properties may cause trust calibration errors.
3. **Selection and Implementation Phase**: Identify design interventions (design principles and guidelines) to mitigate identified trust calibration risks. Four key design principles: Persuasive Design, Challenging Habitual Actions, Attention Guidance, Training and Learning.
4. **Evaluation Phase**: Iterative evaluation using behavioral metrics — agreement percentage, compliance percentage, incorrect decisions, and correct decisions — to measure whether trust calibration has improved.

C-XAI is evaluated in two phases:
- **Phase 1 (Expert Evaluation)**: Six domain experts (AI, HCI, requirements engineering, psychology; 5–12 years experience) reviewed framework documents, provided structured feedback, and assessed completeness, understandability, and usefulness. This produced C-XAIv2.
- **Phase 2 (Case Study Evaluation)**: 14 stakeholders (medical doctors, pharmacists, ML engineers, HCI researchers, psychologists, requirement engineers; from UK, Germany, US, Italy) used C-XAI to design an XAI interface for an AI-based Screening Prescription (SP) healthcare tool. This produced C-XAIv3.

The domain spans **healthcare (prescription screening)** as the primary case study, with relevance to **criminal justice** and any critical decision-making domain.

## Key Findings

- Expert evaluation confirmed C-XAI is a practical, comprehensive, and complete method for designing XAI interfaces. Five of six experts rated it positively on completeness. Experts requested examples and heuristics mapping XAI technical properties to trust calibration risks, a glossary of key terms, and shortened guidelines adapted for practitioners rather than academics. (Domain: framework evaluation, multi-domain)
- Case study evaluation with healthcare stakeholders confirmed C-XAI's usefulness and effectiveness in guiding XAI interface design toward trust calibration goals. Participants emphasized that the framework facilitated effective communication between diverse stakeholders (medical, technical, design, and behavioral science professionals). (Domain: healthcare)
- The framework identified that purely "yes/no" assessments of XAI method properties are insufficient; graduated scales (low/medium/high) better represent the degree of property manifestation. This has implications for how transparency properties of XAI systems are measured and communicated. (Domain: general XAI design)
- The C-XAI framework explicitly acknowledges it cannot eliminate all trust calibration risks, but rather provides a systematic approach to anticipating and mitigating them at the design stage, before deployment.
- A key finding from the framework's development is that trust calibration errors can arise from XAI technical properties themselves (e.g., high "novelty" in explanation outputs may cause habituation and over-trust; static explanations may cause under-engagement). Design interventions must be matched to specific technical risk profiles.

## Transparency Constructs

C-XAI addresses transparency primarily through the lens of **explainability** — the technical properties of XAI methods (accuracy, completeness, soundness, interactivity) that determine what information is communicated to users ([[explainability]]). The framework's assessment dimensions reflect multiple transparency sub-types:

- **Functional** and **Operational** dimensions map to [[process-transparency]] (how the AI makes decisions, and how users can interact with the explanation)
- **Usability** dimension incorporates [[causability]] — soundness and coherence of explanations in terms of human-understandable causal reasoning
- The **Traceability** of explanations (whether they allow auditing of model behavior) is implicitly addressed through the Safety and Validation dimensions ([[traceability]])

The framework introduces the concept of **trust calibration risks** arising from XAI design properties, such as:
- Habituation (users become accustomed to explanations and stop engaging — risking over-trust)
- Misapplication (users misinterpret explanations — risking miscalibrated trust)
- Skipping (users ignore explanations — risking under-engagement)

These risks show that transparency mechanisms can be actively undermined by the design of the interface delivering them.

## Trust Constructs

C-XAI is specifically organized around **trust calibration** ([[trust-calibration]]) — the goal is neither maximum trust nor minimum trust, but appropriately calibrated trust that reflects the AI system's actual reliability. The framework distinguishes:

- **Over-trust**: Users follow AI recommendations without appropriate scrutiny, including when the AI is wrong — a behavioral trust failure ([[behavioural-trust]])
- **Under-trust**: Users ignore valid AI recommendations, failing to leverage AI capabilities — also a behavioral trust failure
- **Calibrated trust**: Agreement and compliance rates that appropriately track AI accuracy

Behavioral metrics proposed to measure trust calibration include agreement percentage (how often users agree with AI), compliance percentage (how often users comply even when they initially disagree), incorrect decisions (when human-AI collaboration produces wrong outcomes), and correct decisions.

The framework situates trust calibration within broader human-AI teaming literature and connects to **cognitive trust** (users' mental models of AI capabilities; see [[cognitive-trust]]) and **appropriate reliance** ([[appropriate-reliance]]).

## Relevance to Research Questions

**RQ1**: Provides a framework-level conceptualization of transparency as a design variable that must be actively managed to achieve trust calibration, not merely added to a system as an afterthought. Defines trust calibration as the primary target of XAI design and specifies behavioral metrics for measuring it. Contributes a structured methodology for how transparency and trust should be jointly operationalized in design processes, particularly in high-stakes domains.

**RQ2**: The paper's core argument is that the relationship between XAI/transparency and trust is not linear or guaranteed positive. Specific XAI properties (novelty, complexity, static vs. interactive) can introduce trust calibration risks that produce over-trust or under-trust. This is a significant theoretical contribution to understanding conditional and potentially negative effects in the transparency–trust relationship — different explanation designs create different trust trajectories. Empirical support comes from prior work by the authors (Naiseh et al., 2023) referenced throughout.

**RQ3**: C-XAI explicitly incorporates **user expertise** and **domain knowledge** as factors in the XAI requirements elicitation process. The identification phase recommends recruiting diverse stakeholders including representative users, domain experts, and psychologists. The framework cites evidence that AI literacy, domain knowledge, and curiosity level enrich explainability requirements, and that there is no one-size-fits-all explanation. The case study demonstrates this in practice: healthcare professionals (doctors, pharmacists), ML engineers, and behavioral scientists all bring different needs and risk perceptions to the XAI design process.

## Related pages

- [[trust-calibration]]
- [[appropriate-reliance]]
- [[explainability]]
- [[causability]]
- [[traceability]]
- [[user-expertise]]
- [[domain-context]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
