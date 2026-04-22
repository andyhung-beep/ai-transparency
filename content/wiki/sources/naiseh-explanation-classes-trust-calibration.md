# How the Different Explanation Classes Impact Trust Calibration: The Case of Clinical Decision Support Systems

**Source file**: [Original article](../../raw/Naiseh et al._How the different explanation classes impact trust calibration.pdf)

**Summary**: An empirical within-subject study with 41 medical practitioners comparing how four XAI classes (Local, Example-based, Counterfactual, and Global explanations) affect trust calibration in a clinical decision support system; finds that explanation class significantly shapes perceived understandability and technical competence but that all classes risk increasing over-reliance on incorrect AI recommendations.

**Sources**: Naiseh et al._How the different explanation classes impact trust calibration.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in the *International Journal of Human-Computer Studies* (2023), this study by Naiseh, Al-Thani, Jiang, and Ali investigates whether different XAI explanation classes help or hinder appropriate trust calibration in Human-AI collaborative decision-making. Using a mock chemotherapy prescription screening tool as the case study, participants encountered correct and incorrect AI recommendations accompanied by one of four explanation classes (or no explanation). The study combines quantitative trust ratings with semi-structured interviews.

[[Trust-calibration]] is defined as "an appropriate trust judgement made by humans regarding the current state of AI capabilities … and a successful assessment of whether to follow or reject AI recommendations" (Lee and See, 2004). The paper distinguishes trust calibration from simply increasing trust: calibrated trust requires cognitive engagement with the explanation, not merely exposure to it.

## Key Findings

- Example-based and Counterfactual explanations produced significantly higher **perceived understandability** than Local, Global, and No-explanation conditions. (Domain: healthcare/clinical decision support)
- Counterfactual explanations produced significantly higher **perceived technical competence** than all other conditions; participants attributed this to counterfactuals making the AI's causal reasoning visible. (Domain: healthcare)
- **Perceived reliability** did not differ significantly across explanation classes, suggesting reliability perceptions are tied to overall AI performance rather than explanation type. (Domain: healthcare)
- All four explanation classes significantly improved **overall Human-AI team performance** compared to No-explanation, consistent with prior work. (Domain: healthcare)
- Critically, **no explanation class helped participants identify incorrect AI recommendations**. Participants agreed more with the AI in all explanation conditions, indicating increased over-reliance (confirmation and automation bias). (Domain: healthcare)
- Qualitative analysis identified six interface needs across XAI classes: task-centred explanation, usability, assurances, guidance (especially for Local/Global), tailoring, and multi-step explainability.
- Local and Global explanations required additional guidance and domain-contextualisation to be interpretable by clinical end-users; participants misread feature-importance values as clinical advice.

## Transparency Constructs

- **Explainability**: The central construct. Four classes are systematically compared: Local (feature importance scores), Example-based (similar cases from training data), Counterfactual (what-if feature changes), and Global (model-wide feature rankings). See [[explainability]], [[counterfactual-explanations]], [[example-based-explanations]].
- **Causability**: Multi-step explainability needs and participants' desire to understand why a feature matters are framed in terms of causability. See [[causability]].
- **Process transparency**: Participants wanted explanations embedded within clinical workflow constraints, not generic model outputs. See [[process-transparency]].

## Trust Constructs

- **Cognitive trust**: Measured via Madsen and Gregor's (2000) Human-Computer Trust (HCT) scale across three components—perceived understandability, perceived reliability, and perceived technical competence. See [[cognitive-trust]].
- **Behavioural trust**: Measured via three indicators—agreement with AI recommendation, switch from AI recommendation, and Human-AI team performance on the classification task. See [[behavioural-trust]], [[appropriate-reliance]].
- **Trust calibration**: Defined as aligning trust with actual AI capability; over-reliance (following incorrect recommendations) and under-reliance (rejecting correct ones) are both failures. See [[trust-calibration]].
- **Algorithm aversion**: Addressed indirectly; some participants gave low scores to Local/Global explanations they could not interpret, risking rejection of functional AI suggestions. See [[algorithm-aversion]].

## Relevance to Research Questions

**RQ1**: The paper operationalises trust calibration via both self-reported cognitive trust (HCT scale) and behavioural indicators (agreement, switch rate, task performance). It also operationalises explainability as four discrete, model-agnostic output classes, making this a rich source for understanding construct definitions. See [[rq1-conceptualizations]].

**RQ2**: Key finding is a conditional, non-linear pattern: explanations improve overall performance but exacerbate over-reliance on incorrect recommendations. Counterfactual and Example-based classes benefit understandability; Global and Local classes can reduce trust when poorly contextualised. Explains apparent contradiction in prior literature—effects depend on explanation class and task. See [[rq2-relationships]].

**RQ3**: Study sample is expert clinicians (doctors and pharmacists) with experience in prescription screening. Participants' professional knowledge shaped their interaction: they misinterpreted Local/Global feature-importance scores through clinical rather than statistical lenses, suggesting user expertise (clinical, not AI expertise) modulates explanation effectiveness. See [[rq3-user-roles]], [[user-expertise]].

## Related pages

- [[trust-calibration]]
- [[explainability]]
- [[counterfactual-explanations]]
- [[example-based-explanations]]
- [[appropriate-reliance]]
- [[rq2-relationships]]
