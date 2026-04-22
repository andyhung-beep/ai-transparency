# Co-design of Human-centered, Explainable AI for Clinical Decision Support

**Source file**: [Original article](../../raw/Panigutti et al._Co-design of human-centered, explainable AI for clinical decision.pdf)

**Summary**: An iterative co-design study presenting Doctor XAI—an ontology-aware, local, rule-based explainer for clinical decision support—and its user interface, validated in an online study with 41 healthcare providers; finds that explanations significantly increase implicit trust (weight-of-advice) but not explicit trust, behavioural intention, or confidence, and that user feedback drives a redesign to progressive-disclosure interface.

**Sources**: Panigutti et al._Co-design of human-centered, explainable AI for clinical decision.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Published in *ACM Transactions on Interactive Intelligent Systems* (December 2023) by Panigutti, Beretta, Fadda, Giannotti, Pedreschi, Perotti, and Rinzivillo, this article presents one full cycle of an iterative, human-centred design process for an XAI system in healthcare. The technical contribution is Doctor XAI, a model-agnostic, local explainer tailored to sequential, ontology-linked patient data (ICD-9 codes) and multi-label prediction tasks. The human validation uses a within-subject online experiment (N = 41 healthcare providers) to evaluate the impact of explanations on trust.

The experiment is structured as a Judge-Advisor System (JAS): participants estimate a patient's risk of acute myocardial infarction before and after receiving either (a) an AI suggestion only or (b) an AI suggestion plus explanation. The primary trust measure is the Weight of Advice (WOA)—how much the participant shifts their estimate toward the AI's prediction. Explicit trust, confidence, and behavioural intention are also measured.

The paper then redesigns the explanation user interface (XUI) based on open-ended feedback, implementing progressive disclosure of information to reduce information overload.

## Key Findings

- Participants showed significantly higher **Weight of Advice (WOA) for the interface with explanation** (Mdn = 0.33) than without (Mdn = 0.12), indicating that explanations increased implicit trust in the AI's suggestion. (Domain: healthcare)
- **No significant difference in explicit trust** (self-reported reliability, predictability, efficiency) was found between the explanation and no-explanation conditions. (Domain: healthcare)
- **No significant difference in behavioural intention** to use the system was found; however, behavioural intention was strongly positively correlated with perceived explanation quality (rs = 0.60, p < 0.001). (Domain: healthcare)
- **Explanation quality—not mere presence—drives adoption intention**: since Doctor XAI's initial explanations were perceived as ill-suited (too technical, ICD-code-heavy), the absence of a behavioural intention effect is attributed to explanation inadequacy rather than a failure of XAI as a category. (Domain: healthcare)
- Open-ended responses revealed **information overload** as the primary complaint: participants liked having more information but found the explanation interface cognitively demanding and slow.
- Qualitative feedback identified a recurring fear of being **replaced by AI**, linked to algorithm aversion. Participants accepted the AI as a tool but resisted reliance on it. (Domain: healthcare)
- The **redesigned interface** (progressive disclosure: natural language first → highlighted diagnoses → full ICD-coded timeline) was rated more usable on Nielsen's heuristics, particularly for recognition-over-recall and minimalist design.
- A **familiarity-with-task confound** was identified: WOA in the no-explanation condition was significantly negatively correlated with task familiarity (rs = -0.51, p < 0.001), meaning less familiar participants relied more on the AI without explanation.

## Transparency Constructs

- **Explainability / interpretability**: Doctor XAI produces local, rule-based, natural-language explanations from a multi-label decision tree trained on a synthetic neighbourhood of the patient instance. See [[explainability]], [[natural-language-explanations]].
- **Algorithmic transparency**: The paper distinguishes the XAI technique (extracting the explanation from the black box) from the explanation user interface (presenting it to the user)—a conceptually important separation. See [[algorithmic-transparency]].
- **Process transparency**: The first prototype displays the full patient ICD-code history with colour-coded relevance marks—a highly process-transparent but cognitively demanding interface. See [[process-transparency]].
- **Outcome transparency**: The redesigned interface leads with a natural language prediction statement and an explanation, before revealing the technical substrate, privileging outcome-level transparency. See [[outcome-transparency]].
- **Uncertainty visualisation**: Participants in open questions explicitly requested accuracy/reliability information ("we don't know how reliable it is"); the system did not provide uncertainty estimates, and this was identified as a limitation requiring future technical work. See [[uncertainty-visualization]].

## Trust Constructs

- **Cognitive trust (implicit)**: Operationalised as WOA—a behavioural proxy for how much a user is influenced by the AI's advice. See [[cognitive-trust]], [[algorithmic-trust]].
- **Cognitive trust (explicit)**: Measured via a 5-item questionnaire on reliability, predictability, and efficiency. See [[cognitive-trust]].
- **Behavioural trust**: Measured as behavioural intention to use the system (UTAUT/TAM constructs). See [[behavioural-trust]].
- **Algorithm aversion**: Expressed in open-ended comments; participants feared replacement, resisted uncritical reliance, and emphasised human judgment. See [[algorithm-aversion]].
- **Trust calibration**: The paper explicitly frames the co-design goal as appropriate trust calibration (not just trust maximisation), noting that the increase in WOA with explanations may partly reflect automation bias risk, since only correct AI predictions were used. See [[trust-calibration]].

## Relevance to Research Questions

**RQ1**: The paper operationalises trust in three ways—implicit (WOA), explicit (questionnaire), and intentional (BI)—and finds divergent results across measures, reinforcing the need to distinguish trust types. Explainability is operationalised as rule-based natural language explanations from a domain-specific XAI method. Explanation quality (satisfaction scale) is measured separately from explanation presence. See [[rq1-conceptualizations]].

**RQ2**: Reports a dissociation: explanations increase implicit trust (WOA) but not explicit trust or behavioural intention. The explanation quality × trust relationship is the operative mechanism: poorly suited explanations (designed for ML debugging, not clinical use) fail to raise explicit trust or BI, while still shifting estimates through a persuasion-like implicit channel. This is a conditional effect suggesting that naive provision of explanations is insufficient. See [[rq2-relationships]].

**RQ3**: All participants are healthcare professionals (doctors, nurses, paramedics); the study focuses on how domain experts engage with AI explanations in their professional context. Algorithm aversion and fear-of-replacement emerge as occupationally grounded responses. Task familiarity moderates implicit trust (WOA) in the no-explanation condition. See [[rq3-user-roles]], [[user-expertise]], [[perceived-risk]].

## Related pages

- [[natural-language-explanations]]
- [[trust-calibration]]
- [[algorithm-aversion]]
- [[algorithmic-transparency]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
