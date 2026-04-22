# Ihongbe et al. 2024 — Methods

**Summary**: A human-centered evaluation study (N=26 medical professionals) comparing two visual XAI techniques (Grad-CAM and LIME) applied to CNN-based chest X-ray and CT scan classifiers, assessing clinical relevance, comprehensibility, and trust impact via an online questionnaire.

**Sources**: Ihongbe et al._Evaluating_Explainable_Artific.pdf

**Research questions addressed**: RQ1, RQ2, RQ3

**Last updated**: 2026-04-19

---

## Study design
survey (online questionnaire-based evaluation; within-subjects comparison of two XAI techniques on fixed clinical case studies)

## Sample
- N: 26 (8 radiologists; 18 other medical specialists)
- Population: domain professionals (medical professionals — radiologists and other clinicians)
- Domain: healthcare (chest radiology — pneumonia from chest X-rays; COVID-19 from CT scans)
- Country / region: not reported
- Recruitment method: not reported (professional convenience sample)

## Transparency operationalization
- Type: explainability — visual XAI techniques applied to deep learning image classifiers:
  (1) Grad-CAM — gradient-based heatmap overlaid on chest X-ray/CT images highlighting prediction-relevant regions;
  (2) LIME — local interpretable model-agnostic explanations using superpixel segmentation to identify and highlight/mask prediction-contributing regions
- Manipulation or measure: within-subjects presentation — participants evaluated both Grad-CAM and LIME explanations for two clinical case studies (pneumonia CNN, MobileNetV2, 91% accuracy; COVID-19 CNN, ResNet-101, 98% accuracy); evaluated using researcher-constructed questionnaire items covering usefulness, usability, accuracy/truthfulness, and comprehensibility (coherency)
- Scale / instrument name: researcher-constructed evaluation criteria adapted from Jin et al. (2023): understandability, clinical relevance, truthfulness, informative plausibility, computational efficiency
- Number of items: not reported (multiple Likert items per criterion; exact count not specified)

## Trust operationalization
- Type: cognitive trust / confidence — self-reported confidence in whether XAI visualizations truthfully reflect the AI model's decision process, and whether XAI improved trust in AI diagnostic systems
- Measure: single or few Likert items on confidence in XAI accuracy and trust impact; ordinal response distributions reported (e.g., "9 expressed confidence," "12 were uncertain," "11 reported improved trust")
- Scale / instrument name: not applicable (researcher-constructed single items, not a validated trust scale)
- Number of items: not reported (appears to be one or two items addressing trust/confidence in XAI)
- Behavioural vs self-report: self-report

## Moderators and covariates tested
- Prior exposure to AI-based medical imaging tools: recorded; 16 of 26 participants had no prior exposure — identified as a mediating factor in trust and confidence responses; relevant to RQ3 (low AI literacy in clinical expert population)
- Prior knowledge of XAI: recorded; only 4 of 26 had prior knowledge of XAI — contributes to understanding of AI-novice domain experts
- Specialty (radiologist vs. other specialist): implicitly relevant; not formally tested as a moderator
- User expertise / AI literacy: measured descriptively; participants are domain experts but AI novices — a specific expertise configuration relevant to RQ3

## Statistical approach
- Primary analysis method: descriptive statistics (frequency counts and ordinal distributions of Likert responses); no inferential statistical tests reported
- Software: not reported
- Key model fit or effect size reported: not reported (descriptive only; e.g., "20 of 26 participants gave positive usefulness scores for Grad-CAM")

## Author-noted limitations
- Very small sample (N=26) limits statistical power and generalisability
- No inferential statistics reported; findings are descriptive
- Low prior AI and XAI awareness among participants may have influenced evaluations
- Grad-CAM color scheme negatively impacted readability for 13 of 26 participants; color blindness not accommodated
- Study used static clinical case studies, not real-time clinical workflow integration
- Only two XAI methods compared; other visual explanation approaches not evaluated
- Trust measure is a single or few ad-hoc items, not a validated scale

## Related pages
- [[ihongbe-xai-chest-radiology]]
- [[explainability]]
- [[outcome-transparency]]
- [[natural-language-explanations]]
- [[cognitive-trust]]
- [[user-expertise]]
- [[domain-context]]

## References
Ihongbe, T. O., et al. (2024). Evaluating explainable artificial intelligence (XAI) techniques in chest radiology imaging through a human-centered lens. *PLOS ONE*.
