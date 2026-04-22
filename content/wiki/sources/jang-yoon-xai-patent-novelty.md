# An Explainable Artificial Intelligence–Human Collaborative Model for Investigating Patent Novelty

**Source file**: [Original article](../../raw/Jang & Yoon_An explainable artificial intelligence-human collaborative model.pdf)

**Summary**: This paper proposes and evaluates an XAI–human collaborative framework for patent novelty classification, where a self-explaining deep neural network provides claim-level relevance scores to technical experts, who then provide feedback that is incorporated into a refined model, achieving improved performance (accuracy 0.890, F1 0.916) over the source model.

**Sources**: Jang & Yoon_An explainable artificial intelligence-human collaborative model.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Jang and Yoon (2025), published in *Engineering Applications of Artificial Intelligence*, propose an XAI–human collaborative model for patent novelty assessment. The framework operates in two sequential stages: (1) a source XAI model — a self-explaining deep neural network based on RoBERTa embeddings — classifies patent pairs as novel or novelty-prejudicial and provides claim-level relevance scores as explanations; (2) technical expert users review these explanations and provide feedback (advice) on which claims are relevant to novelty judgment, which is then used to refine the model via a modified loss function. Two experimental types are compared: feedback provided independently of XAI explanations (Type 1) and feedback provided guided by XAI explanations (Type 2). The study uses the European Patent Office (EPO) full-text dataset and evaluates on 30,918 patent pairs.

## Key Findings

- The XAI–human collaborative refined model (lambda = 0.6) achieved accuracy 0.890 and F1 score 0.916, compared to the source model accuracy of 0.589 and F1 of 0.652 — an improvement of 0.301 in accuracy. [domain: intellectual property/patent analysis]
- The refined model outperformed the base model (trained for additional iterations without advice) by 0.041 F1, confirming that expert feedback (not just additional training) drove performance improvement. [domain: intellectual property/patent analysis]
- Type 1 advice (independent of XAI explanations, all claims reviewed) slightly outperformed Type 2 (guided by XAI explanations, top-3 claims only), with an F1 difference of only 0.001 at lambda = 0.6 — suggesting XAI-guided feedback is nearly as effective as exhaustive independent review. [domain: intellectual property/patent analysis]
- The self-explaining approach shows a trade-off at the source model level: higher lambda (greater self-explainability) reduced source model accuracy. However, this trade-off was overcome in the refined model when human advice was incorporated. [domain: intellectual property/patent analysis]
- The model provides both a binary novelty classification and a relevance score for each claim pair between target and prior patents, operationalizing explainability as local, claim-level attributions. [domain: intellectual property/patent analysis]
- The framework is framed as a "control type" XAI–human interaction: the model updates its behavior to converge toward user requirements, going beyond passive information transmission. [domain: intellectual property/patent analysis]
- The approach assumes unconditional trust in expert advice as a known limitation — if experts provide incorrect advice, model performance could degrade. [domain: intellectual property/patent analysis]

## Transparency Constructs

The paper operationalizes [[explainability]] as a self-explaining neural network that provides claim-level relevance scores (saliency weights) as part of the model's loss function. Unlike post-hoc explanation methods (such as LIME or SHAP), the explanation is intrinsic to the model architecture — a locally self-explainable approach producing interpretable attribution scores per claim pair. This is related to [[traceability]] (the model's decision path is linked to specific textual evidence in patent claims) and [[causability]] (scores indicate how strongly specific claim segments causally influenced the novelty prediction). The framework is model-specific, not model-agnostic.

## Trust Constructs

The paper is primarily concerned with model performance improvement through collaboration rather than user trust measurement per se. Trust is treated as an implicit motivator for the XAI framework: lack of trust in black-box AI creates barriers to adoption in technology management contexts, and the proposed transparency is meant to address this. The paper does not measure trust directly. However, it references the risk of over-reliance on AI explanations (automation bias from Bond et al., 2019) as the rationale for including the comparison between explanation-guided (Type 2) and independent (Type 1) feedback — addressing [[appropriate-reliance]] design considerations.

## Relevance to Research Questions

**RQ1**: The paper provides a distinctive operationalization of XAI in a text-based, domain-expert context (patent examination and R&D technology management). The self-explaining model approach contrasts with post-hoc surrogate methods: explanations are co-produced with the model's prediction rather than generated after the fact. The paper also conceptualizes a user-facing explanation type (claim-level relevance scores) tailored to technical expert users, contributing to how explainability is operationalized for non-public expert audiences.

**RQ2**: The paper does not directly test transparency–trust relationships in a user study sense. Instead, it demonstrates that XAI explanations can improve model performance when used as scaffolding for expert feedback. The finding that Type 2 (XAI-guided) advice yields near-equivalent performance to Type 1 (independent advice) suggests that XAI explanations do not substantially distort expert judgment in this domain — a weak positive finding for the value of transparency in collaborative human-AI work without measurable over-reliance.

**RQ3**: The study explicitly focuses on domain expert users (patent examiners and R&D practitioners) as the intended human collaborators. Expert domain knowledge is treated as both a prerequisite for and a resource in the collaboration — the model explicitly benefits from expert advice. The paper reviews prior literature showing that non-expert participants have been overrepresented in XAI collaboration studies, and argues that stakeholder composition (including domain experts, developers, regulators) is critical. This directly addresses RQ3's concern with user roles and expertise.

## Related pages

- [[explainability]]
- [[traceability]]
- [[causability]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[behavioural-trust]]
- [[domain-context]]
- [[rq3-user-roles]]
