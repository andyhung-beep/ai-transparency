# FCE: Feedback-Based Counterfactual Explanations for Explainable AI

**Source file**: [Original article](../../raw/Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf)

**Summary**: Proposes FCE, a user-feedback-driven counterfactual explanation method for XAI that constrains counterfactual generation to user-specified feature ranges and categorical choices, thereby producing more actionable and human-aligned explanations, evaluated on a bank loan classification task.

**Sources**: Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf

**Research questions addressed**: RQ1

**Last updated**: 2026-04-18

---

## Overview

Suffian et al. (2022), published in *IEEE Access*, introduce the Feedback-based Counterfactual Explanation (FCE) method. The core motivation is that existing XAI approaches — including LIME and SHAP — generate surrogate-model explanations without human involvement, often producing feature attributions that are technically valid but practically infeasible (e.g., suggesting users double their income to obtain a loan). FCE addresses this by using user feedback at two stages: (1) before generation, users specify the acceptable ranges (for numerical features) and binary change preferences (for categorical features) within which counterfactuals should be searched; (2) after generation, users evaluate the produced counterfactuals. The method is implemented in Python and evaluated on a bank loan classification dataset (N = 100 test instances) using Support Vector Machines (SVM) and Random Forests (RF).

The paper is primarily a technical/methodological contribution, but it addresses the human-centered XAI literature's concern that the lack of user involvement in explanation design causes trust deficits and reduced acceptance. This makes it relevant to RQ1 (operationalization of transparency through counterfactual explanation) within the financial / credit domain.

## Key Findings

- **FCE achieves 84% target-class validity**: 84 of 100 user-feedback-informed counterfactual instances were classified into the desired target class by the ML model, demonstrating the method's viability (domain: finance / credit scoring).
- **Continuous proximity is maintained**: generated counterfactuals show reasonable proximity (low MAD distance) to original instances for most features; the main exceptions are income and mortgage, where real-world dataset distributions differ from user-provided feedback ranges (domain: finance).
- **User feedback reduces infeasible counterfactuals**: by constraining search to user-specified feature ranges, FCE avoids the classic counterfactual problem of suggesting unrealistic changes (e.g., extreme income increases). 16% of generated counterfactuals failed the actionability criterion, primarily due to overly constrained feedback parameters (domain: finance).
- **Random Forest outperforms SVM** on the bank loan dataset (higher accuracy and F-measure in 10-fold cross-validation), and RF-generated counterfactuals are used for the main evaluation (domain: finance).
- The authors argue that user-provided feature changes are more likely to reflect genuine causal reasoning (e.g., if a user cannot increase income, they will not select CCAvg and Mortgage as features to change), giving FCE counterfactuals a latent causal structure absent from purely algorithmic approaches.

## Transparency Constructs

FCE is positioned as an implementation of **[[counterfactual-explanations]]** — a form of contrastive explanation that answers "what minimal changes would flip the AI's decision?" This belongs to the broader [[explainability]] construct. The user-feedback loop introduces a participatory design dimension to transparency:

- **[[counterfactual-explanations]]**: The central output of FCE; "what-if" explanations specifying the minimal feature changes needed to obtain a different (desired) AI outcome.
- **[[process-transparency]]**: Implicitly addressed — by involving users in defining the explanation space, FCE makes the decision boundary partially transparent to the user in terms of which features are relevant.
- **[[outcome-transparency]]**: The counterfactual directly shows how a different outcome is achievable, making the outcome logic transparent.

The method connects to GDPR's "right to explanation" and the EU AI Act's transparency requirements, which are explicitly cited as motivating the need for user-centric XAI (source: Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf).

## Trust Constructs

The paper does not empirically measure trust as a dependent variable. Trust is discussed conceptually:

- Lack of user involvement in explanation generation is identified as a primary cause of **[[algorithmic-trust]]** deficits and reduced system acceptance.
- The assumption is that aligning counterfactual explanations with user expectations (through their own feedback) will improve **[[behavioural-trust]]** (adoption, reliance) and **[[cognitive-trust]]** (perceived competence and reliability of the AI system).
- The paper frames FCE as a tool for [[trust-calibration]]: by making the explanation space navigable and actionable, users can form more accurate mental models of the AI's decision boundary.

[NEEDS SOURCE for empirical trust measurement — the FCE paper does not include a user study on trust outcomes; see the companion paper Suffian et al. 2025 (IJHCS) for empirical trust evaluation: [[suffian-user-feedback-understanding-trust]].]

## Relevance to Research Questions

**RQ1**: Contributes a technical operationalization of counterfactual transparency as a user-participatory process. Frames XAI transparency not as a static explanation output but as a human-in-the-loop co-construction. The dual feedback mechanism (pre-generation constraints + post-generation evaluation) is a novel operationalization of [[counterfactual-explanations]] within the [[explainability]] taxonomy (source: Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf).

**RQ2**: Not directly addressed empirically; the paper does not measure trust outcomes or test transparency–trust relationships. The claim that user-aligned explanations will reduce trust deficits is theoretical rather than tested (domain: finance). [NEEDS SOURCE]

**RQ3**: Not addressed. The evaluation does not examine user expertise or role differences in how FCE counterfactuals are interpreted or trusted. This is identified as future work (source: Suffian et al._FCE_Feedback_Based_Counterfactual_Explanations_for_Explainable_AI.pdf).

## Related pages

- [[counterfactual-explanations]]
- [[explainability]]
- [[algorithmic-trust]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[suffian-user-feedback-understanding-trust]]
