# "If It Is Easy to Understand Then It Will Have Value": Examining Perceptions of Explainable AI with Community Health Workers in Rural India

**Source file**: [Original article](../../raw/Okolo et al._If it is easy to understand then it will have value.pdf)

**Summary**: A qualitative field study with 35 low-literacy community health workers (CHWs) in rural Uttar Pradesh, India, examining how they perceive and engage with simplified LIME and SHAP explanations via a neonatal jaundice diagnostic probe; finds that standard XAI visualisations are largely incomprehensible to CHWs but that CHWs nonetheless strongly value explanations for skill-building and community trust.

**Sources**: Okolo et al._If it is easy to understand then it will have value.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *Proceedings of the ACM on Human-Computer Interaction* (CSCW, April 2024) by Okolo, Agarwal, Dell, and Vashistha, this paper conducts semi-structured interviews and design-probe interactions with 35 female CHWs in rural Uttar Pradesh. Participants interacted with a Figma prototype that simulated an AI-based neonatal jaundice diagnostic tool displaying simplified LIME and SHAP explanations. The study contributes to human-centred XAI (HCXAI) research by decentring Western perspectives and examining a novice, low-AI-literacy, high-stakes user population.

The design probe presented two simplified XAI visualisations:
- **LIME-based**: Yellow/grey colour overlay highlighting contributing body regions.
- **SHAP-based**: Multiple annotated images with coloured boxes and a horizontal colour bar.

Colours were modified from standard red/green to yellow/grey (LIME) and yellow/green (SHAP) to avoid triggering medical danger associations with red. The research iteratively redesigned visualisations across interviews in response to CHW feedback.

## Key Findings

- CHWs were almost entirely unable to correctly interpret the LIME and SHAP visualisations; they systematically **misread feature-importance highlights as symptoms of jaundice** rather than as the model's feature contributions. (Domain: primary/community healthcare, rural India)
- CHWs displayed **high AI techno-determinism** ("a machine can never be wrong") and treated AI predictions as definitive diagnoses rather than probabilistic estimates, indicating over-reliance risk. (Domain: healthcare, Global South)
- The **presence of explanations reinforced, rather than mitigated, over-reliance**: explanations were taken as additional confirmation that the AI was correct, even when CHWs could not understand them. (Domain: healthcare)
- Despite confusion, CHWs **strongly preferred to have explanations** included in any future tool, citing benefits for personal skill development, patient communication, and community trust in AI. (Domain: healthcare)
- **Colour mental models** profoundly disrupted XAI interpretation: CHWs applied public-health colour conventions (green=safe, yellow=warning, red=danger, grey=lack of blood), leading to systematic misinterpretation of LIME/SHAP colour schemes. (Domain: healthcare, cross-cultural design)
- Replacing colour with shape-based cues (circles/squares) reduced colour-association interference and helped a subset of CHWs form more accurate, domain-grounded interpretations, though confusion persisted. (Domain: healthcare)
- CHWs consistently **ignored or could not interpret textual and numerical elements** (legends, colorbars, percentage confidence labels, decimal values), restricting interpretability to purely visual/graphical elements. (Domain: healthcare, low-literacy)
- CHWs compared the AI app to familiar diagnostic devices (thermometer, blood pressure monitor), drawing on device-based rather than AI-based mental models. (Domain: healthcare)
- The study generates design recommendations: remove colour-coded gradients for low-literate users; use contextually grounded labels and analogies; provide scaffolding training; develop accessible XAI terminology in local languages. (Domain: healthcare, Global South)

## Transparency Constructs

- **Explainability**: The study evaluates simplified LIME and SHAP as visual explainability methods for end-users who are novice AI users. See [[explainability]].
- **Outcome transparency**: CHWs primarily understood the AI's prediction output (severity level), not its underlying reasoning. See [[outcome-transparency]].
- **Process transparency**: The gap between feature-importance explanations (what LIME/SHAP provide) and the symptom-based reasoning CHWs expected points to a fundamental process-transparency mismatch. See [[process-transparency]].
- **Uncertainty visualisation**: Confidence values (percentages, size of images, "most/least confidence" labels) were consistently misinterpreted; the concept of probabilistic prediction was foreign to the CHW mental model. See [[uncertainty-visualization]].

## Trust Constructs

- **Behavioural trust / over-reliance**: CHWs exhibited uncritical acceptance of AI outputs; explanations exacerbated this. See [[behavioural-trust]], [[appropriate-reliance]], [[algorithm-aversion]].
- **Cognitive trust**: CHWs attributed high competence to the AI system based on analogy with trusted medical devices, not based on understanding of the AI. See [[cognitive-trust]].
- **Institutional trust**: Community and patient trust in CHWs is identified as a downstream benefit of deploying explainable AI tools—CHWs believed that showing the app and its explanation to patients would increase their own legitimacy. See [[institutional-trust]].
- **Algorithmic trust**: The paper documents a form of uncritical algorithmic trust (AI authority) that is culturally amplified in the Indian rural context. See [[algorithmic-trust]].

## Relevance to Research Questions

**RQ1**: The paper problematises standard HCXAI operationalisations of explainability by showing that constructs like "feature importance" are entirely foreign to CHW mental models. It also introduces an important distinction: CHWs valued explanations for social and communicative functions (legitimacy, trust with patients) rather than for their primary epistemic function (understanding model logic). Transparency is operationalised via two visual XAI methods (LIME, SHAP) evaluated through interview data and iterative prototype refinement. See [[rq1-conceptualizations]].

**RQ2**: Finds a paradoxical positive relationship: explanations increased CHWs' reported desire for AI use while failing to increase accurate understanding, and appeared to strengthen over-reliance rather than calibrate trust. This is a null-to-negative calibration effect—the opposite of the intended function of XAI—with domain-specific amplification in a low-AI-literacy, high-AI-authority context. See [[rq2-relationships]].

**RQ3**: The entire paper is structured around a low-expertise, non-Western user population whose characteristics (low digital/AI literacy, high dispositional AI trust, strong colour-association mental models, low familiarity with probabilistic reasoning) fundamentally shape every aspect of XAI effectiveness. The study is a critical reference for moderating effects of user expertise and cultural context. See [[rq3-user-roles]], [[user-expertise]], [[domain-context]], [[perceived-risk]].

## Related pages

- [[explainability]]
- [[uncertainty-visualization]]
- [[appropriate-reliance]]
- [[user-expertise]]
- [[domain-context]]
- [[rq3-user-roles]]
