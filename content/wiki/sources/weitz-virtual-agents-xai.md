# "Let Me Explain!": Exploring the Potential of Virtual Agents in Explainable AI Interaction Design

**Source file**: [Original article](../../raw/Weitz_Let me explain.pdf)

**Summary**: This paper reports a user study exploring how incorporating a virtual agent with varying degrees of human-likeness (text, voice, or embodied visual presence) into an XAI interface affects end-users' perceived trust in an AI speech recognition system. Results show a significant linear trend: as the human-likeness of the agent increases, trust in the AI increases proportionately, with the embodied visual agent producing the highest trust.

**Sources**: Weitz_Let me explain.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Published in the Journal on Multimodal User Interfaces (Vol. 15, 2021), this paper by Weitz, Schiller, Schlagowski, Huber, and André from Augsburg University investigates whether the humanization of AI explanation delivery — via a virtual agent named Gloria — increases user trust in a deep learning speech recognition model. The underlying XAI technique used was LIME (Local Interpretable Model-Agnostic Explanations), which highlighted relevant segments of spectrograms corresponding to spoken keyword classifications.

Sixty participants were divided equally into four groups: no-agent (XAI only), text-agent, voice-agent, and embodied-visual-agent. All groups received LIME visualizations; agent groups also received commentary from Gloria via their respective modality. Trust was measured post-experiment using the Trust in Automation (TiA) questionnaire.

## Key Findings

- A significant linear trend in trust was confirmed: trust increased with human-likeness of the agent (R² = .16, F(3,56) = 3.45, p = .02, f = 0.42, medium effect size) (source: Weitz_Let me explain.txt; domain: speech recognition / human-computer interaction).
- Mean trust scores: no agent (M = 4.48), text agent (M = 4.89), voice agent (M = 5.12), embodied visual agent (M = 5.42), all on a 7-point scale (source: Weitz_Let me explain.txt; domain: speech recognition / HCI).
- XAI visualizations alone (no agent) were not rated as highly sufficient by participants (average around 4 out of 7), indicating room for improvement in purely visual explanation methods (source: Weitz_Let me explain.txt; domain: speech recognition / HCI).
- Ratings of LIME visualizations did not differ significantly between groups (F(1,58) = 0.47, p = .495), but participants in agent groups rated them more positively — suggesting a halo effect from increased trust in the system (source: Weitz_Let me explain.txt; domain: speech recognition / HCI).
- Participants requested more linguistic (natural language) explanations, comparative visualizations (showing what a correct prediction would look like), and greater interactivity with the system (source: Weitz_Let me explain.txt; domain: speech recognition / HCI).
- Body gestures of the embodied agent (e.g., pointing at spectrograms) were perceived as helpful for directing attention to XAI visualizations (source: Weitz_Let me explain.txt; domain: speech recognition / HCI).

## Transparency Constructs

The study operationalizes [[explainability]] through LIME-generated visual explanations (saliency-map-style highlights on spectrograms showing which audio segments most influenced the neural network's keyword classification). This represents a **local, post-hoc, model-agnostic** explanation technique.

The paper also explores the delivery medium as a transparency dimension: how explanations are communicated (text, voice, embodied agent) independently modulates the perceived transparency and trustworthiness of the system. This is framed as an interaction design question for [[process-transparency]].

The virtual agent's commentary operationalizes a form of [[natural-language-explanations]], providing verbalized highlights (e.g., "Phoneme number two was found to have a particularly positive effect toward the prediction") alongside the visual XAI output.

## Trust Constructs

Trust is measured via the Trust in Automation (TiA) questionnaire (Jian et al., 2000), capturing situational [[cognitive-trust]] in an AI system. The authors frame this as primarily **situational trust** — strongly dependent on external interface features (agent type, task difficulty, system complexity) rather than dispositional or learned trust.

The paper acknowledges that increasing trust through humanization could raise concerns about inappropriately elevated trust (over-trust), connecting to [[trust-calibration]] and [[algorithm-aversion]] literature.

## Relevance to Research Questions

**RQ1**: Contributes to the conceptualization of transparency not merely as information content but as a delivery modality. The study shows that the same LIME explanations produce different levels of trust depending on how they are presented, suggesting that the social/communicative form of explanation is a distinct transparency dimension. Relevant to [[rq1-conceptualizations]].

**RQ2**: Provides clear evidence of a positive, linear transparency–trust relationship where the mechanism is the human-likeness of the explanation interface rather than the informational content itself. The effect is significant and replicable from a prior pilot study (Weitz et al., 2019). The non-informational pathway to trust building (interface humanization rather than explanation quality) is a distinct conditional pattern for [[rq2-relationships]].

**RQ3**: The study uses non-expert participants and does not segment by expertise. Participants varied in background experience with voice assistants and audio processing, but these were not analyzed as moderators. The study notes that background knowledge (e.g., signal processing expertise) could constitute an internal trust factor worth examining in future research. Marginally relevant to [[rq3-user-roles]].

## Related pages

- [[explainability]]
- [[natural-language-explanations]]
- [[process-transparency]]
- [[cognitive-trust]]
- [[trust-calibration]]
- [[rq2-relationships]]
