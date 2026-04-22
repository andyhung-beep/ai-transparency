# Unlocking the Black Box: Enhancing Human-AI Collaboration in High-Stakes Healthcare Scenarios Through Explainable AI

**Source file**: [Original article](../../raw/Hassan et al._Unlocking the black box.pdf)

**Summary**: A qualitative study using 28 scenario-based semi-structured interviews with clinicians from Norway and Egypt shows that AI opacity triggers "interrogation practices" in expert users, and that introducing XAI to explain cerebral palsy risk predictions increases expert trust, willingness to learn from AI, and readiness to revise prior judgments, while also raising concerns about learning myopia and over-reliance.

**Sources**: Hassan et al._Unlocking the black box.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Hassan, Nguyen, Finserås, Adde, Strømke, and Støen (2025), published in *Technological Forecasting & Social Change* (vol. 219, 124265; doi: 10.1016/j.techfore.2025.124265), investigate how clinicians respond to AI opacity and the transition to explainability in a high-stakes medical context. The AI system studied is a Graph Convolutional Network (GCN) that predicts cerebral palsy (CP) risk by analyzing infant movement videos. The study uses a scenario-based methodology: 28 semi-structured interviews and observations with clinicians from Norway (n ≈ 17+) and Egypt, confronting them with the AI system's predictions first in opaque form and then with XAI insights.

The paper is qualitative and grounded in organizational science and knowledge work theory. It frames human-AI collaboration as a knowledge-sharing activity in which opacity creates epistemic barriers, and XAI facilitates the reconciliation of divergent human and AI knowledge claims.

## Key Findings

- When facing opaque AI predictions, clinicians engage in "AI interrogation practices" — actively questioning, probing, and seeking rationale for AI outputs — as a means of coping with epistemic uncertainty. Opacity does not simply cause rejection; it generates a work burden of interpretation. (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- When XAI insights are introduced (visualizations of which body movement features contributed to the CP risk prediction), clinicians demonstrate increased trust in the AI system and engage in deeper, more constructive interrogation. (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- XAI fosters a "willingness to learn from AI": clinicians described the explainability features as a pedagogical resource, especially valuable in specialties where experienced mentors and case exposure are scarce (e.g., neonatal CP assessment). (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- XAI can cause expert judgment revision: when XAI reveals that the AI identifies features the clinician had not weighted heavily, some experts reconsidered or updated their initial clinical judgments. Some experienced self-doubt about their own competence. (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- The authors warn that over-reliance on XAI-mediated AI evaluations could lead to "learning myopia" in organizations, whereby the development of human clinical skill is atrophied by dependence on AI explanations for standardized evaluation tasks. (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- AI opacity is characterized as creating epistemic uncertainty, which undermines user trust, error detection, and accountability in critical decision-making — consistent with algorithm aversion and black-box criticism literature (Rudin, 2019; Dietvorst et al., 2018). (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)
- The study proposes design guidelines for human-AI interactions in critical judgment contexts, emphasizing that XAI should support but not replace expert judgment formation. (source: Hassan et al._Unlocking the black box.txt; domain: healthcare / neonatology)

## Transparency Constructs

The study treats transparency/explainability in terms of whether the AI system reveals the features or reasoning behind its predictions to expert users. The XAI system in question uses a GCN and provides spatial and temporal body movement features as visual explanations — a form of [[explainability]] and [[process-transparency]] specific to the model's feature-importance reasoning.

Key transparency concepts in the paper:
- **AI opacity / black box**: The absence of explanation — the baseline condition that triggers interrogation practices and undermines trust. Equivalent to zero [[algorithmic-transparency]].
- **XAI insights**: Feature-importance visualizations that make visible which aspects of infant movement drive the CP risk prediction, constituting local [[explainability]] and [[causability]] in the sense of Holzinger et al. (enabling clinicians to understand the causal basis of predictions).
- **Epistemic uncertainty**: The cognitive state produced by opacity; resolved (partially) by XAI.

The paper is notable for distinguishing between the transition from opaque to explainable states as an event that changes expert cognitive processes and decision confidence — not merely a static feature of the system.

## Trust Constructs

Trust is studied qualitatively and is primarily [[cognitive-trust]] in the sense of clinicians' belief in the AI system's reliability and the validity of its predictions. Key trust-related observations:

- Prior to XAI: clinicians show guardedness, skepticism, and interrogation behaviors — characteristic of low or conditional trust.
- After XAI: clinicians exhibit increased trust and learning readiness — suggesting XAI shifts trust from conditional to higher-confidence.
- Expert self-doubt: some clinicians revised their own judgments after XAI disclosure, raising the possibility that XAI can produce inappropriate over-trust or unwarranted deference to AI.

The paper also engages [[appropriate-reliance]] as a normative ideal: XAI should help experts use AI appropriately (neither ignoring it nor deferring to it uncritically), but the risk of learning myopia suggests this goal is non-trivially achieved. The construct of [[algorithm-aversion]] appears implicitly: opacity drives non-compliance with AI recommendations.

## Relevance to Research Questions

**RQ1**: The paper provides a rich qualitative conceptualization of how explainability functions as an epistemic resource in clinical judgment formation. It foregrounds interrogation practices as an intermediary mechanism between opacity and trust, contributing to RQ1 by showing how transparency is not merely a feature of systems but an active process in human-AI knowledge integration. The paper also contributes a clear operational context: high-stakes neonatal assessment in a clinical setting.

**RQ2**: The study finds a positive transition from opaque to explainable states in terms of trust (more trust, more learning readiness, judgment revision with XAI) in the healthcare domain. This is consistent with a positive transparency–trust relationship. However, the paper also documents non-linear risks: XAI-enabled trust may tip into over-reliance and learning myopia, suggesting that the relationship is not monotonically positive and depends on how XAI is integrated into clinical workflows. This contributes to RQ2's interest in conditional and potentially U-shaped effects.

**RQ3**: This paper is among the strongest contributions to RQ3 in the collection. Expert clinicians are the study population, and the entire analysis concerns how professional expertise interacts with AI transparency. Key findings: experts use professional judgment as a reference point for evaluating AI predictions; XAI influences expert confidence and willingness to revise judgment; less experienced clinicians in sparse-expertise settings may be more susceptible to learning myopia. The cross-national sample (Norway and Egypt) also hints at potential cultural or systemic moderators of expert–AI interaction.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[causability]]
- [[cognitive-trust]]
- [[appropriate-reliance]]
- [[algorithm-aversion]]
- [[user-expertise]]
- [[domain-context]]
- [[perceived-risk]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
