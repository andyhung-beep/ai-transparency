# Explaining Recommendations through Conversations: Dialog Model and the Effects of Interface Type and Degree of Interactivity

**Source file**: [Original article](../../raw/Hernandez-Bocanegra & Ziegler_Explaining recommendations through conversations.pdf)

**Summary**: This paper proposes and empirically evaluates conversational, interactive explanations for recommender systems, finding that higher interactivity (allowing users to drill into supporting arguments) and GUI-based navigation both positively influence perceived explanation quality, which in turn mediates trust and transparency perceptions via a structural equation model.

**Sources**: Hernandez-Bocanegra & Ziegler_Explaining recommendations through conversations.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Hernandez-Bocanegra and Ziegler (2023), published in *ACM Transactions on Interactive Intelligent Systems*, investigate the potential of interactive, conversational explanations in hotel recommender systems (RS). The paper argues that static, single-presentation explanations fail to meet individual users' varying information needs. The authors propose explanations as interactive argumentation, grounded in dialog models and formal argument structures (claim, premise, backing, rebuttal, refutation). Two interface types are implemented: a GUI-based navigation interface and a natural language chatbot (ConvEx). A user study (N = 223) tests the effects of interface type and degree of interactivity on perceived explanation quality, transparency, trust, and effectiveness using Structural Equation Modeling (SEM).

The paper also develops ConvEx-DS, a dataset of 1,806 annotated user questions in the hotel domain, and an intent model covering dimensions of scope, comparison, assessment, and detail.

## Key Findings

- Higher interactivity (access to filtered customer comments supporting or rebutting aggregated aspect ratings) had a significant positive direct effect on perceived explanation quality, compared to lower interactivity conditions. [domain: e-commerce/hospitality]
- GUI navigation yielded higher perceived explanation quality scores (M = 3.87) than the natural language chatbot (M = 3.69), contrary to the hypothesis that conversational interfaces would be more beneficial. [domain: e-commerce/hospitality]
- SEM revealed a causal chain: perceived explanation quality → information provision (transparency) → understanding input/output → interaction transparency → trusting beliefs. [domain: e-commerce/hospitality]
- Perceived explanation quality and trusting beliefs both had direct positive effects on perceived effectiveness (usefulness of the RS for decision-making). [domain: e-commerce/hospitality]
- Rational decision-making style moderated the relationship between interactivity degree and explanation quality: more rational users in high-interactivity conditions rated explanation quality significantly higher. [domain: e-commerce/hospitality]
- Intuitive decision-making style and visualization familiarity did not significantly moderate the effect of interface type on explanation quality. [domain: e-commerce/hospitality]
- Transparency sub-constructs (information provision, understanding input/output, interaction) were significantly related but empirically distinct; interestingly, trusting intentions and perceived effectiveness could not be discriminated and were merged in the model. [domain: e-commerce/hospitality]
- Users asked primarily factoid and evaluation questions; only 24 of 1,806 questions addressed system-level concerns (algorithm, input type), suggesting general-public users are less concerned with system internals than AI-expert users. [domain: e-commerce/hospitality]
- System answers to user questions were rated as helpful on average (M = 3.58 on a 1–5 scale), with the most refined system version reaching M = 3.70. [domain: e-commerce/hospitality]

## Transparency Constructs

The paper makes a fine-grained distinction among [[process-transparency]] constructs, operationalizing transparency as four sub-constructs following Hellmann et al.: information provision (functions explicitly disclosing how recommendations are generated), understanding input (what data the system uses), understanding output (why/how well an item fits preferences), and interaction (what to change for a different prediction). This is a multi-dimensional operationalization of [[algorithmic-transparency]] applied to RS. The interactive argumentation interface also enacts [[outcome-transparency]] by allowing users to probe supporting and opposing evidence for recommendations.

## Trust Constructs

The paper separately measures [[cognitive-trust]] as trusting beliefs (the system is honest and competent) and trusting intentions (willingness to act on recommendations), though discriminant validity analysis led to dropping trusting intentions and retaining only trusting beliefs in the final SEM. Perceived effectiveness captures a behavioural dimension related to [[behavioural-trust]]. The SEM demonstrates that perceived transparency mediates the path from explanation quality to trust.

## Relevance to Research Questions

**RQ1**: The paper provides a detailed multi-dimensional operationalization of transparency in RS (information provision, understanding input/output, interaction) and links these to explanation quality and trust. It also contributes a rich operationalization of conversational/interactive explainability beyond static XAI.

**RQ2**: The SEM results establish a positive causal chain from explanation quality to transparency, and from transparency to trust — broadly consistent with a positive, mediated transparency–trust relationship. However, the direct effect on trust of interface type was not found; rather, explanation quality mediated the relationship. The paper thus documents a conditional pattern: interactivity benefits explanation quality, which then benefits trust.

**RQ3**: Rational decision-making style (a proxy for information-processing preference rather than domain expertise per se) moderated the high-interactivity advantage. More rational users benefited more from the interactive, detail-rich explanations. This is relevant to RQ3 as a user-characteristic moderator of the explanation–evaluation link.

## Related pages

- [[process-transparency]]
- [[algorithmic-transparency]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
