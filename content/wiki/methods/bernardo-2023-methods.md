# Bernardo & Seva (2023) — Methods

**Summary**: Two-phase study (pre-study online survey N = 202; main testbed experiment) using structural equation modeling to propose and test the XAI Trust Calibration (XAITC) model, demonstrating that affective processing (discrete emotional responses to XAI design) mediates trust calibration in parallel with cognitive processing routes.

**Sources**: Bernardo & Seva_Affective_Design_Analysis_of_Explainable.pdf

**Research questions addressed**: RQ1 / RQ2 / RQ3

**Last updated**: 2026-04-19

---

## Study design
mixed-methods (pre-study online survey for scale development and preference identification; main experiment with SEM for model testing)

## Sample
- N: 202 (pre-study online survey phase; main experiment sample size not separately reported in source summary)
- Population: general AI/technology users; 71.78% reported more than five years of AI experience
- Domain: general AI/XAI interface design (no specific applied domain; study conducted at De La Salle University, Manila)
- Country / region: Philippines (De La Salle University, Manila)
- Recruitment method: not reported

## Transparency operationalization
- Type: explanation design (explanation form, communication style, supplementary information)
- Manipulation or measure: experimental design varying three XAI design components — (1) explanation form: type/modality of explanation (example-based, feature importance/saliency, rule-based); (2) communication style: tone/register (logic-robotic vs. humanized); (3) supplementary information: presence or absence of background contextual information accompanying the explanation. These were presented as design configurations in a testbed XAI interface.
- Scale / instrument name: XAI Emotion Set (XES), developed by Bernardo & Seva; perceived usefulness scale; perceived trust scale (3-item self-report)
- Number of items: 3 (perceived trust scale); XES items not reported in source summary

## Trust operationalization
- Type: cognitive (perceived trust, measured via 3-item self-report); affective (operationalized via discrete emotional states from the XES — "interestingly surprised," "trusting," "fearfully dismayed," "anxiously suspicious"); behavioural (reliance intention, self-report scale)
- Measure: perceived trust measured with a 3-item self-report scale; affective trust operationalized indirectly through the XAI Emotion Set (XES) discrete emotional states; behavioral reliance measured as self-reported intention to rely on the AI system
- Scale / instrument name: custom 3-item perceived trust scale; XAI Emotion Set (XES); custom reliance intention scale
- Number of items: 3 (perceived trust); not reported (XES items); not reported (reliance intention items)
- Behavioural vs self-report: self-report (reliance intention scale); no direct behavioral observation

## Moderators and covariates tested
- AI anxiety (individual difference, measured): significant moderator — high AI anxiety amplified negative emotional responses ("fearfully dismayed") and reduced trust and reliance; low AI anxiety users showed more stable trust under logic-robotic communication (relevant to RQ3 as an AI-literacy-adjacent user characteristic)
- Incidental emotion (affective state, measured): significant moderator of the emotion-to-trust pathway
- Perceived AI reliability (measured): significant moderator of the transparency-to-trust relationship
- User experience with AI systems (measured, continuous): significant moderator — users with >5 years AI experience showed different moderation patterns than short-experience users (directly relevant to RQ3)
- Trust disposition / dispositional trust (measured): not a significant moderator
- Learning capability (measured): not a significant moderator

## Statistical approach
- Primary analysis method: structural equation modeling (SEM) with 2000 bootstrap iterations for indirect effect testing; exploratory factor analysis (EFA) and confirmatory factor analysis (CFA) for scale validation
- Software: not reported
- Key model fit or effect size reported: KMO = 0.919 (p < 0.001) for EFA; CFI = 0.991, RMSEA = 0.039 for CFA; selected β coefficients reported (e.g., example-based form → "interestingly surprised": β = 0.530, p = 0.001; perceived trust → reliance: β = 0.439, p = 0.001)

## Author-noted limitations
- The main experiment sample size and composition are not detailed in the source summary; replication with larger, more diverse samples recommended
- The XAI Emotion Set (XES) is a purpose-built instrument requiring further validation across different populations and domains
- Reliance is measured as self-report intention rather than actual behavioral reliance, limiting ecological validity
- The study domain is general AI/XAI without a specific applied context; generalizability to high-stakes domains (healthcare, legal) is uncertain
- Affective processing route was tested in a relatively favorable AI experience context (Philippines university); cultural variation in emotional responses to AI is unexplored

## Related pages
- [[bernardo-seva-affective-design-xai]]
- [[explainability]]
- [[example-based-explanations]]
- [[affective-trust]]
- [[cognitive-trust]]
- [[behavioural-trust]]
- [[trust-calibration]]
- [[user-expertise]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
- [[rq3-user-roles]]

## References
Bernardo, G., & Seva, R. (2023). *Affective design analysis of explainable artificial intelligence (XAI): A user-centric perspective*. [Journal not reported in source summary.]

Lee, J. D., & See, K. A. (2004). Trust in automation: Designing for appropriate reliance. *Human Factors, 46*(1), 50–80.
