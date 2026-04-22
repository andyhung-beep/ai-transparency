# Personalized Explanations for Clinician-AI Interaction in Breast Imaging Diagnosis by Adapting Communication to Expertise Levels

**Source file**: [Original article](../../raw/Calisto et al._Personalized explanations for clinician-AI interaction in breast image.pdf)

**Summary**: This study examines how adapting AI communication style (assertive vs. non-assertive vs. conventional) to clinicians' expertise level (interns, juniors, middles, seniors) affects diagnostic efficiency, accuracy, trust, and workload in a breast cancer imaging context, finding that personalized assertiveness-based communication significantly reduces diagnostic time and that preferred communication style differs by experience level.

**Sources**: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-18

---

## Overview

Calisto, Abrantes, Santiago, Nunes, and Nascimento (2025, published in International Journal of Human-Computer Studies) report a within-subject user study involving 52 clinicians from eleven Portuguese clinical institutions, investigating how the tone and style of AI communication influence breast cancer diagnostic performance. The clinical context involves multimodal imaging (mammography, ultrasound, and MRI) and AI-generated BIRADS severity predictions.

The study compares three conditions: (1) a conventional agent that provides only numerical BIRADS scores and model accuracy metrics; (2) an assertive agent that actively imposes AI recommendations with direct, confident language and detailed clinical explanations (lesion morphology, patient history, visual severity indicators); and (3) a non-assertive agent that suggests recommendations tentatively. Clinicians were categorized as interns, juniors, middles, and seniors based on years of clinical experience, and interacted with each condition in counterbalanced order while diagnosing a dataset of 289 patients. Measures included diagnostic time, classification accuracy (precision, recall, F1), trust (understanding, competence, thoughtfulness dimensions), cognitive workload (NASA-TLX), and system usability (SUS).

The study extends a prior CHI 2023 paper (Calisto et al., 2023a) by using more granular expertise categories (four groups rather than a simple novice/expert distinction) and focusing on specific measurable outcomes. The AI backend uses DenseNet for 2D MG and US images and 3D ResNet for MRI volumes.

## Key Findings

- Assertiveness-based AI communication significantly reduced diagnostic time across all expertise levels (F = 11.32, p = 0.005, large effect size r = 0.49), with interns and juniors improving by a factor of approximately 1.38 and middle and senior clinicians by approximately 1.37 compared to the no-AI baseline (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)
- Assertive communication was more effective for interns and juniors: novice clinicians achieved 81.59% overall correct classification with assertive agents versus 69.70% with conventional assistance, a 39.2% reduction in diagnostic errors (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)
- Non-assertive, suggestive communication was more effective for middle and senior clinicians: this style yielded 66.41% correct classification versus 65.76% with assertive agents, a 5.5% reduction in errors for experienced clinicians, and non-assertive yielded a 14.2% improvement in decision accuracy compared to assertive for this group (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)
- The assertiveness-based agent was significantly preferred by 66% of all clinicians (F = 8.35, p = 0.001), with 85% of interns and juniors favoring it and 78% of expert clinicians appreciating its guidance, though experts valued collaborative rather than directive communication (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)
- Assertiveness-based agents were rated significantly higher on perceived competence (p = 0.04) and elicited greater thoughtfulness (p = 0.001) compared to conventional agents; differences in overall trust and understanding were directionally positive but non-significant (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)
- No significant differences in workload or usability were found between conventional and assertiveness-based agents (p = 0.38), while perceived workload was reportedly reduced by 48% and usability improved by 3.41% (healthcare/breast imaging domain). (source: Calisto et al._Personalized explanations for clinician-AI interaction in breast image.txt)

## Transparency Constructs

The study's central transparency mechanism is **personalized, contextual explanation** rather than a single uniform output. The assertiveness-based agents provided: AI BIRADS severity predictions with confidence metrics; visual indicators of lesion morphology (shape, margin, density, calcification patterns); natural language clinical arguments explaining the AI's reasoning; patient-specific contextual information (family and personal history); and visual highlights marking regions of interest in images. This maps to [[natural-language-explanations]], [[explainability]], and [[causability]] (providing medically meaningful justifications). The conventional agent represented minimal [[outcome-transparency]] (numeric outputs only). The comparison thus operationalizes the difference between outcome transparency alone and richer process-level explanations contextualized to clinical reasoning. The personalization dimension — adapting communication assertiveness to expertise — connects to [[user-expertise]] as a moderator.

## Trust Constructs

Trust is measured using three dimensions: understanding (whether the clinician comprehends the agent's reasoning), competence (whether the agent is seen as capable), and thoughtfulness (whether the agent appears to reflect care for the patient). These map to [[cognitive-trust]] (competence and understanding evaluations) and [[affective-trust]] (thoughtfulness, an affective component). The study explicitly frames building trust as contingent on effective communication rather than on raw model accuracy. The qualitative data highlight that 92% of clinicians preferred human-interpretable clinical arguments over numerical outputs, aligning with the argument that [[explainability]] supports trust formation. The study also captures behavioral acceptance/rejection rates of AI suggestions as a proxy for [[behavioural-trust]] and [[appropriate-reliance]].

## Relevance to Research Questions

**RQ1**: The study contributes a domain-specific operationalization of AI transparency tailored to clinical imaging: assertiveness-based natural language explanation encompassing morphological details, severity visualization, and patient history. It also operationalizes trust as a multi-dimensional clinician-perceived construct with competence and thoughtfulness components, advancing precision in how trust is measured in healthcare AI contexts.

**RQ2**: The paper reports a conditional effect: assertiveness-based communication broadly improves diagnostic efficiency (for all groups) and accuracy (particularly for novices), but the direction of the effect on accuracy differs between novice and expert clinicians. This is a within-expertise non-linear pattern where more directive communication helps beginners but slightly impedes experts who prefer autonomy-preserving suggestions. The effect on trust dimensions (competence perceived higher with assertive, but overall trust not significantly different) also reflects a nuanced, non-straightforward relationship.

**RQ3**: User expertise/role is the central moderating variable. The study systematically compares four expertise strata (interns, juniors, middles, seniors) and demonstrates that the most effective AI communication style is expertise-contingent: assertive for novices, non-assertive for experts. This is one of the more detailed empirical treatments of expertise as a moderator of AI transparency effects available in the literature.

## Related pages

- [[user-expertise]]
- [[explainability]]
- [[causability]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[rq3-user-roles]]
