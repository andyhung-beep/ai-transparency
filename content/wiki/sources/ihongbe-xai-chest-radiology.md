# Evaluating Explainable Artificial Intelligence (XAI) Techniques in Chest Radiology Imaging through a Human-Centered Lens

**Source file**: [Original article](../../raw/Ihongbe et al._Evaluating_Explainable_Artific.pdf)

**Summary**: This study conducts a human-centered evaluation of two visual XAI techniques (Grad-CAM and LIME) for AI-assisted chest disease diagnosis, finding that medical professionals generally preferred Grad-CAM over LIME in terms of comprehensibility and usefulness, but responses on whether XAI improved trust in AI were predominantly neutral or uncertain.

**Sources**: Ihongbe et al._Evaluating_Explainable_Artific.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Ihongbe et al. (2024), published in *PLOS ONE*, address the gap in human-centered evaluation of visual XAI systems in chest radiology. The authors developed two clinical case studies — CNN-based diagnosis of pneumonia from chest X-rays (MobileNetV2, 91% accuracy) and COVID-19 from CT scans (ResNet-101, 98% accuracy) — and applied Grad-CAM and LIME to generate visual explanations. These were then evaluated by 26 medical professionals (8 radiologists, 18 other specialists) via an online questionnaire assessing clinical relevance (usefulness, usability, accuracy), comprehensibility (coherency), and confidence/trust. The study also collected future recommendations for XAI design in clinical imaging contexts.

## Key Findings

- 20 of 26 participants gave positive usefulness scores (3 or higher) for Grad-CAM; only 2 of 26 assigned the highest score (5) for LIME, and 9 participants scored LIME below 2 for usefulness. [domain: healthcare/chest radiology]
- 22 of 26 participants rated Grad-CAM comprehensibility positively (3 or higher); for LIME only 6 of 26 scored 4 or 5. Overall, 19 participants preferred Grad-CAM over LIME. [domain: healthcare/chest radiology]
- 9 participants expressed confidence in XAI visualization accuracy; 7 lacked confidence; 12 were uncertain about whether XAI improved trust in AI diagnostic systems; 11 reported improved trust after reviewing XAI; 3 reported trust unchanged. [domain: healthcare/chest radiology]
- Trust item ("did XAI improve your trust in AI?") received the most neutral scores of all questions, indicating clinician indifference or uncertainty about XAI's trust impact. [domain: healthcare/chest radiology]
- 13 of 26 participants found Grad-CAM's color scheme had a negative impact on scan readability, with color blindness cited as a concern. [domain: healthcare/chest radiology]
- Most participants (16 of 26) had no prior exposure to AI-based medical imaging tools; only 4 had prior knowledge of XAI, highlighting low awareness of XAI among clinicians. [domain: healthcare/chest radiology]
- 21 of 26 participants agreed or strongly agreed that clinicians should be involved in XAI design and development. [domain: healthcare/chest radiology]
- 15 of 24 participants supported adding descriptive textual explanations alongside visual XAI to improve clarity — indicating demand for multi-modal, [[natural-language-explanations]]. [domain: healthcare/chest radiology]
- 19 of 26 participants believed XAI visualizations have the potential to enhance radiology practices overall. [domain: healthcare/chest radiology]
- Participants identified key factors that would increase AI acceptance: transparency in training/testing processes, human supervision, high accuracy, and understanding of AI decision-making rationale. [domain: healthcare/chest radiology]

## Transparency Constructs

The paper evaluates [[explainability]] operationalized as visual XAI techniques applied to deep learning image classifiers:
- **Grad-CAM**: gradient-based heatmap overlaid on input images highlighting regions most influential for classification — a form of [[outcome-transparency]] at the feature level.
- **LIME**: local interpretable model-agnostic explanations using superpixel segmentation to identify and highlight/mask regions contributing to prediction.

Evaluation criteria for transparency follow Jin et al. (2023): understandability, clinical relevance, truthfulness, informative plausibility, and computational efficiency. The paper calls for multi-modal explainability combining visual and textual elements.

## Trust Constructs

Trust is primarily measured as [[cognitive-trust]]/confidence: participants rate the extent to which explanations "truthfully reflect the AI model's decision process, influencing trust and confidence in the results." The questionnaire captures self-reported confidence in the AI system's outputs with and without XAI. No behavioural trust measure (e.g., reliance, adoption) is included. The paper documents that trust effects of XAI on medical professionals are predominantly neutral or uncertain — a finding contributing to the evidence on null effects in [[rq2-relationships]].

## Relevance to Research Questions

**RQ1**: The paper contributes a domain-specific operationalization of XAI in chest radiology, adapting clinical evaluation criteria (clinical relevance, comprehensibility, confidence/trust) from Jin et al. It highlights awareness gaps among medical practitioners as a factor limiting the uptake and meaningful evaluation of XAI.

**RQ2**: The study finds largely neutral or mixed effects of XAI on self-reported trust among clinicians — the trust question received the most neutral scores of all questionnaire items. This is consistent with other null or mixed trust-effect findings in the XAI literature, and the study underscores domain-specificity: in healthcare, trust effects may be especially hard to detect given clinicians' professional caution. The study also finds differential performance between XAI methods (Grad-CAM > LIME on comprehensibility and usefulness).

**RQ3**: The study recruits exclusively from clinicians and radiologists (domain experts) and explicitly examines their AI/XAI awareness and experience. Participants' low prior AI exposure is identified as a mediating factor in trust and confidence responses. This study thus contributes to understanding how experienced domain experts (but AI novices) respond to XAI — a specific expertise configuration relevant to RQ3.

## Related pages

- [[explainability]]
- [[outcome-transparency]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[domain-context]]
- [[rq2-relationships]]
- [[rq3-user-roles]]
